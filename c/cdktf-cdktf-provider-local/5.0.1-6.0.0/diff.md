# Comparing `tmp/cdktf-cdktf-provider-local-5.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-local-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-local-5.0.1.tar", last modified: Thu Mar  9 03:22:09 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-local-6.0.0.tar", last modified: Tue Apr 18 20:46:15 2023, max compression
```

## Comparing `cdktf-cdktf-provider-local-5.0.1.tar` & `cdktf-cdktf-provider-local-6.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.258063 cdktf-cdktf-provider-local-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.262063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/
--rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97041 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/_jsii/provider-local@5.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/data_local_file/
--rw-r--r--   0 runner    (1001) docker     (123)    16135 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/data_local_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/data_local_sensitive_file/
--rw-r--r--   0 runner    (1001) docker     (123)    16352 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/file/
--rw-r--r--   0 runner    (1001) docker     (123)    34002 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.266063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/sensitive_file/
--rw-r--r--   0 runner    (1001) docker     (123)    30787 2023-03-09 03:21:55.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-09 03:22:09.262063 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-03-09 03:22:09.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-03-09 03:22:09.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-09 03:22:09.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-09 03:22:09.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-09 03:22:09.000000 cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98057 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/_jsii/provider-local@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    16618 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_sensitive_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/file/
+-rw-r--r--   0 runner    (1001) docker     (123)    34989 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.166419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/sensitive_file/
+-rw-r--r--   0 runner    (1001) docker     (123)    31687 2023-04-18 20:46:03.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:46:15.162419 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4109 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 20:46:15.000000 cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/LICENSE` & `cdktf-cdktf-provider-local-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-5.0.1/PKG-INFO` & `cdktf-cdktf-provider-local-6.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-local
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt local Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-local.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-local.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/README.md` & `cdktf-cdktf-provider-local-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-5.0.1/setup.py` & `cdktf-cdktf-provider-local-6.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-local",
-    "version": "5.0.1",
+    "version": "6.0.0",
     "description": "Prebuilt local Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-local.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -27,25 +27,25 @@
         "cdktf_cdktf_provider_local.data_local_sensitive_file",
         "cdktf_cdktf_provider_local.file",
         "cdktf_cdktf_provider_local.provider",
         "cdktf_cdktf_provider_local.sensitive_file"
     ],
     "package_data": {
         "cdktf_cdktf_provider_local._jsii": [
-            "provider-local@5.0.1.jsii.tgz"
+            "provider-local@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_local": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.77.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/__init__.py` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/data_local_file/__init__.py` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_local_file`
+# `data_local_sensitive_file`
 
-Refer to the Terraform Registory for docs: [`data_local_file`](https://www.terraform.io/docs/providers/local/d/file).
+Refer to the Terraform Registory for docs: [`data_local_sensitive_file`](https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/sensitive_file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,53 +17,53 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataLocalFile(
+class DataLocalSensitiveFile(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-local.dataLocalFile.DataLocalFile",
+    jsii_type="@cdktf/provider-local.dataLocalSensitiveFile.DataLocalSensitiveFile",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/local/d/file local_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/sensitive_file local_sensitive_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         filename: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/local/d/file local_file} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/sensitive_file local_sensitive_file} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/d/file#filename DataLocalFile#filename}
+        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/sensitive_file#filename DataLocalSensitiveFile#filename}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7c40b22cb4bf074114ed2d5a45f236b5970720ad7cc28a16c755e5ec69bded2a)
+            type_hints = typing.get_type_hints(_typecheckingstub__f6b32e8e1ae72f2e8255b5d19c323d5a9e477f6cecf373f437a1d6d857449067)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        config = DataLocalFileConfig(
+        config = DataLocalSensitiveFileConfig(
             filename=filename,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
@@ -135,39 +135,39 @@
     @jsii.member(jsii_name="filename")
     def filename(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "filename"))
 
     @filename.setter
     def filename(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__a0420f5a22cba44fbaed45ef366ce72ba27189f3e75a5e2a928d339e7a302bc9)
+            type_hints = typing.get_type_hints(_typecheckingstub__c96ef78dd9f935f17069f0469de9977073b0399feff782682a5bcb3f6f676325)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "filename", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-local.dataLocalFile.DataLocalFileConfig",
+    jsii_type="@cdktf/provider-local.dataLocalSensitiveFile.DataLocalSensitiveFileConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "filename": "filename",
     },
 )
-class DataLocalFileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class DataLocalSensitiveFileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         filename: builtins.str,
     ) -> None:
@@ -175,20 +175,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/d/file#filename DataLocalFile#filename}
+        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/sensitive_file#filename DataLocalSensitiveFile#filename}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__7e704d91da597985ed1a812d55e188fedd61b090dd23dd9118ca1472cf767a2b)
+            type_hints = typing.get_type_hints(_typecheckingstub__41d6f47472569baae63911a6d9020d78f0efadf281f903d60bc6432fa2455ac0)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
@@ -218,20 +218,22 @@
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
@@ -275,65 +277,65 @@
 
     @builtins.property
     def filename(self) -> builtins.str:
         '''Path to the file that will be read.
 
         The data source will return an error if the file does not exist.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/d/file#filename DataLocalFile#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/sensitive_file#filename DataLocalSensitiveFile#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataLocalFileConfig(%s)" % ", ".join(
+        return "DataLocalSensitiveFileConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataLocalFile",
-    "DataLocalFileConfig",
+    "DataLocalSensitiveFile",
+    "DataLocalSensitiveFileConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__7c40b22cb4bf074114ed2d5a45f236b5970720ad7cc28a16c755e5ec69bded2a(
+def _typecheckingstub__f6b32e8e1ae72f2e8255b5d19c323d5a9e477f6cecf373f437a1d6d857449067(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     filename: builtins.str,
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
     pass
 
-def _typecheckingstub__a0420f5a22cba44fbaed45ef366ce72ba27189f3e75a5e2a928d339e7a302bc9(
+def _typecheckingstub__c96ef78dd9f935f17069f0469de9977073b0399feff782682a5bcb3f6f676325(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__7e704d91da597985ed1a812d55e188fedd61b090dd23dd9118ca1472cf767a2b(
+def _typecheckingstub__41d6f47472569baae63911a6d9020d78f0efadf281f903d60bc6432fa2455ac0(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     filename: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/data_local_file/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
-# `data_local_sensitive_file`
+# `data_local_file`
 
-Refer to the Terraform Registory for docs: [`data_local_sensitive_file`](https://www.terraform.io/docs/providers/local/d/sensitive_file).
+Refer to the Terraform Registory for docs: [`data_local_file`](https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -17,53 +17,53 @@
 
 from .._jsii import *
 
 import cdktf as _cdktf_9a9027ec
 import constructs as _constructs_77d1e7e8
 
 
-class DataLocalSensitiveFile(
+class DataLocalFile(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
-    jsii_type="@cdktf/provider-local.dataLocalSensitiveFile.DataLocalSensitiveFile",
+    jsii_type="@cdktf/provider-local.dataLocalFile.DataLocalFile",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/local/d/sensitive_file local_sensitive_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/file local_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         filename: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/local/d/sensitive_file local_sensitive_file} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/file local_file} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/d/sensitive_file#filename DataLocalSensitiveFile#filename}
+        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/file#filename DataLocalFile#filename}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__f6b32e8e1ae72f2e8255b5d19c323d5a9e477f6cecf373f437a1d6d857449067)
+            type_hints = typing.get_type_hints(_typecheckingstub__7c40b22cb4bf074114ed2d5a45f236b5970720ad7cc28a16c755e5ec69bded2a)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
-        config = DataLocalSensitiveFileConfig(
+        config = DataLocalFileConfig(
             filename=filename,
             connection=connection,
             count=count,
             depends_on=depends_on,
             for_each=for_each,
             lifecycle=lifecycle,
             provider=provider,
@@ -135,39 +135,39 @@
     @jsii.member(jsii_name="filename")
     def filename(self) -> builtins.str:
         return typing.cast(builtins.str, jsii.get(self, "filename"))
 
     @filename.setter
     def filename(self, value: builtins.str) -> None:
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c96ef78dd9f935f17069f0469de9977073b0399feff782682a5bcb3f6f676325)
+            type_hints = typing.get_type_hints(_typecheckingstub__a0420f5a22cba44fbaed45ef366ce72ba27189f3e75a5e2a928d339e7a302bc9)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "filename", value)
 
 
 @jsii.data_type(
-    jsii_type="@cdktf/provider-local.dataLocalSensitiveFile.DataLocalSensitiveFileConfig",
+    jsii_type="@cdktf/provider-local.dataLocalFile.DataLocalFileConfig",
     jsii_struct_bases=[_cdktf_9a9027ec.TerraformMetaArguments],
     name_mapping={
         "connection": "connection",
         "count": "count",
         "depends_on": "dependsOn",
         "for_each": "forEach",
         "lifecycle": "lifecycle",
         "provider": "provider",
         "provisioners": "provisioners",
         "filename": "filename",
     },
 )
-class DataLocalSensitiveFileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
+class DataLocalFileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         filename: builtins.str,
     ) -> None:
@@ -175,20 +175,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/d/sensitive_file#filename DataLocalSensitiveFile#filename}
+        :param filename: Path to the file that will be read. The data source will return an error if the file does not exist. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/file#filename DataLocalFile#filename}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__41d6f47472569baae63911a6d9020d78f0efadf281f903d60bc6432fa2455ac0)
+            type_hints = typing.get_type_hints(_typecheckingstub__7e704d91da597985ed1a812d55e188fedd61b090dd23dd9118ca1472cf767a2b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
             check_type(argname="argument depends_on", value=depends_on, expected_type=type_hints["depends_on"])
             check_type(argname="argument for_each", value=for_each, expected_type=type_hints["for_each"])
             check_type(argname="argument lifecycle", value=lifecycle, expected_type=type_hints["lifecycle"])
             check_type(argname="argument provider", value=provider, expected_type=type_hints["provider"])
             check_type(argname="argument provisioners", value=provisioners, expected_type=type_hints["provisioners"])
@@ -218,20 +218,22 @@
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
@@ -275,65 +277,65 @@
 
     @builtins.property
     def filename(self) -> builtins.str:
         '''Path to the file that will be read.
 
         The data source will return an error if the file does not exist.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/d/sensitive_file#filename DataLocalSensitiveFile#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/data-sources/file#filename DataLocalFile#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DataLocalSensitiveFileConfig(%s)" % ", ".join(
+        return "DataLocalFileConfig(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 __all__ = [
-    "DataLocalSensitiveFile",
-    "DataLocalSensitiveFileConfig",
+    "DataLocalFile",
+    "DataLocalFileConfig",
 ]
 
 publication.publish()
 
-def _typecheckingstub__f6b32e8e1ae72f2e8255b5d19c323d5a9e477f6cecf373f437a1d6d857449067(
+def _typecheckingstub__7c40b22cb4bf074114ed2d5a45f236b5970720ad7cc28a16c755e5ec69bded2a(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     filename: builtins.str,
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
     pass
 
-def _typecheckingstub__c96ef78dd9f935f17069f0469de9977073b0399feff782682a5bcb3f6f676325(
+def _typecheckingstub__a0420f5a22cba44fbaed45ef366ce72ba27189f3e75a5e2a928d339e7a302bc9(
     value: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__41d6f47472569baae63911a6d9020d78f0efadf281f903d60bc6432fa2455ac0(
+def _typecheckingstub__7e704d91da597985ed1a812d55e188fedd61b090dd23dd9118ca1472cf767a2b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     filename: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/file/__init__.py` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/file/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `local_file`
 
-Refer to the Terraform Registory for docs: [`local_file`](https://www.terraform.io/docs/providers/local/r/file).
+Refer to the Terraform Registory for docs: [`local_file`](https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,47 +22,47 @@
 
 
 class File(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-local.file.File",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/local/r/file local_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file local_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         filename: builtins.str,
         content: typing.Optional[builtins.str] = None,
         content_base64: typing.Optional[builtins.str] = None,
         directory_permission: typing.Optional[builtins.str] = None,
         file_permission: typing.Optional[builtins.str] = None,
         sensitive_content: typing.Optional[builtins.str] = None,
         source: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/local/r/file local_file} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file local_file} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#filename File#filename}
-        :param content: Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``sensitive_content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#content File#content}
-        :param content_base64: Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content``, ``sensitive_content`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#content_base64 File#content_base64}
-        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#directory_permission File#directory_permission}
-        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#file_permission File#file_permission}
-        :param sensitive_content: Sensitive content to store in the file, expected to be an UTF-8 encoded string. Will not be displayed in diffs. Conflicts with ``content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. If in need to use *sensitive* content, please use the ```local_sensitive_file`` <./sensitive_file.html>`_ resource instead. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#sensitive_content File#sensitive_content}
-        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content``, ``sensitive_content`` and ``content_base64``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#source File#source}
+        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#filename File#filename}
+        :param content: Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``sensitive_content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#content File#content}
+        :param content_base64: Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content``, ``sensitive_content`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#content_base64 File#content_base64}
+        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#directory_permission File#directory_permission}
+        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#file_permission File#file_permission}
+        :param sensitive_content: Sensitive content to store in the file, expected to be an UTF-8 encoded string. Will not be displayed in diffs. Conflicts with ``content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. If in need to use *sensitive* content, please use the ```local_sensitive_file`` <./sensitive_file.html>`_ resource instead. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#sensitive_content File#sensitive_content}
+        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content``, ``sensitive_content`` and ``content_base64``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#source File#source}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -299,15 +299,15 @@
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
         filename: builtins.str,
         content: typing.Optional[builtins.str] = None,
@@ -321,21 +321,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#filename File#filename}
-        :param content: Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``sensitive_content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#content File#content}
-        :param content_base64: Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content``, ``sensitive_content`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#content_base64 File#content_base64}
-        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#directory_permission File#directory_permission}
-        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#file_permission File#file_permission}
-        :param sensitive_content: Sensitive content to store in the file, expected to be an UTF-8 encoded string. Will not be displayed in diffs. Conflicts with ``content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. If in need to use *sensitive* content, please use the ```local_sensitive_file`` <./sensitive_file.html>`_ resource instead. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#sensitive_content File#sensitive_content}
-        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content``, ``sensitive_content`` and ``content_base64``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#source File#source}
+        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#filename File#filename}
+        :param content: Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``sensitive_content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#content File#content}
+        :param content_base64: Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content``, ``sensitive_content`` and ``source``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#content_base64 File#content_base64}
+        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#directory_permission File#directory_permission}
+        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#file_permission File#file_permission}
+        :param sensitive_content: Sensitive content to store in the file, expected to be an UTF-8 encoded string. Will not be displayed in diffs. Conflicts with ``content``, ``content_base64`` and ``source``. Exactly one of these four arguments must be specified. If in need to use *sensitive* content, please use the ```local_sensitive_file`` <./sensitive_file.html>`_ resource instead. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#sensitive_content File#sensitive_content}
+        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content``, ``sensitive_content`` and ``content_base64``. Exactly one of these four arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#source File#source}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2096116de66f92c58057bacda7e9d95a3670b45b8d98520953ca363dc7fd950b)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -388,20 +388,22 @@
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
@@ -446,85 +448,85 @@
     @builtins.property
     def filename(self) -> builtins.str:
         '''The path to the file that will be created.
 
         Missing parent directories will be created.
         If the file already exists, it will be overridden with the given content.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#filename File#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#filename File#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def content(self) -> typing.Optional[builtins.str]:
         '''Content to store in the file, expected to be a UTF-8 encoded string.
 
         Conflicts with ``sensitive_content``, ``content_base64`` and ``source``.
         Exactly one of these four arguments must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#content File#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#content File#content}
         '''
         result = self._values.get("content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def content_base64(self) -> typing.Optional[builtins.str]:
         '''Content to store in the file, expected to be binary encoded as base64 string.
 
         Conflicts with ``content``, ``sensitive_content`` and ``source``.
         Exactly one of these four arguments must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#content_base64 File#content_base64}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#content_base64 File#content_base64}
         '''
         result = self._values.get("content_base64")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def directory_permission(self) -> typing.Optional[builtins.str]:
         '''Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#directory_permission File#directory_permission}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#directory_permission File#directory_permission}
         '''
         result = self._values.get("directory_permission")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def file_permission(self) -> typing.Optional[builtins.str]:
         '''Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0777"``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#file_permission File#file_permission}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#file_permission File#file_permission}
         '''
         result = self._values.get("file_permission")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def sensitive_content(self) -> typing.Optional[builtins.str]:
         '''Sensitive content to store in the file, expected to be an UTF-8 encoded string.
 
         Will not be displayed in diffs.
         Conflicts with ``content``, ``content_base64`` and ``source``.
         Exactly one of these four arguments must be specified.
         If in need to use *sensitive* content, please use the ```local_sensitive_file`` <./sensitive_file.html>`_
         resource instead.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#sensitive_content File#sensitive_content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#sensitive_content File#sensitive_content}
         '''
         result = self._values.get("sensitive_content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source(self) -> typing.Optional[builtins.str]:
         '''Path to file to use as source for the one we are creating.
 
         Conflicts with ``content``, ``sensitive_content`` and ``content_base64``.
         Exactly one of these four arguments must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/file#source File#source}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/file#source File#source}
         '''
         result = self._values.get("source")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -552,15 +554,15 @@
     content: typing.Optional[builtins.str] = None,
     content_base64: typing.Optional[builtins.str] = None,
     directory_permission: typing.Optional[builtins.str] = None,
     file_permission: typing.Optional[builtins.str] = None,
     sensitive_content: typing.Optional[builtins.str] = None,
     source: typing.Optional[builtins.str] = None,
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
@@ -607,15 +609,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2096116de66f92c58057bacda7e9d95a3670b45b8d98520953ca363dc7fd950b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     filename: builtins.str,
     content: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/provider/__init__.py` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/provider/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`local`](https://www.terraform.io/docs/providers/local).
+Refer to the Terraform Registory for docs: [`local`](https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class LocalProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-local.provider.LocalProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/local local}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs local}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/local local} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs local} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local#alias LocalProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs#alias LocalProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7d22d61fb4ed68f610990262a1621168510888406f1536f801321deb6cdbe957)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = LocalProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-local.provider.LocalProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class LocalProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local#alias LocalProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs#alias LocalProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__64dbc73e09606aa66a4af8e9a0dea1ddd020dc0f7219838f63e50d705d476407)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local#alias LocalProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs#alias LocalProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local/sensitive_file/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `local_sensitive_file`
 
