# Comparing `tmp/cdktf-cdktf-provider-cloudinit-5.0.1.tar.gz` & `tmp/cdktf-cdktf-provider-cloudinit-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-cloudinit-5.0.1.tar", last modified: Thu Mar  2 13:44:53 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-cloudinit-6.0.0.tar", last modified: Tue Apr 18 20:31:59 2023, max compression
```

## Comparing `cdktf-cdktf-provider-cloudinit-5.0.1.tar` & `cdktf-cdktf-provider-cloudinit-6.0.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.492361 cdktf-cdktf-provider-cloudinit-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-02 13:44:53.492361 cdktf-cdktf-provider-cloudinit-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 13:44:53.492361 cdktf-cdktf-provider-cloudinit-5.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.488361 cdktf-cdktf-provider-cloudinit-5.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.488361 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.488361 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      421 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    97421 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@5.0.1.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.488361 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/config/
--rw-r--r--   0 runner    (1001) docker     (123)    42411 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.492361 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/
--rw-r--r--   0 runner    (1001) docker     (123)    43271 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.492361 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5402 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:44:40.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:44:53.488361 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-03-02 13:44:53.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-03-02 13:44:53.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:44:53.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-03-02 13:44:53.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-02 13:44:53.000000 cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.727847 cdktf-cdktf-provider-cloudinit-6.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    97328 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@6.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    43369 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    44298 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:31:45.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:31:59.731847 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4213 2023-04-18 20:31:59.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 20:31:59.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:31:59.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:31:59.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-04-18 20:31:59.000000 cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/LICENSE` & `cdktf-cdktf-provider-cloudinit-6.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/PKG-INFO` & `cdktf-cdktf-provider-cloudinit-6.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-cloudinit
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt cloudinit Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-cloudinit.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-cloudinit.git
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
```

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/README.md` & `cdktf-cdktf-provider-cloudinit-6.0.0/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/setup.py` & `cdktf-cdktf-provider-cloudinit-6.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-cloudinit",
-    "version": "5.0.1",
+    "version": "6.0.0",
     "description": "Prebuilt cloudinit Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-cloudinit.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -25,37 +25,38 @@
         "cdktf_cdktf_provider_cloudinit._jsii",
         "cdktf_cdktf_provider_cloudinit.config",
         "cdktf_cdktf_provider_cloudinit.data_cloudinit_config",
         "cdktf_cdktf_provider_cloudinit.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_cloudinit._jsii": [
-            "provider-cloudinit@5.0.1.jsii.tgz"
+            "provider-cloudinit@6.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_cloudinit": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.76.0, <2.0.0",
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

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/__init__.py` & `cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/config/__init__.py` & `cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/config/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `cloudinit_config`
 
-Refer to the Terraform Registory for docs: [`cloudinit_config`](https://www.terraform.io/docs/providers/cloudinit/r/config).
+Refer to the Terraform Registory for docs: [`cloudinit_config`](https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class Config(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-cloudinit.config.Config",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/cloudinit/r/config cloudinit_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config cloudinit_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         boundary: typing.Optional[builtins.str] = None,
         gzip: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         part: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["ConfigPart", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/cloudinit/r/config cloudinit_config} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config cloudinit_config} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#base64_encode Config#base64_encode}
-        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#boundary Config#boundary}
-        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#gzip Config#gzip}
-        :param part: part block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#part Config#part}
+        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#base64_encode Config#base64_encode}
+        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#boundary Config#boundary}
+        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#gzip Config#gzip}
+        :param part: part block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#part Config#part}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -221,15 +221,15 @@
     },
 )
 class ConfigConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         boundary: typing.Optional[builtins.str] = None,
@@ -240,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#base64_encode Config#base64_encode}
-        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#boundary Config#boundary}
-        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#gzip Config#gzip}
-        :param part: part block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#part Config#part}
+        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#base64_encode Config#base64_encode}
+        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#boundary Config#boundary}
+        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#gzip Config#gzip}
+        :param part: part block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#part Config#part}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__b6518f0322408809a87b0713f41a8eb39e8f2aeeb04828147592a0138bd68c13)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -295,20 +295,22 @@
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
@@ -354,46 +356,46 @@
     def base64_encode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specify whether or not to base64 encode the ``rendered`` output.
 
         Defaults to ``true``, and cannot be disabled if gzip is ``true``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#base64_encode Config#base64_encode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#base64_encode Config#base64_encode}
         '''
         result = self._values.get("base64_encode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def boundary(self) -> typing.Optional[builtins.str]:
         '''Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#boundary Config#boundary}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#boundary Config#boundary}
         '''
         result = self._values.get("boundary")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def gzip(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#gzip Config#gzip}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#gzip Config#gzip}
         '''
         result = self._values.get("gzip")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def part(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ConfigPart"]]]:
         '''part block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#part Config#part}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#part Config#part}
         '''
         result = self._values.get("part")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["ConfigPart"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -422,18 +424,18 @@
         *,
         content: builtins.str,
         content_type: typing.Optional[builtins.str] = None,
         filename: typing.Optional[builtins.str] = None,
         merge_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param content: Body content for the part. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#content Config#content}
-        :param content_type: A MIME-style content type to report in the header for the part. Defaults to ``text/plain``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#content_type Config#content_type}
-        :param filename: A filename to report in the header for the part. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#filename Config#filename}
-        :param merge_type: A value for the ``X-Merge-Type`` header of the part, to control `cloud-init merging behavior <https://cloudinit.readthedocs.io/en/latest/reference/merging.html>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#merge_type Config#merge_type}
+        :param content: Body content for the part. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#content Config#content}
+        :param content_type: A MIME-style content type to report in the header for the part. Defaults to ``text/plain``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#content_type Config#content_type}
+        :param filename: A filename to report in the header for the part. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#filename Config#filename}
+        :param merge_type: A value for the ``X-Merge-Type`` header of the part, to control `cloud-init merging behavior <https://cloudinit.readthedocs.io/en/latest/reference/merging.html>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#merge_type Config#merge_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3fca1fd9b19d9488a9f1e13ebfe26564a2653c20e9beb3184c76273e00c9b862)
             check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             check_type(argname="argument content_type", value=content_type, expected_type=type_hints["content_type"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
             check_type(argname="argument merge_type", value=merge_type, expected_type=type_hints["merge_type"])
@@ -447,43 +449,43 @@
         if merge_type is not None:
             self._values["merge_type"] = merge_type
 
     @builtins.property
     def content(self) -> builtins.str:
         '''Body content for the part.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#content Config#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#content Config#content}
         '''
         result = self._values.get("content")
         assert result is not None, "Required property 'content' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def content_type(self) -> typing.Optional[builtins.str]:
         '''A MIME-style content type to report in the header for the part. Defaults to ``text/plain``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#content_type Config#content_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#content_type Config#content_type}
         '''
         result = self._values.get("content_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def filename(self) -> typing.Optional[builtins.str]:
         '''A filename to report in the header for the part.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#filename Config#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#filename Config#filename}
         '''
         result = self._values.get("filename")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def merge_type(self) -> typing.Optional[builtins.str]:
         '''A value for the ``X-Merge-Type`` header of the part, to control `cloud-init merging behavior <https://cloudinit.readthedocs.io/en/latest/reference/merging.html>`_.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/r/config#merge_type Config#merge_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/resources/config#merge_type Config#merge_type}
         '''
         result = self._values.get("merge_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -725,15 +727,15 @@
     id: builtins.str,
     *,
     base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     boundary: typing.Optional[builtins.str] = None,
     gzip: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     part: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[ConfigPart, typing.Dict[builtins.str, typing.Any]]]]] = None,
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
@@ -762,15 +764,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__b6518f0322408809a87b0713f41a8eb39e8f2aeeb04828147592a0138bd68c13(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     boundary: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py` & `cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_cloudinit_config`
 
-Refer to the Terraform Registory for docs: [`data_cloudinit_config`](https://www.terraform.io/docs/providers/cloudinit/d/config).
+Refer to the Terraform Registory for docs: [`data_cloudinit_config`](https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataCloudinitConfig(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-cloudinit.dataCloudinitConfig.DataCloudinitConfig",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/cloudinit/d/config cloudinit_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config cloudinit_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         boundary: typing.Optional[builtins.str] = None,
         gzip: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         part: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union["DataCloudinitConfigPart", typing.Dict[builtins.str, typing.Any]]]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/cloudinit/d/config cloudinit_config} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config cloudinit_config} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#base64_encode DataCloudinitConfig#base64_encode}
-        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#boundary DataCloudinitConfig#boundary}
-        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#gzip DataCloudinitConfig#gzip}
-        :param part: part block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#part DataCloudinitConfig#part}
+        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#base64_encode DataCloudinitConfig#base64_encode}
+        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#boundary DataCloudinitConfig#boundary}
+        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#gzip DataCloudinitConfig#gzip}
+        :param part: part block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#part DataCloudinitConfig#part}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -221,15 +221,15 @@
     },
 )
 class DataCloudinitConfigConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         boundary: typing.Optional[builtins.str] = None,
@@ -240,18 +240,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#base64_encode DataCloudinitConfig#base64_encode}
-        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#boundary DataCloudinitConfig#boundary}
-        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#gzip DataCloudinitConfig#gzip}
-        :param part: part block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#part DataCloudinitConfig#part}
+        :param base64_encode: Specify whether or not to base64 encode the ``rendered`` output. Defaults to ``true``, and cannot be disabled if gzip is ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#base64_encode DataCloudinitConfig#base64_encode}
+        :param boundary: Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#boundary DataCloudinitConfig#boundary}
+        :param gzip: Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#gzip DataCloudinitConfig#gzip}
+        :param part: part block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#part DataCloudinitConfig#part}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__efaaac9d450e4a06aa8939d9f4c75b399518eebda45480835cd3721f6db15620)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -295,20 +295,22 @@
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
@@ -354,46 +356,46 @@
     def base64_encode(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specify whether or not to base64 encode the ``rendered`` output.
 
         Defaults to ``true``, and cannot be disabled if gzip is ``true``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#base64_encode DataCloudinitConfig#base64_encode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#base64_encode DataCloudinitConfig#base64_encode}
         '''
         result = self._values.get("base64_encode")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def boundary(self) -> typing.Optional[builtins.str]:
         '''Specify the Writer's default boundary separator. Defaults to ``MIMEBOUNDARY``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#boundary DataCloudinitConfig#boundary}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#boundary DataCloudinitConfig#boundary}
         '''
         result = self._values.get("boundary")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def gzip(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Specify whether or not to gzip the ``rendered`` output. Defaults to ``true``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#gzip DataCloudinitConfig#gzip}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#gzip DataCloudinitConfig#gzip}
         '''
         result = self._values.get("gzip")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def part(
         self,
     ) -> typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataCloudinitConfigPart"]]]:
         '''part block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#part DataCloudinitConfig#part}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#part DataCloudinitConfig#part}
         '''
         result = self._values.get("part")
         return typing.cast(typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.List["DataCloudinitConfigPart"]]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -422,18 +424,18 @@
         *,
         content: builtins.str,
         content_type: typing.Optional[builtins.str] = None,
         filename: typing.Optional[builtins.str] = None,
         merge_type: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param content: Body content for the part. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#content DataCloudinitConfig#content}
-        :param content_type: A MIME-style content type to report in the header for the part. Defaults to ``text/plain``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#content_type DataCloudinitConfig#content_type}
-        :param filename: A filename to report in the header for the part. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#filename DataCloudinitConfig#filename}
-        :param merge_type: A value for the ``X-Merge-Type`` header of the part, to control `cloud-init merging behavior <https://cloudinit.readthedocs.io/en/latest/reference/merging.html>`_. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#merge_type DataCloudinitConfig#merge_type}
+        :param content: Body content for the part. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#content DataCloudinitConfig#content}
+        :param content_type: A MIME-style content type to report in the header for the part. Defaults to ``text/plain``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#content_type DataCloudinitConfig#content_type}
+        :param filename: A filename to report in the header for the part. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#filename DataCloudinitConfig#filename}
+        :param merge_type: A value for the ``X-Merge-Type`` header of the part, to control `cloud-init merging behavior <https://cloudinit.readthedocs.io/en/latest/reference/merging.html>`_. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#merge_type DataCloudinitConfig#merge_type}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dea5c45b8e764d44009d8dd7b67f37257ed52656524d9c5100424d963623134a)
             check_type(argname="argument content", value=content, expected_type=type_hints["content"])
             check_type(argname="argument content_type", value=content_type, expected_type=type_hints["content_type"])
             check_type(argname="argument filename", value=filename, expected_type=type_hints["filename"])
             check_type(argname="argument merge_type", value=merge_type, expected_type=type_hints["merge_type"])
@@ -447,43 +449,43 @@
         if merge_type is not None:
             self._values["merge_type"] = merge_type
 
     @builtins.property
     def content(self) -> builtins.str:
         '''Body content for the part.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#content DataCloudinitConfig#content}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#content DataCloudinitConfig#content}
         '''
         result = self._values.get("content")
         assert result is not None, "Required property 'content' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def content_type(self) -> typing.Optional[builtins.str]:
         '''A MIME-style content type to report in the header for the part. Defaults to ``text/plain``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#content_type DataCloudinitConfig#content_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#content_type DataCloudinitConfig#content_type}
         '''
         result = self._values.get("content_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def filename(self) -> typing.Optional[builtins.str]:
         '''A filename to report in the header for the part.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#filename DataCloudinitConfig#filename}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#filename DataCloudinitConfig#filename}
         '''
         result = self._values.get("filename")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def merge_type(self) -> typing.Optional[builtins.str]:
         '''A value for the ``X-Merge-Type`` header of the part, to control `cloud-init merging behavior <https://cloudinit.readthedocs.io/en/latest/reference/merging.html>`_.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit/d/config#merge_type DataCloudinitConfig#merge_type}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs/data-sources/config#merge_type DataCloudinitConfig#merge_type}
         '''
         result = self._values.get("merge_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -725,15 +727,15 @@
     id: builtins.str,
     *,
     base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     boundary: typing.Optional[builtins.str] = None,
     gzip: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     part: typing.Optional[typing.Union[_cdktf_9a9027ec.IResolvable, typing.Sequence[typing.Union[DataCloudinitConfigPart, typing.Dict[builtins.str, typing.Any]]]]] = None,
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
@@ -762,15 +764,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__efaaac9d450e4a06aa8939d9f4c75b399518eebda45480835cd3721f6db15620(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     base64_encode: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     boundary: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py` & `cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit/provider/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`cloudinit`](https://www.terraform.io/docs/providers/cloudinit).
+Refer to the Terraform Registory for docs: [`cloudinit`](https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class CloudinitProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-cloudinit.provider.CloudinitProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/cloudinit cloudinit}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs cloudinit}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/cloudinit cloudinit} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs cloudinit} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit#alias CloudinitProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs#alias CloudinitProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e65a5f1a69abda797cb40efc9f614a0c93e86ed6ee8f37e99f7897263ba39d1e)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = CloudinitProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-cloudinit.provider.CloudinitProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class CloudinitProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit#alias CloudinitProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs#alias CloudinitProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9334b1e49a7a41a60e3916e16f4a16677b832ce861e824ed7a32eaa7fb84f490)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/cloudinit#alias CloudinitProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/cloudinit/2.3.2/docs#alias CloudinitProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO` & `cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-cloudinit
-Version: 5.0.1
+Version: 6.0.0
 Summary: Prebuilt cloudinit Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-cloudinit.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-cloudinit.git
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
```

### Comparing `cdktf-cdktf-provider-cloudinit-5.0.1/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-cloudinit-6.0.0/src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 src/cdktf_cdktf_provider_cloudinit/py.typed
 src/cdktf_cdktf_provider_cloudinit.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_cloudinit.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_cloudinit.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_cloudinit.egg-info/requires.txt
 src/cdktf_cdktf_provider_cloudinit.egg-info/top_level.txt
 src/cdktf_cdktf_provider_cloudinit/_jsii/__init__.py
-src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@5.0.1.jsii.tgz
+src/cdktf_cdktf_provider_cloudinit/_jsii/provider-cloudinit@6.0.0.jsii.tgz
 src/cdktf_cdktf_provider_cloudinit/config/__init__.py
 src/cdktf_cdktf_provider_cloudinit/data_cloudinit_config/__init__.py
 src/cdktf_cdktf_provider_cloudinit/provider/__init__.py
```

