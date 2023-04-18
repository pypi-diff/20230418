# Comparing `tmp/yellowdog-python-examples-5.0.4.tar.gz` & `tmp/yellowdog-python-examples-5.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yellowdog-python-examples-5.0.4.tar", last modified: Mon Apr 17 15:22:50 2023, max compression
+gzip compressed data, was "yellowdog-python-examples-5.0.5.tar", last modified: Tue Apr 18 12:14:44 2023, max compression
```

## Comparing `yellowdog-python-examples-5.0.4.tar` & `yellowdog-python-examples-5.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-17 15:22:50.404493 yellowdog-python-examples-5.0.4/
--rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.4/LICENSE
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-17 15:22:50.404555 yellowdog-python-examples-5.0.4/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.4/PYPI_README.md
--rw-r--r--   0 pwt        (501) staff       (20)   109332 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.4/README.md
--rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.4/pyproject.toml
--rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.4/requirements.txt
--rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-17 15:22:50.404832 yellowdog-python-examples-5.0.4/setup.cfg
--rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.4/setup.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-17 15:22:50.403625 yellowdog-python-examples-5.0.4/yd_commands/
--rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-17 15:22:18.000000 yellowdog-python-examples-5.0.4/yd_commands/__init__.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.4/yd_commands/abort.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.4/yd_commands/admin.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.4/yd_commands/args.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.4/yd_commands/cancel.py
--rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.4/yd_commands/check_imports.py
--rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.4/yd_commands/compact_json.py
--rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.4/yd_commands/config.py
--rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.4/yd_commands/config_keys.py
--rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.4/yd_commands/csv_data.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.4/yd_commands/delete.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.4/yd_commands/download.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.4/yd_commands/instantiate.py
--rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.4/yd_commands/interactive.py
--rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.4/yd_commands/jsonnet2json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.4/yd_commands/list.py
--rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.4/yd_commands/object_utilities.py
--rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.4/yd_commands/printing.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.4/yd_commands/provision.py
--rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.4/yd_commands/provision_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.4/yd_commands/reformat_json.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.4/yd_commands/shutdown.py
--rwxr-xr-x   0 pwt        (501) staff       (20)    40028 2023-04-17 15:22:18.000000 yellowdog-python-examples-5.0.4/yd_commands/submit.py
--rw-r--r--   0 pwt        (501) staff       (20)     6051 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.4/yd_commands/submit_utils.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.4/yd_commands/terminate.py
--rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.4/yd_commands/type_check.py
--rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.4/yd_commands/upload.py
--rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.4/yd_commands/upload_utils.py
--rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.4/yd_commands/validate_properties.py
--rw-r--r--   0 pwt        (501) staff       (20)    11055 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.4/yd_commands/variables.py
--rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.4/yd_commands/version.py
--rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.4/yd_commands/wrapper.py
-drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-17 15:22:50.404395 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/
--rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-17 15:22:50.000000 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/PKG-INFO
--rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-17 15:22:50.000000 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/SOURCES.txt
--rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-17 15:22:50.000000 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/dependency_links.txt
--rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-17 15:22:50.000000 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/entry_points.txt
--rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-17 15:22:50.000000 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/requires.txt
--rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-17 15:22:50.000000 yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/top_level.txt
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-18 12:14:44.358337 yellowdog-python-examples-5.0.5/
+-rw-r--r--   0 pwt        (501) staff       (20)    11357 2022-11-18 20:55:26.000000 yellowdog-python-examples-5.0.5/LICENSE
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-18 12:14:44.358406 yellowdog-python-examples-5.0.5/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)      676 2022-11-22 08:58:59.000000 yellowdog-python-examples-5.0.5/PYPI_README.md
+-rw-r--r--   0 pwt        (501) staff       (20)   109332 2023-04-18 11:54:44.000000 yellowdog-python-examples-5.0.5/README.md
+-rw-r--r--   0 pwt        (501) staff       (20)     1806 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.5/pyproject.toml
+-rw-r--r--   0 pwt        (501) staff       (20)       46 2023-03-31 14:34:07.000000 yellowdog-python-examples-5.0.5/requirements.txt
+-rw-r--r--   0 pwt        (501) staff       (20)     1366 2023-04-18 12:14:44.358706 yellowdog-python-examples-5.0.5/setup.cfg
+-rw-r--r--   0 pwt        (501) staff       (20)      125 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/setup.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-18 12:14:44.357434 yellowdog-python-examples-5.0.5/yd_commands/
+-rw-r--r--   0 pwt        (501) staff       (20)       22 2023-04-18 12:14:05.000000 yellowdog-python-examples-5.0.5/yd_commands/__init__.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3378 2023-03-28 12:34:54.000000 yellowdog-python-examples-5.0.5/yd_commands/abort.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      982 2023-01-31 15:59:12.000000 yellowdog-python-examples-5.0.5/yd_commands/admin.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    17864 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/args.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     5077 2023-02-22 19:37:56.000000 yellowdog-python-examples-5.0.5/yd_commands/cancel.py
+-rw-r--r--   0 pwt        (501) staff       (20)      579 2022-12-12 15:56:41.000000 yellowdog-python-examples-5.0.5/yd_commands/check_imports.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3757 2022-11-27 20:53:08.000000 yellowdog-python-examples-5.0.5/yd_commands/compact_json.py
+-rw-r--r--   0 pwt        (501) staff       (20)    18238 2023-03-31 13:51:41.000000 yellowdog-python-examples-5.0.5/yd_commands/config.py
+-rw-r--r--   0 pwt        (501) staff       (20)     5474 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/config_keys.py
+-rw-r--r--   0 pwt        (501) staff       (20)    12183 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.5/yd_commands/csv_data.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1647 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/delete.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3616 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/download.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     9203 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.5/yd_commands/instantiate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3749 2022-12-01 11:00:21.000000 yellowdog-python-examples-5.0.5/yd_commands/interactive.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)      749 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/jsonnet2json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     7539 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.5/yd_commands/list.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3012 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/object_utilities.py
+-rw-r--r--   0 pwt        (501) staff       (20)     9590 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/printing.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    16885 2023-03-28 14:27:45.000000 yellowdog-python-examples-5.0.5/yd_commands/provision.py
+-rw-r--r--   0 pwt        (501) staff       (20)      789 2023-03-13 13:46:12.000000 yellowdog-python-examples-5.0.5/yd_commands/provision_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1479 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/reformat_json.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     3231 2023-02-14 10:40:48.000000 yellowdog-python-examples-5.0.5/yd_commands/shutdown.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)    40102 2023-04-18 12:14:05.000000 yellowdog-python-examples-5.0.5/yd_commands/submit.py
+-rw-r--r--   0 pwt        (501) staff       (20)     6051 2023-04-14 14:20:07.000000 yellowdog-python-examples-5.0.5/yd_commands/submit_utils.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     2756 2023-02-20 09:23:16.000000 yellowdog-python-examples-5.0.5/yd_commands/terminate.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1678 2022-12-07 08:38:57.000000 yellowdog-python-examples-5.0.5/yd_commands/type_check.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2252 2023-03-15 09:01:37.000000 yellowdog-python-examples-5.0.5/yd_commands/upload.py
+-rw-r--r--   0 pwt        (501) staff       (20)     3389 2023-03-14 20:22:33.000000 yellowdog-python-examples-5.0.5/yd_commands/upload_utils.py
+-rw-r--r--   0 pwt        (501) staff       (20)     1630 2023-03-02 09:05:10.000000 yellowdog-python-examples-5.0.5/yd_commands/validate_properties.py
+-rw-r--r--   0 pwt        (501) staff       (20)    11055 2023-04-17 15:00:55.000000 yellowdog-python-examples-5.0.5/yd_commands/variables.py
+-rwxr-xr-x   0 pwt        (501) staff       (20)     1247 2023-03-24 08:40:30.000000 yellowdog-python-examples-5.0.5/yd_commands/version.py
+-rw-r--r--   0 pwt        (501) staff       (20)     2200 2023-02-04 22:01:25.000000 yellowdog-python-examples-5.0.5/yd_commands/wrapper.py
+drwxr-xr-x   0 pwt        (501) staff       (20)        0 2023-04-18 12:14:44.358233 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/
+-rw-r--r--   0 pwt        (501) staff       (20)     1418 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/PKG-INFO
+-rw-r--r--   0 pwt        (501) staff       (20)     1187 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/SOURCES.txt
+-rw-r--r--   0 pwt        (501) staff       (20)        1 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/dependency_links.txt
+-rw-r--r--   0 pwt        (501) staff       (20)      574 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/entry_points.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       61 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/requires.txt
+-rw-r--r--   0 pwt        (501) staff       (20)       12 2023-04-18 12:14:44.000000 yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/top_level.txt
```

### Comparing `yellowdog-python-examples-5.0.4/LICENSE` & `yellowdog-python-examples-5.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/PKG-INFO` & `yellowdog-python-examples-5.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.4
+Version: 5.0.5
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.4/PYPI_README.md` & `yellowdog-python-examples-5.0.5/PYPI_README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/README.md` & `yellowdog-python-examples-5.0.5/README.md`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/pyproject.toml` & `yellowdog-python-examples-5.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/setup.cfg` & `yellowdog-python-examples-5.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/abort.py` & `yellowdog-python-examples-5.0.5/yd_commands/abort.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/admin.py` & `yellowdog-python-examples-5.0.5/yd_commands/admin.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/args.py` & `yellowdog-python-examples-5.0.5/yd_commands/args.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/cancel.py` & `yellowdog-python-examples-5.0.5/yd_commands/cancel.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/check_imports.py` & `yellowdog-python-examples-5.0.5/yd_commands/check_imports.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/compact_json.py` & `yellowdog-python-examples-5.0.5/yd_commands/compact_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/config.py` & `yellowdog-python-examples-5.0.5/yd_commands/config.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/config_keys.py` & `yellowdog-python-examples-5.0.5/yd_commands/config_keys.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/csv_data.py` & `yellowdog-python-examples-5.0.5/yd_commands/csv_data.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/delete.py` & `yellowdog-python-examples-5.0.5/yd_commands/delete.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/download.py` & `yellowdog-python-examples-5.0.5/yd_commands/download.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/instantiate.py` & `yellowdog-python-examples-5.0.5/yd_commands/instantiate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/interactive.py` & `yellowdog-python-examples-5.0.5/yd_commands/interactive.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/jsonnet2json.py` & `yellowdog-python-examples-5.0.5/yd_commands/jsonnet2json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/list.py` & `yellowdog-python-examples-5.0.5/yd_commands/list.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/object_utilities.py` & `yellowdog-python-examples-5.0.5/yd_commands/object_utilities.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/printing.py` & `yellowdog-python-examples-5.0.5/yd_commands/printing.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/provision.py` & `yellowdog-python-examples-5.0.5/yd_commands/provision.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/provision_utils.py` & `yellowdog-python-examples-5.0.5/yd_commands/provision_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/reformat_json.py` & `yellowdog-python-examples-5.0.5/yd_commands/reformat_json.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/shutdown.py` & `yellowdog-python-examples-5.0.5/yd_commands/shutdown.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/submit.py` & `yellowdog-python-examples-5.0.5/yd_commands/submit.py`

 * *Files 0% similar despite different names*

