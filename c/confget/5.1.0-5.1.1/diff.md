# Comparing `tmp/confget-5.1.0.tar.gz` & `tmp/confget-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "confget-5.1.0.tar", last modified: Mon Feb 13 23:33:26 2023, max compression
+gzip compressed data, was "confget-5.1.1.tar", last modified: Tue Apr 18 10:28:33 2023, max compression
```

## Comparing `confget-5.1.0.tar` & `confget-5.1.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/
--rw-r--r--   0 roam      (1000) roam      (1000)      134 2023-02-13 14:40:44.000000 confget-5.1.0/MANIFEST.in
--rw-r--r--   0 roam      (1000) roam      (1000)     4588 2023-02-13 23:33:26.536742 confget-5.1.0/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     3336 2021-10-05 11:23:09.000000 confget-5.1.0/README.md
--rw-r--r--   0 roam      (1000) roam      (1000)     1512 2023-02-13 22:20:14.000000 confget-5.1.0/pyproject.toml
--rw-r--r--   0 roam      (1000) roam      (1000)     1472 2023-02-13 23:33:26.536742 confget-5.1.0/setup.cfg
--rw-r--r--   0 roam      (1000) roam      (1000)     1485 2023-02-13 12:40:07.000000 confget-5.1.0/setup.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.532742 confget-5.1.0/src/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.532742 confget-5.1.0/src/confget/
--rw-r--r--   0 roam      (1000) roam      (1000)     5539 2023-02-13 20:36:10.000000 confget-5.1.0/src/confget/__init__.py
--rwxr-xr-x   0 roam      (1000) roam      (1000)    10212 2023-02-13 20:46:21.000000 confget-5.1.0/src/confget/__main__.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/src/confget/backend/
--rw-r--r--   0 roam      (1000) roam      (1000)     1751 2023-02-13 22:14:33.000000 confget-5.1.0/src/confget/backend/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2265 2023-02-13 12:40:07.000000 confget-5.1.0/src/confget/backend/abstract.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2540 2023-02-13 20:53:21.000000 confget-5.1.0/src/confget/backend/ini_base.py
--rw-r--r--   0 roam      (1000) roam      (1000)     7511 2023-02-13 20:55:40.000000 confget-5.1.0/src/confget/backend/ini_pyp.py
--rw-r--r--   0 roam      (1000) roam      (1000)     4918 2023-02-13 22:13:21.000000 confget-5.1.0/src/confget/backend/ini_re.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2379 2023-02-13 23:29:15.000000 confget-5.1.0/src/confget/defs.py
--rw-r--r--   0 roam      (1000) roam      (1000)     5711 2023-02-13 19:55:10.000000 confget-5.1.0/src/confget/format.py
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-05-12 08:45:55.000000 confget-5.1.0/src/confget/py.typed
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/src/confget.egg-info/
--rw-r--r--   0 roam      (1000) roam      (1000)     4588 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/PKG-INFO
--rw-r--r--   0 roam      (1000) roam      (1000)     1250 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/SOURCES.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/dependency_links.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       50 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/entry_points.txt
--rw-r--r--   0 roam      (1000) roam      (1000)       16 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/requires.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        8 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/top_level.txt
--rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-02-13 23:33:26.000000 confget-5.1.0/src/confget.egg-info/zip-safe
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/test_data/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.532742 confget-5.1.0/test_data/defs/
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/test_data/defs/tests/
--rw-r--r--   0 roam      (1000) roam      (1000)     4199 2023-02-13 14:59:24.000000 confget-5.1.0/test_data/defs/tests/01-get-values.json
--rw-r--r--   0 roam      (1000) roam      (1000)     2959 2023-02-13 14:59:29.000000 confget-5.1.0/test_data/defs/tests/02-check-values.json
--rw-r--r--   0 roam      (1000) roam      (1000)     1454 2021-10-05 11:23:09.000000 confget-5.1.0/test_data/defs/tests/03-list-all.json
--rw-r--r--   0 roam      (1000) roam      (1000)     1300 2021-10-05 11:23:09.000000 confget-5.1.0/test_data/defs/tests/05-match-names.json
--rw-r--r--   0 roam      (1000) roam      (1000)     1241 2021-10-05 11:23:09.000000 confget-5.1.0/test_data/defs/tests/06-get-default.json
--rw-r--r--   0 roam      (1000) roam      (1000)     2726 2021-10-05 11:23:09.000000 confget-5.1.0/test_data/defs/tests/07-match-values.json
--rw-r--r--   0 roam      (1000) roam      (1000)     2653 2021-10-05 11:23:09.000000 confget-5.1.0/test_data/defs/tests/11-no-default.json
--rw-r--r--   0 roam      (1000) roam      (1000)     3682 2021-10-05 11:23:09.000000 confget-5.1.0/test_data/defs/tests/12-last-value.json
--rw-r--r--   0 roam      (1000) roam      (1000)     1183 2023-02-13 12:40:07.000000 confget-5.1.0/test_data/t1.ini
--rw-r--r--   0 roam      (1000) roam      (1000)     1043 2021-05-12 08:45:55.000000 confget-5.1.0/test_data/t2.ini
--rw-r--r--   0 roam      (1000) roam      (1000)      247 2021-05-12 08:45:55.000000 confget-5.1.0/test_data/t3.ini
--rw-r--r--   0 roam      (1000) roam      (1000)      274 2021-05-12 08:45:55.000000 confget-5.1.0/test_data/t4.ini
--rw-r--r--   0 roam      (1000) roam      (1000)       82 2023-02-13 12:40:07.000000 confget-5.1.0/test_data/t5.ini
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2023-02-13 14:59:39.000000 confget-5.1.0/test_data/t6.ini
--rw-r--r--   0 roam      (1000) roam      (1000)       10 2023-02-13 14:59:39.000000 confget-5.1.0/test_data/t7.ini
--rw-r--r--   0 roam      (1000) roam      (1000)       17 2023-02-13 14:59:39.000000 confget-5.1.0/test_data/t8.ini
--rw-r--r--   0 roam      (1000) roam      (1000)        7 2023-02-13 14:59:39.000000 confget-5.1.0/test_data/t9.ini
--rwxr-xr-x   0 roam      (1000) roam      (1000)     1772 2021-11-21 16:49:56.000000 confget-5.1.0/tox-devel.sh
--rw-r--r--   0 roam      (1000) roam      (1000)     3724 2023-02-13 22:20:14.000000 confget-5.1.0/tox.ini
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/unit_tests/
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-05-12 08:45:55.000000 confget-5.1.0/unit_tests/__init__.py
-drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-02-13 23:33:26.536742 confget-5.1.0/unit_tests/data/
--rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-05-12 08:45:55.000000 confget-5.1.0/unit_tests/data/__init__.py
--rw-r--r--   0 roam      (1000) roam      (1000)     8370 2023-02-13 20:56:29.000000 confget-5.1.0/unit_tests/data/test_defs.py
--rw-r--r--   0 roam      (1000) roam      (1000)     3403 2023-02-13 21:50:52.000000 confget-5.1.0/unit_tests/data/test_load.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2486 2023-02-13 20:56:17.000000 confget-5.1.0/unit_tests/test_parser.py
--rw-r--r--   0 roam      (1000) roam      (1000)     3733 2023-02-13 21:17:26.000000 confget-5.1.0/unit_tests/test_run.py
--rw-r--r--   0 roam      (1000) roam      (1000)     2558 2023-02-13 12:40:07.000000 confget-5.1.0/unit_tests/test_test_data.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/
+-rw-r--r--   0 roam      (1000) roam      (1000)      134 2023-02-13 14:40:44.000000 confget-5.1.1/MANIFEST.in
+-rw-r--r--   0 roam      (1000) roam      (1000)     4588 2023-04-18 10:28:33.589914 confget-5.1.1/PKG-INFO
+-rw-r--r--   0 roam      (1000) roam      (1000)     3336 2021-10-05 11:23:09.000000 confget-5.1.1/README.md
+-rw-r--r--   0 roam      (1000) roam      (1000)     1512 2023-02-13 22:20:14.000000 confget-5.1.1/pyproject.toml
+-rw-r--r--   0 roam      (1000) roam      (1000)     1546 2023-04-18 10:28:33.589914 confget-5.1.1/setup.cfg
+-rw-r--r--   0 roam      (1000) roam      (1000)     1485 2023-02-13 12:40:07.000000 confget-5.1.1/setup.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.585914 confget-5.1.1/src/
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/src/confget/
+-rw-r--r--   0 roam      (1000) roam      (1000)     5539 2023-02-13 20:36:10.000000 confget-5.1.1/src/confget/__init__.py
+-rwxr-xr-x   0 roam      (1000) roam      (1000)    10212 2023-02-13 20:46:21.000000 confget-5.1.1/src/confget/__main__.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/src/confget/backend/
+-rw-r--r--   0 roam      (1000) roam      (1000)     1751 2023-02-13 22:14:33.000000 confget-5.1.1/src/confget/backend/__init__.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     2265 2023-02-13 12:40:07.000000 confget-5.1.1/src/confget/backend/abstract.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     2540 2023-02-13 20:53:21.000000 confget-5.1.1/src/confget/backend/ini_base.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     7511 2023-02-13 20:55:40.000000 confget-5.1.1/src/confget/backend/ini_pyp.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     4918 2023-02-13 22:13:21.000000 confget-5.1.1/src/confget/backend/ini_re.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     2379 2023-04-18 10:25:16.000000 confget-5.1.1/src/confget/defs.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     5711 2023-02-13 19:55:10.000000 confget-5.1.1/src/confget/format.py
+-rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-05-12 08:45:55.000000 confget-5.1.1/src/confget/py.typed
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/src/confget.egg-info/
+-rw-r--r--   0 roam      (1000) roam      (1000)     4588 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/PKG-INFO
+-rw-r--r--   0 roam      (1000) roam      (1000)     1250 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/SOURCES.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/dependency_links.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)       50 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/entry_points.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)       55 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/requires.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        8 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/top_level.txt
+-rw-r--r--   0 roam      (1000) roam      (1000)        1 2023-04-18 10:28:33.000000 confget-5.1.1/src/confget.egg-info/zip-safe
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/test_data/
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.585914 confget-5.1.1/test_data/defs/
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/test_data/defs/tests/
+-rw-r--r--   0 roam      (1000) roam      (1000)     4199 2023-02-13 14:59:24.000000 confget-5.1.1/test_data/defs/tests/01-get-values.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     2959 2023-02-13 14:59:29.000000 confget-5.1.1/test_data/defs/tests/02-check-values.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     1454 2021-10-05 11:23:09.000000 confget-5.1.1/test_data/defs/tests/03-list-all.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     1300 2021-10-05 11:23:09.000000 confget-5.1.1/test_data/defs/tests/05-match-names.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     1241 2021-10-05 11:23:09.000000 confget-5.1.1/test_data/defs/tests/06-get-default.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     2726 2021-10-05 11:23:09.000000 confget-5.1.1/test_data/defs/tests/07-match-values.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     2653 2021-10-05 11:23:09.000000 confget-5.1.1/test_data/defs/tests/11-no-default.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     3682 2021-10-05 11:23:09.000000 confget-5.1.1/test_data/defs/tests/12-last-value.json
+-rw-r--r--   0 roam      (1000) roam      (1000)     1183 2023-02-13 12:40:07.000000 confget-5.1.1/test_data/t1.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)     1043 2021-05-12 08:45:55.000000 confget-5.1.1/test_data/t2.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)      247 2021-05-12 08:45:55.000000 confget-5.1.1/test_data/t3.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)      274 2021-05-12 08:45:55.000000 confget-5.1.1/test_data/t4.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)       82 2023-02-13 12:40:07.000000 confget-5.1.1/test_data/t5.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)        0 2023-02-13 14:59:39.000000 confget-5.1.1/test_data/t6.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)       10 2023-02-13 14:59:39.000000 confget-5.1.1/test_data/t7.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)       17 2023-02-13 14:59:39.000000 confget-5.1.1/test_data/t8.ini
+-rw-r--r--   0 roam      (1000) roam      (1000)        7 2023-02-13 14:59:39.000000 confget-5.1.1/test_data/t9.ini
+-rwxr-xr-x   0 roam      (1000) roam      (1000)     1772 2021-11-21 16:49:56.000000 confget-5.1.1/tox-devel.sh
+-rw-r--r--   0 roam      (1000) roam      (1000)     3724 2023-02-13 22:20:14.000000 confget-5.1.1/tox.ini
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/unit_tests/
+-rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-05-12 08:45:55.000000 confget-5.1.1/unit_tests/__init__.py
+drwxr-xr-x   0 roam      (1000) roam      (1000)        0 2023-04-18 10:28:33.589914 confget-5.1.1/unit_tests/data/
+-rw-r--r--   0 roam      (1000) roam      (1000)        0 2021-05-12 08:45:55.000000 confget-5.1.1/unit_tests/data/__init__.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     8370 2023-02-13 20:56:29.000000 confget-5.1.1/unit_tests/data/test_defs.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     3403 2023-02-13 21:50:52.000000 confget-5.1.1/unit_tests/data/test_load.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     2486 2023-02-13 20:56:17.000000 confget-5.1.1/unit_tests/test_parser.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     3733 2023-02-13 21:17:26.000000 confget-5.1.1/unit_tests/test_run.py
+-rw-r--r--   0 roam      (1000) roam      (1000)     2558 2023-02-13 12:40:07.000000 confget-5.1.1/unit_tests/test_test_data.py
```

### Comparing `confget-5.1.0/PKG-INFO` & `confget-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confget
-Version: 5.1.0
+Version: 5.1.1
 Summary: Parse configuration files and extract values from them
 Home-page: https://devel.ringlet.net/textproc/confget/
 Author: Peter Pentchev
 Author-email: roam@ringlet.net
 License: BSD-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `confget-5.1.0/README.md` & `confget-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/pyproject.toml` & `confget-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/setup.cfg` & `confget-5.1.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -34,15 +34,17 @@
 zip_safe = True
 package_dir = 
 	=src
 packages = 
 	confget
 	confget.backend
 setup_requires = 
+	dataclasses; python_version < '3.7'
 install_requires = 
+	dataclasses; python_version < '3.7'
 	pyparsing >= 3, < 4
 python_requires = >= 3.6
 
 [options.entry_points]
 console_scripts = 
 	confget = confget.__main__:main
```

