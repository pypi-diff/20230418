# Comparing `tmp/aws-ddk-core-1.0.0b0.tar.gz` & `tmp/aws-ddk-core-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ddk-core-1.0.0b0.tar", last modified: Fri Mar 31 17:45:07 2023, max compression
+gzip compressed data, was "aws-ddk-core-1.0.0b1.tar", last modified: Mon Apr 17 23:35:42 2023, max compression
```

## Comparing `aws-ddk-core-1.0.0b0.tar` & `aws-ddk-core-1.0.0b1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-03-31 17:45:07.091531 aws-ddk-core-1.0.0b0/
--rw-r--r--   0 hansonlu (569507325) 1896053708    11358 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/LICENSE
--rw-r--r--   0 hansonlu (569507325) 1896053708       23 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/MANIFEST.in
--rw-r--r--   0 hansonlu (569507325) 1896053708       67 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/NOTICE
--rw-r--r--   0 hansonlu (569507325) 1896053708     8819 2023-03-31 17:45:07.091102 aws-ddk-core-1.0.0b0/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) 1896053708     7891 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/README.md
--rw-r--r--   0 hansonlu (569507325) 1896053708      236 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/pyproject.toml
--rw-r--r--   0 hansonlu (569507325) 1896053708       38 2023-03-31 17:45:07.091646 aws-ddk-core-1.0.0b0/setup.cfg
--rw-r--r--   0 hansonlu (569507325) 1896053708     1979 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/setup.py
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-03-31 17:45:07.082503 aws-ddk-core-1.0.0b0/src/
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-03-31 17:45:07.086591 aws-ddk-core-1.0.0b0/src/aws_ddk_core/
--rw-r--r--   0 hansonlu (569507325) 1896053708   430142 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core/__init__.py
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-03-31 17:45:07.089423 aws-ddk-core-1.0.0b0/src/aws_ddk_core/_jsii/
--rw-r--r--   0 hansonlu (569507325) 1896053708      600 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core/_jsii/__init__.py
--rw-r--r--   0 hansonlu (569507325) 1896053708   838894 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.0-beta.0.jsii.tgz
--rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-03-31 17:44:51.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core/py.typed
-drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-03-31 17:45:07.088590 aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/
--rw-r--r--   0 hansonlu (569507325) 1896053708     8819 2023-03-31 17:45:06.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) 1896053708      407 2023-03-31 17:45:07.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/SOURCES.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-03-31 17:45:06.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/dependency_links.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708      313 2023-03-31 17:45:06.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/requires.txt
--rw-r--r--   0 hansonlu (569507325) 1896053708       13 2023-03-31 17:45:06.000000 aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/top_level.txt
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.045497 aws-ddk-core-1.0.0b1/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)    11358 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/LICENSE
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       23 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/MANIFEST.in
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       67 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/NOTICE
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     8819 2023-04-17 23:35:42.045054 aws-ddk-core-1.0.0b1/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     7891 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/README.md
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      236 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/pyproject.toml
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       38 2023-04-17 23:35:42.045613 aws-ddk-core-1.0.0b1/setup.cfg
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     1979 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/setup.py
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.036244 aws-ddk-core-1.0.0b1/src/
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.040506 aws-ddk-core-1.0.0b1/src/aws_ddk_core/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)   474193 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/__init__.py
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.043344 aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      600 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/__init__.py
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)   850443 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.0-beta.1.jsii.tgz
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-04-17 23:35:27.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core/py.typed
+drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-04-17 23:35:42.042548 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     8819 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      407 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      313 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/requires.txt
+-rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       13 2023-04-17 23:35:41.000000 aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/top_level.txt
```

### Comparing `aws-ddk-core-1.0.0b0/LICENSE` & `aws-ddk-core-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.0.0b0/PKG-INFO` & `aws-ddk-core-1.0.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: AWS DataOps Development Kit
 Home-page: https://github.com/awslabs/aws-ddk
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-ddk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