-Refer to the Terraform Registory for docs: [`local_sensitive_file`](https://www.terraform.io/docs/providers/local/r/sensitive_file).
+Refer to the Terraform Registory for docs: [`local_sensitive_file`](https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class SensitiveFile(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-local.sensitiveFile.SensitiveFile",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/local/r/sensitive_file local_sensitive_file}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file local_sensitive_file}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         filename: builtins.str,
         content: typing.Optional[builtins.str] = None,
         content_base64: typing.Optional[builtins.str] = None,
         directory_permission: typing.Optional[builtins.str] = None,
         file_permission: typing.Optional[builtins.str] = None,
         source: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/local/r/sensitive_file local_sensitive_file} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file local_sensitive_file} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#filename SensitiveFile#filename}
-        :param content: Sensitive Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``content_base64`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#content SensitiveFile#content}
-        :param content_base64: Sensitive Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#content_base64 SensitiveFile#content_base64}
-        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#directory_permission SensitiveFile#directory_permission}
-        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#file_permission SensitiveFile#file_permission}
-        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content`` and ``content_base64``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#source SensitiveFile#source}
+        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#filename SensitiveFile#filename}
+        :param content: Sensitive Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``content_base64`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#content SensitiveFile#content}
+        :param content_base64: Sensitive Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#content_base64 SensitiveFile#content_base64}
+        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#directory_permission SensitiveFile#directory_permission}
+        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#file_permission SensitiveFile#file_permission}
+        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content`` and ``content_base64``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#source SensitiveFile#source}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -274,15 +274,15 @@
     },
 )
 class SensitiveFileConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         filename: builtins.str,
         content: typing.Optional[builtins.str] = None,
