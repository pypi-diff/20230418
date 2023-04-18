# Comparing `tmp/cdktf-cdktf-provider-http-3.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-http-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-http-3.0.0.tar", last modified: Tue Jan 17 14:53:12 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-http-4.0.0.tar", last modified: Tue Apr 18 20:44:52 2023, max compression
```

## Comparing `cdktf-cdktf-provider-http-3.0.0.tar` & `cdktf-cdktf-provider-http-4.0.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/
--rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27426 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/_jsii/provider-http@3.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/data_http/
--rw-r--r--   0 runner    (1001) docker     (123)    28990 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/provider/
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:53:00.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:53:12.543513 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-01-17 14:53:12.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-01-17 14:53:12.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:53:12.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:53:12.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-01-17 14:53:12.000000 cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3139 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1918 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.244869 cdktf-cdktf-provider-http-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/
+-rw-r--r--   0 runner    (1001) docker     (123)     3533 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50098 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/data_http/
+-rw-r--r--   0 runner    (1001) docker     (123)    29953 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)     5418 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:44:39.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:44:52.248869 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 20:44:52.000000 cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/LICENSE` & `cdktf-cdktf-provider-http-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-http-3.0.0/PKG-INFO` & `cdktf-cdktf-provider-http-4.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-http-go`](https://github.com/cdktf/cdktf-provider-http-go) package.
 
 `go get github.com/cdktf/cdktf-provider-http-go/http`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-http).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform http Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/README.md` & `cdktf-cdktf-provider-http-4.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-http-go`](https://github.com/cdktf/cdktf-provider-http-go) package.
 
 `go get github.com/cdktf/cdktf-provider-http-go/http`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-http).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform http Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/setup.py` & `cdktf-cdktf-provider-http-4.0.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-http",