### Comparing `aws-ddk-core-1.0.0b0/README.md` & `aws-ddk-core-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.0.0b0/setup.py` & `aws-ddk-core-1.0.0b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ddk-core",
-    "version": "1.0.0.b0",
+    "version": "1.0.0.b1",
     "description": "AWS DataOps Development Kit",
     "license": "Apache-2.0",
     "url": "https://github.com/awslabs/aws-ddk",
     "long_description_content_type": "text/markdown",
     "author": "AWS Professional Services<aws-proserve-orion-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "aws_ddk_core",
         "aws_ddk_core._jsii"
     ],
     "package_data": {
         "aws_ddk_core._jsii": [
-            "aws-ddk-core@1.0.0-beta.0.jsii.tgz"
+            "aws-ddk-core@1.0.0-beta.1.jsii.tgz"
         ],
         "aws_ddk_core": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `aws-ddk-core-1.0.0b0/src/aws_ddk_core/__init__.py` & `aws-ddk-core-1.0.0b1/src/aws_ddk_core/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1021,15 +1021,15 @@
     jsii_type="aws-ddk-core.BaseStack",
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
-        config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+        config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
@@ -1071,14 +1071,42 @@
             synthesizer=synthesizer,
             tags=tags,
             termination_protection=termination_protection,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
+    @jsii.member(jsii_name="createDefaultPermissionsBoundary")
+    @builtins.classmethod
+    def create_default_permissions_boundary(
+        cls,
+        scope: _constructs_77d1e7e8.Construct,
+        id: builtins.str,
+        *,
+        environment_id: typing.Optional[builtins.str] = None,
+        prefix: typing.Optional[builtins.str] = None,
+        qualifier: typing.Optional[builtins.str] = None,
+    ) -> _aws_cdk_aws_iam_ceddda9d.IManagedPolicy:
+        '''
+        :param scope: -
+        :param id: -
+        :param environment_id: 
+        :param prefix: 
+        :param qualifier: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c52c78b6e97cce4b370cb75d9552fff81495ba02218c70f1c8947488c2c0604a)
+            check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
+            check_type(argname="argument id", value=id, expected_type=type_hints["id"])
+        props = PermissionsBoundaryProps(
+            environment_id=environment_id, prefix=prefix, qualifier=qualifier
+        )
+
+        return typing.cast(_aws_cdk_aws_iam_ceddda9d.IManagedPolicy, jsii.sinvoke(cls, "createDefaultPermissionsBoundary", [scope, id, props]))
+
     @builtins.property
     @jsii.member(jsii_name="terminationProtection")
     def termination_protection(self) -> typing.Optional[builtins.bool]:
         '''Whether termination protection is enabled for this stack.'''
         return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "terminationProtection"))
 
 
@@ -1109,15 +1137,15 @@
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
-        config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+        config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
         :param cross_region_references: Enable this flag to allow native cross region stack references. Enabling this will create a CloudFormation custom resource in both the producing stack and consuming stack in order to perform the export/import This feature is currently experimental Default: false
         :param description: A description of the stack. Default: - No description.
@@ -1332,19 +1360,17 @@
 
         :default: false
         '''
         result = self._values.get("termination_protection")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def config(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]]:
+    def config(self) -> typing.Optional[typing.Union[builtins.str, "Configuration"]]:
         result = self._values.get("config")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, "Configuration"]], result)
 
     @builtins.property
     def environment_id(self) -> typing.Optional[builtins.str]:
         result = self._values.get("environment_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
@@ -1537,15 +1563,15 @@
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         cdk_language: typing.Optional[builtins.str] = None,
         pipeline_name: typing.Optional[builtins.str] = None,
-        config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+        config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         analytics_reporting: typing.Optional[builtins.bool] = None,
         cross_region_references: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
@@ -1943,15 +1969,15 @@
         description: typing.Optional[builtins.str] = None,
         env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
         permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
         stack_name: typing.Optional[builtins.str] = None,
         synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         termination_protection: typing.Optional[builtins.bool] = None,
-        config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+        config: typing.Optional[typing.Union[builtins.str, typing.Union["Configuration", typing.Dict[builtins.str, typing.Any]]]] = None,
         environment_id: typing.Optional[builtins.str] = None,
         permissions_boundary_arn: typing.Optional[builtins.str] = None,
         cdk_language: typing.Optional[builtins.str] = None,
         pipeline_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param analytics_reporting: Include runtime versioning information in this Stack. Default: ``analyticsReporting`` setting of containing ``App``, or value of 'aws:cdk:version-reporting' context key
@@ -2176,19 +2202,17 @@
 
         :default: false
         '''
         result = self._values.get("termination_protection")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    def config(
-        self,
-    ) -> typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]]:
+    def config(self) -> typing.Optional[typing.Union[builtins.str, "Configuration"]]:
         result = self._values.get("config")
-        return typing.cast(typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]], result)
+        return typing.cast(typing.Optional[typing.Union[builtins.str, "Configuration"]], result)
 
     @builtins.property
     def environment_id(self) -> typing.Optional[builtins.str]:
         result = self._values.get("environment_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
@@ -2403,19 +2427,115 @@
 
     def __repr__(self) -> str:
         return "CodeCommitSourceActionProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="aws-ddk-core.Configuration",
+    jsii_struct_bases=[],
+    name_mapping={
+        "environments": "environments",
+        "account": "account",
+        "bootstrap": "bootstrap",
+        "ddk_bootstrap_config_key": "ddkBootstrapConfigKey",
+        "region": "region",
+        "tags": "tags",
+    },
+)
+class Configuration:
+    def __init__(
+        self,
+        *,
+        environments: typing.Mapping[builtins.str, typing.Union["EnvironmentConfiguration", typing.Dict[builtins.str, typing.Any]]],
+        account: typing.Optional[builtins.str] = None,
+        bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        ddk_bootstrap_config_key: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+        tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    ) -> None:
+        '''
+        :param environments: 
+        :param account: 
+        :param bootstrap: 
+        :param ddk_bootstrap_config_key: 
+        :param region: 
+        :param tags: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__daeed9e6cb5e50c39b922933d297c173f25183423bf700dfd9f8b0fe3765c923)
+            check_type(argname="argument environments", value=environments, expected_type=type_hints["environments"])
+            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
+            check_type(argname="argument bootstrap", value=bootstrap, expected_type=type_hints["bootstrap"])
+            check_type(argname="argument ddk_bootstrap_config_key", value=ddk_bootstrap_config_key, expected_type=type_hints["ddk_bootstrap_config_key"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "environments": environments,
+        }
+        if account is not None:
+            self._values["account"] = account
+        if bootstrap is not None:
+            self._values["bootstrap"] = bootstrap
+        if ddk_bootstrap_config_key is not None:
+            self._values["ddk_bootstrap_config_key"] = ddk_bootstrap_config_key
+        if region is not None:
+            self._values["region"] = region
+        if tags is not None:
+            self._values["tags"] = tags
+
+    @builtins.property
+    def environments(self) -> typing.Mapping[builtins.str, "EnvironmentConfiguration"]:
+        result = self._values.get("environments")
+        assert result is not None, "Required property 'environments' is missing"
+        return typing.cast(typing.Mapping[builtins.str, "EnvironmentConfiguration"], result)
+
+    @builtins.property
+    def account(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("account")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def bootstrap(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("bootstrap")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def ddk_bootstrap_config_key(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("ddk_bootstrap_config_key")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def region(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("region")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "Configuration(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class Configurator(metaclass=jsii.JSIIMeta, jsii_type="aws-ddk-core.Configurator"):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
-        config: typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]],
+        config: typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]],
         environment_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param config: -
         :param environment_id: -
         '''
@@ -2429,24 +2549,58 @@
     @jsii.member(jsii_name="getEnvConfig")
     @builtins.classmethod
     def get_env_config(
         cls,
         *,
         config_path: builtins.str,
         environment_id: builtins.str,
-    ) -> typing.Any:
+    ) -> "EnvironmentConfiguration":
         '''
         :param config_path: 
         :param environment_id: 
         '''
         props = GetEnvConfigProps(
             config_path=config_path, environment_id=environment_id
         )
 
-        return typing.cast(typing.Any, jsii.sinvoke(cls, "getEnvConfig", [props]))
+        return typing.cast("EnvironmentConfiguration", jsii.sinvoke(cls, "getEnvConfig", [props]))
+
+    @jsii.member(jsii_name="getEnvironment")
+    @builtins.classmethod
+    def get_environment(
+        cls,
+        *,
+        config_path: builtins.str,
+        environment_id: typing.Optional[builtins.str] = None,
+    ) -> "EnvironmentResult":
+        '''
+        :param config_path: 
+        :param environment_id: 
+        '''
+        props = GetEnvironmentProps(
+            config_path=config_path, environment_id=environment_id
+        )
+
+        return typing.cast("EnvironmentResult", jsii.sinvoke(cls, "getEnvironment", [props]))
+
+    @jsii.member(jsii_name="getTags")
+    @builtins.classmethod
+    def get_tags(
+        cls,
+        *,
+        config_path: builtins.str,
+        environment_id: typing.Optional[builtins.str] = None,
+    ) -> typing.Mapping[builtins.str, builtins.str]:
+        '''
+        :param config_path: 
+        :param environment_id: 
+        '''
+        props = GetTagsProps(config_path=config_path, environment_id=environment_id)
+
+        return typing.cast(typing.Mapping[builtins.str, builtins.str], jsii.sinvoke(cls, "getTags", [props]))
 
     @jsii.member(jsii_name="getConfigAttribute")
     def get_config_attribute(self, attribute: builtins.str) -> typing.Any:
         '''
         :param attribute: -
         '''
         if __debug__:
@@ -2468,16 +2622,16 @@
             type_hints = typing.get_type_hints(_typecheckingstub__5ebebaeeabeb2e14afe10bb65476a72e653389f44163949f819c5b260fc48e7c)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
         return typing.cast(None, jsii.invoke(self, "tagConstruct", [scope, tags]))
 
     @builtins.property
     @jsii.member(jsii_name="config")
-    def config(self) -> typing.Any:
-        return typing.cast(typing.Any, jsii.get(self, "config"))
+    def config(self) -> Configuration:
+        return typing.cast(Configuration, jsii.get(self, "config"))
 
     @builtins.property
     @jsii.member(jsii_name="environmentId")
     def environment_id(self) -> typing.Optional[builtins.str]:
         return typing.cast(typing.Optional[builtins.str], jsii.get(self, "environmentId"))
 
 
@@ -2699,14 +2853,245 @@
     def __repr__(self) -> str:
         return "DataPipelineProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="aws-ddk-core.DeliveryStreamProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "delivery_stream_name": "deliveryStreamName",
+        "destinations": "destinations",
+        "encryption": "encryption",
+        "encryption_key": "encryptionKey",
+        "role": "role",
+        "source_stream": "sourceStream",
+    },
+)
+class DeliveryStreamProps:
+    def __init__(
+        self,
+        *,
+        delivery_stream_name: typing.Optional[builtins.str] = None,
+        destinations: typing.Optional[typing.Sequence[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]] = None,
+        encryption: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption] = None,
+        encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+        role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+        source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
+    ) -> None:
+        '''
+        :param delivery_stream_name: 
+        :param destinations: 
+        :param encryption: 
+        :param encryption_key: 
+        :param role: 
+        :param source_stream: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__ef7997fe1d9215e0814459fdbbb95740e62a7f0437cd0df0dcd43ac255b163e4)
+            check_type(argname="argument delivery_stream_name", value=delivery_stream_name, expected_type=type_hints["delivery_stream_name"])
+            check_type(argname="argument destinations", value=destinations, expected_type=type_hints["destinations"])
+            check_type(argname="argument encryption", value=encryption, expected_type=type_hints["encryption"])
+            check_type(argname="argument encryption_key", value=encryption_key, expected_type=type_hints["encryption_key"])
+            check_type(argname="argument role", value=role, expected_type=type_hints["role"])
+            check_type(argname="argument source_stream", value=source_stream, expected_type=type_hints["source_stream"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if delivery_stream_name is not None:
+            self._values["delivery_stream_name"] = delivery_stream_name
+        if destinations is not None:
+            self._values["destinations"] = destinations
+        if encryption is not None:
+            self._values["encryption"] = encryption
+        if encryption_key is not None:
+            self._values["encryption_key"] = encryption_key
+        if role is not None:
+            self._values["role"] = role
+        if source_stream is not None:
+            self._values["source_stream"] = source_stream
+
+    @builtins.property
+    def delivery_stream_name(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("delivery_stream_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def destinations(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]]:
+        result = self._values.get("destinations")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]], result)
+
+    @builtins.property
+    def encryption(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption]:
+        result = self._values.get("encryption")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption], result)
+
+    @builtins.property
+    def encryption_key(self) -> typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey]:
+        result = self._values.get("encryption_key")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey], result)
+
+    @builtins.property
+    def role(self) -> typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole]:
+        result = self._values.get("role")
+        return typing.cast(typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole], result)
+
+    @builtins.property
+    def source_stream(self) -> typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream]:
+        result = self._values.get("source_stream")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "DeliveryStreamProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="aws-ddk-core.EnvironmentConfiguration",
+    jsii_struct_bases=[],
+    name_mapping={
+        "account": "account",
+        "bootstrap": "bootstrap",
+        "region": "region",
+        "resources": "resources",
+        "tags": "tags",
+    },
+)
+class EnvironmentConfiguration:
+    def __init__(
+        self,
+        *,
+        account: typing.Optional[builtins.str] = None,
+        bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+        region: typing.Optional[builtins.str] = None,
+        resources: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+        tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    ) -> None:
+        '''
+        :param account: 
+        :param bootstrap: 
+        :param region: 
+        :param resources: 
+        :param tags: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__cf306c436463dcb56197f32e9c4793604595ef2ca8f42b2d72de058d5806870c)
+            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
+            check_type(argname="argument bootstrap", value=bootstrap, expected_type=type_hints["bootstrap"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+            check_type(argname="argument resources", value=resources, expected_type=type_hints["resources"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if account is not None:
+            self._values["account"] = account
+        if bootstrap is not None:
+            self._values["bootstrap"] = bootstrap
+        if region is not None:
+            self._values["region"] = region
+        if resources is not None:
+            self._values["resources"] = resources
+        if tags is not None:
+            self._values["tags"] = tags
+
+    @builtins.property
+    def account(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("account")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def bootstrap(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("bootstrap")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    @builtins.property
+    def region(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("region")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def resources(self) -> typing.Optional[typing.Mapping[builtins.str, typing.Any]]:
+        result = self._values.get("resources")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, typing.Any]], result)
+
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "EnvironmentConfiguration(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
+    jsii_type="aws-ddk-core.EnvironmentResult",
+    jsii_struct_bases=[],
+    name_mapping={"account": "account", "region": "region"},
+)
+class EnvironmentResult:
+    def __init__(
+        self,
+        *,
+        account: typing.Optional[builtins.str] = None,
+        region: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param account: 
+        :param region: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c2515674b45134976862352edd7f3a4f56dddd10e860df69a14d633b55dfe768)
+            check_type(argname="argument account", value=account, expected_type=type_hints["account"])
+            check_type(argname="argument region", value=region, expected_type=type_hints["region"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if account is not None:
+            self._values["account"] = account
+        if region is not None:
+            self._values["region"] = region
+
+    @builtins.property
+    def account(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("account")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def region(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("region")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "EnvironmentResult(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="aws-ddk-core.GetEnvConfigProps",
     jsii_struct_bases=[],
     name_mapping={"config_path": "configPath", "environment_id": "environmentId"},
 )
 class GetEnvConfigProps:
     def __init__(
         self,
@@ -2748,14 +3133,63 @@
     def __repr__(self) -> str:
         return "GetEnvConfigProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
+    jsii_type="aws-ddk-core.GetEnvironmentProps",
+    jsii_struct_bases=[],
+    name_mapping={"config_path": "configPath", "environment_id": "environmentId"},
+)
+class GetEnvironmentProps:
+    def __init__(
+        self,
+        *,
+        config_path: builtins.str,
+        environment_id: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param config_path: 
+        :param environment_id: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f1d1864ebb63e794b66b601804d8a186ccc2fe70e5c1aeea9def8ecd1ab83dde)
+            check_type(argname="argument config_path", value=config_path, expected_type=type_hints["config_path"])
+            check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "config_path": config_path,
+        }
+        if environment_id is not None:
+            self._values["environment_id"] = environment_id
+
+    @builtins.property
+    def config_path(self) -> builtins.str:
+        result = self._values.get("config_path")
+        assert result is not None, "Required property 'config_path' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def environment_id(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("environment_id")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "GetEnvironmentProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
+@jsii.data_type(
     jsii_type="aws-ddk-core.GetSynthActionProps",
     jsii_struct_bases=[],
     name_mapping={
         "account": "account",
         "additional_install_commands": "additionalInstallCommands",
         "cdk_version": "cdkVersion",
         "codeartifact_domain": "codeartifactDomain",
@@ -2890,14 +3324,63 @@
 
     def __repr__(self) -> str:
         return "GetSynthActionProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
+@jsii.data_type(
+    jsii_type="aws-ddk-core.GetTagsProps",
+    jsii_struct_bases=[],
+    name_mapping={"config_path": "configPath", "environment_id": "environmentId"},
+)
+class GetTagsProps:
+    def __init__(
+        self,
+        *,
+        config_path: builtins.str,
+        environment_id: typing.Optional[builtins.str] = None,
+    ) -> None:
+        '''
+        :param config_path: 
+        :param environment_id: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__f80411a398b3a95cafcc083fedf809e35c9f9d3c872682fa20c2c416251da930)
+            check_type(argname="argument config_path", value=config_path, expected_type=type_hints["config_path"])
+            check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "config_path": config_path,
+        }
+        if environment_id is not None:
+            self._values["environment_id"] = environment_id
+
+    @builtins.property
+    def config_path(self) -> builtins.str:
+        result = self._values.get("config_path")
+        assert result is not None, "Required property 'config_path' is missing"
+        return typing.cast(builtins.str, result)
+
+    @builtins.property
+    def environment_id(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("environment_id")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
+
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
+
+    def __repr__(self) -> str:
+        return "GetTagsProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
+
+
 class GlueFactory(metaclass=jsii.JSIIMeta, jsii_type="aws-ddk-core.GlueFactory"):
     def __init__(self) -> None:
         jsii.create(self.__class__, self, [])
 
     @jsii.member(jsii_name="job")
     @builtins.classmethod
     def job(
@@ -4858,20 +5341,34 @@
         "additional_role_policy_statements": "additionalRolePolicyStatements",
         "alarms_enabled": "alarmsEnabled",
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "create_job": "createJob",
+        "database_outputs": "databaseOutputs",
+        "data_catalog_outputs": "dataCatalogOutputs",
         "dataset_name": "datasetName",
+        "encryption_key_arn": "encryptionKeyArn",
+        "encryption_mode": "encryptionMode",
         "job_name": "jobName",
         "job_role_arn": "jobRoleArn",
+        "job_sample": "jobSample",
         "job_type": "jobType",
+        "log_subscription": "logSubscription",
+        "max_capacity": "maxCapacity",
+        "max_retries": "maxRetries",
+        "output_location": "outputLocation",
         "outputs": "outputs",
+        "profile_configuration": "profileConfiguration",
+        "project_name": "projectName",
         "recipe": "recipe",
+        "tags": "tags",
+        "timeout": "timeout",
+        "validation_configurations": "validationConfigurations",
     },
 )
 class DataBrewTransformStageProps(StateMachineStageProps):
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
@@ -4879,57 +5376,105 @@
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         create_job: typing.Optional[builtins.bool] = None,
+        database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        data_catalog_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         dataset_name: typing.Optional[builtins.str] = None,
+        encryption_key_arn: typing.Optional[builtins.str] = None,
+        encryption_mode: typing.Optional[builtins.str] = None,
         job_name: typing.Optional[builtins.str] = None,
         job_role_arn: typing.Optional[builtins.str] = None,
+        job_sample: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         job_type: typing.Optional[builtins.str] = None,
+        log_subscription: typing.Optional[builtins.str] = None,
+        max_capacity: typing.Optional[jsii.Number] = None,
+        max_retries: typing.Optional[jsii.Number] = None,
+        output_location: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        profile_configuration: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+        project_name: typing.Optional[builtins.str] = None,
         recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+        timeout: typing.Optional[jsii.Number] = None,
+        validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     ) -> None:
         '''
         :param description: 
         :param name: 
         :param additional_role_policy_statements: 
         :param alarms_enabled: 
         :param state_machine_failed_executions_alarm_evaluation_periods: 
         :param state_machine_failed_executions_alarm_threshold: 
         :param state_machine_input: 
         :param state_machine_name: 
         :param create_job: 
+        :param database_outputs: 
+        :param data_catalog_outputs: 
         :param dataset_name: 
+        :param encryption_key_arn: 
+        :param encryption_mode: 
         :param job_name: 
         :param job_role_arn: 
+        :param job_sample: 
         :param job_type: 
+        :param log_subscription: 
+        :param max_capacity: 
+        :param max_retries: 
+        :param output_location: 
         :param outputs: 
+        :param profile_configuration: 
+        :param project_name: 
         :param recipe: 
+        :param tags: 
+        :param timeout: 
+        :param validation_configurations: 
         '''
+        if isinstance(job_sample, dict):
+            job_sample = _aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty(**job_sample)
+        if isinstance(output_location, dict):
+            output_location = _aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty(**output_location)
+        if isinstance(profile_configuration, dict):
+            profile_configuration = _aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty(**profile_configuration)
         if isinstance(recipe, dict):
             recipe = _aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty(**recipe)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f6be6b9ec4e805f427307a7bc1c743a3f56ffd52c0cc37a1436d75ce69e31b9f)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument create_job", value=create_job, expected_type=type_hints["create_job"])
+            check_type(argname="argument database_outputs", value=database_outputs, expected_type=type_hints["database_outputs"])
+            check_type(argname="argument data_catalog_outputs", value=data_catalog_outputs, expected_type=type_hints["data_catalog_outputs"])
             check_type(argname="argument dataset_name", value=dataset_name, expected_type=type_hints["dataset_name"])
+            check_type(argname="argument encryption_key_arn", value=encryption_key_arn, expected_type=type_hints["encryption_key_arn"])
+            check_type(argname="argument encryption_mode", value=encryption_mode, expected_type=type_hints["encryption_mode"])
             check_type(argname="argument job_name", value=job_name, expected_type=type_hints["job_name"])
             check_type(argname="argument job_role_arn", value=job_role_arn, expected_type=type_hints["job_role_arn"])
+            check_type(argname="argument job_sample", value=job_sample, expected_type=type_hints["job_sample"])
             check_type(argname="argument job_type", value=job_type, expected_type=type_hints["job_type"])
+            check_type(argname="argument log_subscription", value=log_subscription, expected_type=type_hints["log_subscription"])
+            check_type(argname="argument max_capacity", value=max_capacity, expected_type=type_hints["max_capacity"])
+            check_type(argname="argument max_retries", value=max_retries, expected_type=type_hints["max_retries"])
+            check_type(argname="argument output_location", value=output_location, expected_type=type_hints["output_location"])
             check_type(argname="argument outputs", value=outputs, expected_type=type_hints["outputs"])
+            check_type(argname="argument profile_configuration", value=profile_configuration, expected_type=type_hints["profile_configuration"])
+            check_type(argname="argument project_name", value=project_name, expected_type=type_hints["project_name"])
             check_type(argname="argument recipe", value=recipe, expected_type=type_hints["recipe"])
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument timeout", value=timeout, expected_type=type_hints["timeout"])
+            check_type(argname="argument validation_configurations", value=validation_configurations, expected_type=type_hints["validation_configurations"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
@@ -4941,26 +5486,54 @@
             self._values["state_machine_failed_executions_alarm_threshold"] = state_machine_failed_executions_alarm_threshold
         if state_machine_input is not None:
             self._values["state_machine_input"] = state_machine_input
         if state_machine_name is not None:
             self._values["state_machine_name"] = state_machine_name
         if create_job is not None:
             self._values["create_job"] = create_job
+        if database_outputs is not None:
+            self._values["database_outputs"] = database_outputs
+        if data_catalog_outputs is not None:
+            self._values["data_catalog_outputs"] = data_catalog_outputs
         if dataset_name is not None:
             self._values["dataset_name"] = dataset_name
+        if encryption_key_arn is not None:
+            self._values["encryption_key_arn"] = encryption_key_arn
+        if encryption_mode is not None:
+            self._values["encryption_mode"] = encryption_mode
         if job_name is not None:
             self._values["job_name"] = job_name
         if job_role_arn is not None:
             self._values["job_role_arn"] = job_role_arn
+        if job_sample is not None:
+            self._values["job_sample"] = job_sample
         if job_type is not None:
             self._values["job_type"] = job_type
+        if log_subscription is not None:
+            self._values["log_subscription"] = log_subscription
+        if max_capacity is not None:
+            self._values["max_capacity"] = max_capacity
+        if max_retries is not None:
+            self._values["max_retries"] = max_retries
+        if output_location is not None:
+            self._values["output_location"] = output_location
         if outputs is not None:
             self._values["outputs"] = outputs
+        if profile_configuration is not None:
+            self._values["profile_configuration"] = profile_configuration
+        if project_name is not None:
+            self._values["project_name"] = project_name
         if recipe is not None:
             self._values["recipe"] = recipe
+        if tags is not None:
+            self._values["tags"] = tags
+        if timeout is not None:
+            self._values["timeout"] = timeout
+        if validation_configurations is not None:
+            self._values["validation_configurations"] = validation_configurations
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
@@ -5008,47 +5581,129 @@
 
     @builtins.property
     def create_job(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("create_job")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
+    def database_outputs(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty]]:
+        result = self._values.get("database_outputs")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty]], result)
+
+    @builtins.property
+    def data_catalog_outputs(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty]]:
+        result = self._values.get("data_catalog_outputs")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty]], result)
+
+    @builtins.property
     def dataset_name(self) -> typing.Optional[builtins.str]:
         result = self._values.get("dataset_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def encryption_key_arn(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("encryption_key_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def encryption_mode(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("encryption_mode")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def job_name(self) -> typing.Optional[builtins.str]:
         result = self._values.get("job_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_role_arn(self) -> typing.Optional[builtins.str]:
         result = self._values.get("job_role_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def job_sample(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty]:
+        result = self._values.get("job_sample")
+        return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty], result)
+
+    @builtins.property
     def job_type(self) -> typing.Optional[builtins.str]:
         result = self._values.get("job_type")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def log_subscription(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("log_subscription")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def max_capacity(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("max_capacity")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def max_retries(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("max_retries")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def output_location(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty]:
+        result = self._values.get("output_location")
+        return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty], result)
+
+    @builtins.property
     def outputs(
         self,
     ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty]]:
         result = self._values.get("outputs")
         return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty]], result)
 
     @builtins.property
+    def profile_configuration(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty]:
+        result = self._values.get("profile_configuration")
+        return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty], result)
+
+    @builtins.property
+    def project_name(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("project_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def recipe(
         self,
     ) -> typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty]:
         result = self._values.get("recipe")
         return typing.cast(typing.Optional[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty], result)
 
+    @builtins.property
+    def tags(self) -> typing.Optional[typing.List[_aws_cdk_ceddda9d.CfnTag]]:
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_ceddda9d.CfnTag]], result)
+
+    @builtins.property
+    def timeout(self) -> typing.Optional[jsii.Number]:
+        result = self._values.get("timeout")
+        return typing.cast(typing.Optional[jsii.Number], result)
+
+    @builtins.property
+    def validation_configurations(
+        self,
+    ) -> typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty]]:
+        result = self._values.get("validation_configurations")
+        return typing.cast(typing.Optional[typing.List[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty]], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -5300,49 +5955,55 @@
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         data_output_prefix: typing.Optional[builtins.str] = None,
+        data_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream] = None,
         data_stream_enabled: typing.Optional[builtins.bool] = None,
         delivery_stream_data_freshness_errors_alarm_threshold: typing.Optional[jsii.Number] = None,
         delivery_stream_data_freshness_errors_evaluation_periods: typing.Optional[jsii.Number] = None,
-        firehose_delivery_stream_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        firehose_delivery_stream: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream] = None,
+        firehose_delivery_stream_props: typing.Optional[typing.Union[DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
         kinesis_firehose_destinations_s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
         s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param data_output_prefix: 
+        :param data_stream: 
         :param data_stream_enabled: 
         :param delivery_stream_data_freshness_errors_alarm_threshold: 
         :param delivery_stream_data_freshness_errors_evaluation_periods: 
+        :param firehose_delivery_stream: 
         :param firehose_delivery_stream_props: 
         :param kinesis_firehose_destinations_s3_bucket_props: 
         :param s3_bucket: 
         :param s3_bucket_props: 
         :param alarms_enabled: 
         :param description: 
         :param name: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__3f9217104050cf03ef7cf7519808ce659edfe6c1ba00722ea6601239921cfd56)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = FirehoseToS3StageProps(
             data_output_prefix=data_output_prefix,
+            data_stream=data_stream,
             data_stream_enabled=data_stream_enabled,
             delivery_stream_data_freshness_errors_alarm_threshold=delivery_stream_data_freshness_errors_alarm_threshold,
             delivery_stream_data_freshness_errors_evaluation_periods=delivery_stream_data_freshness_errors_evaluation_periods,
+            firehose_delivery_stream=firehose_delivery_stream,
             firehose_delivery_stream_props=firehose_delivery_stream_props,
             kinesis_firehose_destinations_s3_bucket_props=kinesis_firehose_destinations_s3_bucket_props,
             s3_bucket=s3_bucket,
             s3_bucket_props=s3_bucket_props,
             alarms_enabled=alarms_enabled,
             description=description,
             name=name,
@@ -5386,86 +6047,98 @@
     jsii_type="aws-ddk-core.FirehoseToS3StageProps",
     jsii_struct_bases=[DataStageProps],
     name_mapping={
         "description": "description",
         "name": "name",
         "alarms_enabled": "alarmsEnabled",
         "data_output_prefix": "dataOutputPrefix",
+        "data_stream": "dataStream",
         "data_stream_enabled": "dataStreamEnabled",
         "delivery_stream_data_freshness_errors_alarm_threshold": "deliveryStreamDataFreshnessErrorsAlarmThreshold",
         "delivery_stream_data_freshness_errors_evaluation_periods": "deliveryStreamDataFreshnessErrorsEvaluationPeriods",
+        "firehose_delivery_stream": "firehoseDeliveryStream",
         "firehose_delivery_stream_props": "firehoseDeliveryStreamProps",
         "kinesis_firehose_destinations_s3_bucket_props": "kinesisFirehoseDestinationsS3BucketProps",
         "s3_bucket": "s3Bucket",
         "s3_bucket_props": "s3BucketProps",
     },
 )
 class FirehoseToS3StageProps(DataStageProps):
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         data_output_prefix: typing.Optional[builtins.str] = None,
+        data_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream] = None,
         data_stream_enabled: typing.Optional[builtins.bool] = None,
         delivery_stream_data_freshness_errors_alarm_threshold: typing.Optional[jsii.Number] = None,
         delivery_stream_data_freshness_errors_evaluation_periods: typing.Optional[jsii.Number] = None,
-        firehose_delivery_stream_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        firehose_delivery_stream: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream] = None,
+        firehose_delivery_stream_props: typing.Optional[typing.Union[DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
         kinesis_firehose_destinations_s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
         s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
         s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param description: 
         :param name: 
         :param alarms_enabled: 
         :param data_output_prefix: 
+        :param data_stream: 
         :param data_stream_enabled: 
         :param delivery_stream_data_freshness_errors_alarm_threshold: 
         :param delivery_stream_data_freshness_errors_evaluation_periods: 
+        :param firehose_delivery_stream: 
         :param firehose_delivery_stream_props: 
         :param kinesis_firehose_destinations_s3_bucket_props: 
         :param s3_bucket: 
         :param s3_bucket_props: 
         '''
         if isinstance(firehose_delivery_stream_props, dict):
-            firehose_delivery_stream_props = _aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps(**firehose_delivery_stream_props)
+            firehose_delivery_stream_props = DeliveryStreamProps(**firehose_delivery_stream_props)
         if isinstance(kinesis_firehose_destinations_s3_bucket_props, dict):
             kinesis_firehose_destinations_s3_bucket_props = _aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps(**kinesis_firehose_destinations_s3_bucket_props)
         if isinstance(s3_bucket_props, dict):
             s3_bucket_props = _aws_cdk_aws_s3_ceddda9d.BucketProps(**s3_bucket_props)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__701f035bba059b01929f2b8055755baf96f72f5089bc32da86d2dc3cacf0f767)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
             check_type(argname="argument data_output_prefix", value=data_output_prefix, expected_type=type_hints["data_output_prefix"])
+            check_type(argname="argument data_stream", value=data_stream, expected_type=type_hints["data_stream"])
             check_type(argname="argument data_stream_enabled", value=data_stream_enabled, expected_type=type_hints["data_stream_enabled"])
             check_type(argname="argument delivery_stream_data_freshness_errors_alarm_threshold", value=delivery_stream_data_freshness_errors_alarm_threshold, expected_type=type_hints["delivery_stream_data_freshness_errors_alarm_threshold"])
             check_type(argname="argument delivery_stream_data_freshness_errors_evaluation_periods", value=delivery_stream_data_freshness_errors_evaluation_periods, expected_type=type_hints["delivery_stream_data_freshness_errors_evaluation_periods"])
+            check_type(argname="argument firehose_delivery_stream", value=firehose_delivery_stream, expected_type=type_hints["firehose_delivery_stream"])
             check_type(argname="argument firehose_delivery_stream_props", value=firehose_delivery_stream_props, expected_type=type_hints["firehose_delivery_stream_props"])
             check_type(argname="argument kinesis_firehose_destinations_s3_bucket_props", value=kinesis_firehose_destinations_s3_bucket_props, expected_type=type_hints["kinesis_firehose_destinations_s3_bucket_props"])
             check_type(argname="argument s3_bucket", value=s3_bucket, expected_type=type_hints["s3_bucket"])
             check_type(argname="argument s3_bucket_props", value=s3_bucket_props, expected_type=type_hints["s3_bucket_props"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if alarms_enabled is not None:
             self._values["alarms_enabled"] = alarms_enabled
         if data_output_prefix is not None:
             self._values["data_output_prefix"] = data_output_prefix
+        if data_stream is not None:
+            self._values["data_stream"] = data_stream
         if data_stream_enabled is not None:
             self._values["data_stream_enabled"] = data_stream_enabled
         if delivery_stream_data_freshness_errors_alarm_threshold is not None:
             self._values["delivery_stream_data_freshness_errors_alarm_threshold"] = delivery_stream_data_freshness_errors_alarm_threshold
         if delivery_stream_data_freshness_errors_evaluation_periods is not None:
             self._values["delivery_stream_data_freshness_errors_evaluation_periods"] = delivery_stream_data_freshness_errors_evaluation_periods
+        if firehose_delivery_stream is not None:
+            self._values["firehose_delivery_stream"] = firehose_delivery_stream
         if firehose_delivery_stream_props is not None:
             self._values["firehose_delivery_stream_props"] = firehose_delivery_stream_props
         if kinesis_firehose_destinations_s3_bucket_props is not None:
             self._values["kinesis_firehose_destinations_s3_bucket_props"] = kinesis_firehose_destinations_s3_bucket_props
         if s3_bucket is not None:
             self._values["s3_bucket"] = s3_bucket
         if s3_bucket_props is not None:
@@ -5488,14 +6161,19 @@
 
     @builtins.property
     def data_output_prefix(self) -> typing.Optional[builtins.str]:
         result = self._values.get("data_output_prefix")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def data_stream(self) -> typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream]:
+        result = self._values.get("data_stream")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream], result)
+
+    @builtins.property
     def data_stream_enabled(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("data_stream_enabled")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def delivery_stream_data_freshness_errors_alarm_threshold(
         self,
@@ -5507,19 +6185,24 @@
     def delivery_stream_data_freshness_errors_evaluation_periods(
         self,
     ) -> typing.Optional[jsii.Number]:
         result = self._values.get("delivery_stream_data_freshness_errors_evaluation_periods")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    def firehose_delivery_stream_props(
+    def firehose_delivery_stream(
         self,
-    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps]:
+    ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream]:
+        result = self._values.get("firehose_delivery_stream")
+        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream], result)
+
+    @builtins.property
+    def firehose_delivery_stream_props(self) -> typing.Optional[DeliveryStreamProps]:
         result = self._values.get("firehose_delivery_stream_props")
-        return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps], result)
+        return typing.cast(typing.Optional[DeliveryStreamProps], result)
 
     @builtins.property
     def kinesis_firehose_destinations_s3_bucket_props(
         self,
     ) -> typing.Optional[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps]:
         result = self._values.get("kinesis_firehose_destinations_s3_bucket_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps], result)
@@ -5557,20 +6240,23 @@
         "state_machine_failed_executions_alarm_evaluation_periods": "stateMachineFailedExecutionsAlarmEvaluationPeriods",
         "state_machine_failed_executions_alarm_threshold": "stateMachineFailedExecutionsAlarmThreshold",
         "state_machine_input": "stateMachineInput",
         "state_machine_name": "stateMachineName",
         "crawler_allow_failure": "crawlerAllowFailure",
         "crawler_name": "crawlerName",
         "crawler_props": "crawlerProps",
+        "crawler_role": "crawlerRole",
+        "database_name": "databaseName",
         "job_name": "jobName",
         "job_props": "jobProps",
         "job_run_args": "jobRunArgs",
         "state_machine_retry_backoff_rate": "stateMachineRetryBackoffRate",
         "state_machine_retry_interval": "stateMachineRetryInterval",
         "state_machine_retry_max_attempts": "stateMachineRetryMaxAttempts",
+        "targets": "targets",
     },
 )
 class GlueTransformStageProps(StateMachineStageProps):
     def __init__(
         self,
         *,
         description: typing.Optional[builtins.str] = None,
@@ -5580,63 +6266,74 @@
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         crawler_allow_failure: typing.Optional[builtins.bool] = None,
         crawler_name: typing.Optional[builtins.str] = None,
         crawler_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        crawler_role: typing.Optional[builtins.str] = None,
+        database_name: typing.Optional[builtins.str] = None,
         job_name: typing.Optional[builtins.str] = None,
         job_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_alpha_ce674d29.JobProps, typing.Dict[builtins.str, typing.Any]]] = None,
         job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
         state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
+        targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     ) -> None:
         '''
         :param description: 
         :param name: 
         :param additional_role_policy_statements: 
         :param alarms_enabled: 
         :param state_machine_failed_executions_alarm_evaluation_periods: 
         :param state_machine_failed_executions_alarm_threshold: 
         :param state_machine_input: 
         :param state_machine_name: 
         :param crawler_allow_failure: 
         :param crawler_name: 
         :param crawler_props: 
+        :param crawler_role: 
+        :param database_name: 
         :param job_name: 
         :param job_props: 
         :param job_run_args: 
         :param state_machine_retry_backoff_rate: 
         :param state_machine_retry_interval: 
         :param state_machine_retry_max_attempts: 
+        :param targets: 
         '''
         if isinstance(crawler_props, dict):
             crawler_props = _aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps(**crawler_props)
         if isinstance(job_props, dict):
             job_props = _aws_cdk_aws_glue_alpha_ce674d29.JobProps(**job_props)
+        if isinstance(targets, dict):
+            targets = _aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty(**targets)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__36c864b97313236b09b597808a1574a4f4d21024bac872f4e182edbd9a3d0175)
             check_type(argname="argument description", value=description, expected_type=type_hints["description"])
             check_type(argname="argument name", value=name, expected_type=type_hints["name"])
             check_type(argname="argument additional_role_policy_statements", value=additional_role_policy_statements, expected_type=type_hints["additional_role_policy_statements"])
             check_type(argname="argument alarms_enabled", value=alarms_enabled, expected_type=type_hints["alarms_enabled"])
             check_type(argname="argument state_machine_failed_executions_alarm_evaluation_periods", value=state_machine_failed_executions_alarm_evaluation_periods, expected_type=type_hints["state_machine_failed_executions_alarm_evaluation_periods"])
             check_type(argname="argument state_machine_failed_executions_alarm_threshold", value=state_machine_failed_executions_alarm_threshold, expected_type=type_hints["state_machine_failed_executions_alarm_threshold"])
             check_type(argname="argument state_machine_input", value=state_machine_input, expected_type=type_hints["state_machine_input"])
             check_type(argname="argument state_machine_name", value=state_machine_name, expected_type=type_hints["state_machine_name"])
             check_type(argname="argument crawler_allow_failure", value=crawler_allow_failure, expected_type=type_hints["crawler_allow_failure"])
             check_type(argname="argument crawler_name", value=crawler_name, expected_type=type_hints["crawler_name"])
             check_type(argname="argument crawler_props", value=crawler_props, expected_type=type_hints["crawler_props"])
+            check_type(argname="argument crawler_role", value=crawler_role, expected_type=type_hints["crawler_role"])
+            check_type(argname="argument database_name", value=database_name, expected_type=type_hints["database_name"])
             check_type(argname="argument job_name", value=job_name, expected_type=type_hints["job_name"])
             check_type(argname="argument job_props", value=job_props, expected_type=type_hints["job_props"])
             check_type(argname="argument job_run_args", value=job_run_args, expected_type=type_hints["job_run_args"])
             check_type(argname="argument state_machine_retry_backoff_rate", value=state_machine_retry_backoff_rate, expected_type=type_hints["state_machine_retry_backoff_rate"])
             check_type(argname="argument state_machine_retry_interval", value=state_machine_retry_interval, expected_type=type_hints["state_machine_retry_interval"])
             check_type(argname="argument state_machine_retry_max_attempts", value=state_machine_retry_max_attempts, expected_type=type_hints["state_machine_retry_max_attempts"])
+            check_type(argname="argument targets", value=targets, expected_type=type_hints["targets"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if description is not None:
             self._values["description"] = description
         if name is not None:
             self._values["name"] = name
         if additional_role_policy_statements is not None:
             self._values["additional_role_policy_statements"] = additional_role_policy_statements
@@ -5652,26 +6349,32 @@
             self._values["state_machine_name"] = state_machine_name
         if crawler_allow_failure is not None:
             self._values["crawler_allow_failure"] = crawler_allow_failure
         if crawler_name is not None:
             self._values["crawler_name"] = crawler_name
         if crawler_props is not None:
             self._values["crawler_props"] = crawler_props
+        if crawler_role is not None:
+            self._values["crawler_role"] = crawler_role
+        if database_name is not None:
+            self._values["database_name"] = database_name
         if job_name is not None:
             self._values["job_name"] = job_name
         if job_props is not None:
             self._values["job_props"] = job_props
         if job_run_args is not None:
             self._values["job_run_args"] = job_run_args
         if state_machine_retry_backoff_rate is not None:
             self._values["state_machine_retry_backoff_rate"] = state_machine_retry_backoff_rate
         if state_machine_retry_interval is not None:
             self._values["state_machine_retry_interval"] = state_machine_retry_interval
         if state_machine_retry_max_attempts is not None:
             self._values["state_machine_retry_max_attempts"] = state_machine_retry_max_attempts
+        if targets is not None:
+            self._values["targets"] = targets
 
     @builtins.property
     def description(self) -> typing.Optional[builtins.str]:
         result = self._values.get("description")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
@@ -5731,14 +6434,24 @@
     def crawler_props(
         self,
     ) -> typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps]:
         result = self._values.get("crawler_props")
         return typing.cast(typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps], result)
 
     @builtins.property
+    def crawler_role(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("crawler_role")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def database_name(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("database_name")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def job_name(self) -> typing.Optional[builtins.str]:
         result = self._values.get("job_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def job_props(self) -> typing.Optional[_aws_cdk_aws_glue_alpha_ce674d29.JobProps]:
         result = self._values.get("job_props")
@@ -5762,14 +6475,21 @@
         return typing.cast(typing.Optional[_aws_cdk_ceddda9d.Duration], result)
 
     @builtins.property
     def state_machine_retry_max_attempts(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("state_machine_retry_max_attempts")
         return typing.cast(typing.Optional[jsii.Number], result)
 
+    @builtins.property
+    def targets(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty]:
+        result = self._values.get("targets")
+        return typing.cast(typing.Optional[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -6665,39 +7385,67 @@
 ):
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         create_job: typing.Optional[builtins.bool] = None,
+        database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        data_catalog_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         dataset_name: typing.Optional[builtins.str] = None,
+        encryption_key_arn: typing.Optional[builtins.str] = None,
+        encryption_mode: typing.Optional[builtins.str] = None,
         job_name: typing.Optional[builtins.str] = None,
         job_role_arn: typing.Optional[builtins.str] = None,
+        job_sample: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         job_type: typing.Optional[builtins.str] = None,
+        log_subscription: typing.Optional[builtins.str] = None,
+        max_capacity: typing.Optional[jsii.Number] = None,
+        max_retries: typing.Optional[jsii.Number] = None,
+        output_location: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+        profile_configuration: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+        project_name: typing.Optional[builtins.str] = None,
         recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+        tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+        timeout: typing.Optional[jsii.Number] = None,
+        validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
         name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param create_job: 
+        :param database_outputs: 
+        :param data_catalog_outputs: 
         :param dataset_name: 
+        :param encryption_key_arn: 
+        :param encryption_mode: 
         :param job_name: 
         :param job_role_arn: 
+        :param job_sample: 
         :param job_type: 
+        :param log_subscription: 
+        :param max_capacity: 
+        :param max_retries: 
+        :param output_location: 
         :param outputs: 
+        :param profile_configuration: 
+        :param project_name: 
         :param recipe: 
+        :param tags: 
+        :param timeout: 
+        :param validation_configurations: 
         :param additional_role_policy_statements: 
         :param alarms_enabled: 
         :param state_machine_failed_executions_alarm_evaluation_periods: 
         :param state_machine_failed_executions_alarm_threshold: 
         :param state_machine_input: 
         :param state_machine_name: 
         :param description: 
@@ -6705,20 +7453,34 @@
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a9214d4641d831e11d83d601cf5e13ef25bd3d55977b689c3cefd7aaa9fb0fb5)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DataBrewTransformStageProps(
             create_job=create_job,
+            database_outputs=database_outputs,
+            data_catalog_outputs=data_catalog_outputs,
             dataset_name=dataset_name,
+            encryption_key_arn=encryption_key_arn,
+            encryption_mode=encryption_mode,
             job_name=job_name,
             job_role_arn=job_role_arn,
+            job_sample=job_sample,
             job_type=job_type,
+            log_subscription=log_subscription,
+            max_capacity=max_capacity,
+            max_retries=max_retries,
+            output_location=output_location,
             outputs=outputs,
+            profile_configuration=profile_configuration,
+            project_name=project_name,
             recipe=recipe,
+            tags=tags,
+            timeout=timeout,
+            validation_configurations=validation_configurations,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
@@ -6771,20 +7533,23 @@
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         crawler_allow_failure: typing.Optional[builtins.bool] = None,
         crawler_name: typing.Optional[builtins.str] = None,
         crawler_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps, typing.Dict[builtins.str, typing.Any]]] = None,
+        crawler_role: typing.Optional[builtins.str] = None,
+        database_name: typing.Optional[builtins.str] = None,
         job_name: typing.Optional[builtins.str] = None,
         job_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_alpha_ce674d29.JobProps, typing.Dict[builtins.str, typing.Any]]] = None,
         job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
         state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
         state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
+        targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
         additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
         alarms_enabled: typing.Optional[builtins.bool] = None,
         state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
         state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
         state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
         state_machine_name: typing.Optional[builtins.str] = None,
         description: typing.Optional[builtins.str] = None,
@@ -6792,20 +7557,23 @@
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param crawler_allow_failure: 
         :param crawler_name: 
         :param crawler_props: 
+        :param crawler_role: 
+        :param database_name: 
         :param job_name: 
         :param job_props: 
         :param job_run_args: 
         :param state_machine_retry_backoff_rate: 
         :param state_machine_retry_interval: 
         :param state_machine_retry_max_attempts: 
+        :param targets: 
         :param additional_role_policy_statements: 
         :param alarms_enabled: 
         :param state_machine_failed_executions_alarm_evaluation_periods: 
         :param state_machine_failed_executions_alarm_threshold: 
         :param state_machine_input: 
         :param state_machine_name: 
         :param description: 
@@ -6815,20 +7583,23 @@
             type_hints = typing.get_type_hints(_typecheckingstub__8ddc56c43fee5e5dc6737d945cf18cb6800a5b74340125036ae173083ba761f2)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = GlueTransformStageProps(
             crawler_allow_failure=crawler_allow_failure,
             crawler_name=crawler_name,
             crawler_props=crawler_props,
+            crawler_role=crawler_role,
+            database_name=database_name,
             job_name=job_name,
             job_props=job_props,
             job_run_args=job_run_args,
             state_machine_retry_backoff_rate=state_machine_retry_backoff_rate,
             state_machine_retry_interval=state_machine_retry_interval,
             state_machine_retry_max_attempts=state_machine_retry_max_attempts,
+            targets=targets,
             additional_role_policy_statements=additional_role_policy_statements,
             alarms_enabled=alarms_enabled,
             state_machine_failed_executions_alarm_evaluation_periods=state_machine_failed_executions_alarm_evaluation_periods,
             state_machine_failed_executions_alarm_threshold=state_machine_failed_executions_alarm_threshold,
             state_machine_input=state_machine_input,
             state_machine_name=state_machine_name,
             description=description,
@@ -7320,28 +8091,34 @@
     "BaseStack",
     "BaseStackProps",
     "CICDActions",
     "CICDPipelineStack",
     "CICDPipelineStackProps",
     "CodeArtifactPublishActionProps",
     "CodeCommitSourceActionProps",
+    "Configuration",
     "Configurator",
     "CreateStateMachineResult",
     "DataBrewTransformStage",
     "DataBrewTransformStageProps",
     "DataPipeline",
     "DataPipelineProps",
     "DataStage",
     "DataStageProps",
+    "DeliveryStreamProps",
+    "EnvironmentConfiguration",
+    "EnvironmentResult",
     "EventStage",
     "EventStageProps",
     "FirehoseToS3Stage",
     "FirehoseToS3StageProps",
     "GetEnvConfigProps",
+    "GetEnvironmentProps",
     "GetSynthActionProps",
+    "GetTagsProps",
     "GlueFactory",
     "GlueTransformStage",
     "GlueTransformStageProps",
     "KmsFactory",
     "PermissionsBoundaryProps",
     "RedshiftDataApiStage",
     "RedshiftDataApiStageProps",
@@ -7465,15 +8242,15 @@
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__403bc1fd4d529dd1acdcfdf6824076a7e78329d131f442981f447f8f5298a7cc(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
-    config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+    config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     environment_id: typing.Optional[builtins.str] = None,
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
@@ -7481,26 +8258,37 @@
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__c52c78b6e97cce4b370cb75d9552fff81495ba02218c70f1c8947488c2c0604a(
+    scope: _constructs_77d1e7e8.Construct,
+    id: builtins.str,
+    *,
+    environment_id: typing.Optional[builtins.str] = None,
+    prefix: typing.Optional[builtins.str] = None,
+    qualifier: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__a429ca722d1fec889b8120d065d6c339e922faac9a9e70454e565500ff82514c(
     *,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
-    config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+    config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     environment_id: typing.Optional[builtins.str] = None,
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__fab9ea5d8746e6c137eb1d92124b75da65dab030241ebf0002427b6ad8676aa2(
@@ -7551,15 +8339,15 @@
 
 def _typecheckingstub__2a4f7374970c6409060af558e7802348870a4c4a3b9f9232e789f1488d18fb90(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     cdk_language: typing.Optional[builtins.str] = None,
     pipeline_name: typing.Optional[builtins.str] = None,
-    config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+    config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     environment_id: typing.Optional[builtins.str] = None,
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
     analytics_reporting: typing.Optional[builtins.bool] = None,
     cross_region_references: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
@@ -7608,15 +8396,15 @@
     description: typing.Optional[builtins.str] = None,
     env: typing.Optional[typing.Union[_aws_cdk_ceddda9d.Environment, typing.Dict[builtins.str, typing.Any]]] = None,
     permissions_boundary: typing.Optional[_aws_cdk_ceddda9d.PermissionsBoundary] = None,
     stack_name: typing.Optional[builtins.str] = None,
     synthesizer: typing.Optional[_aws_cdk_ceddda9d.IStackSynthesizer] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     termination_protection: typing.Optional[builtins.bool] = None,
-    config: typing.Optional[typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]]] = None,
+    config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
     environment_id: typing.Optional[builtins.str] = None,
     permissions_boundary_arn: typing.Optional[builtins.str] = None,
     cdk_language: typing.Optional[builtins.str] = None,
     pipeline_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
@@ -7640,17 +8428,29 @@
     branch: builtins.str,
     repository_name: builtins.str,
     props: typing.Optional[typing.Union[_aws_cdk_pipelines_ceddda9d.ConnectionSourceOptions, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__daeed9e6cb5e50c39b922933d297c173f25183423bf700dfd9f8b0fe3765c923(
+    *,
+    environments: typing.Mapping[builtins.str, typing.Union[EnvironmentConfiguration, typing.Dict[builtins.str, typing.Any]]],
+    account: typing.Optional[builtins.str] = None,
+    bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    ddk_bootstrap_config_key: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__83dd06108e5a02547d07299060f92123340b3d7ec7e9e6f36a8e28ce02b22a22(
     scope: _constructs_77d1e7e8.Construct,
-    config: typing.Union[builtins.str, typing.Mapping[typing.Any, typing.Any]],
+    config: typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]],
     environment_id: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ce369044fa737e8a329b15db41cbef0ecf3e52cea663d9bd55b6edfe486a7705(
     attribute: builtins.str,
@@ -7694,22 +8494,61 @@
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__ef7997fe1d9215e0814459fdbbb95740e62a7f0437cd0df0dcd43ac255b163e4(
+    *,
+    delivery_stream_name: typing.Optional[builtins.str] = None,
+    destinations: typing.Optional[typing.Sequence[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.IDestination]] = None,
+    encryption: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.StreamEncryption] = None,
+    encryption_key: typing.Optional[_aws_cdk_aws_kms_ceddda9d.IKey] = None,
+    role: typing.Optional[_aws_cdk_aws_iam_ceddda9d.IRole] = None,
+    source_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.IStream] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__cf306c436463dcb56197f32e9c4793604595ef2ca8f42b2d72de058d5806870c(
+    *,
+    account: typing.Optional[builtins.str] = None,
+    bootstrap: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+    region: typing.Optional[builtins.str] = None,
+    resources: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
+    tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
+def _typecheckingstub__c2515674b45134976862352edd7f3a4f56dddd10e860df69a14d633b55dfe768(
+    *,
+    account: typing.Optional[builtins.str] = None,
+    region: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__392d4bf9e0a3416c4cbfe2cfcca884cc2b98f96b99a23a03e386497b6cfd2fef(
     *,
     config_path: builtins.str,
     environment_id: builtins.str,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__f1d1864ebb63e794b66b601804d8a186ccc2fe70e5c1aeea9def8ecd1ab83dde(
+    *,
+    config_path: builtins.str,
+    environment_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__b411e230303f93f36fe42f88f3ae59e51d4746a608fa21c8fe560bb5fe18a352(
     *,
     account: typing.Optional[builtins.str] = None,
     additional_install_commands: typing.Optional[typing.Sequence[builtins.str]] = None,
     cdk_version: typing.Optional[builtins.str] = None,
     codeartifact_domain: typing.Optional[builtins.str] = None,
     codeartifact_domain_owner: typing.Optional[builtins.str] = None,
@@ -7718,14 +8557,22 @@
     partition: typing.Optional[builtins.str] = None,
     region: typing.Optional[builtins.str] = None,
     role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__f80411a398b3a95cafcc083fedf809e35c9f9d3c872682fa20c2c416251da930(
+    *,
+    config_path: builtins.str,
+    environment_id: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__de56c47dda07ed1c4eda1133b7152caa819140d8ea5277eaf41f2802c2c16bfd(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     executable: _aws_cdk_aws_glue_alpha_ce674d29.JobExecutable,
     connections: typing.Optional[typing.Sequence[_aws_cdk_aws_glue_alpha_ce674d29.IConnection]] = None,
     continuous_logging: typing.Optional[typing.Union[_aws_cdk_aws_glue_alpha_ce674d29.ContinuousLoggingProps, typing.Dict[builtins.str, typing.Any]]] = None,
@@ -7968,20 +8815,34 @@
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     create_job: typing.Optional[builtins.bool] = None,
+    database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    data_catalog_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     dataset_name: typing.Optional[builtins.str] = None,
+    encryption_key_arn: typing.Optional[builtins.str] = None,
+    encryption_mode: typing.Optional[builtins.str] = None,
     job_name: typing.Optional[builtins.str] = None,
     job_role_arn: typing.Optional[builtins.str] = None,
+    job_sample: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     job_type: typing.Optional[builtins.str] = None,
+    log_subscription: typing.Optional[builtins.str] = None,
+    max_capacity: typing.Optional[jsii.Number] = None,
+    max_retries: typing.Optional[jsii.Number] = None,
+    output_location: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    profile_configuration: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+    project_name: typing.Optional[builtins.str] = None,
     recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+    timeout: typing.Optional[jsii.Number] = None,
+    validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a7ee0133925b96b521f696b544f087847c2e6916f79bbdcf76306ed73653fdb2(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
@@ -8032,18 +8893,20 @@
     pass
 
 def _typecheckingstub__3f9217104050cf03ef7cf7519808ce659edfe6c1ba00722ea6601239921cfd56(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     data_output_prefix: typing.Optional[builtins.str] = None,
+    data_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream] = None,
     data_stream_enabled: typing.Optional[builtins.bool] = None,
     delivery_stream_data_freshness_errors_alarm_threshold: typing.Optional[jsii.Number] = None,
     delivery_stream_data_freshness_errors_evaluation_periods: typing.Optional[jsii.Number] = None,
-    firehose_delivery_stream_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    firehose_delivery_stream: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream] = None,
+    firehose_delivery_stream_props: typing.Optional[typing.Union[DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
     kinesis_firehose_destinations_s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
     s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
 ) -> None:
@@ -8052,18 +8915,20 @@
 
 def _typecheckingstub__701f035bba059b01929f2b8055755baf96f72f5089bc32da86d2dc3cacf0f767(
     *,
     description: typing.Optional[builtins.str] = None,
     name: typing.Optional[builtins.str] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     data_output_prefix: typing.Optional[builtins.str] = None,
+    data_stream: typing.Optional[_aws_cdk_aws_kinesis_ceddda9d.Stream] = None,
     data_stream_enabled: typing.Optional[builtins.bool] = None,
     delivery_stream_data_freshness_errors_alarm_threshold: typing.Optional[jsii.Number] = None,
     delivery_stream_data_freshness_errors_evaluation_periods: typing.Optional[jsii.Number] = None,
-    firehose_delivery_stream_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    firehose_delivery_stream: typing.Optional[_aws_cdk_aws_kinesisfirehose_alpha_30daaf29.DeliveryStream] = None,
+    firehose_delivery_stream_props: typing.Optional[typing.Union[DeliveryStreamProps, typing.Dict[builtins.str, typing.Any]]] = None,
     kinesis_firehose_destinations_s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_kinesisfirehose_destinations_alpha_8ee8dbdc.S3BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
     s3_bucket: typing.Optional[_aws_cdk_aws_s3_ceddda9d.IBucket] = None,
     s3_bucket_props: typing.Optional[typing.Union[_aws_cdk_aws_s3_ceddda9d.BucketProps, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
@@ -8076,20 +8941,23 @@
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     crawler_allow_failure: typing.Optional[builtins.bool] = None,
     crawler_name: typing.Optional[builtins.str] = None,
     crawler_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    crawler_role: typing.Optional[builtins.str] = None,
+    database_name: typing.Optional[builtins.str] = None,
     job_name: typing.Optional[builtins.str] = None,
     job_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_alpha_ce674d29.JobProps, typing.Dict[builtins.str, typing.Any]]] = None,
     job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
     state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
+    targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__defbc9333f2b8b3e2d55373f9b0155e5f6e83609e9153dc24f619d747ca4f133(
     *,
     description: typing.Optional[builtins.str] = None,
@@ -8248,20 +9116,34 @@
     pass
 
 def _typecheckingstub__a9214d4641d831e11d83d601cf5e13ef25bd3d55977b689c3cefd7aaa9fb0fb5(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     create_job: typing.Optional[builtins.bool] = None,
+    database_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DatabaseOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    data_catalog_outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.DataCatalogOutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     dataset_name: typing.Optional[builtins.str] = None,
+    encryption_key_arn: typing.Optional[builtins.str] = None,
+    encryption_mode: typing.Optional[builtins.str] = None,
     job_name: typing.Optional[builtins.str] = None,
     job_role_arn: typing.Optional[builtins.str] = None,
+    job_sample: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.JobSampleProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     job_type: typing.Optional[builtins.str] = None,
+    log_subscription: typing.Optional[builtins.str] = None,
+    max_capacity: typing.Optional[jsii.Number] = None,
+    max_retries: typing.Optional[jsii.Number] = None,
+    output_location: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputLocationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     outputs: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.OutputProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
+    profile_configuration: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ProfileConfigurationProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+    project_name: typing.Optional[builtins.str] = None,
     recipe: typing.Optional[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.RecipeProperty, typing.Dict[builtins.str, typing.Any]]] = None,
+    tags: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_ceddda9d.CfnTag, typing.Dict[builtins.str, typing.Any]]]] = None,
+    timeout: typing.Optional[jsii.Number] = None,
+    validation_configurations: typing.Optional[typing.Sequence[typing.Union[_aws_cdk_aws_databrew_ceddda9d.CfnJob.ValidationConfigurationProperty, typing.Dict[builtins.str, typing.Any]]]] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
@@ -8273,20 +9155,23 @@
 def _typecheckingstub__8ddc56c43fee5e5dc6737d945cf18cb6800a5b74340125036ae173083ba761f2(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     crawler_allow_failure: typing.Optional[builtins.bool] = None,
     crawler_name: typing.Optional[builtins.str] = None,
     crawler_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawlerProps, typing.Dict[builtins.str, typing.Any]]] = None,
+    crawler_role: typing.Optional[builtins.str] = None,
+    database_name: typing.Optional[builtins.str] = None,
     job_name: typing.Optional[builtins.str] = None,
     job_props: typing.Optional[typing.Union[_aws_cdk_aws_glue_alpha_ce674d29.JobProps, typing.Dict[builtins.str, typing.Any]]] = None,
     job_run_args: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_retry_backoff_rate: typing.Optional[jsii.Number] = None,
     state_machine_retry_interval: typing.Optional[_aws_cdk_ceddda9d.Duration] = None,
     state_machine_retry_max_attempts: typing.Optional[jsii.Number] = None,
+    targets: typing.Optional[typing.Union[_aws_cdk_aws_glue_ceddda9d.CfnCrawler.TargetsProperty, typing.Dict[builtins.str, typing.Any]]] = None,
     additional_role_policy_statements: typing.Optional[typing.Sequence[_aws_cdk_aws_iam_ceddda9d.PolicyStatement]] = None,
     alarms_enabled: typing.Optional[builtins.bool] = None,
     state_machine_failed_executions_alarm_evaluation_periods: typing.Optional[jsii.Number] = None,
     state_machine_failed_executions_alarm_threshold: typing.Optional[jsii.Number] = None,
     state_machine_input: typing.Optional[typing.Mapping[builtins.str, typing.Any]] = None,
     state_machine_name: typing.Optional[builtins.str] = None,
     description: typing.Optional[builtins.str] = None,
```

### Comparing `aws-ddk-core-1.0.0b0/src/aws_ddk_core/_jsii/__init__.py` & `aws-ddk-core-1.0.0b1/src/aws_ddk_core/_jsii/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii
 import aws_cdk.integ_tests_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "aws-ddk-core",
-    "1.0.0-beta.0",
+    "1.0.0-beta.1",
     __name__[0:-6],
-    "aws-ddk-core@1.0.0-beta.0.jsii.tgz",
+    "aws-ddk-core@1.0.0-beta.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-ddk-core-1.0.0b0/src/aws_ddk_core.egg-info/PKG-INFO` & `aws-ddk-core-1.0.0b1/src/aws_ddk_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: AWS DataOps Development Kit
 Home-page: https://github.com/awslabs/aws-ddk
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awslabs/aws-ddk
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

