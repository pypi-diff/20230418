# Comparing `tmp/cdktf-cdktf-provider-hcs-3.0.0.tar.gz` & `tmp/cdktf-cdktf-provider-hcs-4.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-cdktf-provider-hcs-3.0.0.tar", last modified: Tue Jan 17 14:55:44 2023, max compression
+gzip compressed data, was "cdktf-cdktf-provider-hcs-4.0.0.tar", last modified: Tue Apr 18 20:42:56 2023, max compression
```

## Comparing `cdktf-cdktf-provider-hcs-3.0.0.tar` & `cdktf-cdktf-provider-hcs-4.0.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2322 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.034664 cdktf-cdktf-provider-hcs-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   120222 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@3.0.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    78698 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/
--rw-r--r--   0 runner    (1001) docker     (123)    29093 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/
--rw-r--r--   0 runner    (1001) docker     (123)    37933 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/
--rw-r--r--   0 runner    (1001) docker     (123)    29435 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/
--rw-r--r--   0 runner    (1001) docker     (123)    36522 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/
--rw-r--r--   0 runner    (1001) docker     (123)    24090 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/
--rw-r--r--   0 runner    (1001) docker     (123)    28978 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/
--rw-r--r--   0 runner    (1001) docker     (123)    24086 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/provider/
--rw-r--r--   0 runner    (1001) docker     (123)    40842 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/snapshot/
--rw-r--r--   0 runner    (1001) docker     (123)    37130 2023-01-17 14:55:30.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-17 14:55:44.038664 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3888 2023-01-17 14:55:43.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-01-17 14:55:44.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-17 14:55:43.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-01-17 14:55:43.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-01-17 14:55:43.000000 cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    16012 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   371955 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@4.0.0.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    80990 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    29906 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/
+-rw-r--r--   0 runner    (1001) docker     (123)    39088 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/
+-rw-r--r--   0 runner    (1001) docker     (123)    30302 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)    37485 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/
+-rw-r--r--   0 runner    (1001) docker     (123)    24765 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/
+-rw-r--r--   0 runner    (1001) docker     (123)    29845 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)    24761 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/provider/
+-rw-r--r--   0 runner    (1001) docker     (123)    41724 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.635041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (123)    38291 2023-04-18 20:42:41.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:42:56.631041 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 20:42:56.000000 cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/top_level.txt
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/LICENSE` & `cdktf-cdktf-provider-hcs-4.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/PKG-INFO` & `cdktf-cdktf-provider-hcs-4.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcs
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt hcs Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcs.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcs.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hcs-go`](https://github.com/cdktf/cdktf-provider-hcs-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hcs-go/hcs`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hcs).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/README.md` & `cdktf-cdktf-provider-hcs-4.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -38,15 +38,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hcs-go`](https://github.com/cdktf/cdktf-provider-hcs-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hcs-go/hcs`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hcs).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/setup.py` & `cdktf-cdktf-provider-hcs-4.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-cdktf-provider-hcs",
-    "version": "3.0.0",
+    "version": "4.0.0",
     "description": "Prebuilt hcs Provider for Terraform CDK (cdktf)",
     "license": "MPL-2.0",
     "url": "https://github.com/cdktf/cdktf-provider-hcs.git",
     "long_description_content_type": "text/markdown",
     "author": "HashiCorp",
     "bdist_wheel": {
         "universal": true
@@ -32,37 +32,38 @@
         "cdktf_cdktf_provider_hcs.data_hcs_federation_token",
         "cdktf_cdktf_provider_hcs.data_hcs_plan_defaults",
         "cdktf_cdktf_provider_hcs.provider",
         "cdktf_cdktf_provider_hcs.snapshot"
     ],
     "package_data": {
         "cdktf_cdktf_provider_hcs._jsii": [
-            "provider-hcs@3.0.0.jsii.tgz"
+            "provider-hcs@4.0.0.jsii.tgz"
         ],
         "cdktf_cdktf_provider_hcs": [
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

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,22 @@
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hcs-go`](https://github.com/cdktf/cdktf-provider-hcs-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hcs-go/hcs`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hcs).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/cluster/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcs_cluster`
 
-Refer to the Terraform Registory for docs: [`hcs_cluster`](https://www.terraform.io/docs/providers/hcs/r/cluster).
+Refer to the Terraform Registory for docs: [`hcs_cluster`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class Cluster(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.cluster.Cluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/r/cluster hcs_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster hcs_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         cluster_mode: builtins.str,
@@ -48,43 +48,43 @@
         managed_resource_group_name: typing.Optional[builtins.str] = None,
         min_consul_version: typing.Optional[builtins.str] = None,
         plan_name: typing.Optional[builtins.str] = None,
         tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
         timeouts: typing.Optional[typing.Union["ClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         vnet_cidr: typing.Optional[builtins.str] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/r/cluster hcs_cluster} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster hcs_cluster} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param cluster_mode: The mode of the cluster ('Development' or 'Production'). Development clusters only have a single Consul server. Production clusters are fully supported, full featured, and deploy with a minimum of three hosts. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#cluster_mode Cluster#cluster_mode}
-        :param email: The contact email for the primary owner of the cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#email Cluster#email}
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#managed_application_name Cluster#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#resource_group_name Cluster#resource_group_name}
-        :param audit_logging_enabled: Enables Consul audit logging for the cluster resource. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#audit_logging_enabled Cluster#audit_logging_enabled}
-        :param audit_log_storage_container_url: The url of the Azure blob storage container to write audit logs to if ``audit_logging_enabled`` is ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#audit_log_storage_container_url Cluster#audit_log_storage_container_url}
-        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#cluster_name Cluster#cluster_name}
-        :param consul_datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_datacenter Cluster#consul_datacenter}
-        :param consul_external_endpoint: Denotes that the cluster has an external endpoint for the Consul UI. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_external_endpoint Cluster#consul_external_endpoint}
-        :param consul_federation_token: The token used to join a federation of Consul clusters. If the cluster is not part of a federation, this field will be empty. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_federation_token Cluster#consul_federation_token}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#id Cluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param location: The Azure region that the cluster is deployed to. If not specified, it is defaulted to the region of the Resource Group the Managed Application belongs to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#location Cluster#location}
-        :param managed_resource_group_name: The name of the Managed Resource Group in which the cluster resources belong. If not specified, it is defaulted to the value of ``managed_application_name`` with 'mrg-' prepended. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#managed_resource_group_name Cluster#managed_resource_group_name}
-        :param min_consul_version: The minimum Consul version of the cluster. If not specified, it is defaulted to the version that is currently recommended by HCS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#min_consul_version Cluster#min_consul_version}
-        :param plan_name: The name of the Azure Marketplace HCS plan for the cluster. If not specified, it will default to the current HCS default plan (see the ``hcs_plan_defaults`` data source). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#plan_name Cluster#plan_name}
-        :param tags: A mapping of tags to assign to the HCS Azure Managed Application resource. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#tags Cluster#tags}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#timeouts Cluster#timeouts}
-        :param vnet_cidr: The VNET CIDR range of the Consul cluster. Defaults to ``172.25.16.0/24``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#vnet_cidr Cluster#vnet_cidr}
+        :param cluster_mode: The mode of the cluster ('Development' or 'Production'). Development clusters only have a single Consul server. Production clusters are fully supported, full featured, and deploy with a minimum of three hosts. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#cluster_mode Cluster#cluster_mode}
+        :param email: The contact email for the primary owner of the cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#email Cluster#email}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#managed_application_name Cluster#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#resource_group_name Cluster#resource_group_name}
+        :param audit_logging_enabled: Enables Consul audit logging for the cluster resource. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#audit_logging_enabled Cluster#audit_logging_enabled}
+        :param audit_log_storage_container_url: The url of the Azure blob storage container to write audit logs to if ``audit_logging_enabled`` is ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#audit_log_storage_container_url Cluster#audit_log_storage_container_url}
+        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#cluster_name Cluster#cluster_name}
+        :param consul_datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_datacenter Cluster#consul_datacenter}
+        :param consul_external_endpoint: Denotes that the cluster has an external endpoint for the Consul UI. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_external_endpoint Cluster#consul_external_endpoint}
+        :param consul_federation_token: The token used to join a federation of Consul clusters. If the cluster is not part of a federation, this field will be empty. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_federation_token Cluster#consul_federation_token}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#id Cluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param location: The Azure region that the cluster is deployed to. If not specified, it is defaulted to the region of the Resource Group the Managed Application belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#location Cluster#location}
+        :param managed_resource_group_name: The name of the Managed Resource Group in which the cluster resources belong. If not specified, it is defaulted to the value of ``managed_application_name`` with 'mrg-' prepended. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#managed_resource_group_name Cluster#managed_resource_group_name}
+        :param min_consul_version: The minimum Consul version of the cluster. If not specified, it is defaulted to the version that is currently recommended by HCS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#min_consul_version Cluster#min_consul_version}
+        :param plan_name: The name of the Azure Marketplace HCS plan for the cluster. If not specified, it will default to the current HCS default plan (see the ``hcs_plan_defaults`` data source). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#plan_name Cluster#plan_name}
+        :param tags: A mapping of tags to assign to the HCS Azure Managed Application resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#tags Cluster#tags}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#timeouts Cluster#timeouts}
+        :param vnet_cidr: The VNET CIDR range of the Consul cluster. Defaults to ``172.25.16.0/24``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#vnet_cidr Cluster#vnet_cidr}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -129,18 +129,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#create Cluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#default Cluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#delete Cluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#update Cluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#create Cluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#default Cluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#delete Cluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#update Cluster#update}.
         '''
         value = ClusterTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -662,15 +662,15 @@
     },
 )
 class ClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         cluster_mode: builtins.str,
         email: builtins.str,
@@ -695,32 +695,32 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param cluster_mode: The mode of the cluster ('Development' or 'Production'). Development clusters only have a single Consul server. Production clusters are fully supported, full featured, and deploy with a minimum of three hosts. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#cluster_mode Cluster#cluster_mode}
-        :param email: The contact email for the primary owner of the cluster. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#email Cluster#email}
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#managed_application_name Cluster#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#resource_group_name Cluster#resource_group_name}
-        :param audit_logging_enabled: Enables Consul audit logging for the cluster resource. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#audit_logging_enabled Cluster#audit_logging_enabled}
-        :param audit_log_storage_container_url: The url of the Azure blob storage container to write audit logs to if ``audit_logging_enabled`` is ``true``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#audit_log_storage_container_url Cluster#audit_log_storage_container_url}
-        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#cluster_name Cluster#cluster_name}
-        :param consul_datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_datacenter Cluster#consul_datacenter}
-        :param consul_external_endpoint: Denotes that the cluster has an external endpoint for the Consul UI. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_external_endpoint Cluster#consul_external_endpoint}
-        :param consul_federation_token: The token used to join a federation of Consul clusters. If the cluster is not part of a federation, this field will be empty. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_federation_token Cluster#consul_federation_token}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#id Cluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param location: The Azure region that the cluster is deployed to. If not specified, it is defaulted to the region of the Resource Group the Managed Application belongs to. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#location Cluster#location}
-        :param managed_resource_group_name: The name of the Managed Resource Group in which the cluster resources belong. If not specified, it is defaulted to the value of ``managed_application_name`` with 'mrg-' prepended. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#managed_resource_group_name Cluster#managed_resource_group_name}
-        :param min_consul_version: The minimum Consul version of the cluster. If not specified, it is defaulted to the version that is currently recommended by HCS. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#min_consul_version Cluster#min_consul_version}
-        :param plan_name: The name of the Azure Marketplace HCS plan for the cluster. If not specified, it will default to the current HCS default plan (see the ``hcs_plan_defaults`` data source). Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#plan_name Cluster#plan_name}
-        :param tags: A mapping of tags to assign to the HCS Azure Managed Application resource. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#tags Cluster#tags}
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#timeouts Cluster#timeouts}
-        :param vnet_cidr: The VNET CIDR range of the Consul cluster. Defaults to ``172.25.16.0/24``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#vnet_cidr Cluster#vnet_cidr}
+        :param cluster_mode: The mode of the cluster ('Development' or 'Production'). Development clusters only have a single Consul server. Production clusters are fully supported, full featured, and deploy with a minimum of three hosts. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#cluster_mode Cluster#cluster_mode}
+        :param email: The contact email for the primary owner of the cluster. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#email Cluster#email}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#managed_application_name Cluster#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#resource_group_name Cluster#resource_group_name}
+        :param audit_logging_enabled: Enables Consul audit logging for the cluster resource. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#audit_logging_enabled Cluster#audit_logging_enabled}
+        :param audit_log_storage_container_url: The url of the Azure blob storage container to write audit logs to if ``audit_logging_enabled`` is ``true``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#audit_log_storage_container_url Cluster#audit_log_storage_container_url}
+        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#cluster_name Cluster#cluster_name}
+        :param consul_datacenter: The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_datacenter Cluster#consul_datacenter}
+        :param consul_external_endpoint: Denotes that the cluster has an external endpoint for the Consul UI. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_external_endpoint Cluster#consul_external_endpoint}
+        :param consul_federation_token: The token used to join a federation of Consul clusters. If the cluster is not part of a federation, this field will be empty. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_federation_token Cluster#consul_federation_token}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#id Cluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param location: The Azure region that the cluster is deployed to. If not specified, it is defaulted to the region of the Resource Group the Managed Application belongs to. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#location Cluster#location}
+        :param managed_resource_group_name: The name of the Managed Resource Group in which the cluster resources belong. If not specified, it is defaulted to the value of ``managed_application_name`` with 'mrg-' prepended. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#managed_resource_group_name Cluster#managed_resource_group_name}
+        :param min_consul_version: The minimum Consul version of the cluster. If not specified, it is defaulted to the version that is currently recommended by HCS. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#min_consul_version Cluster#min_consul_version}
+        :param plan_name: The name of the Azure Marketplace HCS plan for the cluster. If not specified, it will default to the current HCS default plan (see the ``hcs_plan_defaults`` data source). Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#plan_name Cluster#plan_name}
+        :param tags: A mapping of tags to assign to the HCS Azure Managed Application resource. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#tags Cluster#tags}
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#timeouts Cluster#timeouts}
+        :param vnet_cidr: The VNET CIDR range of the Consul cluster. Defaults to ``172.25.16.0/24``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#vnet_cidr Cluster#vnet_cidr}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__c63368dfdd2ff38e35ab9bb268933364f25c1ab1479d0d08849b566e1aba6d57)
@@ -805,20 +805,22 @@
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
@@ -862,187 +864,187 @@
 
     @builtins.property
     def cluster_mode(self) -> builtins.str:
         '''The mode of the cluster ('Development' or 'Production').
 
         Development clusters only have a single Consul server. Production clusters are fully supported, full featured, and deploy with a minimum of three hosts.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#cluster_mode Cluster#cluster_mode}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#cluster_mode Cluster#cluster_mode}
         '''
         result = self._values.get("cluster_mode")
         assert result is not None, "Required property 'cluster_mode' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def email(self) -> builtins.str:
         '''The contact email for the primary owner of the cluster.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#email Cluster#email}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#email Cluster#email}
         '''
         result = self._values.get("email")
         assert result is not None, "Required property 'email' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#managed_application_name Cluster#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#managed_application_name Cluster#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#resource_group_name Cluster#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#resource_group_name Cluster#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def audit_logging_enabled(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Enables Consul audit logging for the cluster resource. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#audit_logging_enabled Cluster#audit_logging_enabled}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#audit_logging_enabled Cluster#audit_logging_enabled}
         '''
         result = self._values.get("audit_logging_enabled")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def audit_log_storage_container_url(self) -> typing.Optional[builtins.str]:
         '''The url of the Azure blob storage container to write audit logs to if ``audit_logging_enabled`` is ``true``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#audit_log_storage_container_url Cluster#audit_log_storage_container_url}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#audit_log_storage_container_url Cluster#audit_log_storage_container_url}
         '''
         result = self._values.get("audit_log_storage_container_url")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def cluster_name(self) -> typing.Optional[builtins.str]:
         '''The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#cluster_name Cluster#cluster_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#cluster_name Cluster#cluster_name}
         '''
         result = self._values.get("cluster_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def consul_datacenter(self) -> typing.Optional[builtins.str]:
         '''The Consul data center name of the cluster. If not specified, it is defaulted to the value of ``managed_application_name``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_datacenter Cluster#consul_datacenter}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_datacenter Cluster#consul_datacenter}
         '''
         result = self._values.get("consul_datacenter")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def consul_external_endpoint(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the cluster has an external endpoint for the Consul UI. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_external_endpoint Cluster#consul_external_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_external_endpoint Cluster#consul_external_endpoint}
         '''
         result = self._values.get("consul_external_endpoint")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def consul_federation_token(self) -> typing.Optional[builtins.str]:
         '''The token used to join a federation of Consul clusters.
 
         If the cluster is not part of a federation, this field will be empty.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#consul_federation_token Cluster#consul_federation_token}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#consul_federation_token Cluster#consul_federation_token}
         '''
         result = self._values.get("consul_federation_token")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#id Cluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#id Cluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def location(self) -> typing.Optional[builtins.str]:
         '''The Azure region that the cluster is deployed to.
 
         If not specified, it is defaulted to the region of the Resource Group the Managed Application belongs to.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#location Cluster#location}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#location Cluster#location}
         '''
         result = self._values.get("location")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def managed_resource_group_name(self) -> typing.Optional[builtins.str]:
         '''The name of the Managed Resource Group in which the cluster resources belong.
 
         If not specified, it is defaulted to the value of ``managed_application_name`` with 'mrg-' prepended.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#managed_resource_group_name Cluster#managed_resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#managed_resource_group_name Cluster#managed_resource_group_name}
         '''
         result = self._values.get("managed_resource_group_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def min_consul_version(self) -> typing.Optional[builtins.str]:
         '''The minimum Consul version of the cluster.
 
         If not specified, it is defaulted to the version that is currently recommended by HCS.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#min_consul_version Cluster#min_consul_version}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#min_consul_version Cluster#min_consul_version}
         '''
         result = self._values.get("min_consul_version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def plan_name(self) -> typing.Optional[builtins.str]:
         '''The name of the Azure Marketplace HCS plan for the cluster.
 
         If not specified, it will default to the current HCS default plan (see the ``hcs_plan_defaults`` data source).
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#plan_name Cluster#plan_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#plan_name Cluster#plan_name}
         '''
         result = self._values.get("plan_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def tags(self) -> typing.Optional[typing.Mapping[builtins.str, builtins.str]]:
         '''A mapping of tags to assign to the HCS Azure Managed Application resource.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#tags Cluster#tags}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#tags Cluster#tags}
         '''
         result = self._values.get("tags")
         return typing.cast(typing.Optional[typing.Mapping[builtins.str, builtins.str]], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#timeouts Cluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#timeouts Cluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ClusterTimeouts"], result)
 
     @builtins.property
     def vnet_cidr(self) -> typing.Optional[builtins.str]:
         '''The VNET CIDR range of the Consul cluster. Defaults to ``172.25.16.0/24``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#vnet_cidr Cluster#vnet_cidr}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#vnet_cidr Cluster#vnet_cidr}
         '''
         result = self._values.get("vnet_cidr")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -1071,18 +1073,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#create Cluster#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#default Cluster#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#delete Cluster#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#update Cluster#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#create Cluster#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#default Cluster#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#delete Cluster#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#update Cluster#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__adb1c8914ba141a3043ca4f69a745e8abe29b095e34a214799e108d8e8f0fb58)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -1094,33 +1096,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#create Cluster#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#create Cluster#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#default Cluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#default Cluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#delete Cluster#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#delete Cluster#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster#update Cluster#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster#update Cluster#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -1282,15 +1284,15 @@
     managed_resource_group_name: typing.Optional[builtins.str] = None,
     min_consul_version: typing.Optional[builtins.str] = None,
     plan_name: typing.Optional[builtins.str] = None,
     tags: typing.Optional[typing.Mapping[builtins.str, builtins.str]] = None,
     timeouts: typing.Optional[typing.Union[ClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
     vnet_cidr: typing.Optional[builtins.str] = None,
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
@@ -1397,15 +1399,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c63368dfdd2ff38e35ab9bb268933364f25c1ab1479d0d08849b566e1aba6d57(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     cluster_mode: builtins.str,
     email: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcs_cluster_root_token`
 
-Refer to the Terraform Registory for docs: [`hcs_cluster_root_token`](https://www.terraform.io/docs/providers/hcs/r/cluster_root_token).
+Refer to the Terraform Registory for docs: [`hcs_cluster_root_token`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class ClusterRootToken(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.clusterRootToken.ClusterRootToken",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token hcs_cluster_root_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token hcs_cluster_root_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["ClusterRootTokenTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token hcs_cluster_root_token} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token hcs_cluster_root_token} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#managed_application_name ClusterRootToken#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#resource_group_name ClusterRootToken#resource_group_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#id ClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#timeouts ClusterRootToken#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#managed_application_name ClusterRootToken#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#resource_group_name ClusterRootToken#resource_group_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#id ClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#timeouts ClusterRootToken#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#default ClusterRootToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#default ClusterRootToken#default}.
         '''
         value = ClusterRootTokenTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -204,15 +204,15 @@
     },
 )
 class ClusterRootTokenConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
@@ -223,18 +223,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#managed_application_name ClusterRootToken#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#resource_group_name ClusterRootToken#resource_group_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#id ClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#timeouts ClusterRootToken#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#managed_application_name ClusterRootToken#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#resource_group_name ClusterRootToken#resource_group_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#id ClusterRootToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#timeouts ClusterRootToken#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = ClusterRootTokenTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__eb4d5a0488d994a289314017052a55e0f9dcd6c7949f3de7e5e76a9b168e5d5f)
@@ -279,20 +279,22 @@
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
@@ -334,45 +336,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#managed_application_name ClusterRootToken#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#managed_application_name ClusterRootToken#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#resource_group_name ClusterRootToken#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#resource_group_name ClusterRootToken#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#id ClusterRootToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#id ClusterRootToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["ClusterRootTokenTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#timeouts ClusterRootToken#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#timeouts ClusterRootToken#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["ClusterRootTokenTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -389,26 +391,26 @@
     jsii_type="@cdktf/provider-hcs.clusterRootToken.ClusterRootTokenTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class ClusterRootTokenTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#default ClusterRootToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#default ClusterRootToken#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__fdf792dccf70d0f7598c834dc02d0ef42fdb09ab6d14f82591d49058e3449e42)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/cluster_root_token#default ClusterRootToken#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/cluster_root_token#default ClusterRootToken#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -493,15 +495,15 @@
     id_: builtins.str,
     *,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[ClusterRootTokenTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -524,15 +526,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__eb4d5a0488d994a289314017052a55e0f9dcd6c7949f3de7e5e76a9b168e5d5f(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcs_agent_helm_config`
 
-Refer to the Terraform Registory for docs: [`data_hcs_agent_helm_config`](https://www.terraform.io/docs/providers/hcs/d/agent_helm_config).
+Refer to the Terraform Registory for docs: [`data_hcs_agent_helm_config`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,47 +22,47 @@
 
 
 class DataHcsAgentHelmConfig(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.dataHcsAgentHelmConfig.DataHcsAgentHelmConfig",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config hcs_agent_helm_config}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config hcs_agent_helm_config}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         aks_cluster_name: builtins.str,
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
         aks_resource_group: typing.Optional[builtins.str] = None,
         expose_gossip_ports: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsAgentHelmConfigTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config hcs_agent_helm_config} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config hcs_agent_helm_config} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param aks_cluster_name: The name of the AKS cluster that will consume the Helm config. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#aks_cluster_name DataHcsAgentHelmConfig#aks_cluster_name}
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#managed_application_name DataHcsAgentHelmConfig#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#resource_group_name DataHcsAgentHelmConfig#resource_group_name}
-        :param aks_resource_group: The resource group name of the AKS cluster that will consume the Helm config. If not specified, it is defaulted to the value of ``resource_group_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#aks_resource_group DataHcsAgentHelmConfig#aks_resource_group}
-        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#expose_gossip_ports DataHcsAgentHelmConfig#expose_gossip_ports}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#id DataHcsAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#timeouts DataHcsAgentHelmConfig#timeouts}
+        :param aks_cluster_name: The name of the AKS cluster that will consume the Helm config. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#aks_cluster_name DataHcsAgentHelmConfig#aks_cluster_name}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#managed_application_name DataHcsAgentHelmConfig#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#resource_group_name DataHcsAgentHelmConfig#resource_group_name}
+        :param aks_resource_group: The resource group name of the AKS cluster that will consume the Helm config. If not specified, it is defaulted to the value of ``resource_group_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#aks_resource_group DataHcsAgentHelmConfig#aks_resource_group}
+        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#expose_gossip_ports DataHcsAgentHelmConfig#expose_gossip_ports}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#id DataHcsAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#timeouts DataHcsAgentHelmConfig#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -89,15 +89,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#default DataHcsAgentHelmConfig#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#default DataHcsAgentHelmConfig#default}.
         '''
         value = DataHcsAgentHelmConfigTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetAksResourceGroup")
     def reset_aks_resource_group(self) -> None:
@@ -272,15 +272,15 @@
     },
 )
 class DataHcsAgentHelmConfigConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         aks_cluster_name: builtins.str,
         managed_application_name: builtins.str,