```diff
@@ -472,15 +472,15 @@
                 "Tasks: ignoring 'taskCount'"
             )
 
     num_task_groups = len(wr_data[TASK_GROUPS])
 
     # Determine Task batching
     tasks = wr_data[TASK_GROUPS][tg_number][TASKS]
-    num_tasks = len(tasks)
+    num_tasks = len(tasks) if task_count is None else task_count
     num_task_batches: int = ceil(num_tasks / TASK_BATCH_SIZE)
     tasks_list: List[Task] = []
     if num_task_batches > 1 and not ARGS_PARSER.dry_run:
         print_log(
             f"Adding Tasks to Task Group '{task_group.name}' in "
             f"{num_task_batches} batches"
         )
@@ -497,15 +497,15 @@
     for batch_number in range(num_task_batches):
         # Iterate through tasks in the batch
         for task_number in range(
             (TASK_BATCH_SIZE * batch_number),
             min(TASK_BATCH_SIZE * (batch_number + 1), num_tasks),
         ):
             task_group_data = wr_data[TASK_GROUPS][tg_number]
-            task = tasks[task_number]
+            task = tasks[task_number] if task_count is None else tasks[0]
             task_name = format_yd_name(
                 get_task_name(
                     task.get(NAME, task.get(TASK_NAME, CONFIG_WR.task_name)),
                     task_number,
                     num_tasks,
                     tg_number,
                     num_task_groups,
```

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/submit_utils.py` & `yellowdog-python-examples-5.0.5/yd_commands/submit_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/terminate.py` & `yellowdog-python-examples-5.0.5/yd_commands/terminate.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/type_check.py` & `yellowdog-python-examples-5.0.5/yd_commands/type_check.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/upload.py` & `yellowdog-python-examples-5.0.5/yd_commands/upload.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/upload_utils.py` & `yellowdog-python-examples-5.0.5/yd_commands/upload_utils.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/validate_properties.py` & `yellowdog-python-examples-5.0.5/yd_commands/validate_properties.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/variables.py` & `yellowdog-python-examples-5.0.5/yd_commands/variables.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/version.py` & `yellowdog-python-examples-5.0.5/yd_commands/version.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yd_commands/wrapper.py` & `yellowdog-python-examples-5.0.5/yd_commands/wrapper.py`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/PKG-INFO` & `yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yellowdog-python-examples
-Version: 5.0.4
+Version: 5.0.5
 Summary: Example Python commands using the YellowDog Python SDK
 Home-page: https://github.com/yellowdog/python-examples
 Author: YellowDog Limited
 Author-email: YellowDog Limited <support@yellowdog.co>
 Project-URL: Homepage, https://github.com/yellowdog/python-examples
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/SOURCES.txt` & `yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `yellowdog-python-examples-5.0.4/yellowdog_python_examples.egg-info/entry_points.txt` & `yellowdog-python-examples-5.0.5/yellowdog_python_examples.egg-info/entry_points.txt`

 * *Files identical despite different names*

