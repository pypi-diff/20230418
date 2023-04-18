# Comparing `tmp/cdk8s-operator-0.1.87.tar.gz` & `tmp/cdk8s-operator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-operator-0.1.87.tar", last modified: Tue Apr 18 21:25:27 2023, max compression
+gzip compressed data, was "cdk8s-operator-0.1.9.tar", last modified: Thu Aug  4 00:34:36 2022, max compression
```

## Comparing `cdk8s-operator-0.1.87.tar` & `cdk8s-operator-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5387 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:27.100269 cdk8s-operator-0.1.87/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/src/cdk8s_operator/
--rw-r--r--   0 runner    (1001) docker     (123)    18320 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/src/cdk8s_operator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/src/cdk8s_operator/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/src/cdk8s_operator/_jsii/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/src/cdk8s_operator/_jsii/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/src/cdk8s_operator/_jsii/bin/cdk8s-server
--rw-r--r--   0 runner    (1001) docker     (123)   123581 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.87.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:25:15.000000 cdk8s-operator-0.1.87/src/cdk8s_operator/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:25:27.104270 cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-04-18 21:25:27.000000 cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-04-18 21:25:27.000000 cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:25:27.000000 cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 21:25:27.000000 cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 21:25:27.000000 cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6310 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1798 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 00:34:36.665989 cdk8s-operator-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/src/cdk8s_operator/
+-rw-r--r--   0 runner    (1001) docker     (121)    16787 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/src/cdk8s_operator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/src/cdk8s_operator/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (121)      393 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/src/cdk8s_operator/_jsii/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/src/cdk8s_operator/_jsii/bin/
+-rw-r--r--   0 runner    (1001) docker     (121)      257 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/src/cdk8s_operator/_jsii/bin/cdk8s-server
+-rw-r--r--   0 runner    (1001) docker     (121)   124248 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/src/cdk8s_operator/_jsii/cdk8s-operator@0.1.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 00:34:21.000000 cdk8s-operator-0.1.9/src/cdk8s_operator/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-04 00:34:36.669989 cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6310 2022-08-04 00:34:35.000000 cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-08-04 00:34:36.000000 cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-04 00:34:36.000000 cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-04 00:34:36.000000 cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-04 00:34:36.000000 cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/top_level.txt
```

### Comparing `cdk8s-operator-0.1.87/LICENSE` & `cdk8s-operator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.87/PKG-INFO` & `cdk8s-operator-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.87
+Version: 0.1.9
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
-Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
+Home-page: https://github.com/eladb/cdk8s-pack-prototype.git
 Author: Amazon Web Services
 License: Apache-2.0
-Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
+Project-URL: Source, https://github.com/eladb/cdk8s-pack-prototype.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -272,7 +272,9 @@
 $ curl -d @input.json http://localhost:8080
 MANIFEST...
 ```
 
 ## License
 
 Apache 2.0
+
+
```

### Comparing `cdk8s-operator-0.1.87/README.md` & `cdk8s-operator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-operator-0.1.87/setup.py` & `cdk8s-operator-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,58 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-operator",
-    "version": "0.1.87",
+    "version": "0.1.9",
     "description": "Create Kubernetes CRD Operators using CDK8s Constructs",
     "license": "Apache-2.0",
-    "url": "https://github.com/cdk8s-team/cdk8s-operator.git",
+    "url": "https://github.com/eladb/cdk8s-pack-prototype.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
-        "Source": "https://github.com/cdk8s-team/cdk8s-operator.git"
+        "Source": "https://github.com/eladb/cdk8s-pack-prototype.git"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "cdk8s_operator",
         "cdk8s_operator._jsii"
     ],
     "package_data": {
         "cdk8s_operator._jsii": [
-            "cdk8s-operator@0.1.87.jsii.tgz"
+            "cdk8s-operator@0.1.9.jsii.tgz"
         ],
         "cdk8s_operator": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdk8s>=2.7.55, <3.0.0",
+        "cdk8s>=2.3.74, <3.0.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.63.2, <2.0.0",
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
-        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": [
         "src/cdk8s_operator/_jsii/bin/cdk8s-server"
     ]