@@ -294,21 +294,21 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param aks_cluster_name: The name of the AKS cluster that will consume the Helm config. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#aks_cluster_name DataHcsAgentHelmConfig#aks_cluster_name}
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#managed_application_name DataHcsAgentHelmConfig#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#resource_group_name DataHcsAgentHelmConfig#resource_group_name}
-        :param aks_resource_group: The resource group name of the AKS cluster that will consume the Helm config. If not specified, it is defaulted to the value of ``resource_group_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#aks_resource_group DataHcsAgentHelmConfig#aks_resource_group}
-        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Defaults to ``false``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#expose_gossip_ports DataHcsAgentHelmConfig#expose_gossip_ports}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#id DataHcsAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#timeouts DataHcsAgentHelmConfig#timeouts}
+        :param aks_cluster_name: The name of the AKS cluster that will consume the Helm config. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#aks_cluster_name DataHcsAgentHelmConfig#aks_cluster_name}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#managed_application_name DataHcsAgentHelmConfig#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#resource_group_name DataHcsAgentHelmConfig#resource_group_name}
+        :param aks_resource_group: The resource group name of the AKS cluster that will consume the Helm config. If not specified, it is defaulted to the value of ``resource_group_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#aks_resource_group DataHcsAgentHelmConfig#aks_resource_group}
+        :param expose_gossip_ports: Denotes that the gossip ports should be exposed. Defaults to ``false``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#expose_gossip_ports DataHcsAgentHelmConfig#expose_gossip_ports}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#id DataHcsAgentHelmConfig#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#timeouts DataHcsAgentHelmConfig#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcsAgentHelmConfigTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__386071b81fe90224564de50429e997464ad66eabe8214cdeea78f41581953ab9)
@@ -361,20 +361,22 @@
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
@@ -416,77 +418,77 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def aks_cluster_name(self) -> builtins.str:
         '''The name of the AKS cluster that will consume the Helm config.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#aks_cluster_name DataHcsAgentHelmConfig#aks_cluster_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#aks_cluster_name DataHcsAgentHelmConfig#aks_cluster_name}
         '''
         result = self._values.get("aks_cluster_name")
         assert result is not None, "Required property 'aks_cluster_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#managed_application_name DataHcsAgentHelmConfig#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#managed_application_name DataHcsAgentHelmConfig#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#resource_group_name DataHcsAgentHelmConfig#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#resource_group_name DataHcsAgentHelmConfig#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def aks_resource_group(self) -> typing.Optional[builtins.str]:
         '''The resource group name of the AKS cluster that will consume the Helm config.
 
         If not specified, it is defaulted to the value of ``resource_group_name``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#aks_resource_group DataHcsAgentHelmConfig#aks_resource_group}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#aks_resource_group DataHcsAgentHelmConfig#aks_resource_group}
         '''
         result = self._values.get("aks_resource_group")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def expose_gossip_ports(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Denotes that the gossip ports should be exposed. Defaults to ``false``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#expose_gossip_ports DataHcsAgentHelmConfig#expose_gossip_ports}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#expose_gossip_ports DataHcsAgentHelmConfig#expose_gossip_ports}
         '''
         result = self._values.get("expose_gossip_ports")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#id DataHcsAgentHelmConfig#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#id DataHcsAgentHelmConfig#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcsAgentHelmConfigTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#timeouts DataHcsAgentHelmConfig#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#timeouts DataHcsAgentHelmConfig#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcsAgentHelmConfigTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -503,26 +505,26 @@
     jsii_type="@cdktf/provider-hcs.dataHcsAgentHelmConfig.DataHcsAgentHelmConfigTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcsAgentHelmConfigTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#default DataHcsAgentHelmConfig#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#default DataHcsAgentHelmConfig#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__dce99136ec54c0e4bb9f792a7b65a267abaca3501d49144f19fbbacb451d309c)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_helm_config#default DataHcsAgentHelmConfig#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_helm_config#default DataHcsAgentHelmConfig#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -610,15 +612,15 @@
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
     aks_resource_group: typing.Optional[builtins.str] = None,
     expose_gossip_ports: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsAgentHelmConfigTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -659,15 +661,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__386071b81fe90224564de50429e997464ad66eabe8214cdeea78f41581953ab9(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     aks_cluster_name: builtins.str,
     managed_application_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcs_agent_kubernetes_secret`
 
-Refer to the Terraform Registory for docs: [`data_hcs_agent_kubernetes_secret`](https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret).
+Refer to the Terraform Registory for docs: [`data_hcs_agent_kubernetes_secret`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataHcsAgentKubernetesSecret(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.dataHcsAgentKubernetesSecret.DataHcsAgentKubernetesSecret",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret hcs_agent_kubernetes_secret}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret hcs_agent_kubernetes_secret}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsAgentKubernetesSecretTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret hcs_agent_kubernetes_secret} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret hcs_agent_kubernetes_secret} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#managed_application_name DataHcsAgentKubernetesSecret#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#resource_group_name DataHcsAgentKubernetesSecret#resource_group_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#id DataHcsAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#timeouts DataHcsAgentKubernetesSecret#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#managed_application_name DataHcsAgentKubernetesSecret#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#resource_group_name DataHcsAgentKubernetesSecret#resource_group_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#id DataHcsAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#timeouts DataHcsAgentKubernetesSecret#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#default DataHcsAgentKubernetesSecret#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#default DataHcsAgentKubernetesSecret#default}.
         '''
         value = DataHcsAgentKubernetesSecretTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -194,15 +194,15 @@
     },
 )
 class DataHcsAgentKubernetesSecretConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
