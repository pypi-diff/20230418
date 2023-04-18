# Comparing `tmp/ota-0.0.8.tar.gz` & `tmp/ota-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ota-0.0.8.tar", last modified: Tue Apr 18 00:10:49 2023, max compression
+gzip compressed data, was "ota-0.0.9.tar", last modified: Tue Apr 18 08:10:08 2023, max compression
```

## Comparing `ota-0.0.8.tar` & `ota-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 00:10:49.407697 ota-0.0.8/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       86 2023-03-14 12:40:11.000000 ota-0.0.8/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       19 2023-04-17 15:16:42.000000 ota-0.0.8/ota/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:51:29.000000 ota-0.0.8/ota/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4262 2023-04-17 22:08:40.000000 ota-0.0.8/ota/cli/analyze.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      680 2023-04-17 20:34:39.000000 ota-0.0.8/ota/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      882 2023-04-17 20:35:26.000000 ota-0.0.8/ota/cli/download.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3949 2023-04-17 22:14:07.000000 ota-0.0.8/ota/cli/inspect.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1151 2023-04-17 20:35:49.000000 ota-0.0.8/ota/cli/send.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-02-20 19:45:43.000000 ota-0.0.8/ota/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     7774 2023-04-18 00:06:22.000000 ota-0.0.8/ota/core/analyze.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      530 2023-04-17 22:03:04.000000 ota-0.0.8/ota/core/console.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2389 2023-04-17 22:03:41.000000 ota-0.0.8/ota/core/models.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5437 2023-04-17 22:03:53.000000 ota-0.0.8/ota/core/rpc.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3135 2023-04-17 23:50:50.000000 ota-0.0.8/ota/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)    10964 2023-04-17 23:21:49.000000 ota-0.0.8/ota/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      545 2023-04-17 15:15:25.000000 ota-0.0.8/ota/main.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/odoo/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1618 2023-04-17 22:00:54.000000 ota-0.0.8/ota/odoo/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1309 2023-04-17 21:59:02.000000 ota-0.0.8/ota/odoo/field.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4200 2023-04-17 21:59:31.000000 ota-0.0.8/ota/odoo/model.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3951 2023-04-17 22:00:24.000000 ota-0.0.8/ota/odoo/module.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      533 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       37 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      113 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        4 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-04-18 00:10:49.407697 ota-0.0.8/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      744 2023-04-18 00:10:42.000000 ota-0.0.8/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 08:10:08.374230 ota-0.0.9/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 08:10:08.374230 ota-0.0.9/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       86 2023-03-14 12:40:11.000000 ota-0.0.9/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 08:10:08.370230 ota-0.0.9/ota/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       19 2023-04-17 15:16:42.000000 ota-0.0.9/ota/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 08:10:08.370230 ota-0.0.9/ota/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:51:29.000000 ota-0.0.9/ota/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4262 2023-04-17 22:08:40.000000 ota-0.0.9/ota/cli/analyze.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      792 2023-04-18 00:18:57.000000 ota-0.0.9/ota/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      882 2023-04-17 20:35:26.000000 ota-0.0.9/ota/cli/download.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3949 2023-04-17 22:14:07.000000 ota-0.0.9/ota/cli/inspect.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1151 2023-04-17 20:35:49.000000 ota-0.0.9/ota/cli/send.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 08:10:08.374230 ota-0.0.9/ota/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-02-20 19:45:43.000000 ota-0.0.9/ota/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     7774 2023-04-18 00:06:22.000000 ota-0.0.9/ota/core/analyze.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      530 2023-04-17 22:03:04.000000 ota-0.0.9/ota/core/console.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2389 2023-04-17 22:03:41.000000 ota-0.0.9/ota/core/models.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5437 2023-04-17 22:03:53.000000 ota-0.0.9/ota/core/rpc.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3292 2023-04-18 00:24:36.000000 ota-0.0.9/ota/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)    11039 2023-04-18 00:24:12.000000 ota-0.0.9/ota/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      545 2023-04-17 15:15:25.000000 ota-0.0.9/ota/main.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 08:10:08.374230 ota-0.0.9/ota/odoo/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1618 2023-04-17 22:00:54.000000 ota-0.0.9/ota/odoo/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1309 2023-04-17 21:59:02.000000 ota-0.0.9/ota/odoo/field.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4200 2023-04-17 21:59:31.000000 ota-0.0.9/ota/odoo/model.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3951 2023-04-17 22:00:24.000000 ota-0.0.9/ota/odoo/module.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 08:10:08.370230 ota-0.0.9/ota.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 08:10:08.000000 ota-0.0.9/ota.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      533 2023-04-18 08:10:08.000000 ota-0.0.9/ota.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-04-18 08:10:08.000000 ota-0.0.9/ota.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       37 2023-04-18 08:10:08.000000 ota-0.0.9/ota.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      121 2023-04-18 08:10:08.000000 ota-0.0.9/ota.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        4 2023-04-18 08:10:08.000000 ota-0.0.9/ota.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-04-18 08:10:08.374230 ota-0.0.9/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      752 2023-04-18 08:10:02.000000 ota-0.0.9/setup.py
```

### Comparing `ota-0.0.8/ota/cli/analyze.py` & `ota-0.0.9/ota/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/cli/config.py` & `ota-0.0.9/ota/cli/config.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,15 +26,22 @@
 
 @click.command()
 def view():
     """View configuration"""
     console.print(settings)
 
 
