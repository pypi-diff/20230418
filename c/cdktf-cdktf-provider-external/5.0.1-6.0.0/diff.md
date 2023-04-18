# Comparing `tmp/cdktf-cdktf-provider-external-5.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-external-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-external-5.0.1.tar", last modified: Tue Mar  7 03:24:22 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-external-6.0.0.tar", last modified: Tue Apr 18 20:37:46 2023, max compression
```

## Comparing `cdktf-cdktf-provider-external-5.0.1.tar` & `cdktf-cdktf-provider-external-6.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.893195 cdktf-cdktf-provider-external-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39776 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/_jsii/provider-external@5.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/data_external/
--rw-r--r--   0 runner    (1001) docker     (123)    21127 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/data_external/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 03:24:08.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 03:24:22.897195 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-03-07 03:24:22.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-03-07 03:24:22.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 03:24:22.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-07 03:24:22.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-07 03:24:22.000000 cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39509 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/_jsii/provider-external@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/data_external/
+-rw-r--r--   0 runner    (1001) docker     (123)    21802 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/data_external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:33.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:46.214299 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 20:37:46.000000 cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-external-5.0.1/LICENSE` & `cdktf-cdktf-provider-external-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-external-5.0.1/PKG-INFO` & `cdktf-cdktf-provider-external-6.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-external
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt external Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-external.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-external.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-external-5.0.1/README.md` & `cdktf-cdktf-provider-external-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-external-5.0.1/setup.py` & `cdktf-cdktf-provider-external-6.0.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-external",
-    "version": "5.0.1",
+    "version": "6.0.0",
     "description": "Prebuilt external Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-external.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -24,25 +24,25 @@
         "cdktf_cdktf_provider_external",
         "cdktf_cdktf_provider_external._jsii",
         "cdktf_cdktf_provider_external.data_external",
         "cdktf_cdktf_provider_external.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_external._jsii": [
-            "provider-external@5.0.1.jsii.tgz"
+            "provider-external@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_external": [
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

### Comparing `cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/__init__.py` & `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/data_external/__init__.py` & `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/data_external/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_external`
 
-Refer to the Terraform Registory for docs: [`data_external`](https://www.terraform.io/docs/providers/external/d/external).
+Refer to the Terraform Registory for docs: [`data_external`](https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class DataExternal(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-external.dataExternal.DataExternal",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/external/d/external external}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external external}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         program: typing.Sequence[builtins.str],
         query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         working_dir: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/external/d/external external} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external external} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param program: A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program. Terraform does not execute the program through a shell, so it is not necessary to escape shell metacharacters nor add quotes around arguments containing spaces. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#program DataExternal#program}
-        :param query: A map of string values to pass to the external program as the query arguments. If not supplied, the program will receive an empty object as its input. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#query DataExternal#query}
-        :param working_dir: Working directory of the program. If not supplied, the program will run in the current directory. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#working_dir DataExternal#working_dir}
+        :param program: A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program. Terraform does not execute the program through a shell, so it is not necessary to escape shell metacharacters nor add quotes around arguments containing spaces. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#program DataExternal#program}
+        :param query: A map of string values to pass to the external program as the query arguments. If not supplied, the program will receive an empty object as its input. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#query DataExternal#query}
+        :param working_dir: Working directory of the program. If not supplied, the program will run in the current directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#working_dir DataExternal#working_dir}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -176,15 +176,15 @@
     },
 )
 class DataExternalConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         program: typing.Sequence[builtins.str],
         query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
@@ -194,17 +194,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param program: A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program. Terraform does not execute the program through a shell, so it is not necessary to escape shell metacharacters nor add quotes around arguments containing spaces. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#program DataExternal#program}
-        :param query: A map of string values to pass to the external program as the query arguments. If not supplied, the program will receive an empty object as its input. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#query DataExternal#query}
-        :param working_dir: Working directory of the program. If not supplied, the program will run in the current directory. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#working_dir DataExternal#working_dir}
+        :param program: A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program. Terraform does not execute the program through a shell, so it is not necessary to escape shell metacharacters nor add quotes around arguments containing spaces. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#program DataExternal#program}
+        :param query: A map of string values to pass to the external program as the query arguments. If not supplied, the program will receive an empty object as its input. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#query DataExternal#query}
+        :param working_dir: Working directory of the program. If not supplied, the program will run in the current directory. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#working_dir DataExternal#working_dir}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__20f223c2f51321f1b1c070c94a8d810144471c382dd510e7ec880d19b1d07877)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -245,20 +245,22 @@
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
@@ -302,36 +304,36 @@
 
     @builtins.property
     def program(self) -> typing.List[builtins.str]:
         '''A list of strings, whose first element is the program to run and whose subsequent elements are optional command line arguments to the program.
 
         Terraform does not execute the program through a shell, so it is not necessary to escape shell metacharacters nor add quotes around arguments containing spaces.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#program DataExternal#program}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#program DataExternal#program}
         '''
         result = self._values.get("program")
         assert result is not None, "Required property 'program' is missing"
         return typing.cast(typing.List[builtins.str], result)
 
     @builtins.property
     def query(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A map of string values to pass to the external program as the query arguments.
 
         If not supplied, the program will receive an empty object as its input.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#query DataExternal#query}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#query DataExternal#query}
         '''
         result = self._values.get("query")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def working_dir(self) -> typing.Optional[builtins.str]:
         '''Working directory of the program. If not supplied, the program will run in the current directory.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external/d/external#working_dir DataExternal#working_dir}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs/data-sources/external#working_dir DataExternal#working_dir}
         '''
         result = self._values.get("working_dir")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -355,15 +357,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     program: typing.Sequence[builtins.str],
     query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     working_dir: typing.Optional[builtins.str] = None,
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
@@ -386,15 +388,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__20f223c2f51321f1b1c070c94a8d810144471c382dd510e7ec880d19b1d07877(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     program: typing.Sequence[builtins.str],
     query: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
```

### Comparing `cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external/provider/__init__.py` & `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external/provider/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`external`](https://www.terraform.io/docs/providers/external).
+Refer to the Terraform Registory for docs: [`external`](https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class ExternalProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-external.provider.ExternalProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/external external}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs external}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/external external} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs external} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external#alias ExternalProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs#alias ExternalProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__5897ed52158114f2fcca2f46a9b4605920a201dd37eb8f75baeccc95bf9a930a)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = ExternalProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-external.provider.ExternalProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class ExternalProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external#alias ExternalProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs#alias ExternalProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__128fc9b7d9e2a0186b8efb7aba666d1d80bc3d2b0df164a32bc4af6f41583e0e)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/external#alias ExternalProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/external/2.3.1/docs#alias ExternalProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO` & `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-external
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt external Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-external.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-external.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-cdktf-provider-external-5.0.1/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-external-6.0.0/src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/cdktf_cdktf_provider_external/py.typed
 src/cdktf_cdktf_provider_external.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_external.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_external.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_external.egg-info/requires.txt
 src/cdktf_cdktf_provider_external.egg-info/top_level.txt
 src/cdktf_cdktf_provider_external/_jsii/__init__.py
-src/cdktf_cdktf_provider_external/_jsii/provider-external@5.0.1.jsii.tgz
+src/cdktf_cdktf_provider_external/_jsii/provider-external@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_external/data_external/__init__.py
 src/cdktf_cdktf_provider_external/provider/__init__.py
```

