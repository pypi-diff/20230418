# Comparing `tmp/codepiper-0.1.9.tar.gz` & `tmp/codepiper-0.1.9a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codepiper-0.1.9.tar", last modified: Tue Apr 18 21:36:39 2023, max compression
+gzip compressed data, was "codepiper-0.1.9a2.tar", last modified: Tue Apr 18 21:28:15 2023, max compression
```

## Comparing `codepiper-0.1.9.tar` & `codepiper-0.1.9a2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:36:39.443960 codepiper-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-18 21:36:22.000000 codepiper-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 21:36:22.000000 codepiper-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-18 21:36:39.443960 codepiper-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-18 21:36:22.000000 codepiper-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 21:36:22.000000 codepiper-0.1.9/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:36:39.439960 codepiper-0.1.9/codepiper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/pipeline_clear.py
--rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/rollback.py
--rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-18 21:36:22.000000 codepiper-0.1.9/codepiper/watch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:36:39.439960 codepiper-0.1.9/codepiper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-18 21:36:39.000000 codepiper-0.1.9/codepiper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 21:36:39.000000 codepiper-0.1.9/codepiper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:36:39.000000 codepiper-0.1.9/codepiper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 21:36:39.000000 codepiper-0.1.9/codepiper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 21:36:39.000000 codepiper-0.1.9/codepiper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 21:36:39.000000 codepiper-0.1.9/codepiper.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:36:39.443960 codepiper-0.1.9/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 21:36:22.000000 codepiper-0.1.9/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:36:39.443960 codepiper-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-18 21:36:22.000000 codepiper-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:36:39.443960 codepiper-0.1.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-18 21:36:22.000000 codepiper-0.1.9/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 21:36:22.000000 codepiper-0.1.9/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-18 21:36:22.000000 codepiper-0.1.9/tests/test_rollback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 21:36:22.000000 codepiper-0.1.9/tests/test_watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:15.580094 codepiper-0.1.9a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-18 21:28:15.580094 codepiper-0.1.9a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:15.576094 codepiper-0.1.9a2/codepiper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/pipeline_clear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8921 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/rollback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10332 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/codepiper/watch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:15.576094 codepiper-0.1.9a2/codepiper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-04-18 21:28:15.000000 codepiper-0.1.9a2/codepiper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 21:28:15.000000 codepiper-0.1.9a2/codepiper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:28:15.000000 codepiper-0.1.9a2/codepiper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 21:28:15.000000 codepiper-0.1.9a2/codepiper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 21:28:15.000000 codepiper-0.1.9a2/codepiper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 21:28:15.000000 codepiper-0.1.9a2/codepiper.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:15.576094 codepiper-0.1.9a2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:28:15.580094 codepiper-0.1.9a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:28:15.580094 codepiper-0.1.9a2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/tests/test_rollback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 21:27:51.000000 codepiper-0.1.9a2/tests/test_watch.py
```

### Comparing `codepiper-0.1.9/LICENSE` & `codepiper-0.1.9a2/LICENSE`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/PKG-INFO` & `codepiper-0.1.9a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codepiper
-Version: 0.1.9
+Version: 0.1.9a2
 Summary: Tools for AWS CodePipeline.
 Home-page: https://github.com/gaggle-net/codepiper
 Author: Gaggle Devops
 Author-email: devops@gaggle.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codepiper-0.1.9/README.md` & `codepiper-0.1.9a2/README.md`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper/build.py` & `codepiper-0.1.9a2/codepiper/build.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper/cli.py` & `codepiper-0.1.9a2/codepiper/cli.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper/context.py` & `codepiper-0.1.9a2/codepiper/context.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper/pipeline_clear.py` & `codepiper-0.1.9a2/codepiper/pipeline_clear.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper/rollback.py` & `codepiper-0.1.9a2/codepiper/rollback.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper/watch.py` & `codepiper-0.1.9a2/codepiper/watch.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/codepiper.egg-info/PKG-INFO` & `codepiper-0.1.9a2/codepiper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: codepiper
-Version: 0.1.9
+Version: 0.1.9a2
 Summary: Tools for AWS CodePipeline.
 Home-page: https://github.com/gaggle-net/codepiper
 Author: Gaggle Devops
 Author-email: devops@gaggle.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `codepiper-0.1.9/setup.py` & `codepiper-0.1.9a2/setup.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/tests/test_build.py` & `codepiper-0.1.9a2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `codepiper-0.1.9/tests/test_watch.py` & `codepiper-0.1.9a2/tests/test_watch.py`

 * *Files identical despite different names*

