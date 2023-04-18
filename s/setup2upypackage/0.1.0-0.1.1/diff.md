# Comparing `tmp/setup2upypackage-0.1.0.tar.gz` & `tmp/setup2upypackage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "setup2upypackage-0.1.0.tar", last modified: Tue Mar 28 07:33:14 2023, max compression
+gzip compressed data, was "setup2upypackage-0.1.1.tar", last modified: Tue Apr 18 20:32:35 2023, max compression
```

## Comparing `setup2upypackage-0.1.0.tar` & `setup2upypackage-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/src/setup2upypackage/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/src/setup2upypackage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/src/setup2upypackage/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/src/setup2upypackage/setup2upypackage.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-03-28 07:33:07.000000 setup2upypackage-0.1.0/src/setup2upypackage/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-03-28 07:33:14.000000 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-03-28 07:33:14.000000 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 07:33:14.000000 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-03-28 07:33:14.000000 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-03-28 07:33:14.000000 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-28 07:33:14.000000 setup2upypackage-0.1.0/src/setup2upypackage.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 07:33:14.594459 setup2upypackage-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/tests/test_absolute_truth.py
--rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-03-28 07:32:54.000000 setup2upypackage-0.1.0/tests/test_setup2upypackage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5295 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 20:32:35.758973 setup2upypackage-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.750972 setup2upypackage-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/src/setup2upypackage/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/src/setup2upypackage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6123 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/src/setup2upypackage/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/src/setup2upypackage/setup2upypackage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-18 20:32:29.000000 setup2upypackage-0.1.1/src/setup2upypackage/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6445 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 20:32:35.000000 setup2upypackage-0.1.1/src/setup2upypackage.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 20:32:35.754973 setup2upypackage-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/tests/test_absolute_truth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13035 2023-04-18 20:32:19.000000 setup2upypackage-0.1.1/tests/test_setup2upypackage.py
```

### Comparing `setup2upypackage-0.1.0/LICENSE.txt` & `setup2upypackage-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.0/PKG-INFO` & `setup2upypackage-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
```

### Comparing `setup2upypackage-0.1.0/README.md` & `setup2upypackage-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.0/setup.py` & `setup2upypackage-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.0/src/setup2upypackage/main.py` & `setup2upypackage-0.1.1/src/setup2upypackage/main.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.0/src/setup2upypackage/setup2upypackage.py` & `setup2upypackage-0.1.1/src/setup2upypackage/setup2upypackage.py`

 * *Files 2% similar despite different names*

```diff
@@ -309,15 +309,22 @@
     def validate(self) -> bool:
         """
         Validate existing package.json with setup.py based data
 
         :returns:   Result of validation, True on success, False otherwise
         :rtype:     bool
         """
-        return self.package_json_data == self.package_data
+        # list of URL entries might be sorted differently
+        package_json_data = dict(self.package_json_data)
+        package_data = dict(self.package_data)
+
+        package_json_data.get("urls", []).sort()
+        package_data.get("urls", []).sort()
+
+        return package_json_data == package_data
 
     @property
     def validation_diff(self) -> DeepDiff:
         """
         Get difference of package.json and setup.py
 
         :returns:   The deep difference.
```

### Comparing `setup2upypackage-0.1.0/src/setup2upypackage.egg-info/PKG-INFO` & `setup2upypackage-0.1.1/src/setup2upypackage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: setup2upypackage
-Version: 0.1.0
+Version: 0.1.1
 Summary: Validate and create MicroPython package JSON file
 Home-page: https://github.com/brainelectronics/micropython-package-validation
 Author: brainelectronics
 Author-email: info@brainelectronics.de
 Project-URL: Bug Reports, https://github.com/brainelectronics/micropython-package-validation/issues
 Project-URL: Source, https://github.com/brainelectronics/micropython-package-validation/
 Keywords: micropython,package,mip-helper,validation
```

### Comparing `setup2upypackage-0.1.0/src/setup2upypackage.egg-info/SOURCES.txt` & `setup2upypackage-0.1.1/src/setup2upypackage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.0/tests/test_absolute_truth.py` & `setup2upypackage-0.1.1/tests/test_absolute_truth.py`

 * *Files identical despite different names*

### Comparing `setup2upypackage-0.1.0/tests/test_setup2upypackage.py` & `setup2upypackage-0.1.1/tests/test_setup2upypackage.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # -*- coding: UTF-8 -*-
 """Unittest for testing the setup2upypackage file"""
 
 import json
 import logging
 import unittest
 from pathlib import Path
+from random import shuffle
 from sys import stdout
 from unittest.mock import PropertyMock, mock_open, patch
 
 from nose2.tools import params
 
 from setup2upypackage.setup2upypackage import (Setup2uPyPackage,
                                                Setup2uPyPackageError)
@@ -302,14 +303,29 @@
         )
         is_valid = s2pp.validate()
         if is_valid:
             self.assertTrue(is_valid)
         else:
             self.test_logger.warning(s2pp.validation_diff)
 
+        # check for differently sorted URL list entries
+        shuffeled_package_json_data = dict(s2pp.package_json_data)
+        shuffle(shuffeled_package_json_data["urls"])
+        self.assertNotEqual(
+            shuffeled_package_json_data["urls"],
+            s2pp.package_json_data
+        )
+        with patch('setup2upypackage.setup2upypackage.Setup2uPyPackage.package_json_data', new_callable=PropertyMock) as patched:     # noqa: E501
+            patched.return_value = shuffeled_package_json_data
+            is_valid = s2pp.validate()
+            if is_valid:
+                self.assertTrue(is_valid)
+            else:
+                self.test_logger.warning(s2pp.validation_diff)
+
     @unittest.skip("Not yet implemented")
     def test_validation_diff(self) -> None:
         """Test validation difference property"""
         pass
 
     @params(
         ("asdf.json", False),   # path, pretty
```

