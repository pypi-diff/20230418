# Comparing `tmp/xh-dual-layer-app-engine-0.0.2.tar.gz` & `tmp/xh-dual-layer-app-engine-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xh-dual-layer-app-engine-0.0.2.tar", last modified: Tue Apr 18 02:15:01 2023, max compression
+gzip compressed data, was "xh-dual-layer-app-engine-0.0.3.tar", last modified: Tue Apr 18 02:24:00 2023, max compression
```

## Comparing `xh-dual-layer-app-engine-0.0.2.tar` & `xh-dual-layer-app-engine-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:15:01.652695 xh-dual-layer-app-engine-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 02:15:01.652695 xh-dual-layer-app-engine-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 02:15:01.652695 xh-dual-layer-app-engine-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:15:01.648695 xh-dual-layer-app-engine-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:15:01.652695 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/CommandTemplate.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/ExtractFromFile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/Layer1AppEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-18 02:14:46.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:15:01.652695 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 02:15:01.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 02:15:01.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:15:01.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 02:15:01.000000 xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:24:00.761333 xh-dual-layer-app-engine-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35821 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 02:24:00.757333 xh-dual-layer-app-engine-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 02:24:00.761333 xh-dual-layer-app-engine-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:24:00.757333 xh-dual-layer-app-engine-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:24:00.757333 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/CommandTemplate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/ExtractFromFile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2227 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/Layer1AppEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 02:23:48.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 02:24:00.757333 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-04-18 02:24:00.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 02:24:00.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 02:24:00.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 02:24:00.000000 xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine.egg-info/top_level.txt
```

### Comparing `xh-dual-layer-app-engine-0.0.2/LICENSE.txt` & `xh-dual-layer-app-engine-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xh-dual-layer-app-engine-0.0.2/PKG-INFO` & `xh-dual-layer-app-engine-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dual-layer-app-engine
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library re-orangize the builtin argparser api to simply bootstrap app with second layer command
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dual-layer-app-engine
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dual-layer-app-engine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `xh-dual-layer-app-engine-0.0.2/pyproject.toml` & `xh-dual-layer-app-engine-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xh-dual-layer-app-engine"
-version = "0.0.2"
+version = "0.0.3"
 description = "A library re-orangize the builtin argparser api to simply bootstrap app with second layer command"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 
 [[project.authors]]
 name = "xethhung"
```

### Comparing `xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/ExtractFromFile.py` & `xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/ExtractFromFile.py`

 * *Files identical despite different names*

### Comparing `xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine/Layer1AppEngine.py` & `xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine/Layer1AppEngine.py`

 * *Files identical despite different names*

### Comparing `xh-dual-layer-app-engine-0.0.2/src/xh_dual_layer_app_engine.egg-info/PKG-INFO` & `xh-dual-layer-app-engine-0.0.3/src/xh_dual_layer_app_engine.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xh-dual-layer-app-engine
-Version: 0.0.2
+Version: 0.0.3
 Summary: A library re-orangize the builtin argparser api to simply bootstrap app with second layer command
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev/xh-dual-layer-app-engine
 Project-URL: Bug Tracker, https://github.com/xh-dev/xh-dual-layer-app-engine
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

