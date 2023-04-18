# Comparing `tmp/receptorctl-1.4.0.dev1.tar.gz` & `tmp/receptorctl-1.4.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "receptorctl-1.4.0.dev1.tar", last modified: Tue Apr 18 00:08:57 2023, max compression
+gzip compressed data, was "receptorctl-1.4.0.dev2.tar", last modified: Tue Apr 18 17:17:31 2023, max compression
```

## Comparing `receptorctl-1.4.0.dev1.tar` & `receptorctl-1.4.0.dev2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:57.792880 receptorctl-1.4.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 00:08:40.000000 receptorctl-1.4.0.dev1/.VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 00:08:57.792880 receptorctl-1.4.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:57.792880 receptorctl-1.4.0.dev1/receptorctl/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/receptorctl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/receptorctl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/receptorctl/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/receptorctl/socket_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:57.792880 receptorctl-1.4.0.dev1/receptorctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 00:08:57.000000 receptorctl-1.4.0.dev1/receptorctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 00:08:57.000000 receptorctl-1.4.0.dev1/receptorctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:08:57.000000 receptorctl-1.4.0.dev1/receptorctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 00:08:57.000000 receptorctl-1.4.0.dev1/receptorctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 00:08:57.000000 receptorctl-1.4.0.dev1/receptorctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 00:08:57.000000 receptorctl-1.4.0.dev1/receptorctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 00:08:57.792880 receptorctl-1.4.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:08:57.792880 receptorctl-1.4.0.dev1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/tests/test_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/tests/test_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-18 00:08:32.000000 receptorctl-1.4.0.dev1/tests/test_workunit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:17:31.136935 receptorctl-1.4.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 17:17:17.000000 receptorctl-1.4.0.dev2/.VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 17:17:31.136935 receptorctl-1.4.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:17:31.132935 receptorctl-1.4.0.dev2/receptorctl/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/receptorctl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/receptorctl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18198 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/receptorctl/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9768 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/receptorctl/socket_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:17:31.136935 receptorctl-1.4.0.dev2/receptorctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 17:17:31.000000 receptorctl-1.4.0.dev2/receptorctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 17:17:31.000000 receptorctl-1.4.0.dev2/receptorctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:17:31.000000 receptorctl-1.4.0.dev2/receptorctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-18 17:17:31.000000 receptorctl-1.4.0.dev2/receptorctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-18 17:17:31.000000 receptorctl-1.4.0.dev2/receptorctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 17:17:31.000000 receptorctl-1.4.0.dev2/receptorctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-18 17:17:31.136935 receptorctl-1.4.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:17:31.136935 receptorctl-1.4.0.dev2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/tests/test_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/tests/test_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5495 2023-04-18 17:17:09.000000 receptorctl-1.4.0.dev2/tests/test_workunit.py
```

### Comparing `receptorctl-1.4.0.dev1/receptorctl/cli.py` & `receptorctl-1.4.0.dev2/receptorctl/cli.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.0.dev1/receptorctl/socket_interface.py` & `receptorctl-1.4.0.dev2/receptorctl/socket_interface.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.0.dev1/setup.cfg` & `receptorctl-1.4.0.dev2/setup.cfg`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.0.dev1/tests/test_cli.py` & `receptorctl-1.4.0.dev2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.0.dev1/tests/test_connection.py` & `receptorctl-1.4.0.dev2/tests/test_connection.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.0.dev1/tests/test_mesh.py` & `receptorctl-1.4.0.dev2/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `receptorctl-1.4.0.dev1/tests/test_workunit.py` & `receptorctl-1.4.0.dev2/tests/test_workunit.py`

 * *Files identical despite different names*

