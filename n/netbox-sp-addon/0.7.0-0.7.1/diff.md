# Comparing `tmp/netbox_sp_addon-0.7.0.tar.gz` & `tmp/netbox_sp_addon-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_sp_addon-0.7.0.tar", max compression
+gzip compressed data, was "netbox_sp_addon-0.7.1.tar", max compression
```

## Comparing `netbox_sp_addon-0.7.0.tar` & `netbox_sp_addon-0.7.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    10174 2020-08-19 12:46:44.245428 netbox_sp_addon-0.7.0/LICENSE.txt
--rw-r--r--   0        0        0       18 2023-04-18 06:36:09.409522 netbox_sp_addon-0.7.0/README.md
--rw-r--r--   0        0        0      855 2023-04-18 06:42:58.141525 netbox_sp_addon-0.7.0/netbox_sp_addon/__init__.py
--rw-r--r--   0        0        0       33 2020-08-19 06:52:21.758355 netbox_sp_addon-0.7.0/netbox_sp_addon/admin.py
--rw-r--r--   0        0        0        0 2020-08-19 06:50:54.486440 netbox_sp_addon-0.7.0/netbox_sp_addon/api/serializers.py
--rw-r--r--   0        0        0       96 2020-08-19 06:50:48.874445 netbox_sp_addon-0.7.0/netbox_sp_addon/api/urls.py
--rw-r--r--   0        0        0        0 2020-08-19 06:50:37.790456 netbox_sp_addon-0.7.0/netbox_sp_addon/api/views.py
--rw-r--r--   0        0        0      314 2022-07-15 06:25:44.678883 netbox_sp_addon-0.7.0/netbox_sp_addon/filters.py
--rw-r--r--   0        0        0     1072 2023-04-18 06:41:16.389118 netbox_sp_addon-0.7.0/netbox_sp_addon/forms.py
--rw-r--r--   0        0        0        0 2020-08-19 06:45:45.614774 netbox_sp_addon-0.7.0/netbox_sp_addon/migrations/__init__.py
--rw-r--r--   0        0        0       29 2020-08-19 06:52:25.914351 netbox_sp_addon-0.7.0/netbox_sp_addon/models.py
--rw-r--r--   0        0        0      340 2020-08-19 11:55:42.757704 netbox_sp_addon-0.7.0/netbox_sp_addon/navigation.py
--rw-r--r--   0        0        0      203 2020-08-19 11:56:02.973697 netbox_sp_addon-0.7.0/netbox_sp_addon/template_content.py
--rw-r--r--   0        0        0      292 2020-08-19 11:56:02.981697 netbox_sp_addon-0.7.0/netbox_sp_addon/urls.py
--rw-r--r--   0        0        0      326 2020-08-19 11:56:02.977697 netbox_sp_addon-0.7.0/netbox_sp_addon/views.py
--rw-r--r--   0        0        0      732 2023-04-18 06:35:01.440290 netbox_sp_addon-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 netbox_sp_addon-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    10174 2020-08-19 12:46:44.245428 netbox_sp_addon-0.7.1/LICENSE.txt
+-rw-r--r--   0        0        0       18 2023-04-18 06:36:09.409522 netbox_sp_addon-0.7.1/README.md
+-rw-r--r--   0        0        0      859 2023-04-18 06:53:10.347558 netbox_sp_addon-0.7.1/netbox_sp_addon/__init__.py
+-rw-r--r--   0        0        0       33 2020-08-19 06:52:21.758355 netbox_sp_addon-0.7.1/netbox_sp_addon/admin.py
+-rw-r--r--   0        0        0        0 2020-08-19 06:50:54.486440 netbox_sp_addon-0.7.1/netbox_sp_addon/api/serializers.py
+-rw-r--r--   0        0        0       96 2020-08-19 06:50:48.874445 netbox_sp_addon-0.7.1/netbox_sp_addon/api/urls.py
+-rw-r--r--   0        0        0        0 2020-08-19 06:50:37.790456 netbox_sp_addon-0.7.1/netbox_sp_addon/api/views.py
+-rw-r--r--   0        0        0      314 2022-07-15 06:25:44.678883 netbox_sp_addon-0.7.1/netbox_sp_addon/filters.py
+-rw-r--r--   0        0        0     1072 2023-04-18 06:41:16.389118 netbox_sp_addon-0.7.1/netbox_sp_addon/forms.py
+-rw-r--r--   0        0        0        0 2020-08-19 06:45:45.614774 netbox_sp_addon-0.7.1/netbox_sp_addon/migrations/__init__.py
+-rw-r--r--   0        0        0       29 2020-08-19 06:52:25.914351 netbox_sp_addon-0.7.1/netbox_sp_addon/models.py
+-rw-r--r--   0        0        0      340 2020-08-19 11:55:42.757704 netbox_sp_addon-0.7.1/netbox_sp_addon/navigation.py
+-rw-r--r--   0        0        0      203 2020-08-19 11:56:02.973697 netbox_sp_addon-0.7.1/netbox_sp_addon/template_content.py
+-rw-r--r--   0        0        0      292 2020-08-19 11:56:02.981697 netbox_sp_addon-0.7.1/netbox_sp_addon/urls.py
+-rw-r--r--   0        0        0      326 2020-08-19 11:56:02.977697 netbox_sp_addon-0.7.1/netbox_sp_addon/views.py
+-rw-r--r--   0        0        0      732 2023-04-18 06:53:04.915326 netbox_sp_addon-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 netbox_sp_addon-0.7.1/PKG-INFO
```

### Comparing `netbox_sp_addon-0.7.0/LICENSE.txt` & `netbox_sp_addon-0.7.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netbox_sp_addon-0.7.0/netbox_sp_addon/__init__.py` & `netbox_sp_addon-0.7.1/netbox_sp_addon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     name = "netbox_sp_addon"
 
     # Human-friendly name and description
     verbose_name = "qbeyond Addon"
     description = "Add functions used by qbeyond AG"
 
     # Plugin version
-    version = "0.7.0"
+    version = "0.7.1"
 
     # Plugin author
     author = "Tobias Genannt"
     author_email = "tobias.genannt@qbeyond.de"
 
     # Configuration parameters that MUST be defined by the user (if any)
     required_settings = []
@@ -26,11 +26,11 @@
     # Default configuration parameter values, if not set by the user
     default_settings = {}
 
     # Base URL path. If not set, the plugin name will be used.
     base_url = "sp-addon"
 
     # Minimun Netbox version
-    min_version = "3.5.0"
+    min_version = "3.5.0-dev"
 
 
 config = SPAddonConfig
```

### Comparing `netbox_sp_addon-0.7.0/netbox_sp_addon/forms.py` & `netbox_sp_addon-0.7.1/netbox_sp_addon/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_sp_addon-0.7.0/pyproject.toml` & `netbox_sp_addon-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
   "Topic :: System :: Systems Administration"
 ]
 description = "Adds some functions used by scanplus GmbH"
 license = "Apache-2.0"
 name = "netbox-sp-addon"
 readme = "README.md"
 repository = "https://github.com/scanplus/netbox-sp-addon"
-version = "0.7.0"
+version = "0.7.1"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
```

### Comparing `netbox_sp_addon-0.7.0/PKG-INFO` & `netbox_sp_addon-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-sp-addon
-Version: 0.7.0
+Version: 0.7.1
 Summary: Adds some functions used by scanplus GmbH
 Home-page: https://github.com/scanplus/netbox-sp-addon
 License: Apache-2.0
 Author: Tobias Genannt
 Author-email: tobias.genannt@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Environment :: Plugins
```

