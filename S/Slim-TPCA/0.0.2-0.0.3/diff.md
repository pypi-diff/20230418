# Comparing `tmp/Slim-TPCA-0.0.2.tar.gz` & `tmp/Slim-TPCA-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slim-TPCA-0.0.2.tar", last modified: Tue Nov  8 05:40:51 2022, max compression
+gzip compressed data, was "Slim-TPCA-0.0.3.tar", last modified: Tue Apr 18 05:55:11 2023, max compression
```

## Comparing `Slim-TPCA-0.0.2.tar` & `Slim-TPCA-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2022-11-08 05:40:51.563349 Slim-TPCA-0.0.2/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1091 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.2/LICENSE
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3266 2022-11-08 05:40:51.563349 Slim-TPCA-0.0.2/PKG-INFO
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     2618 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.2/README.md
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      650 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.2/pyproject.toml
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       38 2022-11-08 05:40:51.563349 Slim-TPCA-0.0.2/setup.cfg
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2022-11-08 05:40:51.563349 Slim-TPCA-0.0.2/src/
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2022-11-08 05:40:51.563349 Slim-TPCA-0.0.2/src/Slim_TPCA/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)    12827 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.2/src/Slim_TPCA/Slim_TPCA.py
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        0 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.2/src/Slim_TPCA/__init__.py
-drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2022-11-08 05:40:51.563349 Slim-TPCA-0.0.2/src/Slim_TPCA.egg-info/
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3266 2022-11-08 05:40:51.000000 Slim-TPCA-0.0.2/src/Slim_TPCA.egg-info/PKG-INFO
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      233 2022-11-08 05:40:51.000000 Slim-TPCA-0.0.2/src/Slim_TPCA.egg-info/SOURCES.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2022-11-08 05:40:51.000000 Slim-TPCA-0.0.2/src/Slim_TPCA.egg-info/dependency_links.txt
--rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       10 2022-11-08 05:40:51.000000 Slim-TPCA-0.0.2/src/Slim_TPCA.egg-info/top_level.txt
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 05:55:11.063089 Slim-TPCA-0.0.3/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1091 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.3/LICENSE
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 05:55:11.063089 Slim-TPCA-0.0.3/PKG-INFO
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     2618 2022-11-08 05:40:40.000000 Slim-TPCA-0.0.3/README.md
+drwxrwxr-x   0 wangjun   (1000) wangjun   (1000)        0 2023-04-18 05:55:11.059089 Slim-TPCA-0.0.3/Slim_TPCA.egg-info/
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     3346 2023-04-18 05:55:10.000000 Slim-TPCA-0.0.3/Slim_TPCA.egg-info/PKG-INFO
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      205 2023-04-18 05:55:10.000000 Slim-TPCA-0.0.3/Slim_TPCA.egg-info/SOURCES.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 05:55:10.000000 Slim-TPCA-0.0.3/Slim_TPCA.egg-info/dependency_links.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       88 2023-04-18 05:55:10.000000 Slim-TPCA-0.0.3/Slim_TPCA.egg-info/requires.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)        1 2023-04-18 05:55:10.000000 Slim-TPCA-0.0.3/Slim_TPCA.egg-info/top_level.txt
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)      652 2023-04-18 05:49:54.000000 Slim-TPCA-0.0.3/pyproject.toml
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)       38 2023-04-18 05:55:11.063089 Slim-TPCA-0.0.3/setup.cfg
+-rw-rw-r--   0 wangjun   (1000) wangjun   (1000)     1079 2023-04-18 05:42:23.000000 Slim-TPCA-0.0.3/setup.py
```

### Comparing `Slim-TPCA-0.0.2/LICENSE` & `Slim-TPCA-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `Slim-TPCA-0.0.2/PKG-INFO` & `Slim-TPCA-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: Slim-TPCA
-Version: 0.0.2
+Version: 0.0.3
 Summary: Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations
+Home-page: https://github.com/wangjun258/Slim_TPCA
+Author: Siyuan Sun, Jun Wang
 Author-email: Siyuan Sun <11930100@mail.sustech.edu.cn>
 Project-URL: Homepage, https://github.com/pypa/Slim_TPCA
 Project-URL: Bug Tracker, https://github.com/pypa/Slim_TPCA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `Slim-TPCA-0.0.2/README.md` & `Slim-TPCA-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `Slim-TPCA-0.0.2/pyproject.toml` & `Slim-TPCA-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "Slim-TPCA"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Siyuan Sun", email="11930100@mail.sustech.edu.cn" },
 ]
 description = "Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/Slim_TPCA"
-"Bug Tracker" = "https://github.com/pypa/Slim_TPCA/issues"
+"Bug Tracker" = "https://github.com/pypa/Slim_TPCA/issues"
```

### Comparing `Slim-TPCA-0.0.2/src/Slim_TPCA.egg-info/PKG-INFO` & `Slim-TPCA-0.0.3/Slim_TPCA.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Metadata-Version: 2.1
 Name: Slim-TPCA
-Version: 0.0.2
+Version: 0.0.3
 Summary: Slim-TPCA: a python package to expediate functional characterization of existing and newly identified protein complexes by optimizing existing TPCA algorithm implementations
+Home-page: https://github.com/wangjun258/Slim_TPCA
+Author: Siyuan Sun, Jun Wang
 Author-email: Siyuan Sun <11930100@mail.sustech.edu.cn>
 Project-URL: Homepage, https://github.com/pypa/Slim_TPCA
 Project-URL: Bug Tracker, https://github.com/pypa/Slim_TPCA/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

