# Comparing `tmp/ota-0.0.3.tar.gz` & `tmp/ota-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ota-0.0.3.tar", last modified: Mon Apr 17 23:45:53 2023, max compression
+gzip compressed data, was "ota-0.0.5.tar", last modified: Mon Apr 17 23:53:03 2023, max compression
```

## Comparing `ota-0.0.3.tar` & `ota-0.0.5.tar`

### file list

```diff
@@ -1,28 +1,35 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:45:53.280135 ota-0.0.3/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-17 23:45:53.280135 ota-0.0.3/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       86 2023-03-14 12:40:11.000000 ota-0.0.3/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:45:53.280135 ota-0.0.3/ota/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       19 2023-04-17 15:16:42.000000 ota-0.0.3/ota/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:45:53.280135 ota-0.0.3/ota/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-02-20 19:45:43.000000 ota-0.0.3/ota/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     7748 2023-04-17 22:02:54.000000 ota-0.0.3/ota/core/analyze.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      530 2023-04-17 22:03:04.000000 ota-0.0.3/ota/core/console.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2389 2023-04-17 22:03:41.000000 ota-0.0.3/ota/core/models.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5437 2023-04-17 22:03:53.000000 ota-0.0.3/ota/core/rpc.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3152 2023-04-17 23:44:35.000000 ota-0.0.3/ota/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)    10964 2023-04-17 23:21:49.000000 ota-0.0.3/ota/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      545 2023-04-17 15:15:25.000000 ota-0.0.3/ota/main.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:45:53.280135 ota-0.0.3/ota/odoo/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1618 2023-04-17 22:00:54.000000 ota-0.0.3/ota/odoo/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1309 2023-04-17 21:59:02.000000 ota-0.0.3/ota/odoo/field.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4200 2023-04-17 21:59:31.000000 ota-0.0.3/ota/odoo/model.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3951 2023-04-17 22:00:24.000000 ota-0.0.3/ota/odoo/module.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:45:53.280135 ota-0.0.3/ota.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-17 23:45:53.000000 ota-0.0.3/ota.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      421 2023-04-17 23:45:53.000000 ota-0.0.3/ota.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-04-17 23:45:53.000000 ota-0.0.3/ota.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       37 2023-04-17 23:45:53.000000 ota-0.0.3/ota.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       91 2023-04-17 23:45:53.000000 ota-0.0.3/ota.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        4 2023-04-17 23:45:53.000000 ota-0.0.3/ota.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-04-17 23:45:53.280135 ota-0.0.3/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      722 2023-04-17 23:29:51.000000 ota-0.0.3/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:53:03.513438 ota-0.0.5/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-17 23:53:03.513438 ota-0.0.5/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       86 2023-03-14 12:40:11.000000 ota-0.0.5/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:53:03.513438 ota-0.0.5/ota/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       19 2023-04-17 15:16:42.000000 ota-0.0.5/ota/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:53:03.513438 ota-0.0.5/ota/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:51:29.000000 ota-0.0.5/ota/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4262 2023-04-17 22:08:40.000000 ota-0.0.5/ota/cli/analyze.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      680 2023-04-17 20:34:39.000000 ota-0.0.5/ota/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      882 2023-04-17 20:35:26.000000 ota-0.0.5/ota/cli/download.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3949 2023-04-17 22:14:07.000000 ota-0.0.5/ota/cli/inspect.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1151 2023-04-17 20:35:49.000000 ota-0.0.5/ota/cli/send.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:53:03.513438 ota-0.0.5/ota/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-02-20 19:45:43.000000 ota-0.0.5/ota/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     7748 2023-04-17 22:02:54.000000 ota-0.0.5/ota/core/analyze.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      530 2023-04-17 22:03:04.000000 ota-0.0.5/ota/core/console.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2389 2023-04-17 22:03:41.000000 ota-0.0.5/ota/core/models.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5437 2023-04-17 22:03:53.000000 ota-0.0.5/ota/core/rpc.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3135 2023-04-17 23:50:50.000000 ota-0.0.5/ota/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)    10964 2023-04-17 23:21:49.000000 ota-0.0.5/ota/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      545 2023-04-17 15:15:25.000000 ota-0.0.5/ota/main.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:53:03.513438 ota-0.0.5/ota/odoo/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1618 2023-04-17 22:00:54.000000 ota-0.0.5/ota/odoo/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1309 2023-04-17 21:59:02.000000 ota-0.0.5/ota/odoo/field.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4200 2023-04-17 21:59:31.000000 ota-0.0.5/ota/odoo/model.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3951 2023-04-17 22:00:24.000000 ota-0.0.5/ota/odoo/module.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:53:03.513438 ota-0.0.5/ota.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-17 23:53:03.000000 ota-0.0.5/ota.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      533 2023-04-17 23:53:03.000000 ota-0.0.5/ota.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-04-17 23:53:03.000000 ota-0.0.5/ota.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       37 2023-04-17 23:53:03.000000 ota-0.0.5/ota.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       91 2023-04-17 23:53:03.000000 ota-0.0.5/ota.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        4 2023-04-17 23:53:03.000000 ota-0.0.5/ota.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-04-17 23:53:03.513438 ota-0.0.5/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      722 2023-04-17 23:52:46.000000 ota-0.0.5/setup.py
```

### Comparing `ota-0.0.3/ota/core/analyze.py` & `ota-0.0.5/ota/core/analyze.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/core/console.py` & `ota-0.0.5/ota/core/console.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/core/models.py` & `ota-0.0.5/ota/core/models.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/core/rpc.py` & `ota-0.0.5/ota/core/rpc.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/core/settings.py` & `ota-0.0.5/ota/core/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 from appdirs import AppDirs
 from pydantic import BaseSettings
 from pydantic.error_wrappers import ValidationError
 
 from ota.core.console import console
-from ota.core.tools import get_config_file, save_to
+from ota.core.tools import save_to
 
 CONFIG_FILENAME = "config.json"
 DIRS = AppDirs("ota", "Aurelien ROY")
 
 
 def init_dirs():
     os.makedirs(DIRS.user_data_dir, exist_ok=True)
```

### Comparing `ota-0.0.3/ota/core/tools.py` & `ota-0.0.5/ota/core/tools.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/main.py` & `ota-0.0.5/ota/main.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/odoo/__init__.py` & `ota-0.0.5/ota/odoo/__init__.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/odoo/field.py` & `ota-0.0.5/ota/odoo/field.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/odoo/model.py` & `ota-0.0.5/ota/odoo/model.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/ota/odoo/module.py` & `ota-0.0.5/ota/odoo/module.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.3/setup.py` & `ota-0.0.5/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ota",
-    version="0.0.3",
+    version="0.0.5",
     description="Odoo Technical Analysis",
     url="https://github.com/royaurelien/ota-client",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="BSD 2-clause",
     packages=find_packages(),
     include_package_data=True,
```