```

### Comparing `cdk8s-operator-0.1.87/src/cdk8s_operator/__init__.py` & `cdk8s-operator-0.1.9/src/cdk8s_operator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -264,16 +264,16 @@
 import publication
 import typing_extensions
 
 from typeguard import check_type
 
 from ._jsii import *
 
-import cdk8s as _cdk8s_d3d9af27
-import constructs as _constructs_77d1e7e8
+import cdk8s
+import constructs
 
 
 @jsii.data_type(
     jsii_type="cdk8s-operator.CustomResourceProvider",
     jsii_struct_bases=[],
     name_mapping={"api_version": "apiVersion", "handler": "handler", "kind": "kind"},
 )
@@ -287,19 +287,19 @@
     ) -> None:
         '''
         :param api_version: API version of the custom resource. Default: "v1"
         :param handler: The construct handler.
         :param kind: Kind of this custom resource.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__63bd57a14e8e614c52758046c35e30c05a339d75a654cc92443e130cfb5ccbdc)
+            type_hints = typing.get_type_hints(CustomResourceProvider.__init__)
             check_type(argname="argument api_version", value=api_version, expected_type=type_hints["api_version"])
             check_type(argname="argument handler", value=handler, expected_type=type_hints["handler"])
             check_type(argname="argument kind", value=kind, expected_type=type_hints["kind"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "api_version": api_version,
             "handler": handler,
             "kind": kind,
         }
 
     @builtins.property
     def api_version(self) -> builtins.str:
@@ -340,18 +340,18 @@
 @jsii.interface(jsii_type="cdk8s-operator.ICustomResourceProviderHandler")
 class ICustomResourceProviderHandler(typing_extensions.Protocol):
     '''The handler for this custom resource provider.'''
 
     @jsii.member(jsii_name="apply")
     def apply(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         spec: typing.Any,
-    ) -> _constructs_77d1e7e8.Construct:
+    ) -> constructs.Construct:
         '''
         :param scope: -
         :param id: -
         :param spec: -
         '''
         ...
 
@@ -360,39 +360,35 @@
     '''The handler for this custom resource provider.'''
 
     __jsii_type__: typing.ClassVar[str] = "cdk8s-operator.ICustomResourceProviderHandler"
 
     @jsii.member(jsii_name="apply")
     def apply(
         self,
-        scope: _constructs_77d1e7e8.Construct,
+        scope: constructs.Construct,
         id: builtins.str,
         spec: typing.Any,
-    ) -> _constructs_77d1e7e8.Construct:
+    ) -> constructs.Construct:
         '''
         :param scope: -
         :param id: -
         :param spec: -
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__6ceb167d79d8aecac66e191906cc74b1ab75e0141b457629d880751a5a42735b)
+            type_hints = typing.get_type_hints(ICustomResourceProviderHandler.apply)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
             check_type(argname="argument spec", value=spec, expected_type=type_hints["spec"])
-        return typing.cast(_constructs_77d1e7e8.Construct, jsii.invoke(self, "apply", [scope, id, spec]))
+        return typing.cast(constructs.Construct, jsii.invoke(self, "apply", [scope, id, spec]))
 
 # Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
 typing.cast(typing.Any, ICustomResourceProviderHandler).__jsii_proxy_class__ = lambda : _ICustomResourceProviderHandlerProxy
 
 
