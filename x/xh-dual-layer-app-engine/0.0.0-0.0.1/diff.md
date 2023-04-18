# Comparing `tmp/xh-dual-layer-app-engine-0.0.0.tar.gz` & `tmp/xh-dual-layer-app-engine-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dual-layer-app-engine-0.0.0.tar", last modified: Tue Apr 18 00:32:48 2023, max compression
+gzip compressed data, was "xh-dual-layer-app-engine-0.0.1.tar", last modified: Tue Apr 18 00:39:30 2023, max compression
```

## Comparing `xh-dual-layer-app-engine-0.0.0.tar` & `xh-dual-layer-app-engine-0.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 00:32:48.477550 xh-dual-layer-app-engine-0.0.0/
--rw-r--r--   0 xeth      (1000) xeth      (1000)    35821 2023-04-17 04:08:40.000000 xh-dual-layer-app-engine-0.0.0/LICENSE.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)      850 2023-04-18 00:32:48.477550 xh-dual-layer-app-engine-0.0.0/PKG-INFO
--rw-r--r--   0 xeth      (1000) xeth      (1000)      258 2023-04-17 04:08:45.000000 xh-dual-layer-app-engine-0.0.0/README.md
--rw-r--r--   0 xeth      (1000) xeth      (1000)      662 2023-04-18 00:15:41.000000 xh-dual-layer-app-engine-0.0.0/pyproject.toml
--rw-r--r--   0 xeth      (1000) xeth      (1000)       38 2023-04-18 00:32:48.477550 xh-dual-layer-app-engine-0.0.0/setup.cfg
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 00:32:48.477550 xh-dual-layer-app-engine-0.0.0/src/
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 00:32:48.477550 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine/
--rw-r--r--   0 xeth      (1000) xeth      (1000)      358 2023-04-17 16:34:33.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine/CommandTemplate.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)      926 2023-04-18 00:19:39.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine/ExtractFromFile.py
--rw-r--r--   0 xeth      (1000) xeth      (1000)     2227 2023-04-18 00:25:56.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine/Layer1AppEngine.py
-drwxr-xr-x   0 xeth      (1000) xeth      (1000)        0 2023-04-18 00:32:48.477550 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine.egg-info/
--rw-r--r--   0 xeth      (1000) xeth      (1000)      850 2023-04-18 00:32:48.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine.egg-info/PKG-INFO
--rw-r--r--   0 xeth      (1000) xeth      (1000)      388 2023-04-18 00:32:48.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine.egg-info/SOURCES.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)        1 2023-04-18 00:32:48.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine.egg-info/dependency_links.txt
--rw-r--r--   0 xeth      (1000) xeth      (1000)       25 2023-04-18 00:32:48.000000 xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:30.969439 xh-dual-layer-app-engine-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-18 00:39:18.000000 xh-dual-layer-app-engine-0.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 00:39:30.969439 xh-dual-layer-app-engine-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-18 00:39:18.000000 xh-dual-layer-app-engine-0.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 00:39:18.000000 xh-dual-layer-app-engine-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:39:30.969439 xh-dual-layer-app-engine-0.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:30.965439 xh-dual-layer-app-engine-0.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:30.965439 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 00:39:18.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine/CommandTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-18 00:39:18.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine/ExtractFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-18 00:39:18.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine/Layer1AppEngine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:39:30.969439 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 00:39:30.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 00:39:30.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:39:30.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 00:39:30.000000 xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine.egg-info/top_level.txt
```

### Comparing `xh-dual-layer-app-engine-0.0.0/LICENSE.txt` & `xh-dual-layer-app-engine-0.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dual-layer-app-engine-0.0.0/PKG-INFO` & `xh-dual-layer-app-engine-0.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dual-layer-app-engine
-Version: 0.0.0
+Version: 0.0.1
 Summary: A library re-orangize the builtin argparser api to simply bootstrap app with second layer command
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dual-layer-app-engine
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dual-layer-app-engine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-dual-layer-app-engine-0.0.0/pyproject.toml` & `xh-dual-layer-app-engine-0.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-dual-layer-app-engine"
-version = "0.0.0"
+version = "0.0.1"
 description = "A library re-orangize the builtin argparser api to simply bootstrap app with second layer command"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine/ExtractFromFile.py` & `xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine/ExtractFromFile.py`

 * *Files identical despite different names*

### Comparing `xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine/Layer1AppEngine.py` & `xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine/Layer1AppEngine.py`

 * *Files identical despite different names*

### Comparing `xh-dual-layer-app-engine-0.0.0/src/xh_dual_layer_app_engine.egg-info/PKG-INFO` & `xh-dual-layer-app-engine-0.0.1/src/xh_dual_layer_app_engine.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dual-layer-app-engine
-Version: 0.0.0
+Version: 0.0.1
 Summary: A library re-orangize the builtin argparser api to simply bootstrap app with second layer command
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dual-layer-app-engine
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dual-layer-app-engine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