+@click.command()
+def clear():
+    """Clear configuration"""
+    settings.save(True)
+
+
 @click.group()
 def config():
     """Manage configuration"""
 
 
 config.add_command(set_value)
 config.add_command(get_value)
 config.add_command(view)
+config.add_command(clear)
```

### Comparing `ota-0.0.8/ota/cli/download.py` & `ota-0.0.9/ota/cli/download.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/cli/inspect.py` & `ota-0.0.9/ota/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/cli/send.py` & `ota-0.0.9/ota/cli/send.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/core/analyze.py` & `ota-0.0.9/ota/core/analyze.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/core/console.py` & `ota-0.0.9/ota/core/console.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/core/models.py` & `ota-0.0.9/ota/core/models.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/core/rpc.py` & `ota-0.0.9/ota/core/rpc.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/core/settings.py` & `ota-0.0.9/ota/core/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 import os
 
 from appdirs import AppDirs
 from pydantic import BaseSettings
 from pydantic.error_wrappers import ValidationError
 
 from ota.core.console import console
-from ota.core.tools import save_to
+from ota.core.tools import save_to, ROOT_DIR
 
 CONFIG_FILENAME = "config.json"
 DIRS = AppDirs("ota", "Aurelien ROY")
 
 
 def init_dirs():
     os.makedirs(DIRS.user_data_dir, exist_ok=True)
+    console.log(ROOT_DIR)
 
 
 def get_config_path():
     return DIRS.user_data_dir
 
 
 def get_config_filepath():
@@ -96,19 +97,23 @@
                     if key in data:
                         data.pop(key)
                 self = cls.parse_raw(data)
 
         self.save()
         return self
 
-    def save(self):
+    def save(self, clear=False):
         """Save settings to JSON file"""
         data = self.json()
+        filepath = get_config_filepath()
+
+        if clear and os.path.exists(filepath):
+            os.remove(filepath)
 
-        save_to(data, get_config_filepath())
+        save_to(data, filepath)
 
     def set_value(self, name, value, auto_save=True):
         """Set value"""
         self.__dict__[name] = value
 
         if auto_save:
             self.save()
```

### Comparing `ota-0.0.8/ota/core/tools.py` & `ota-0.0.9/ota/core/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 # requests.packages.urllib3.disable_warnings()
 
 from ota.core.console import console, Table
 from ota.core.models import File, LinterResult
 
 _logger = logging.getLogger(__name__)
 
+ROOT_DIR = os.path.realpath(os.path.join(os.path.dirname(__file__), ".."))
 TEMPLATE_DIR = False
 
 
 def dict_to_list(data, keys=None):
     def function(item):
         return f'{item}="{data[item]}"'
```

### Comparing `ota-0.0.8/ota/main.py` & `ota-0.0.9/ota/main.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/odoo/__init__.py` & `ota-0.0.9/ota/odoo/__init__.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/odoo/field.py` & `ota-0.0.9/ota/odoo/field.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/odoo/model.py` & `ota-0.0.9/ota/odoo/model.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota/odoo/module.py` & `ota-0.0.9/ota/odoo/module.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/ota.egg-info/SOURCES.txt` & `ota-0.0.9/ota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ota-0.0.8/setup.py` & `ota-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ota",
-    version="0.0.8",
+    version="0.0.9",
     description="Odoo Technical Analysis",
     url="https://github.com/royaurelien/ota-client",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="BSD 2-clause",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
-        "pylint-odoo",
         "click",
+        "pylint>=2.15.0",
+        "pylint-odoo>=8.0.19",
         "odoo-analyse>=1.3.0",
-        "pylint>=2.17.2",
         "requests",
         "sh>=2.0.0",
         "rich",
         "black",
         "pydantic",
         "pandas",
         "numpy",
```

