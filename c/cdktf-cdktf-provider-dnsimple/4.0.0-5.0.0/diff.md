# Comparing `tmp/cdktf-cdktf-provider-dnsimple-4.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-dnsimple-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-dnsimple-4.0.0.tar", last modified: Tue Apr 11 13:03:52 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-dnsimple-5.0.0.tar", last modified: Tue Apr 18 20:37:37 2023, max compression
```

## Comparing `cdktf-cdktf-provider-dnsimple-4.0.0.tar` & `cdktf-cdktf-provider-dnsimple-5.0.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.053041 cdktf-cdktf-provider-dnsimple-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.057041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.057041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   127447 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@4.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    17539 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
--rw-r--r--   0 runner    (1001) docker     (123)    14662 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/domain/
--rw-r--r--   0 runner    (1001) docker     (123)    15239 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/
--rw-r--r--   0 runner    (1001) docker     (123)    18758 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
--rw-r--r--   0 runner    (1001) docker     (123)    23052 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.061041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/
--rw-r--r--   0 runner    (1001) docker     (123)    24362 2023-04-11 13:03:36.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 13:03:52.057041 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-11 13:03:52.000000 cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.430281 cdktf-cdktf-provider-dnsimple-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130208 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    18109 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/
+-rw-r--r--   0 runner    (1001) docker     (123)    15139 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)    15698 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/
+-rw-r--r--   0 runner    (1001) docker     (123)    19385 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/
+-rw-r--r--   0 runner    (1001) docker     (123)    23763 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    18898 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.438282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/
+-rw-r--r--   0 runner    (1001) docker     (123)    25241 2023-04-18 20:37:22.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:37:37.434282 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-18 20:37:37.000000 cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/LICENSE` & `cdktf-cdktf-provider-dnsimple-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-5.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 4.0.0
+Version: 5.0.0
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Terraform CDK dnsimple Provider ~> 0.13
+# Terraform CDK dnsimple Provider ~> 1.0
 
 This repo builds and publishes the Terraform dnsimple Provider bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
@@ -74,15 +74,15 @@
 * [C#](./docs/API.csharp.md)
 * [Go](./docs/API.go.md)
 
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dnsimple).
 
 ## Versioning
 
