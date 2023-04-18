# Comparing `tmp/viur_cli-1.0.2.tar.gz` & `tmp/viur_cli-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur_cli-1.0.2.tar", last modified: Mon Apr 17 17:15:37 2023, max compression
+gzip compressed data, was "viur_cli-1.0.3.tar", last modified: Tue Apr 18 06:13:21 2023, max compression
```

## Comparing `viur_cli-1.0.2.tar` & `viur_cli-1.0.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-17 17:15:29.000000 viur_cli-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-17 17:15:37.901606 viur_cli-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-17 17:15:29.000000 viur_cli-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-17 17:15:29.000000 viur_cli-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-17 17:15:37.901606 viur_cli-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-17 17:15:29.000000 viur_cli-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.897606 viur_cli-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    10006 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/deploy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/install.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/npm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/csvwriter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/dialog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/network.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/progressbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/viur.py
--rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/flare.py
--rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/get_pyodide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/scripts/viur_2to3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-17 17:15:29.000000 viur_cli-1.0.2/src/viur_cli/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 17:15:37.901606 viur_cli-1.0.2/src/viur_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-17 17:15:37.000000 viur_cli-1.0.2/src/viur_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.226261 viur_cli-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-18 06:13:12.000000 viur_cli-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-18 06:13:21.226261 viur_cli-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-04-18 06:13:12.000000 viur_cli-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-18 06:13:12.000000 viur_cli-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-18 06:13:21.226261 viur_cli-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-04-18 06:13:12.000000 viur_cli-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.214262 viur_cli-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.218262 viur_cli-1.0.3/src/viur_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10016 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6301 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6023 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/npm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.222262 viur_cli-1.0.3/src/viur_cli/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10180 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.226261 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/csvwriter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/dialog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/progressbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6031 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/viur.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6883 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.226261 viur_cli-1.0.3/src/viur_cli/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9803 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scripts/flare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4470 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scripts/get_pyodide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/scripts/viur_2to3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 06:13:12.000000 viur_cli-1.0.3/src/viur_cli/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:13:21.222262 viur_cli-1.0.3/src/viur_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-04-18 06:13:21.000000 viur_cli-1.0.3/src/viur_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-04-18 06:13:21.000000 viur_cli-1.0.3/src/viur_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:13:21.000000 viur_cli-1.0.3/src/viur_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-18 06:13:21.000000 viur_cli-1.0.3/src/viur_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 06:13:21.000000 viur_cli-1.0.3/src/viur_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 06:13:21.000000 viur_cli-1.0.3/src/viur_cli.egg-info/top_level.txt
```

### Comparing `viur_cli-1.0.2/LICENSE` & `viur_cli-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/PKG-INFO` & `viur_cli-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur_cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur_cli Version: 1.0.2 Summary: Command-line
+Metadata-Version: 2.1 Name: viur_cli Version: 1.0.3 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.2/README.md` & `viur_cli-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/setup.cfg` & `viur_cli-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/build.py` & `viur_cli-1.0.3/src/viur_cli/build.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/cli.py` & `viur_cli-1.0.3/src/viur_cli/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/conf.py` & `viur_cli-1.0.3/src/viur_cli/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
                 })
     return projectConfig
 
 
 def update_config(path=None):
     assert projectConfig, "load_config() must be called first!"
 
-    assert projectConfig["default"]["format"] in ["1.0.0", "1.0.1", "1.1.0"], "Invalid formatversion, you have to fix it manually"
+    assert projectConfig["default"]["format"] in ["1.0.0", "1.0.1", "1.1.0", "1.1.1"], "Invalid formatversion, you have to fix it manually"
 
     if "format" not in projectConfig["default"]:
         projectConfig["default"]["format"] = "1.0.1"
 
     if "pyodide" not in projectConfig["default"]:
         projectConfig["default"]["pyodide"] = DEFAULT_PYODIDE_VERSION
 
@@ -292,13 +292,14 @@
     if projectConfig["default"]["format"] == "1.1.0":
         projectConfig["default"]["format"] = "1.1.1"
         builds = projectConfig["default"]["builds"].copy()
         for k, v in builds.items():
             if builds[k]["kind"] == "script":
                 builds[k]["kind"] = "exec"
         projectConfig["default"]["builds"] = builds
+
     # conf updates must increase format version
     write_config(projectConfig, path)
```

### Comparing `viur_cli-1.0.2/src/viur_cli/deploy.py` & `viur_cli-1.0.3/src/viur_cli/deploy.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/flare.py` & `viur_cli-1.0.3/src/viur_cli/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/install.py` & `viur_cli-1.0.3/src/viur_cli/install.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/local.py` & `viur_cli-1.0.3/src/viur_cli/local.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/npm.py` & `viur_cli-1.0.3/src/viur_cli/npm.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/cli.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/cli.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/__init__.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/__init__.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/csvwriter.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/csvwriter.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/dialog.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/dialog.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/logger.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/logger.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/module.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/module.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/network.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/network.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/readers.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/readers.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/viur.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/viur.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scriptor/scriptor/writer.py` & `viur_cli-1.0.3/src/viur_cli/scriptor/scriptor/writer.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scripts/flare.py` & `viur_cli-1.0.3/src/viur_cli/scripts/flare.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scripts/get_pyodide.py` & `viur_cli-1.0.3/src/viur_cli/scripts/get_pyodide.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/scripts/viur_2to3.py` & `viur_cli-1.0.3/src/viur_cli/scripts/viur_2to3.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/setup.py` & `viur_cli-1.0.3/src/viur_cli/setup.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/tool.py` & `viur_cli-1.0.3/src/viur_cli/tool.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli/utils.py` & `viur_cli-1.0.3/src/viur_cli/utils.py`

 * *Files identical despite different names*

### Comparing `viur_cli-1.0.2/src/viur_cli.egg-info/PKG-INFO` & `viur_cli-1.0.3/src/viur_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-cli
-Version: 1.0.2
+Version: 1.0.3
 Summary: Command-line interface for ViUR application maintenance.
 Home-page: https://github.com/viur-framework/viur-cli
 Author: Andreas H. Kelch
 Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: viur-cli Version: 1.0.2 Summary: Command-line
+Metadata-Version: 2.1 Name: viur-cli Version: 1.0.3 Summary: Command-line
 interface for ViUR application maintenance. Home-page: https://github.com/viur-
 framework/viur-cli Author: Andreas H. Kelch Author-email: ak@mausbrand.de
 Project-URL: Bug Tracker, https://github.com/viur-framework/viur-cli/issues
 Classifier: Programming Language :: Python :: 3 Classifier: Operating System ::
 OS Independent Classifier: License :: OSI Approved :: MIT License Requires-
 Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE
                       [A hexagonal logo of the viur-cli]
```

### Comparing `viur_cli-1.0.2/src/viur_cli.egg-info/SOURCES.txt` & `viur_cli-1.0.3/src/viur_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

