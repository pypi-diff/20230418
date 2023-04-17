# Comparing `tmp/pycrosskit-1.6.9.tar.gz` & `tmp/pycrosskit-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycrosskit-1.6.9.tar", last modified: Tue Feb 21 00:57:41 2023, max compression
+gzip compressed data, was "pycrosskit-1.7.0.tar", last modified: Mon Apr 17 23:12:45 2023, max compression
```

## Comparing `pycrosskit-1.6.9.tar` & `pycrosskit-1.7.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:41.563966 pycrosskit-1.6.9/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-02-21 00:57:41.563966 pycrosskit-1.6.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:41.559965 pycrosskit-1.6.9/pycrosskit/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:41.563966 pycrosskit-1.6.9/pycrosskit/env_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/env_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/env_platforms/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/env_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/env_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/envariables.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:41.563966 pycrosskit-1.6.9/pycrosskit/shortcut_platforms/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/shortcut_platforms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/shortcut_platforms/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/shortcut_platforms/windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/pycrosskit/shortcuts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:41.559965 pycrosskit-1.6.9/pycrosskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      756 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 00:57:41.000000 pycrosskit-1.6.9/pycrosskit.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-21 00:57:41.563966 pycrosskit-1.6.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 00:57:41.563966 pycrosskit-1.6.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/tests/test_env_vars_linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/tests/test_env_vars_windows.py
--rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-02-21 00:57:30.000000 pycrosskit-1.6.9/tests/test_shortcut.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.389373 pycrosskit-1.7.0/pycrosskit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.393373 pycrosskit-1.7.0/pycrosskit/env_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3897 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/env_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/envariables.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.393373 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcut_platforms/windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/pycrosskit/shortcuts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.393373 pycrosskit-1.7.0/pycrosskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 23:12:45.000000 pycrosskit-1.7.0/pycrosskit.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 23:12:45.397373 pycrosskit-1.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/test_env_vars_linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/test_env_vars_windows.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1298 2023-04-17 23:12:31.000000 pycrosskit-1.7.0/tests/test_shortcut.py
```

### Comparing `pycrosskit-1.6.9/LICENSE.md` & `pycrosskit-1.7.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/PKG-INFO` & `pycrosskit-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.6.9
+Version: 1.7.0
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pycrosskit-1.6.9/README.md` & `pycrosskit-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/__init__.py` & `pycrosskit-1.7.0/pycrosskit/__init__.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/env_platforms/linux.py` & `pycrosskit-1.7.0/pycrosskit/env_platforms/linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/env_platforms/windows.py` & `pycrosskit-1.7.0/pycrosskit/env_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/envariables.py` & `pycrosskit-1.7.0/pycrosskit/envariables.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/shortcut_platforms/linux.py` & `pycrosskit-1.7.0/pycrosskit/shortcut_platforms/linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/shortcut_platforms/windows.py` & `pycrosskit-1.7.0/pycrosskit/shortcut_platforms/windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit/shortcuts.py` & `pycrosskit-1.7.0/pycrosskit/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/pycrosskit.egg-info/PKG-INFO` & `pycrosskit-1.7.0/pycrosskit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycrosskit
-Version: 1.6.9
+Version: 1.7.0
 Summary: Cross Platform Toolkit for Windows and Linux in order to make variables and shortcuts easy 
 Home-page: https://github.com/jiri-otoupal/py-cross-kit
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: Apache 2.0
 Keywords: Python Cross Platform Toolkit
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pycrosskit-1.6.9/pycrosskit.egg-info/SOURCES.txt` & `pycrosskit-1.7.0/pycrosskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/setup.py` & `pycrosskit-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     author_email=about["__author_email__"],
     url=about["__url__"],
     packages=find_packages(),
     include_package_data=True,
     python_requires=">=3.6,<4",
     install_requires=["pywin32>=300; sys_platform == 'win32'"],
     extras_require={
-        "dev": ["black>=22,<24", "flake8<6.1", "pre-commit<3.1", "pytest<7.3"],
+        "dev": ["black>=22,<24", "flake8<6.1", "pre-commit<3.3", "pytest<7.3"],
     },
     license=about["__license__"],
     zip_safe=True,
     entry_points={
         "console_scripts": ["pycrosskit=entry_points:main"],
     },
     classifiers=[
```

### Comparing `pycrosskit-1.6.9/tests/test_env_vars_linux.py` & `pycrosskit-1.7.0/tests/test_env_vars_linux.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/tests/test_env_vars_windows.py` & `pycrosskit-1.7.0/tests/test_env_vars_windows.py`

 * *Files identical despite different names*

### Comparing `pycrosskit-1.6.9/tests/test_shortcut.py` & `pycrosskit-1.7.0/tests/test_shortcut.py`

 * *Files identical despite different names*

