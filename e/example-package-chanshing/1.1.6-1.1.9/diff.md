# Comparing `tmp/example-package-chanshing-1.1.6.tar.gz` & `tmp/example-package-chanshing-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example-package-chanshing-1.1.6.tar", last modified: Thu Mar 30 15:45:01 2023, max compression
+gzip compressed data, was "example-package-chanshing-1.1.9.tar", last modified: Thu Mar 30 17:36:41 2023, max compression
```

## Comparing `example-package-chanshing-1.1.6.tar` & `example-package-chanshing-1.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:45:01.212062 example-package-chanshing-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-30 15:45:01.212062 example-package-chanshing-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 15:45:01.212062 example-package-chanshing-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:45:01.208062 example-package-chanshing-1.1.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:45:01.212062 example-package-chanshing-1.1.6/src/example/
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/src/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-30 15:45:01.212062 example-package-chanshing-1.1.6/src/example/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/src/example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 15:45:01.212062 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-30 15:45:01.000000 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-30 15:45:01.000000 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 15:45:01.000000 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 15:45:01.000000 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-30 15:45:01.000000 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 15:45:01.000000 example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-30 15:44:53.000000 example-package-chanshing-1.1.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/src/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/src/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/src/example/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/src/example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-30 17:36:41.373951 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-30 17:36:41.000000 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-03-30 17:36:41.000000 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-30 17:36:41.000000 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-30 17:36:41.000000 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-03-30 17:36:41.000000 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-30 17:36:41.000000 example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83607 2023-03-30 17:36:32.000000 example-package-chanshing-1.1.9/versioneer.py
```

### Comparing `example-package-chanshing-1.1.6/PKG-INFO` & `example-package-chanshing-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-package-chanshing
-Version: 1.1.6
+Version: 1.1.9
 Summary: An example Python project
 Home-page: https://github.com/chanshing/example-package
 Author: Shing Chan
 Maintainer: Shing Chan
 Maintainer-email: cshing.m@gmail.com
 License: See LICENSE file.
 Download-URL: https://github.com/chanshing/example-package
```

### Comparing `example-package-chanshing-1.1.6/pyproject.toml` & `example-package-chanshing-1.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `example-package-chanshing-1.1.6/setup.py` & `example-package-chanshing-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `example-package-chanshing-1.1.6/src/example_package_chanshing.egg-info/PKG-INFO` & `example-package-chanshing-1.1.9/src/example_package_chanshing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example-package-chanshing
-Version: 1.1.6
+Version: 1.1.9
 Summary: An example Python project
 Home-page: https://github.com/chanshing/example-package
 Author: Shing Chan
 Maintainer: Shing Chan
 Maintainer-email: cshing.m@gmail.com
 License: See LICENSE file.
 Download-URL: https://github.com/chanshing/example-package
```

### Comparing `example-package-chanshing-1.1.6/versioneer.py` & `example-package-chanshing-1.1.9/versioneer.py`

 * *Files identical despite different names*