### Comparing `confget-5.1.0/setup.py` & `confget-5.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/__init__.py` & `confget-5.1.1/src/confget/__init__.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/__main__.py` & `confget-5.1.1/src/confget/__main__.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/backend/__init__.py` & `confget-5.1.1/src/confget/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/backend/abstract.py` & `confget-5.1.1/src/confget/backend/abstract.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/backend/ini_base.py` & `confget-5.1.1/src/confget/backend/ini_base.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/backend/ini_pyp.py` & `confget-5.1.1/src/confget/backend/ini_pyp.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/backend/ini_re.py` & `confget-5.1.1/src/confget/backend/ini_re.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget/defs.py` & `confget-5.1.1/src/confget/defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     INI_REGEX = "ini-regex"
 
     def __str__(self) -> str:
         """Return a human-readable representation (the string itself)."""
         return self.value
 
 
-VERSION_STRING = "5.1.0"
+VERSION_STRING = "5.1.1"
 FEATURES = [
     ("BASE", VERSION_STRING),
     ("REGEX", "1.0"),
     (
         "REGEX_IMPL_PYTHON",
         f"{sys.version_info[0]}.{sys.version_info[1]}",
     ),
```

### Comparing `confget-5.1.0/src/confget/format.py` & `confget-5.1.1/src/confget/format.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/src/confget.egg-info/PKG-INFO` & `confget-5.1.1/src/confget.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: confget
-Version: 5.1.0
+Version: 5.1.1
 Summary: Parse configuration files and extract values from them
 Home-page: https://devel.ringlet.net/textproc/confget/
 Author: Peter Pentchev
 Author-email: roam@ringlet.net
 License: BSD-2
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `confget-5.1.0/src/confget.egg-info/SOURCES.txt` & `confget-5.1.1/src/confget.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/01-get-values.json` & `confget-5.1.1/test_data/defs/tests/01-get-values.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/02-check-values.json` & `confget-5.1.1/test_data/defs/tests/02-check-values.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/03-list-all.json` & `confget-5.1.1/test_data/defs/tests/03-list-all.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/05-match-names.json` & `confget-5.1.1/test_data/defs/tests/05-match-names.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/06-get-default.json` & `confget-5.1.1/test_data/defs/tests/06-get-default.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/07-match-values.json` & `confget-5.1.1/test_data/defs/tests/07-match-values.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/11-no-default.json` & `confget-5.1.1/test_data/defs/tests/11-no-default.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/defs/tests/12-last-value.json` & `confget-5.1.1/test_data/defs/tests/12-last-value.json`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/t1.ini` & `confget-5.1.1/test_data/t1.ini`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/test_data/t2.ini` & `confget-5.1.1/test_data/t2.ini`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/tox-devel.sh` & `confget-5.1.1/tox-devel.sh`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/tox.ini` & `confget-5.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/unit_tests/data/test_defs.py` & `confget-5.1.1/unit_tests/data/test_defs.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/unit_tests/data/test_load.py` & `confget-5.1.1/unit_tests/data/test_load.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/unit_tests/test_parser.py` & `confget-5.1.1/unit_tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/unit_tests/test_run.py` & `confget-5.1.1/unit_tests/test_run.py`

 * *Files identical despite different names*

### Comparing `confget-5.1.0/unit_tests/test_test_data.py` & `confget-5.1.1/unit_tests/test_test_data.py`

 * *Files identical despite different names*