@@ -295,20 +295,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#filename SensitiveFile#filename}
-        :param content: Sensitive Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``content_base64`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#content SensitiveFile#content}
-        :param content_base64: Sensitive Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#content_base64 SensitiveFile#content_base64}
-        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#directory_permission SensitiveFile#directory_permission}
-        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#file_permission SensitiveFile#file_permission}
-        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content`` and ``content_base64``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#source SensitiveFile#source}
+        :param filename: The path to the file that will be created. Missing parent directories will be created. If the file already exists, it will be overridden with the given content. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#filename SensitiveFile#filename}
+        :param content: Sensitive Content to store in the file, expected to be a UTF-8 encoded string. Conflicts with ``content_base64`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#content SensitiveFile#content}
+        :param content_base64: Sensitive Content to store in the file, expected to be binary encoded as base64 string. Conflicts with ``content`` and ``source``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#content_base64 SensitiveFile#content_base64}
+        :param directory_permission: Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#directory_permission SensitiveFile#directory_permission}
+        :param file_permission: Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#file_permission SensitiveFile#file_permission}
+        :param source: Path to file to use as source for the one we are creating. Conflicts with ``content`` and ``content_base64``. Exactly one of these three arguments must be specified. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#source SensitiveFile#source}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cb87d8e0300782880f73b41d51c4661b03af412eae6624965aecdac9117a804a)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -358,20 +358,22 @@
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
@@ -416,70 +418,70 @@
     @builtins.property
     def filename(self) -> builtins.str:
         '''The path to the file that will be created.
 
         Missing parent directories will be created.
         If the file already exists, it will be overridden with the given content.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#filename SensitiveFile#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#filename SensitiveFile#filename}
         '''
         result = self._values.get("filename")
         assert result is not None, "Required property 'filename' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def content(self) -> typing.Optional[builtins.str]:
         '''Sensitive Content to store in the file, expected to be a UTF-8 encoded string.
 
         Conflicts with ``content_base64`` and ``source``.
         Exactly one of these three arguments must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#content SensitiveFile#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#content SensitiveFile#content}
         '''
         result = self._values.get("content")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def content_base64(self) -> typing.Optional[builtins.str]:
         '''Sensitive Content to store in the file, expected to be binary encoded as base64 string.
 
         Conflicts with ``content`` and ``source``.
         Exactly one of these three arguments must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#content_base64 SensitiveFile#content_base64}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#content_base64 SensitiveFile#content_base64}
         '''
         result = self._values.get("content_base64")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def directory_permission(self) -> typing.Optional[builtins.str]:
         '''Permissions to set for directories created (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#directory_permission SensitiveFile#directory_permission}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#directory_permission SensitiveFile#directory_permission}
         '''
         result = self._values.get("directory_permission")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def file_permission(self) -> typing.Optional[builtins.str]:
         '''Permissions to set for the output file (before umask), expressed as string in `numeric notation <https://en.wikipedia.org/wiki/File-system_permissions#Numeric_notation>`_. Default value is ``"0700"``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#file_permission SensitiveFile#file_permission}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#file_permission SensitiveFile#file_permission}
         '''
         result = self._values.get("file_permission")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source(self) -> typing.Optional[builtins.str]:
         '''Path to file to use as source for the one we are creating.
 
         Conflicts with ``content`` and ``content_base64``.
         Exactly one of these three arguments must be specified.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/local/r/sensitive_file#source SensitiveFile#source}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/local/2.4.0/docs/resources/sensitive_file#source SensitiveFile#source}
         '''
         result = self._values.get("source")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -506,15 +508,15 @@
     filename: builtins.str,
     content: typing.Optional[builtins.str] = None,
     content_base64: typing.Optional[builtins.str] = None,
     directory_permission: typing.Optional[builtins.str] = None,
     file_permission: typing.Optional[builtins.str] = None,
     source: typing.Optional[builtins.str] = None,
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
@@ -555,15 +557,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__cb87d8e0300782880f73b41d51c4661b03af412eae6624965aecdac9117a804a(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     filename: builtins.str,
     content: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-local
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt local Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-local.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-local.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-local-5.0.1/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-local-6.0.0/src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 src/cdktf_cdktf_provider_local/py.typed
 src/cdktf_cdktf_provider_local.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_local.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_local.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_local.egg-info/requires.txt
 src/cdktf_cdktf_provider_local.egg-info/top_level.txt
 src/cdktf_cdktf_provider_local/_jsii/__init__.py
-src/cdktf_cdktf_provider_local/_jsii/provider-local@5.0.1.jsii.tgz
+src/cdktf_cdktf_provider_local/_jsii/provider-local@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_local/data_local_file/__init__.py
 src/cdktf_cdktf_provider_local/data_local_sensitive_file/__init__.py
 src/cdktf_cdktf_provider_local/file/__init__.py
 src/cdktf_cdktf_provider_local/provider/__init__.py
 src/cdktf_cdktf_provider_local/sensitive_file/__init__.py
```

