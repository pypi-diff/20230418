# Comparing `tmp/ota-0.0.7.tar.gz` & `tmp/ota-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ota-0.0.7.tar", last modified: Tue Apr 18 00:08:02 2023, max compression
+gzip compressed data, was "ota-0.0.8.tar", last modified: Tue Apr 18 00:10:49 2023, max compression
```

## Comparing `ota-0.0.7.tar` & `ota-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:08:02.393470 ota-0.0.7/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 00:08:02.393470 ota-0.0.7/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       86 2023-03-14 12:40:11.000000 ota-0.0.7/README.md
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:08:02.393470 ota-0.0.7/ota/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       19 2023-04-17 15:16:42.000000 ota-0.0.7/ota/__init__.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:08:02.393470 ota-0.0.7/ota/cli/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:51:29.000000 ota-0.0.7/ota/cli/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4262 2023-04-17 22:08:40.000000 ota-0.0.7/ota/cli/analyze.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      680 2023-04-17 20:34:39.000000 ota-0.0.7/ota/cli/config.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      882 2023-04-17 20:35:26.000000 ota-0.0.7/ota/cli/download.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3949 2023-04-17 22:14:07.000000 ota-0.0.7/ota/cli/inspect.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1151 2023-04-17 20:35:49.000000 ota-0.0.7/ota/cli/send.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:08:02.393470 ota-0.0.7/ota/core/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-02-20 19:45:43.000000 ota-0.0.7/ota/core/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     7774 2023-04-18 00:06:22.000000 ota-0.0.7/ota/core/analyze.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      530 2023-04-17 22:03:04.000000 ota-0.0.7/ota/core/console.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     2389 2023-04-17 22:03:41.000000 ota-0.0.7/ota/core/models.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     5437 2023-04-17 22:03:53.000000 ota-0.0.7/ota/core/rpc.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3135 2023-04-17 23:50:50.000000 ota-0.0.7/ota/core/settings.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)    10964 2023-04-17 23:21:49.000000 ota-0.0.7/ota/core/tools.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      545 2023-04-17 15:15:25.000000 ota-0.0.7/ota/main.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:08:02.393470 ota-0.0.7/ota/odoo/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1618 2023-04-17 22:00:54.000000 ota-0.0.7/ota/odoo/__init__.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     1309 2023-04-17 21:59:02.000000 ota-0.0.7/ota/odoo/field.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     4200 2023-04-17 21:59:31.000000 ota-0.0.7/ota/odoo/model.py
--rw-rw-r--   0 aroy      (1000) aroy      (1000)     3951 2023-04-17 22:00:24.000000 ota-0.0.7/ota/odoo/module.py
-drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:08:02.393470 ota-0.0.7/ota.egg-info/
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 00:08:02.000000 ota-0.0.7/ota.egg-info/PKG-INFO
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      533 2023-04-18 00:08:02.000000 ota-0.0.7/ota.egg-info/SOURCES.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-04-18 00:08:02.000000 ota-0.0.7/ota.egg-info/dependency_links.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       37 2023-04-18 00:08:02.000000 ota-0.0.7/ota.egg-info/entry_points.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      105 2023-04-18 00:08:02.000000 ota-0.0.7/ota.egg-info/requires.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)        4 2023-04-18 00:08:02.000000 ota-0.0.7/ota.egg-info/top_level.txt
--rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-04-18 00:08:02.393470 ota-0.0.7/setup.cfg
--rw-rw-r--   0 aroy      (1000) aroy      (1000)      736 2023-04-18 00:07:54.000000 ota-0.0.7/setup.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 00:10:49.407697 ota-0.0.8/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       86 2023-03-14 12:40:11.000000 ota-0.0.8/README.md
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       19 2023-04-17 15:16:42.000000 ota-0.0.8/ota/__init__.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/cli/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-04-17 23:51:29.000000 ota-0.0.8/ota/cli/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4262 2023-04-17 22:08:40.000000 ota-0.0.8/ota/cli/analyze.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      680 2023-04-17 20:34:39.000000 ota-0.0.8/ota/cli/config.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      882 2023-04-17 20:35:26.000000 ota-0.0.8/ota/cli/download.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3949 2023-04-17 22:14:07.000000 ota-0.0.8/ota/cli/inspect.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1151 2023-04-17 20:35:49.000000 ota-0.0.8/ota/cli/send.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/core/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        0 2023-02-20 19:45:43.000000 ota-0.0.8/ota/core/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     7774 2023-04-18 00:06:22.000000 ota-0.0.8/ota/core/analyze.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      530 2023-04-17 22:03:04.000000 ota-0.0.8/ota/core/console.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     2389 2023-04-17 22:03:41.000000 ota-0.0.8/ota/core/models.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     5437 2023-04-17 22:03:53.000000 ota-0.0.8/ota/core/rpc.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3135 2023-04-17 23:50:50.000000 ota-0.0.8/ota/core/settings.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)    10964 2023-04-17 23:21:49.000000 ota-0.0.8/ota/core/tools.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      545 2023-04-17 15:15:25.000000 ota-0.0.8/ota/main.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota/odoo/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1618 2023-04-17 22:00:54.000000 ota-0.0.8/ota/odoo/__init__.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     1309 2023-04-17 21:59:02.000000 ota-0.0.8/ota/odoo/field.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     4200 2023-04-17 21:59:31.000000 ota-0.0.8/ota/odoo/model.py
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)     3951 2023-04-17 22:00:24.000000 ota-0.0.8/ota/odoo/module.py
+drwxrwxr-x   0 aroy      (1000) aroy      (1000)        0 2023-04-18 00:10:49.407697 ota-0.0.8/ota.egg-info/
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      213 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/PKG-INFO
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      533 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/SOURCES.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        1 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/dependency_links.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       37 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/entry_points.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      113 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/requires.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)        4 2023-04-18 00:10:49.000000 ota-0.0.8/ota.egg-info/top_level.txt
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)       38 2023-04-18 00:10:49.407697 ota-0.0.8/setup.cfg
+-rw-rw-r--   0 aroy      (1000) aroy      (1000)      744 2023-04-18 00:10:42.000000 ota-0.0.8/setup.py
```

### Comparing `ota-0.0.7/ota/cli/analyze.py` & `ota-0.0.8/ota/cli/analyze.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/cli/config.py` & `ota-0.0.8/ota/cli/config.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/cli/download.py` & `ota-0.0.8/ota/cli/download.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/cli/inspect.py` & `ota-0.0.8/ota/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/cli/send.py` & `ota-0.0.8/ota/cli/send.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/core/analyze.py` & `ota-0.0.8/ota/core/analyze.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/core/console.py` & `ota-0.0.8/ota/core/console.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/core/models.py` & `ota-0.0.8/ota/core/models.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/core/rpc.py` & `ota-0.0.8/ota/core/rpc.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/core/settings.py` & `ota-0.0.8/ota/core/settings.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/core/tools.py` & `ota-0.0.8/ota/core/tools.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/main.py` & `ota-0.0.8/ota/main.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/odoo/__init__.py` & `ota-0.0.8/ota/odoo/__init__.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/odoo/field.py` & `ota-0.0.8/ota/odoo/field.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/odoo/model.py` & `ota-0.0.8/ota/odoo/model.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota/odoo/module.py` & `ota-0.0.8/ota/odoo/module.py`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/ota.egg-info/SOURCES.txt` & `ota-0.0.8/ota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ota-0.0.7/setup.py` & `ota-0.0.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="ota",
-    version="0.0.7",
+    version="0.0.8",
     description="Odoo Technical Analysis",
     url="https://github.com/royaurelien/ota-client",
     author="Aurelien ROY",
     author_email="roy.aurelien@gmail.com",
     license="BSD 2-clause",
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
+        "pylint-odoo",
         "click",
         "odoo-analyse>=1.3.0",
-        "pylint",
+        "pylint>=2.17.2",
         "requests",
         "sh>=2.0.0",
         "rich",
         "black",
-        "pylint-odoo",
         "pydantic",
         "pandas",
         "numpy",
         "appdirs",
     ],
     extras_require={},
     entry_points={
```

