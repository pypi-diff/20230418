# Comparing `tmp/cdk8s-plus-26-2.3.0.tar.gz` & `tmp/cdk8s-plus-26-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk8s-plus-26-2.3.0.tar", last modified: Mon Apr 10 12:06:16 2023, max compression
+gzip compressed data, was "cdk8s-plus-26-2.3.1.tar", last modified: Tue Apr 18 21:28:06 2023, max compression
```

## Comparing `cdk8s-plus-26-2.3.0.tar` & `cdk8s-plus-26-2.3.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:16.532169 cdk8s-plus-26-2.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-10 12:06:16.528169 cdk8s-plus-26-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:06:16.532169 cdk8s-plus-26-2.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:16.524169 cdk8s-plus-26-2.3.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:16.524169 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/
--rw-r--r--   0 runner    (1001) docker     (123)  1130341 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:16.524169 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)  1285669 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.3.0.jsii.tgz
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:16.528169 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/k8s/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:06:05.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:06:16.524169 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-10 12:06:16.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-10 12:06:16.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:06:16.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-10 12:06:16.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 12:06:16.000000 cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:06.890566 cdk8s-plus-26-2.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-18 21:28:06.890566 cdk8s-plus-26-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:28:06.890566 cdk8s-plus-26-2.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:06.882566 cdk8s-plus-26-2.3.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:06.886566 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/
+-rw-r--r--   0 runner    (1001) docker     (123)  1130341 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:06.886566 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1285669 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/_jsii/cdk8s-plus-26@2.3.1.jsii.tgz
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:06.886566 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)  2771385 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/k8s/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:27:53.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:06.886566 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-04-18 21:28:06.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-04-18 21:28:06.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:28:06.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-04-18 21:28:06.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 21:28:06.000000 cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/top_level.txt
```

### Comparing `cdk8s-plus-26-2.3.0/LICENSE` & `cdk8s-plus-26-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.0/PKG-INFO` & `cdk8s-plus-26-2.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.3.0
+Version: 2.3.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk8s-plus-26-2.3.0/README.md` & `cdk8s-plus-26-2.3.1/README.md`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.0/setup.py` & `cdk8s-plus-26-2.3.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk8s-plus-26",
-    "version": "2.3.0",
+    "version": "2.3.1",
     "description": "cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0",
     "license": "Apache-2.0",
     "url": "https://github.com/cdk8s-team/cdk8s-plus.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services",
     "bdist_wheel": {
         "universal": true
@@ -23,15 +23,15 @@
     "packages": [
         "cdk8s_plus_26",
         "cdk8s_plus_26._jsii",
         "cdk8s_plus_26.k8s"
     ],
     "package_data": {
         "cdk8s_plus_26._jsii": [
-            "cdk8s-plus-26@2.3.0.jsii.tgz"
+            "cdk8s-plus-26@2.3.1.jsii.tgz"
         ],
         "cdk8s_plus_26": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/__init__.py` & `cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.0/src/cdk8s_plus_26/k8s/__init__.py` & `cdk8s-plus-26-2.3.1/src/cdk8s_plus_26/k8s/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk8s-plus-26-2.3.0/src/cdk8s_plus_26.egg-info/PKG-INFO` & `cdk8s-plus-26-2.3.1/src/cdk8s_plus_26.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk8s-plus-26
-Version: 2.3.0
+Version: 2.3.1
 Summary: cdk8s+ is a software development framework that provides high level abstractions for authoring Kubernetes applications. cdk8s-plus-26 synthesizes Kubernetes manifests for Kubernetes 1.26.0
 Home-page: https://github.com/cdk8s-team/cdk8s-plus.git
 Author: Amazon Web Services
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdk8s-team/cdk8s-plus.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