-    "version": "3.0.0",
+    "version": "4.0.0",
     "description": "Prebuilt http Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-http.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -24,37 +24,38 @@
         "cdktf_cdktf_provider_http",
         "cdktf_cdktf_provider_http._jsii",
         "cdktf_cdktf_provider_http.data_http",
         "cdktf_cdktf_provider_http.provider"
     ],
     "package_data": {
         "cdktf_cdktf_provider_http._jsii": [
-            "provider-http@3.0.0.jsii.tgz"
+            "provider-http@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_http": [
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

### Comparing `cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/__init__.py` & `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-http-go`](https://github.com/cdktf/cdktf-provider-http-go) package.
 
 `go get github.com/cdktf/cdktf-provider-http-go/http`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-http).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform http Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py` & `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/data_http/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_http`
 
-Refer to the Terraform Registory for docs: [`data_http`](https://www.terraform.io/docs/providers/http/d/http).
+Refer to the Terraform Registory for docs: [`data_http`](https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class DataHttp(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-http.dataHttp.DataHttp",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/http/d/http http}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http http}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         url: builtins.str,
         ca_cert_pem: typing.Optional[builtins.str] = None,
         insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         method: typing.Optional[builtins.str] = None,
         request_body: typing.Optional[builtins.str] = None,
         request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/http/d/http http} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http http} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#url DataHttp#url}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#ca_cert_pem DataHttp#ca_cert_pem}
-        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#insecure DataHttp#insecure}
-        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#method DataHttp#method}
-        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#request_body DataHttp#request_body}
-        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#request_headers DataHttp#request_headers}
+        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#url DataHttp#url}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#insecure DataHttp#insecure}
+        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#method DataHttp#method}
+        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_body DataHttp#request_body}
+        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_headers DataHttp#request_headers}
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
 class DataHttpConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         url: builtins.str,
         ca_cert_pem: typing.Optional[builtins.str] = None,
@@ -295,20 +295,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#url DataHttp#url}
-        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#ca_cert_pem DataHttp#ca_cert_pem}
-        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#insecure DataHttp#insecure}
-        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#method DataHttp#method}
-        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#request_body DataHttp#request_body}
-        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#request_headers DataHttp#request_headers}
+        :param url: The URL for the request. Supported schemes are ``http`` and ``https``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#url DataHttp#url}
+        :param ca_cert_pem: Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
+        :param insecure: Disables verification of the server's certificate chain and hostname. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#insecure DataHttp#insecure}
+        :param method: The HTTP Method for the request. Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#method DataHttp#method}
+        :param request_body: The request body as a string. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_body DataHttp#request_body}
+        :param request_headers: A map of request header field names and values. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_headers DataHttp#request_headers}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ee2b6a3664a80e642a2ef1d255302a3f3dc3d391999cb8f3d6103cac8420d573)
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
@@ -413,67 +415,67 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def url(self) -> builtins.str:
         '''The URL for the request. Supported schemes are ``http`` and ``https``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#url DataHttp#url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#url DataHttp#url}
         '''
         result = self._values.get("url")
         assert result is not None, "Required property 'url' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def ca_cert_pem(self) -> typing.Optional[builtins.str]:
         '''Certificate data of the Certificate Authority (CA) in `PEM (RFC 1421) <https://datatracker.ietf.org/doc/html/rfc1421>`_ format.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#ca_cert_pem DataHttp#ca_cert_pem}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#ca_cert_pem DataHttp#ca_cert_pem}
         '''
         result = self._values.get("ca_cert_pem")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def insecure(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Disables verification of the server's certificate chain and hostname. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#insecure DataHttp#insecure}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#insecure DataHttp#insecure}
         '''
         result = self._values.get("insecure")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def method(self) -> typing.Optional[builtins.str]:
         '''The HTTP Method for the request.
 
         Allowed methods are a subset of methods defined in `RFC7231 <https://datatracker.ietf.org/doc/html/rfc7231#section-4.3>`_ namely, ``GET``, ``HEAD``, and ``POST``. ``POST`` support is only intended for read-only URLs, such as submitting a search.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#method DataHttp#method}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#method DataHttp#method}
         '''
         result = self._values.get("method")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def request_body(self) -> typing.Optional[builtins.str]:
         '''The request body as a string.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#request_body DataHttp#request_body}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_body DataHttp#request_body}
         '''
         result = self._values.get("request_body")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def request_headers(
         self,
     ) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A map of request header field names and values.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http/d/http#request_headers DataHttp#request_headers}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs/data-sources/http#request_headers DataHttp#request_headers}
         '''
         result = self._values.get("request_headers")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -500,15 +502,15 @@
     url: builtins.str,
     ca_cert_pem: typing.Optional[builtins.str] = None,
     insecure: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     method: typing.Optional[builtins.str] = None,
     request_body: typing.Optional[builtins.str] = None,
     request_headers: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
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
@@ -549,15 +551,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ee2b6a3664a80e642a2ef1d255302a3f3dc3d391999cb8f3d6103cac8420d573(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     url: builtins.str,
     ca_cert_pem: typing.Optional[builtins.str] = None,
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py` & `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http/provider/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`http`](https://www.terraform.io/docs/providers/http).
+Refer to the Terraform Registory for docs: [`http`](https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,28 +22,28 @@
 
 
 class HttpProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-http.provider.HttpProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/http http}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs http}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/http http} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs http} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http#alias HttpProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs#alias HttpProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ed4656733258f821890abe9b576315755fbb2c26c5225d063440932e3244ec0a)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HttpProviderConfig(alias=alias)
 
@@ -84,28 +84,28 @@
     jsii_type="@cdktf/provider-http.provider.HttpProviderConfig",
     jsii_struct_bases=[],
     name_mapping={"alias": "alias"},
 )
 class HttpProviderConfig:
     def __init__(self, *, alias: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http#alias HttpProvider#alias}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs#alias HttpProvider#alias}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c5e292f1b2ced23926cb25076c6e327c7591be5943163c3c72b898964467f963)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if alias is not None:
             self._values["alias"] = alias
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/http#alias HttpProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/http/3.2.1/docs#alias HttpProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO` & `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-http
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt http Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-http.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-http.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-http-go`](https://github.com/cdktf/cdktf-provider-http-go) package.
 
 `go get github.com/cdktf/cdktf-provider-http-go/http`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-http).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform http Provider version 1:1. In fact, it always tracks `latest` of `~> 3.1` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-http-3.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-http-4.0.0/src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 src/cdktf_cdktf_provider_http/py.typed
 src/cdktf_cdktf_provider_http.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_http.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_http.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_http.egg-info/requires.txt
 src/cdktf_cdktf_provider_http.egg-info/top_level.txt
 src/cdktf_cdktf_provider_http/_jsii/__init__.py
-src/cdktf_cdktf_provider_http/_jsii/provider-http@3.0.0.jsii.tgz
+src/cdktf_cdktf_provider_http/_jsii/provider-http@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_http/data_http/__init__.py
 src/cdktf_cdktf_provider_http/provider/__init__.py
```