-class Operator(
-    _cdk8s_d3d9af27.App,
-    metaclass=jsii.JSIIMeta,
-    jsii_type="cdk8s-operator.Operator",
-):
+class Operator(cdk8s.App, metaclass=jsii.JSIIMeta, jsii_type="cdk8s-operator.Operator"):
     '''A CDK8s app which allows implementing Kubernetes operators using CDK8s constructs.'''
 
     def __init__(
         self,
         *,
         input_file: typing.Optional[builtins.str] = None,
         output_file: typing.Optional[builtins.str] = None,
@@ -452,18 +448,18 @@
         output_file: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param input_file: A Kubernetes JSON manifest with a single resource that is matched against one of the providers within this operator. Default: - first position command-line argument or "/dev/stdin"
         :param output_file: Where to write the synthesized output. Default: "/dev/stdout"
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__0a3bf04ab8b6ddadebc84ec5dd2ffb000fdee8d372c0d96b617bcbee11d50da3)
+            type_hints = typing.get_type_hints(OperatorProps.__init__)
             check_type(argname="argument input_file", value=input_file, expected_type=type_hints["input_file"])
             check_type(argname="argument output_file", value=output_file, expected_type=type_hints["output_file"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        self._values: typing.Dict[str, typing.Any] = {}
         if input_file is not None:
             self._values["input_file"] = input_file
         if output_file is not None:
             self._values["output_file"] = output_file
 
     @builtins.property
     def input_file(self) -> typing.Optional[builtins.str]:
@@ -512,15 +508,15 @@
     @jsii.member(jsii_name="listen")
     def listen(self, port: typing.Optional[jsii.Number] = None) -> jsii.Number:
         '''Starts HTTP server.
 
         :param port: The port to listen to. If not specified, the ``PORT`` environment variable will be used. If that's not specified an available port will be auto-selected.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__5f3d6766c69f77f090730ffbc89a6aaabaa54a16a0b1c9d42b8794041ab3db9b)
+            type_hints = typing.get_type_hints(Server.listen)
             check_type(argname="argument port", value=port, expected_type=type_hints["port"])
         return typing.cast(jsii.Number, jsii.ainvoke(self, "listen", [port]))
 
 
 @jsii.data_type(
     jsii_type="cdk8s-operator.ServerProps",
     jsii_struct_bases=[],
@@ -528,17 +524,17 @@
 )
 class ServerProps:
     def __init__(self, *, app_command: builtins.str) -> None:
         '''
         :param app_command: The command to execute in order to synthesize the CDK app.
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__4f1178d58de56b9f0c47904f9ac8087bd2a728fad1032db0aeaf104b854f42d6)
+            type_hints = typing.get_type_hints(ServerProps.__init__)
             check_type(argname="argument app_command", value=app_command, expected_type=type_hints["app_command"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
+        self._values: typing.Dict[str, typing.Any] = {
             "app_command": app_command,
         }
 
     @builtins.property
     def app_command(self) -> builtins.str:
         '''The command to execute in order to synthesize the CDK app.'''
         result = self._values.get("app_command")
@@ -563,45 +559,7 @@
     "Operator",
     "OperatorProps",
     "Server",
     "ServerProps",
 ]
 
 publication.publish()
-
-def _typecheckingstub__63bd57a14e8e614c52758046c35e30c05a339d75a654cc92443e130cfb5ccbdc(
-    *,
-    api_version: builtins.str,
-    handler: ICustomResourceProviderHandler,
-    kind: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__6ceb167d79d8aecac66e191906cc74b1ab75e0141b457629d880751a5a42735b(
-    scope: _constructs_77d1e7e8.Construct,
-    id: builtins.str,
-    spec: typing.Any,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__0a3bf04ab8b6ddadebc84ec5dd2ffb000fdee8d372c0d96b617bcbee11d50da3(
-    *,
-    input_file: typing.Optional[builtins.str] = None,
-    output_file: typing.Optional[builtins.str] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__5f3d6766c69f77f090730ffbc89a6aaabaa54a16a0b1c9d42b8794041ab3db9b(
-    port: typing.Optional[jsii.Number] = None,
-) -> None:
-    """Type checking stubs"""
-    pass
-
-def _typecheckingstub__4f1178d58de56b9f0c47904f9ac8087bd2a728fad1032db0aeaf104b854f42d6(
-    *,
-    app_command: builtins.str,
-) -> None:
-    """Type checking stubs"""
-    pass
```

### Comparing `cdk8s-operator-0.1.87/src/cdk8s_operator.egg-info/PKG-INFO` & `cdk8s-operator-0.1.9/src/cdk8s_operator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk8s-operator
-Version: 0.1.87
+Version: 0.1.9
 Summary: Create Kubernetes CRD Operators using CDK8s Constructs
-Home-page: https://github.com/cdk8s-team/cdk8s-operator.git
+Home-page: https://github.com/eladb/cdk8s-pack-prototype.git
 Author: Amazon Web Services
 License: Apache-2.0
-Project-URL: Source, https://github.com/cdk8s-team/cdk8s-operator.git
+Project-URL: Source, https://github.com/eladb/cdk8s-pack-prototype.git
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -272,7 +272,9 @@
 $ curl -d @input.json http://localhost:8080
 MANIFEST...
 ```
 
 ## License
 
 Apache 2.0
+
+
```