-This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 0.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
+This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
 * [Terraform dnsimple Provider](https://github.com/terraform-providers/terraform-provider-dnsimple)
 * [Terraform Engine](https://terraform.io)
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/README.md` & `cdktf-cdktf-provider-dnsimple-5.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Terraform CDK dnsimple Provider ~> 0.13
+# Terraform CDK dnsimple Provider ~> 1.0
 
 This repo builds and publishes the Terraform dnsimple Provider bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
@@ -50,15 +50,15 @@
 * [C#](./docs/API.csharp.md)
 * [Go](./docs/API.go.md)
 
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dnsimple).
 
 ## Versioning
 
-This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 0.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
+This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
 * [Terraform dnsimple Provider](https://github.com/terraform-providers/terraform-provider-dnsimple)
 * [Terraform Engine](https://terraform.io)
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/setup.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-dnsimple",
-    "version": "4.0.0",
+    "version": "5.0.0",
     "description": "Prebuilt dnsimple Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-dnsimple.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -29,25 +29,25 @@
         "cdktf_cdktf_provider_dnsimple.email_forward",
         "cdktf_cdktf_provider_dnsimple.lets_encrypt_certificate",
         "cdktf_cdktf_provider_dnsimple.provider",
         "cdktf_cdktf_provider_dnsimple.zone_record"
     ],
     "package_data": {
         "cdktf_cdktf_provider_dnsimple._jsii": [
-            "provider-dnsimple@4.0.0.jsii.tgz"
+            "provider-dnsimple@5.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_dnsimple": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
-        "cdktf>=0.15.0, <0.16.0",
+        "cdktf>=0.16.0, <0.17.0",
         "constructs>=10.0.0, <11.0.0",
-        "jsii>=1.79.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 '''
-# Terraform CDK dnsimple Provider ~> 0.13
+# Terraform CDK dnsimple Provider ~> 1.0
 
 This repo builds and publishes the Terraform dnsimple Provider bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
@@ -51,15 +51,15 @@
 * [C#](./docs/API.csharp.md)
 * [Go](./docs/API.go.md)
 
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dnsimple).
 
 ## Versioning
 
-This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 0.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
+This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
 * [Terraform dnsimple Provider](https://github.com/terraform-providers/terraform-provider-dnsimple)
 * [Terraform Engine](https://terraform.io)
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dnsimple_certificate`
 
-Refer to the Terraform Registory for docs: [`data_dnsimple_certificate`](https://www.terraform.io/docs/providers/dnsimple/d/certificate).
+Refer to the Terraform Registory for docs: [`data_dnsimple_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataDnsimpleCertificate(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleCertificate.DataDnsimpleCertificate",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate dnsimple_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate dnsimple_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         certificate_id: jsii.Number,
         domain: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate dnsimple_certificate} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate dnsimple_certificate} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
-        :param domain: Domain name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#domain DataDnsimpleCertificate#domain}
+        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
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
 class DataDnsimpleCertificateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         certificate_id: jsii.Number,
         domain: builtins.str,
@@ -177,16 +177,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
-        :param domain: Domain name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#domain DataDnsimpleCertificate#domain}
+        :param certificate_id: Certificate ID. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        :param domain: Domain name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ca0765b33ca73367b3617b217b7c6b012e403c049ef5b5d2c6c9a819abce38da)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -223,20 +223,22 @@
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
@@ -278,25 +280,25 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def certificate_id(self) -> jsii.Number:
         '''Certificate ID.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#certificate_id DataDnsimpleCertificate#certificate_id}
         '''
         result = self._values.get("certificate_id")
         assert result is not None, "Required property 'certificate_id' is missing"
         return typing.cast(jsii.Number, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
         '''Domain name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/certificate#domain DataDnsimpleCertificate#domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/certificate#domain DataDnsimpleCertificate#domain}
         '''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -320,15 +322,15 @@
 def _typecheckingstub__d2e8d5ec9706be398631839424855548229e0ad79622ff5af4b02339407a3e7a(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     certificate_id: jsii.Number,
     domain: builtins.str,
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
@@ -345,15 +347,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ca0765b33ca73367b3617b217b7c6b012e403c049ef5b5d2c6c9a819abce38da(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     certificate_id: jsii.Number,
     domain: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_dnsimple_zone`
 
-Refer to the Terraform Registory for docs: [`data_dnsimple_zone`](https://www.terraform.io/docs/providers/dnsimple/d/zone).
+Refer to the Terraform Registory for docs: [`data_dnsimple_zone`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class DataDnsimpleZone(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.dataDnsimpleZone.DataDnsimpleZone",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/d/zone dnsimple_zone}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone dnsimple_zone}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/d/zone dnsimple_zone} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone dnsimple_zone} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Zone Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -129,15 +129,15 @@
     },
 )
 class DataDnsimpleZoneConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         name: builtins.str,
     ) -> None:
@@ -145,15 +145,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Zone Name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}
+        :param name: Zone Name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9051fabefb514091998aee3b06ffda795da4195d413ca0bc91120a12dc8cf592)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -188,20 +188,22 @@
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
@@ -243,15 +245,15 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
         '''Zone Name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/d/zone#name DataDnsimpleZone#name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/data-sources/zone#name DataDnsimpleZone#name}
         '''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
@@ -274,15 +276,15 @@
 
 def _typecheckingstub__8597ee60ee2d0bef88ca8a280aa616200a3cfaf788829f9b9a71b54907666f29(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     name: builtins.str,
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
@@ -293,15 +295,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9051fabefb514091998aee3b06ffda795da4195d413ca0bc91120a12dc8cf592(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/domain/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_domain`
 
-Refer to the Terraform Registory for docs: [`dnsimple_domain`](https://www.terraform.io/docs/providers/dnsimple/r/domain).
+Refer to the Terraform Registory for docs: [`dnsimple_domain`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,35 +22,35 @@
 
 
 class Domain(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.domain.Domain",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/domain dnsimple_domain}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain dnsimple_domain}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/domain dnsimple_domain} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain dnsimple_domain} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#name Domain#name}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain#name Domain#name}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -149,15 +149,15 @@
     },
 )
 class DomainConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         name: builtins.str,
     ) -> None:
@@ -165,15 +165,15 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#name Domain#name}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain#name Domain#name}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ccdf96388a7db479d080fabd9b5d7171adf0d0c2a040f80a4128b4e40eddb3d8)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -208,20 +208,22 @@
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
@@ -261,15 +263,15 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/domain#name Domain#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/domain#name Domain#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -291,15 +293,15 @@
 
 def _typecheckingstub__bfdaf63df24e37e02d8156377b8a72815d9c2f794e36891125e09f1d22c393b8(
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     name: builtins.str,
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
@@ -310,15 +312,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ccdf96388a7db479d080fabd9b5d7171adf0d0c2a040f80a4128b4e40eddb3d8(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
 ) -> None:
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_email_forward`
 
-Refer to the Terraform Registory for docs: [`dnsimple_email_forward`](https://www.terraform.io/docs/providers/dnsimple/r/email_forward).
+Refer to the Terraform Registory for docs: [`dnsimple_email_forward`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,39 +22,39 @@
 
 
 class EmailForward(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.emailForward.EmailForward",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward dnsimple_email_forward}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward dnsimple_email_forward}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias_name: builtins.str,
         destination_email: builtins.str,
         domain: builtins.str,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward dnsimple_email_forward} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward dnsimple_email_forward} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.
+        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#domain EmailForward#domain}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -166,15 +166,15 @@
     },
 )
 class EmailForwardConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         alias_name: builtins.str,
         destination_email: builtins.str,
@@ -184,17 +184,17 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param alias_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.
-        :param destination_email: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.
-        :param domain: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.
+        :param alias_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.
+        :param destination_email: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.
+        :param domain: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#domain EmailForward#domain}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -233,20 +233,22 @@
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
@@ -286,29 +288,29 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def alias_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#alias_name EmailForward#alias_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#alias_name EmailForward#alias_name}.'''
         result = self._values.get("alias_name")
         assert result is not None, "Required property 'alias_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def destination_email(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#destination_email EmailForward#destination_email}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#destination_email EmailForward#destination_email}.'''
         result = self._values.get("destination_email")
         assert result is not None, "Required property 'destination_email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def domain(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/email_forward#domain EmailForward#domain}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/email_forward#domain EmailForward#domain}.'''
         result = self._values.get("domain")
         assert result is not None, "Required property 'domain' is missing"
         return typing.cast(builtins.str, result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -332,15 +334,15 @@
     scope: _constructs_77d1e7e8.Construct,
     id: builtins.str,
     *,
     alias_name: builtins.str,
     destination_email: builtins.str,
     domain: builtins.str,
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
@@ -363,15 +365,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__7c6546ae8c4e2ee7d31438ac376a1ff2cb6b6c255b682e868b4941a86fc64016(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     alias_name: builtins.str,
     destination_email: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_lets_encrypt_certificate`
 
-Refer to the Terraform Registory for docs: [`dnsimple_lets_encrypt_certificate`](https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate).
+Refer to the Terraform Registory for docs: [`dnsimple_lets_encrypt_certificate`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class LetsEncryptCertificate(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.letsEncryptCertificate.LetsEncryptCertificate",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         domain_id: builtins.str,
         name: builtins.str,
         signature_algorithm: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate dnsimple_lets_encrypt_certificate} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param auto_renew: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
-        :param domain_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
-        :param signature_algorithm: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
+        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -226,15 +226,15 @@
     },
 )
 class LetsEncryptCertificateConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
         domain_id: builtins.str,
@@ -245,18 +245,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param auto_renew: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
-        :param domain_id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
-        :param signature_algorithm: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
+        :param auto_renew: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.
+        :param domain_id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.
+        :param signature_algorithm: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__850d843c640aa5551388a4b8af50716ee9c777d9927cb4bc9dda2315153cf876)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -298,20 +298,22 @@
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
@@ -351,36 +353,36 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def auto_renew(self) -> typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#auto_renew LetsEncryptCertificate#auto_renew}.'''
         result = self._values.get("auto_renew")
         assert result is not None, "Required property 'auto_renew' is missing"
         return typing.cast(typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable], result)
 
     @builtins.property
     def domain_id(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#domain_id LetsEncryptCertificate#domain_id}.'''
         result = self._values.get("domain_id")
         assert result is not None, "Required property 'domain_id' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#name LetsEncryptCertificate#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def signature_algorithm(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/lets_encrypt_certificate#signature_algorithm LetsEncryptCertificate#signature_algorithm}.'''
         result = self._values.get("signature_algorithm")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -404,15 +406,15 @@
     id: builtins.str,
     *,
     auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     domain_id: builtins.str,
     name: builtins.str,
     signature_algorithm: typing.Optional[builtins.str] = None,
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
@@ -441,15 +443,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__850d843c640aa5551388a4b8af50716ee9c777d9927cb4bc9dda2315153cf876(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     auto_renew: typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable],
     domain_id: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/provider/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`dnsimple`](https://www.terraform.io/docs/providers/dnsimple).
+Refer to the Terraform Registory for docs: [`dnsimple`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,38 +22,38 @@
 
 
 class DnsimpleProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.provider.DnsimpleProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple dnsimple}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs dnsimple}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         account: typing.Optional[builtins.str] = None,
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple dnsimple} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs dnsimple} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param account: The account for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#account DnsimpleProvider#account}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#alias DnsimpleProvider#alias}
-        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#prefetch DnsimpleProvider#prefetch}
-        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#sandbox DnsimpleProvider#sandbox}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
-        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#user_agent DnsimpleProvider#user_agent}
+        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#account DnsimpleProvider#account}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#alias DnsimpleProvider#alias}
+        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#prefetch DnsimpleProvider#prefetch}
+        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#token DnsimpleProvider#token}
+        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__e7ef56b7728822c45a23750e2602fff787208bfb71fa54a96467397e10a6e47c)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = DnsimpleProviderConfig(
             account=account,
@@ -236,20 +236,20 @@
         alias: typing.Optional[builtins.str] = None,
         prefetch: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         sandbox: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         token: typing.Optional[builtins.str] = None,
         user_agent: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param account: The account for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#account DnsimpleProvider#account}
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#alias DnsimpleProvider#alias}
-        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#prefetch DnsimpleProvider#prefetch}
-        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#sandbox DnsimpleProvider#sandbox}
-        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
-        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#user_agent DnsimpleProvider#user_agent}
+        :param account: The account for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#account DnsimpleProvider#account}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#alias DnsimpleProvider#alias}
+        :param prefetch: Flag to enable the prefetch of zone records. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#prefetch DnsimpleProvider#prefetch}
+        :param sandbox: Flag to enable the sandbox API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#sandbox DnsimpleProvider#sandbox}
+        :param token: The API v2 token for API operations. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#token DnsimpleProvider#token}
+        :param user_agent: Custom string to append to the user agent used for sending HTTP requests to the API. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__38b8bc1cdf1e0a8d7a730ac02381391ddfa090074fe8470d004c65b043c59d30)
             check_type(argname="argument account", value=account, expected_type=type_hints["account"])
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument prefetch", value=prefetch, expected_type=type_hints["prefetch"])
             check_type(argname="argument sandbox", value=sandbox, expected_type=type_hints["sandbox"])
@@ -269,64 +269,64 @@
         if user_agent is not None:
             self._values["user_agent"] = user_agent
 
     @builtins.property
     def account(self) -> typing.Optional[builtins.str]:
         '''The account for API operations.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#account DnsimpleProvider#account}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#account DnsimpleProvider#account}
         '''
         result = self._values.get("account")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#alias DnsimpleProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#alias DnsimpleProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def prefetch(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable the prefetch of zone records.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#prefetch DnsimpleProvider#prefetch}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#prefetch DnsimpleProvider#prefetch}
         '''
         result = self._values.get("prefetch")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def sandbox(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Flag to enable the sandbox API.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#sandbox DnsimpleProvider#sandbox}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#sandbox DnsimpleProvider#sandbox}
         '''
         result = self._values.get("sandbox")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def token(self) -> typing.Optional[builtins.str]:
         '''The API v2 token for API operations.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#token DnsimpleProvider#token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#token DnsimpleProvider#token}
         '''
         result = self._values.get("token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def user_agent(self) -> typing.Optional[builtins.str]:
         '''Custom string to append to the user agent used for sending HTTP requests to the API.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple#user_agent DnsimpleProvider#user_agent}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs#user_agent DnsimpleProvider#user_agent}
         '''
         result = self._values.get("user_agent")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `dnsimple_zone_record`
 
-Refer to the Terraform Registory for docs: [`dnsimple_zone_record`](https://www.terraform.io/docs/providers/dnsimple/r/zone_record).
+Refer to the Terraform Registory for docs: [`dnsimple_zone_record`](https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,45 +22,45 @@
 
 
 class ZoneRecord(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-dnsimple.zoneRecord.ZoneRecord",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record dnsimple_zone_record}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record dnsimple_zone_record}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         name: builtins.str,
         type: builtins.str,
         value: builtins.str,
         zone_name: builtins.str,
         priority: typing.Optional[jsii.Number] = None,
         ttl: typing.Optional[jsii.Number] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record dnsimple_zone_record} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record dnsimple_zone_record} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#name ZoneRecord#name}.
-        :param type: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#type ZoneRecord#type}.
-        :param value: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#value ZoneRecord#value}.
-        :param zone_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#zone_name ZoneRecord#zone_name}.
-        :param priority: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#priority ZoneRecord#priority}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#ttl ZoneRecord#ttl}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#priority ZoneRecord#priority}.
+        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -242,15 +242,15 @@
     },
 )
 class ZoneRecordConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         name: builtins.str,
         type: builtins.str,
@@ -263,20 +263,20 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#name ZoneRecord#name}.
-        :param type: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#type ZoneRecord#type}.
-        :param value: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#value ZoneRecord#value}.
-        :param zone_name: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#zone_name ZoneRecord#zone_name}.
-        :param priority: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#priority ZoneRecord#priority}.
-        :param ttl: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#ttl ZoneRecord#ttl}.
+        :param name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#name ZoneRecord#name}.
+        :param type: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#type ZoneRecord#type}.
+        :param value: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#value ZoneRecord#value}.
+        :param zone_name: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.
+        :param priority: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#priority ZoneRecord#priority}.
+        :param ttl: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__2eba6a2da1c8a28778529225bcbec0a1100d603698c12975ebeb143083f2fc0f)
             check_type(argname="argument connection", value=connection, expected_type=type_hints["connection"])
             check_type(argname="argument count", value=count, expected_type=type_hints["count"])
@@ -323,20 +323,22 @@
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
@@ -376,49 +378,49 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#name ZoneRecord#name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#name ZoneRecord#name}.'''
         result = self._values.get("name")
         assert result is not None, "Required property 'name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def type(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#type ZoneRecord#type}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#type ZoneRecord#type}.'''
         result = self._values.get("type")
         assert result is not None, "Required property 'type' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def value(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#value ZoneRecord#value}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#value ZoneRecord#value}.'''
         result = self._values.get("value")
         assert result is not None, "Required property 'value' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def zone_name(self) -> builtins.str:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#zone_name ZoneRecord#zone_name}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#zone_name ZoneRecord#zone_name}.'''
         result = self._values.get("zone_name")
         assert result is not None, "Required property 'zone_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def priority(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#priority ZoneRecord#priority}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#priority ZoneRecord#priority}.'''
         result = self._values.get("priority")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
     def ttl(self) -> typing.Optional[jsii.Number]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/dnsimple/r/zone_record#ttl ZoneRecord#ttl}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/dnsimple/dnsimple/1.0.0/docs/resources/zone_record#ttl ZoneRecord#ttl}.'''
         result = self._values.get("ttl")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -444,15 +446,15 @@
     name: builtins.str,
     type: builtins.str,
     value: builtins.str,
     zone_name: builtins.str,
     priority: typing.Optional[jsii.Number] = None,
     ttl: typing.Optional[jsii.Number] = None,
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
@@ -493,15 +495,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__2eba6a2da1c8a28778529225bcbec0a1100d603698c12975ebeb143083f2fc0f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     name: builtins.str,
     type: builtins.str,
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-dnsimple
-Version: 4.0.0
+Version: 5.0.0
 Summary: Prebuilt dnsimple Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-dnsimple.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-dnsimple.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -18,15 +18,15 @@
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Terraform CDK dnsimple Provider ~> 0.13
+# Terraform CDK dnsimple Provider ~> 1.0
 
 This repo builds and publishes the Terraform dnsimple Provider bindings for [CDK for Terraform](https://cdk.tf).
 
 ## Available Packages
 
 ### NPM
 
@@ -74,15 +74,15 @@
 * [C#](./docs/API.csharp.md)
 * [Go](./docs/API.go.md)
 
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-dnsimple).
 
 ## Versioning
 
-This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 0.13` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
+This project is explicitly not tracking the Terraform dnsimple Provider version 1:1. In fact, it always tracks `latest` of `~> 1.0` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
 
 * [Terraform CDK](https://cdk.tf)
 * [Terraform dnsimple Provider](https://github.com/terraform-providers/terraform-provider-dnsimple)
 * [Terraform Engine](https://terraform.io)
```

### Comparing `cdktf-cdktf-provider-dnsimple-4.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-dnsimple-5.0.0/src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_dnsimple/py.typed
 src/cdktf_cdktf_provider_dnsimple.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_dnsimple.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/requires.txt
 src/cdktf_cdktf_provider_dnsimple.egg-info/top_level.txt
 src/cdktf_cdktf_provider_dnsimple/_jsii/__init__.py
-src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@4.0.0.jsii.tgz
+src/cdktf_cdktf_provider_dnsimple/_jsii/provider-dnsimple@5.0.0.jsii.tgz
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/data_dnsimple_zone/__init__.py
 src/cdktf_cdktf_provider_dnsimple/domain/__init__.py
 src/cdktf_cdktf_provider_dnsimple/email_forward/__init__.py
 src/cdktf_cdktf_provider_dnsimple/lets_encrypt_certificate/__init__.py
 src/cdktf_cdktf_provider_dnsimple/provider/__init__.py
 src/cdktf_cdktf_provider_dnsimple/zone_record/__init__.py
```