@@ -213,18 +213,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#managed_application_name DataHcsAgentKubernetesSecret#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#resource_group_name DataHcsAgentKubernetesSecret#resource_group_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#id DataHcsAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#timeouts DataHcsAgentKubernetesSecret#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#managed_application_name DataHcsAgentKubernetesSecret#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#resource_group_name DataHcsAgentKubernetesSecret#resource_group_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#id DataHcsAgentKubernetesSecret#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#timeouts DataHcsAgentKubernetesSecret#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcsAgentKubernetesSecretTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d1f10b6eba45fb8d9c81d99484d336e751c678dcc99fe7248b9bc061c6ff3a5b)
@@ -269,20 +269,22 @@
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
@@ -324,45 +326,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#managed_application_name DataHcsAgentKubernetesSecret#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#managed_application_name DataHcsAgentKubernetesSecret#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#resource_group_name DataHcsAgentKubernetesSecret#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#resource_group_name DataHcsAgentKubernetesSecret#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#id DataHcsAgentKubernetesSecret#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#id DataHcsAgentKubernetesSecret#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcsAgentKubernetesSecretTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#timeouts DataHcsAgentKubernetesSecret#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#timeouts DataHcsAgentKubernetesSecret#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcsAgentKubernetesSecretTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -379,26 +381,26 @@
     jsii_type="@cdktf/provider-hcs.dataHcsAgentKubernetesSecret.DataHcsAgentKubernetesSecretTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcsAgentKubernetesSecretTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#default DataHcsAgentKubernetesSecret#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#default DataHcsAgentKubernetesSecret#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__4bce64d1f39264b17ef9528479642f6a7c99bdd3393d9c93a5dc50d6be59863d)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/agent_kubernetes_secret#default DataHcsAgentKubernetesSecret#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/agent_kubernetes_secret#default DataHcsAgentKubernetesSecret#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -483,15 +485,15 @@
     id_: builtins.str,
     *,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsAgentKubernetesSecretTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -514,15 +516,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__d1f10b6eba45fb8d9c81d99484d336e751c678dcc99fe7248b9bc061c6ff3a5b(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcs_cluster`
 
-Refer to the Terraform Registory for docs: [`data_hcs_cluster`](https://www.terraform.io/docs/providers/hcs/d/cluster).
+Refer to the Terraform Registory for docs: [`data_hcs_cluster`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class DataHcsCluster(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.dataHcsCluster.DataHcsCluster",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/d/cluster hcs_cluster}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster hcs_cluster}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
         cluster_name: typing.Optional[builtins.str] = None,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsClusterTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/d/cluster hcs_cluster} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster hcs_cluster} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#managed_application_name DataHcsCluster#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#resource_group_name DataHcsCluster#resource_group_name}
-        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#cluster_name DataHcsCluster#cluster_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#id DataHcsCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#timeouts DataHcsCluster#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#managed_application_name DataHcsCluster#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#resource_group_name DataHcsCluster#resource_group_name}
+        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#cluster_name DataHcsCluster#cluster_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#id DataHcsCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#timeouts DataHcsCluster#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -83,15 +83,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#default DataHcsCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#default DataHcsCluster#default}.
         '''
         value = DataHcsClusterTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetClusterName")
     def reset_cluster_name(self) -> None:
@@ -354,15 +354,15 @@
     },
 )
 class DataHcsClusterConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
@@ -374,19 +374,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#managed_application_name DataHcsCluster#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#resource_group_name DataHcsCluster#resource_group_name}
-        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#cluster_name DataHcsCluster#cluster_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#id DataHcsCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#timeouts DataHcsCluster#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#managed_application_name DataHcsCluster#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#resource_group_name DataHcsCluster#resource_group_name}
+        :param cluster_name: The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#cluster_name DataHcsCluster#cluster_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#id DataHcsCluster#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#timeouts DataHcsCluster#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcsClusterTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__36c729d642f7350137229da99c8cfdf49776939a5f268a3fdb15e6315e22279c)
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
@@ -489,54 +491,54 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#managed_application_name DataHcsCluster#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#managed_application_name DataHcsCluster#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#resource_group_name DataHcsCluster#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#resource_group_name DataHcsCluster#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def cluster_name(self) -> typing.Optional[builtins.str]:
         '''The name of the cluster Managed Resource. If not specified, it is defaulted to the value of ``managed_application_name``.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#cluster_name DataHcsCluster#cluster_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#cluster_name DataHcsCluster#cluster_name}
         '''
         result = self._values.get("cluster_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#id DataHcsCluster#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#id DataHcsCluster#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcsClusterTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#timeouts DataHcsCluster#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#timeouts DataHcsCluster#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcsClusterTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -553,26 +555,26 @@
     jsii_type="@cdktf/provider-hcs.dataHcsCluster.DataHcsClusterTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcsClusterTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#default DataHcsCluster#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#default DataHcsCluster#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a9d78d88c5aab42c845f1e64a84dc706ff8a9c9a05782a03b837f8868fc7013a)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/cluster#default DataHcsCluster#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/cluster#default DataHcsCluster#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -658,15 +660,15 @@
     *,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
     cluster_name: typing.Optional[builtins.str] = None,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsClusterTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -695,15 +697,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__36c729d642f7350137229da99c8cfdf49776939a5f268a3fdb15e6315e22279c(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcs_consul_versions`
 
-Refer to the Terraform Registory for docs: [`data_hcs_consul_versions`](https://www.terraform.io/docs/providers/hcs/d/consul_versions).
+Refer to the Terraform Registory for docs: [`data_hcs_consul_versions`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataHcsConsulVersions(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.dataHcsConsulVersions.DataHcsConsulVersions",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions hcs_consul_versions}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions hcs_consul_versions}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsConsulVersionsTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions hcs_consul_versions} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions hcs_consul_versions} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#id DataHcsConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#timeouts DataHcsConsulVersions#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#id DataHcsConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#timeouts DataHcsConsulVersions#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -74,15 +74,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#default DataHcsConsulVersions#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#default DataHcsConsulVersions#default}.
         '''
         value = DataHcsConsulVersionsTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -162,15 +162,15 @@
     },
 )
 class DataHcsConsulVersionsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsConsulVersionsTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
@@ -179,16 +179,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#id DataHcsConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#timeouts DataHcsConsulVersions#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#id DataHcsConsulVersions#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#timeouts DataHcsConsulVersions#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcsConsulVersionsTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a6c79c21b1129523375c26f92217a42670ea81cd8b2165f1a3d1b1dd6b609fa2)
@@ -228,20 +228,22 @@
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
@@ -281,27 +283,27 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#id DataHcsConsulVersions#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#id DataHcsConsulVersions#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcsConsulVersionsTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#timeouts DataHcsConsulVersions#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#timeouts DataHcsConsulVersions#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcsConsulVersionsTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -318,26 +320,26 @@
     jsii_type="@cdktf/provider-hcs.dataHcsConsulVersions.DataHcsConsulVersionsTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcsConsulVersionsTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#default DataHcsConsulVersions#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#default DataHcsConsulVersions#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__d2b1780e25ee30cb986eb526b355e5c8f01d8f6474a40eb0e2dd6b46016d17a1)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/consul_versions#default DataHcsConsulVersions#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/consul_versions#default DataHcsConsulVersions#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -420,15 +422,15 @@
 def _typecheckingstub__3a57b39ffabe0f67d2aeb9021ae6ec47f829185962bafa47a69461c8077b573d(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsConsulVersionsTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -439,15 +441,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__a6c79c21b1129523375c26f92217a42670ea81cd8b2165f1a3d1b1dd6b609fa2(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsConsulVersionsTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcs_federation_token`
 
-Refer to the Terraform Registory for docs: [`data_hcs_federation_token`](https://www.terraform.io/docs/providers/hcs/d/federation_token).
+Refer to the Terraform Registory for docs: [`data_hcs_federation_token`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,41 +22,41 @@
 
 
 class DataHcsFederationToken(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.dataHcsFederationToken.DataHcsFederationToken",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/d/federation_token hcs_federation_token}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token hcs_federation_token}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsFederationTokenTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/d/federation_token hcs_federation_token} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token hcs_federation_token} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#managed_application_name DataHcsFederationToken#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#resource_group_name DataHcsFederationToken#resource_group_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#id DataHcsFederationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#timeouts DataHcsFederationToken#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#managed_application_name DataHcsFederationToken#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#resource_group_name DataHcsFederationToken#resource_group_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#id DataHcsFederationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#timeouts DataHcsFederationToken#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -80,15 +80,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#default DataHcsFederationToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#default DataHcsFederationToken#default}.
         '''
         value = DataHcsFederationTokenTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -194,15 +194,15 @@
     },
 )
 class DataHcsFederationTokenConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
@@ -213,18 +213,18 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#managed_application_name DataHcsFederationToken#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#resource_group_name DataHcsFederationToken#resource_group_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#id DataHcsFederationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#timeouts DataHcsFederationToken#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#managed_application_name DataHcsFederationToken#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#resource_group_name DataHcsFederationToken#resource_group_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#id DataHcsFederationToken#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#timeouts DataHcsFederationToken#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcsFederationTokenTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__46f575f3f7cf776c9c1aecc258655a040ce59d5b88c9287f058138428b09d6b5)
@@ -269,20 +269,22 @@
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
@@ -324,45 +326,45 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#managed_application_name DataHcsFederationToken#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#managed_application_name DataHcsFederationToken#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#resource_group_name DataHcsFederationToken#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#resource_group_name DataHcsFederationToken#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#id DataHcsFederationToken#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#id DataHcsFederationToken#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcsFederationTokenTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#timeouts DataHcsFederationToken#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#timeouts DataHcsFederationToken#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcsFederationTokenTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -379,26 +381,26 @@
     jsii_type="@cdktf/provider-hcs.dataHcsFederationToken.DataHcsFederationTokenTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcsFederationTokenTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#default DataHcsFederationToken#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#default DataHcsFederationToken#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__67f981f626ef5e7680b2d68720a15681a25b7bc8991e659907625840e47dedc3)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/federation_token#default DataHcsFederationToken#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/federation_token#default DataHcsFederationToken#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -483,15 +485,15 @@
     id_: builtins.str,
     *,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsFederationTokenTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -514,15 +516,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__46f575f3f7cf776c9c1aecc258655a040ce59d5b88c9287f058138428b09d6b5(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/data_hcs_plan_defaults/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `data_hcs_plan_defaults`
 
-Refer to the Terraform Registory for docs: [`data_hcs_plan_defaults`](https://www.terraform.io/docs/providers/hcs/d/plan_defaults).
+Refer to the Terraform Registory for docs: [`data_hcs_plan_defaults`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,37 +22,37 @@
 
 
 class DataHcsPlanDefaults(
     _cdktf_9a9027ec.TerraformDataSource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.dataHcsPlanDefaults.DataHcsPlanDefaults",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults hcs_plan_defaults}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults hcs_plan_defaults}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsPlanDefaultsTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults hcs_plan_defaults} Data Source.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults hcs_plan_defaults} Data Source.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#id DataHcsPlanDefaults#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#timeouts DataHcsPlanDefaults#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#id DataHcsPlanDefaults#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#timeouts DataHcsPlanDefaults#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -74,15 +74,15 @@
         )
 
         jsii.create(self.__class__, self, [scope, id_, config])
 
     @jsii.member(jsii_name="putTimeouts")
     def put_timeouts(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#default DataHcsPlanDefaults#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#default DataHcsPlanDefaults#default}.
         '''
         value = DataHcsPlanDefaultsTimeouts(default=default)
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
     @jsii.member(jsii_name="resetId")
     def reset_id(self) -> None:
@@ -167,15 +167,15 @@
     },
 )
 class DataHcsPlanDefaultsConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["DataHcsPlanDefaultsTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
@@ -184,16 +184,16 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#id DataHcsPlanDefaults#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#timeouts DataHcsPlanDefaults#timeouts}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#id DataHcsPlanDefaults#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#timeouts DataHcsPlanDefaults#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = DataHcsPlanDefaultsTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__21af5c161d2a4c6dabdb70ef12d6646e2e5aed2a4bf85d9fd621a5914de4aea6)
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
@@ -286,27 +288,27 @@
         :stability: experimental
         '''
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#id DataHcsPlanDefaults#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#id DataHcsPlanDefaults#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["DataHcsPlanDefaultsTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#timeouts DataHcsPlanDefaults#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#timeouts DataHcsPlanDefaults#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["DataHcsPlanDefaultsTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -323,26 +325,26 @@
     jsii_type="@cdktf/provider-hcs.dataHcsPlanDefaults.DataHcsPlanDefaultsTimeouts",
     jsii_struct_bases=[],
     name_mapping={"default": "default"},
 )
 class DataHcsPlanDefaultsTimeouts:
     def __init__(self, *, default: typing.Optional[builtins.str] = None) -> None:
         '''
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#default DataHcsPlanDefaults#default}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#default DataHcsPlanDefaults#default}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a45a83b05a9054d2f1c30c2bafce2ce57f713bfb97564115ee0e435179d2187b)
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if default is not None:
             self._values["default"] = default
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/d/plan_defaults#default DataHcsPlanDefaults#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/data-sources/plan_defaults#default DataHcsPlanDefaults#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -425,15 +427,15 @@
 def _typecheckingstub__475b63f9acd94ae56d1e2ab35928ffadf55b7dc2c833115e811790b348312dab(
     scope: _constructs_77d1e7e8.Construct,
     id_: builtins.str,
     *,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsPlanDefaultsTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -444,15 +446,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__21af5c161d2a4c6dabdb70ef12d6646e2e5aed2a4bf85d9fd621a5914de4aea6(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[DataHcsPlanDefaultsTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/provider/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/provider/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `provider`
 
-Refer to the Terraform Registory for docs: [`hcs`](https://www.terraform.io/docs/providers/hcs).
+Refer to the Terraform Registory for docs: [`hcs`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,15 +22,15 @@
 
 
 class HcsProvider(
     _cdktf_9a9027ec.TerraformProvider,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.provider.HcsProvider",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs hcs}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs hcs}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id: builtins.str,
         *,
         alias: typing.Optional[builtins.str] = None,
@@ -43,31 +43,31 @@
         azure_msi_endpoint: typing.Optional[builtins.str] = None,
         azure_subscription_id: typing.Optional[builtins.str] = None,
         azure_tenant_id: typing.Optional[builtins.str] = None,
         azure_use_msi: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         hcp_api_domain: typing.Optional[builtins.str] = None,
         hcs_marketplace_product_name: typing.Optional[builtins.str] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs hcs} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs hcs} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#alias HcsProvider#alias}
-        :param azure_client_certificate_password: The password associated with the Azure Client Certificate. For use when authenticating as a Service Principal using a Client Certificate Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_certificate_password HcsProvider#azure_client_certificate_password}
-        :param azure_client_certificate_path: The path to the Azure Client Certificate associated with the Service Principal for use when authenticating as a Service Principal using a Client Certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_certificate_path HcsProvider#azure_client_certificate_path}
-        :param azure_client_id: The Azure Client ID which should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_id HcsProvider#azure_client_id}
-        :param azure_client_secret: The Azure Client Secret which should be used. For use when authenticating as a Service Principal using a Client Secret. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_secret HcsProvider#azure_client_secret}
-        :param azure_environment: The Azure Cloud Environment which should be used. Possible values are public, usgovernment, german, and china. Defaults to public. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_environment HcsProvider#azure_environment}
-        :param azure_metadata_host: The hostname which should be used for the Azure Metadata Service. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_metadata_host HcsProvider#azure_metadata_host}
-        :param azure_msi_endpoint: The path to a custom endpoint for Azure Managed Service Identity - in most circumstances this should be detected automatically. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_msi_endpoint HcsProvider#azure_msi_endpoint}
-        :param azure_subscription_id: The Azure Subscription ID which should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_subscription_id HcsProvider#azure_subscription_id}
-        :param azure_tenant_id: The Azure Tenant ID which should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_tenant_id HcsProvider#azure_tenant_id}
-        :param azure_use_msi: Allowed Azure Managed Service Identity be used for Authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_use_msi HcsProvider#azure_use_msi}
-        :param hcp_api_domain: The HashiCorp Cloud Platform API domain. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#hcp_api_domain HcsProvider#hcp_api_domain}
-        :param hcs_marketplace_product_name: The HashiCorp Consul Service product name on the Azure marketplace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#hcs_marketplace_product_name HcsProvider#hcs_marketplace_product_name}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#alias HcsProvider#alias}
+        :param azure_client_certificate_password: The password associated with the Azure Client Certificate. For use when authenticating as a Service Principal using a Client Certificate Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_certificate_password HcsProvider#azure_client_certificate_password}
+        :param azure_client_certificate_path: The path to the Azure Client Certificate associated with the Service Principal for use when authenticating as a Service Principal using a Client Certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_certificate_path HcsProvider#azure_client_certificate_path}
+        :param azure_client_id: The Azure Client ID which should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_id HcsProvider#azure_client_id}
+        :param azure_client_secret: The Azure Client Secret which should be used. For use when authenticating as a Service Principal using a Client Secret. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_secret HcsProvider#azure_client_secret}
+        :param azure_environment: The Azure Cloud Environment which should be used. Possible values are public, usgovernment, german, and china. Defaults to public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_environment HcsProvider#azure_environment}
+        :param azure_metadata_host: The hostname which should be used for the Azure Metadata Service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_metadata_host HcsProvider#azure_metadata_host}
+        :param azure_msi_endpoint: The path to a custom endpoint for Azure Managed Service Identity - in most circumstances this should be detected automatically. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_msi_endpoint HcsProvider#azure_msi_endpoint}
+        :param azure_subscription_id: The Azure Subscription ID which should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_subscription_id HcsProvider#azure_subscription_id}
+        :param azure_tenant_id: The Azure Tenant ID which should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_tenant_id HcsProvider#azure_tenant_id}
+        :param azure_use_msi: Allowed Azure Managed Service Identity be used for Authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_use_msi HcsProvider#azure_use_msi}
+        :param hcp_api_domain: The HashiCorp Cloud Platform API domain. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#hcp_api_domain HcsProvider#hcp_api_domain}
+        :param hcs_marketplace_product_name: The HashiCorp Consul Service product name on the Azure marketplace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#hcs_marketplace_product_name HcsProvider#hcs_marketplace_product_name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__cf226bfabee3c16ab384996076993793ecb202c153fcffb3dbb2b88e20d01797)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         config = HcsProviderConfig(
             alias=alias,
@@ -420,27 +420,27 @@
         azure_subscription_id: typing.Optional[builtins.str] = None,
         azure_tenant_id: typing.Optional[builtins.str] = None,
         azure_use_msi: typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]] = None,
         hcp_api_domain: typing.Optional[builtins.str] = None,
         hcs_marketplace_product_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param alias: Alias name. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#alias HcsProvider#alias}
-        :param azure_client_certificate_password: The password associated with the Azure Client Certificate. For use when authenticating as a Service Principal using a Client Certificate Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_certificate_password HcsProvider#azure_client_certificate_password}
-        :param azure_client_certificate_path: The path to the Azure Client Certificate associated with the Service Principal for use when authenticating as a Service Principal using a Client Certificate. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_certificate_path HcsProvider#azure_client_certificate_path}
-        :param azure_client_id: The Azure Client ID which should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_id HcsProvider#azure_client_id}
-        :param azure_client_secret: The Azure Client Secret which should be used. For use when authenticating as a Service Principal using a Client Secret. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_secret HcsProvider#azure_client_secret}
-        :param azure_environment: The Azure Cloud Environment which should be used. Possible values are public, usgovernment, german, and china. Defaults to public. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_environment HcsProvider#azure_environment}
-        :param azure_metadata_host: The hostname which should be used for the Azure Metadata Service. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_metadata_host HcsProvider#azure_metadata_host}
-        :param azure_msi_endpoint: The path to a custom endpoint for Azure Managed Service Identity - in most circumstances this should be detected automatically. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_msi_endpoint HcsProvider#azure_msi_endpoint}
-        :param azure_subscription_id: The Azure Subscription ID which should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_subscription_id HcsProvider#azure_subscription_id}
-        :param azure_tenant_id: The Azure Tenant ID which should be used. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_tenant_id HcsProvider#azure_tenant_id}
-        :param azure_use_msi: Allowed Azure Managed Service Identity be used for Authentication. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_use_msi HcsProvider#azure_use_msi}
-        :param hcp_api_domain: The HashiCorp Cloud Platform API domain. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#hcp_api_domain HcsProvider#hcp_api_domain}
-        :param hcs_marketplace_product_name: The HashiCorp Consul Service product name on the Azure marketplace. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#hcs_marketplace_product_name HcsProvider#hcs_marketplace_product_name}
+        :param alias: Alias name. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#alias HcsProvider#alias}
+        :param azure_client_certificate_password: The password associated with the Azure Client Certificate. For use when authenticating as a Service Principal using a Client Certificate Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_certificate_password HcsProvider#azure_client_certificate_password}
+        :param azure_client_certificate_path: The path to the Azure Client Certificate associated with the Service Principal for use when authenticating as a Service Principal using a Client Certificate. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_certificate_path HcsProvider#azure_client_certificate_path}
+        :param azure_client_id: The Azure Client ID which should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_id HcsProvider#azure_client_id}
+        :param azure_client_secret: The Azure Client Secret which should be used. For use when authenticating as a Service Principal using a Client Secret. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_secret HcsProvider#azure_client_secret}
+        :param azure_environment: The Azure Cloud Environment which should be used. Possible values are public, usgovernment, german, and china. Defaults to public. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_environment HcsProvider#azure_environment}
+        :param azure_metadata_host: The hostname which should be used for the Azure Metadata Service. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_metadata_host HcsProvider#azure_metadata_host}
+        :param azure_msi_endpoint: The path to a custom endpoint for Azure Managed Service Identity - in most circumstances this should be detected automatically. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_msi_endpoint HcsProvider#azure_msi_endpoint}
+        :param azure_subscription_id: The Azure Subscription ID which should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_subscription_id HcsProvider#azure_subscription_id}
+        :param azure_tenant_id: The Azure Tenant ID which should be used. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_tenant_id HcsProvider#azure_tenant_id}
+        :param azure_use_msi: Allowed Azure Managed Service Identity be used for Authentication. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_use_msi HcsProvider#azure_use_msi}
+        :param hcp_api_domain: The HashiCorp Cloud Platform API domain. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#hcp_api_domain HcsProvider#hcp_api_domain}
+        :param hcs_marketplace_product_name: The HashiCorp Consul Service product name on the Azure marketplace. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#hcs_marketplace_product_name HcsProvider#hcs_marketplace_product_name}
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__7daeec413a1ea1a80d648e9f8385f97d600dc757cdde224854ecb1d60f466935)
             check_type(argname="argument alias", value=alias, expected_type=type_hints["alias"])
             check_type(argname="argument azure_client_certificate_password", value=azure_client_certificate_password, expected_type=type_hints["azure_client_certificate_password"])
             check_type(argname="argument azure_client_certificate_path", value=azure_client_certificate_path, expected_type=type_hints["azure_client_certificate_path"])
             check_type(argname="argument azure_client_id", value=azure_client_id, expected_type=type_hints["azure_client_id"])
@@ -481,129 +481,129 @@
         if hcs_marketplace_product_name is not None:
             self._values["hcs_marketplace_product_name"] = hcs_marketplace_product_name
 
     @builtins.property
     def alias(self) -> typing.Optional[builtins.str]:
         '''Alias name.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#alias HcsProvider#alias}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#alias HcsProvider#alias}
         '''
         result = self._values.get("alias")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_client_certificate_password(self) -> typing.Optional[builtins.str]:
         '''The password associated with the Azure Client Certificate.
 
         For use when authenticating as a Service Principal using a Client Certificate
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_certificate_password HcsProvider#azure_client_certificate_password}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_certificate_password HcsProvider#azure_client_certificate_password}
         '''
         result = self._values.get("azure_client_certificate_password")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_client_certificate_path(self) -> typing.Optional[builtins.str]:
         '''The path to the Azure Client Certificate associated with the Service Principal for use when authenticating as a Service Principal using a Client Certificate.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_certificate_path HcsProvider#azure_client_certificate_path}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_certificate_path HcsProvider#azure_client_certificate_path}
         '''
         result = self._values.get("azure_client_certificate_path")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_client_id(self) -> typing.Optional[builtins.str]:
         '''The Azure Client ID which should be used.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_id HcsProvider#azure_client_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_id HcsProvider#azure_client_id}
         '''
         result = self._values.get("azure_client_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_client_secret(self) -> typing.Optional[builtins.str]:
         '''The Azure Client Secret which should be used.
 
         For use when authenticating as a Service Principal using a Client Secret.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_client_secret HcsProvider#azure_client_secret}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_client_secret HcsProvider#azure_client_secret}
         '''
         result = self._values.get("azure_client_secret")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_environment(self) -> typing.Optional[builtins.str]:
         '''The Azure Cloud Environment which should be used. Possible values are public, usgovernment, german, and china. Defaults to public.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_environment HcsProvider#azure_environment}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_environment HcsProvider#azure_environment}
         '''
         result = self._values.get("azure_environment")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_metadata_host(self) -> typing.Optional[builtins.str]:
         '''The hostname which should be used for the Azure Metadata Service.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_metadata_host HcsProvider#azure_metadata_host}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_metadata_host HcsProvider#azure_metadata_host}
         '''
         result = self._values.get("azure_metadata_host")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_msi_endpoint(self) -> typing.Optional[builtins.str]:
         '''The path to a custom endpoint for Azure Managed Service Identity - in most circumstances this should be detected automatically.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_msi_endpoint HcsProvider#azure_msi_endpoint}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_msi_endpoint HcsProvider#azure_msi_endpoint}
         '''
         result = self._values.get("azure_msi_endpoint")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_subscription_id(self) -> typing.Optional[builtins.str]:
         '''The Azure Subscription ID which should be used.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_subscription_id HcsProvider#azure_subscription_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_subscription_id HcsProvider#azure_subscription_id}
         '''
         result = self._values.get("azure_subscription_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_tenant_id(self) -> typing.Optional[builtins.str]:
         '''The Azure Tenant ID which should be used.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_tenant_id HcsProvider#azure_tenant_id}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_tenant_id HcsProvider#azure_tenant_id}
         '''
         result = self._values.get("azure_tenant_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def azure_use_msi(
         self,
     ) -> typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]]:
         '''Allowed Azure Managed Service Identity be used for Authentication.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#azure_use_msi HcsProvider#azure_use_msi}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#azure_use_msi HcsProvider#azure_use_msi}
         '''
         result = self._values.get("azure_use_msi")
         return typing.cast(typing.Optional[typing.Union[builtins.bool, _cdktf_9a9027ec.IResolvable]], result)
 
     @builtins.property
     def hcp_api_domain(self) -> typing.Optional[builtins.str]:
         '''The HashiCorp Cloud Platform API domain.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#hcp_api_domain HcsProvider#hcp_api_domain}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#hcp_api_domain HcsProvider#hcp_api_domain}
         '''
         result = self._values.get("hcp_api_domain")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def hcs_marketplace_product_name(self) -> typing.Optional[builtins.str]:
         '''The HashiCorp Consul Service product name on the Azure marketplace.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs#hcs_marketplace_product_name HcsProvider#hcs_marketplace_product_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs#hcs_marketplace_product_name HcsProvider#hcs_marketplace_product_name}
         '''
         result = self._values.get("hcs_marketplace_product_name")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs/snapshot/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 # `hcs_snapshot`
 
-Refer to the Terraform Registory for docs: [`hcs_snapshot`](https://www.terraform.io/docs/providers/hcs/r/snapshot).
+Refer to the Terraform Registory for docs: [`hcs_snapshot`](https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot).
 '''
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
@@ -22,43 +22,43 @@
 
 
 class Snapshot(
     _cdktf_9a9027ec.TerraformResource,
     metaclass=jsii.JSIIMeta,
     jsii_type="@cdktf/provider-hcs.snapshot.Snapshot",
 ):
-    '''Represents a {@link https://www.terraform.io/docs/providers/hcs/r/snapshot hcs_snapshot}.'''
+    '''Represents a {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot hcs_snapshot}.'''
 
     def __init__(
         self,
         scope: _constructs_77d1e7e8.Construct,
         id_: builtins.str,
         *,
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
         snapshot_name: builtins.str,
         id: typing.Optional[builtins.str] = None,
         timeouts: typing.Optional[typing.Union["SnapshotTimeouts", typing.Dict[builtins.str, typing.Any]]] = None,
         connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-        count: typing.Optional[jsii.Number] = None,
+        count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
         depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
         for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
         lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
         provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
         provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     ) -> None:
-        '''Create a new {@link https://www.terraform.io/docs/providers/hcs/r/snapshot hcs_snapshot} Resource.
+        '''Create a new {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot hcs_snapshot} Resource.
 
         :param scope: The scope in which to define this construct.
         :param id_: The scoped construct ID. Must be unique amongst siblings in the same scope
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#managed_application_name Snapshot#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#resource_group_name Snapshot#resource_group_name}
-        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#snapshot_name Snapshot#snapshot_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#id Snapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#timeouts Snapshot#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#managed_application_name Snapshot#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#resource_group_name Snapshot#resource_group_name}
+        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#snapshot_name Snapshot#snapshot_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#id Snapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#timeouts Snapshot#timeouts}
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
@@ -90,18 +90,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#create Snapshot#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#default Snapshot#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#delete Snapshot#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#update Snapshot#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#create Snapshot#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#default Snapshot#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#delete Snapshot#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#update Snapshot#update}.
         '''
         value = SnapshotTimeouts(
             create=create, default=default, delete=delete, update=update
         )
 
         return typing.cast(None, jsii.invoke(self, "putTimeouts", [value]))
 
@@ -247,15 +247,15 @@
     },
 )
 class SnapshotConfig(_cdktf_9a9027ec.TerraformMetaArguments):
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
         managed_application_name: builtins.str,
         resource_group_name: builtins.str,
@@ -267,19 +267,19 @@
         :param connection: 
         :param count: 
         :param depends_on: 
         :param for_each: 
         :param lifecycle: 
         :param provider: 
         :param provisioners: 
-        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#managed_application_name Snapshot#managed_application_name}
-        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#resource_group_name Snapshot#resource_group_name}
-        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#snapshot_name Snapshot#snapshot_name}
-        :param id: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#id Snapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
-        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#timeouts Snapshot#timeouts}
+        :param managed_application_name: The name of the HCS Azure Managed Application. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#managed_application_name Snapshot#managed_application_name}
+        :param resource_group_name: The name of the Resource Group in which the HCS Azure Managed Application belongs. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#resource_group_name Snapshot#resource_group_name}
+        :param snapshot_name: The name of the snapshot. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#snapshot_name Snapshot#snapshot_name}
+        :param id: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#id Snapshot#id}. Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2. If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
+        :param timeouts: timeouts block. Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#timeouts Snapshot#timeouts}
         '''
         if isinstance(lifecycle, dict):
             lifecycle = _cdktf_9a9027ec.TerraformResourceLifecycle(**lifecycle)
         if isinstance(timeouts, dict):
             timeouts = SnapshotTimeouts(**timeouts)
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f04b534a4d5a8f01a4ce64b7d488af032e40d612c8b221fbe0f4f9ce5619d3fa)
@@ -326,20 +326,22 @@
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
@@ -381,55 +383,55 @@
         result = self._values.get("provisioners")
         return typing.cast(typing.Optional[typing.List[typing.Union[_cdktf_9a9027ec.FileProvisioner, _cdktf_9a9027ec.LocalExecProvisioner, _cdktf_9a9027ec.RemoteExecProvisioner]]], result)
 
     @builtins.property
     def managed_application_name(self) -> builtins.str:
         '''The name of the HCS Azure Managed Application.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#managed_application_name Snapshot#managed_application_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#managed_application_name Snapshot#managed_application_name}
         '''
         result = self._values.get("managed_application_name")
         assert result is not None, "Required property 'managed_application_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def resource_group_name(self) -> builtins.str:
         '''The name of the Resource Group in which the HCS Azure Managed Application belongs.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#resource_group_name Snapshot#resource_group_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#resource_group_name Snapshot#resource_group_name}
         '''
         result = self._values.get("resource_group_name")
         assert result is not None, "Required property 'resource_group_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def snapshot_name(self) -> builtins.str:
         '''The name of the snapshot.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#snapshot_name Snapshot#snapshot_name}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#snapshot_name Snapshot#snapshot_name}
         '''
         result = self._values.get("snapshot_name")
         assert result is not None, "Required property 'snapshot_name' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def id(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#id Snapshot#id}.
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#id Snapshot#id}.
 
         Please be aware that the id field is automatically added to all resources in Terraform providers using a Terraform provider SDK version below 2.
         If you experience problems setting this value it might not be settable. Please take a look at the provider documentation to ensure it should be settable.
         '''
         result = self._values.get("id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def timeouts(self) -> typing.Optional["SnapshotTimeouts"]:
         '''timeouts block.
 
-        Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#timeouts Snapshot#timeouts}
+        Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#timeouts Snapshot#timeouts}
         '''
         result = self._values.get("timeouts")
         return typing.cast(typing.Optional["SnapshotTimeouts"], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
@@ -458,18 +460,18 @@
         *,
         create: typing.Optional[builtins.str] = None,
         default: typing.Optional[builtins.str] = None,
         delete: typing.Optional[builtins.str] = None,
         update: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param create: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#create Snapshot#create}.
-        :param default: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#default Snapshot#default}.
-        :param delete: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#delete Snapshot#delete}.
-        :param update: Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#update Snapshot#update}.
+        :param create: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#create Snapshot#create}.
+        :param default: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#default Snapshot#default}.
+        :param delete: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#delete Snapshot#delete}.
+        :param update: Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#update Snapshot#update}.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__a0414c04494757eacb4d0d1a9e681e33813a5e238213e81a2ac1c00189368873)
             check_type(argname="argument create", value=create, expected_type=type_hints["create"])
             check_type(argname="argument default", value=default, expected_type=type_hints["default"])
             check_type(argname="argument delete", value=delete, expected_type=type_hints["delete"])
             check_type(argname="argument update", value=update, expected_type=type_hints["update"])
@@ -481,33 +483,33 @@
         if delete is not None:
             self._values["delete"] = delete
         if update is not None:
             self._values["update"] = update
 
     @builtins.property
     def create(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#create Snapshot#create}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#create Snapshot#create}.'''
         result = self._values.get("create")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def default(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#default Snapshot#default}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#default Snapshot#default}.'''
         result = self._values.get("default")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def delete(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#delete Snapshot#delete}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#delete Snapshot#delete}.'''
         result = self._values.get("delete")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def update(self) -> typing.Optional[builtins.str]:
-        '''Docs at Terraform Registry: {@link https://www.terraform.io/docs/providers/hcs/r/snapshot#update Snapshot#update}.'''
+        '''Docs at Terraform Registry: {@link https://registry.terraform.io/providers/hashicorp/hcs/0.5.1/docs/resources/snapshot#update Snapshot#update}.'''
         result = self._values.get("update")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -656,15 +658,15 @@
     *,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
     snapshot_name: builtins.str,
     id: typing.Optional[builtins.str] = None,
     timeouts: typing.Optional[typing.Union[SnapshotTimeouts, typing.Dict[builtins.str, typing.Any]]] = None,
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
@@ -693,15 +695,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f04b534a4d5a8f01a4ce64b7d488af032e40d612c8b221fbe0f4f9ce5619d3fa(
     *,
     connection: typing.Optional[typing.Union[typing.Union[_cdktf_9a9027ec.SSHProvisionerConnection, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.WinrmProvisionerConnection, typing.Dict[builtins.str, typing.Any]]]] = None,
-    count: typing.Optional[jsii.Number] = None,
+    count: typing.Optional[typing.Union[jsii.Number, _cdktf_9a9027ec.TerraformCount]] = None,
     depends_on: typing.Optional[typing.Sequence[_cdktf_9a9027ec.ITerraformDependable]] = None,
     for_each: typing.Optional[_cdktf_9a9027ec.ITerraformIterator] = None,
     lifecycle: typing.Optional[typing.Union[_cdktf_9a9027ec.TerraformResourceLifecycle, typing.Dict[builtins.str, typing.Any]]] = None,
     provider: typing.Optional[_cdktf_9a9027ec.TerraformProvider] = None,
     provisioners: typing.Optional[typing.Sequence[typing.Union[typing.Union[_cdktf_9a9027ec.FileProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.LocalExecProvisioner, typing.Dict[builtins.str, typing.Any]], typing.Union[_cdktf_9a9027ec.RemoteExecProvisioner, typing.Dict[builtins.str, typing.Any]]]]] = None,
     managed_application_name: builtins.str,
     resource_group_name: builtins.str,
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdktf-cdktf-provider-hcs
-Version: 3.0.0
+Version: 4.0.0
 Summary: Prebuilt hcs Provider for Terraform CDK (cdktf)
 Home-page: https://github.com/cdktf/cdktf-provider-hcs.git
 Author: HashiCorp
 License: MPL-2.0
 Project-URL: Source, https://github.com/cdktf/cdktf-provider-hcs.git
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
 
 The go package is generated into the [`github.com/cdktf/cdktf-provider-hcs-go`](https://github.com/cdktf/cdktf-provider-hcs-go) package.
 
 `go get github.com/cdktf/cdktf-provider-hcs-go/hcs`
 
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
 You can also visit a hosted version of the documentation on [constructs.dev](https://constructs.dev/packages/@cdktf/provider-hcs).
 
 ## Versioning
 
 This project is explicitly not tracking the Terraform hcs Provider version 1:1. In fact, it always tracks `latest` of `~> 0.5` with every release. If there are scenarios where you explicitly have to pin your provider version, you can do so by generating the [provider constructs manually](https://cdk.tf/imports).
 
 These are the upstream dependencies:
@@ -101,9 +108,7 @@
 ### Provider Version
 
 The provider version can be adjusted in [./.projenrc.js](./.projenrc.js).
 
 ### Repository Management
 
 The repository is managed by [Repository Manager](https://github.com/hashicorp/cdktf-repository-manager/)
-
-
```

### Comparing `cdktf-cdktf-provider-hcs-3.0.0/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt` & `cdktf-cdktf-provider-hcs-4.0.0/src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 src/cdktf_cdktf_provider_hcs/py.typed
 src/cdktf_cdktf_provider_hcs.egg-info/PKG-INFO
 src/cdktf_cdktf_provider_hcs.egg-info/SOURCES.txt
 src/cdktf_cdktf_provider_hcs.egg-info/dependency_links.txt
 src/cdktf_cdktf_provider_hcs.egg-info/requires.txt
 src/cdktf_cdktf_provider_hcs.egg-info/top_level.txt
 src/cdktf_cdktf_provider_hcs/_jsii/__init__.py
-src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@3.0.0.jsii.tgz
+src/cdktf_cdktf_provider_hcs/_jsii/provider-hcs@4.0.0.jsii.tgz
 src/cdktf_cdktf_provider_hcs/cluster/__init__.py
 src/cdktf_cdktf_provider_hcs/cluster_root_token/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_agent_helm_config/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_agent_kubernetes_secret/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_cluster/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_consul_versions/__init__.py
 src/cdktf_cdktf_provider_hcs/data_hcs_federation_token/__init__.py
```

