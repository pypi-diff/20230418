# Comparing `tmp/python-matter-server-3.3.0.tar.gz` & `tmp/python-matter-server-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-matter-server-3.3.0.tar", last modified: Mon Apr 17 15:06:08 2023, max compression
+gzip compressed data, was "python-matter-server-3.3.1.tar", last modified: Tue Apr 18 09:07:44 2023, max compression
```

## Comparing `python-matter-server-3.3.0.tar` & `python-matter-server-3.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.416754 python-matter-server-3.3.0/matter_server/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/client/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/client/models/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/models/device_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/client/models/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/common/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/common/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/helpers/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/helpers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/helpers/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/common/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/server/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/client_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/const.py
--rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/device_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/matter_server/server/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/helpers/paa_certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/stack.py
--rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/matter_server/server/vendor_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-17 15:05:54.000000 python-matter-server-3.3.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/python_matter_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-17 15:06:07.000000 python-matter-server-3.3.0/python_matter_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:06:07.000000 python-matter-server-3.3.0/python_matter_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 15:06:06.000000 python-matter-server-3.3.0/python_matter_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-17 15:06:08.000000 python-matter-server-3.3.0/python_matter_server.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-17 15:06:08.420754 python-matter-server-3.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8030 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.153157 python-matter-server-3.3.1/matter_server/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.153157 python-matter-server-3.3.1/matter_server/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16257 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5885 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.153157 python-matter-server-3.3.1/matter_server/client/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14057 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/models/device_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13394 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/client/models/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/common/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/common/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/helpers/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/helpers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10250 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/helpers/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/common/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/client_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24473 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/device_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/matter_server/server/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/helpers/paa_certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7470 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2547 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5292 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/matter_server/server/vendor_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-04-18 09:07:26.000000 python-matter-server-3.3.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/python_matter_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 09:07:44.000000 python-matter-server-3.3.1/python_matter_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:07:41.000000 python-matter-server-3.3.1/python_matter_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 09:07:43.000000 python-matter-server-3.3.1/python_matter_server.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-18 09:07:44.157157 python-matter-server-3.3.1/setup.cfg
```

### Comparing `python-matter-server-3.3.0/LICENSE` & `python-matter-server-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/PKG-INFO` & `python-matter-server-3.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.3.0
+Version: 3.3.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.3.0/README.md` & `python-matter-server-3.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/client/client.py` & `python-matter-server-3.3.1/matter_server/client/client.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/client/connection.py` & `python-matter-server-3.3.1/matter_server/client/connection.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/client/exceptions.py` & `python-matter-server-3.3.1/matter_server/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/client/models/device_types.py` & `python-matter-server-3.3.1/matter_server/client/models/device_types.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/client/models/node.py` & `python-matter-server-3.3.1/matter_server/client/models/node.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/common/errors.py` & `python-matter-server-3.3.1/matter_server/common/errors.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/common/helpers/api.py` & `python-matter-server-3.3.1/matter_server/common/helpers/api.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/common/helpers/json.py` & `python-matter-server-3.3.1/matter_server/common/helpers/json.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/common/helpers/util.py` & `python-matter-server-3.3.1/matter_server/common/helpers/util.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/common/models.py` & `python-matter-server-3.3.1/matter_server/common/models.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/__main__.py` & `python-matter-server-3.3.1/matter_server/server/__main__.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/client_handler.py` & `python-matter-server-3.3.1/matter_server/server/client_handler.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/const.py` & `python-matter-server-3.3.1/matter_server/server/const.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/device_controller.py` & `python-matter-server-3.3.1/matter_server/server/device_controller.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/helpers/paa_certificates.py` & `python-matter-server-3.3.1/matter_server/server/helpers/paa_certificates.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/server.py` & `python-matter-server-3.3.1/matter_server/server/server.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/stack.py` & `python-matter-server-3.3.1/matter_server/server/stack.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/storage.py` & `python-matter-server-3.3.1/matter_server/server/storage.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/matter_server/server/vendor_info.py` & `python-matter-server-3.3.1/matter_server/server/vendor_info.py`

 * *Files identical despite different names*

### Comparing `python-matter-server-3.3.0/pyproject.toml` & `python-matter-server-3.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools~=62.3", "wheel~=0.37.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "python-matter-server"
-version = "3.3.0"
+version = "3.3.1"
 license     = {text = "Apache-2.0"}
 description = "Python Matter WebSocket Server"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
     {name = "The Home Assistant Authors", email = "hello@home-assistant.io"}
 ]
@@ -22,20 +22,20 @@
 ]
 dependencies = [
   "aiohttp",
   "aiorun",
   "coloredlogs",
   "dacite",
   "orjson",
-  "home-assistant-chip-clusters==2023.4.0"
+  "home-assistant-chip-clusters==2023.4.1"
 ]
 
 [project.optional-dependencies]
 server = [
-  "home-assistant-chip-core==2023.4.0",
+  "home-assistant-chip-core==2023.4.1",
   "cryptography==40.0.2"
 ]
 test = [
   "black==23.3.0",
   "flake8==6.0.0",
   "flake8-docstrings==1.7.0",
   "isort==5.12.0",
```

### Comparing `python-matter-server-3.3.0/python_matter_server.egg-info/PKG-INFO` & `python-matter-server-3.3.1/python_matter_server.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-matter-server
-Version: 3.3.0
+Version: 3.3.1
 Summary: Python Matter WebSocket Server
 Author-email: The Home Assistant Authors <hello@home-assistant.io>
 License: Apache-2.0
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
```

### Comparing `python-matter-server-3.3.0/python_matter_server.egg-info/SOURCES.txt` & `python-matter-server-3.3.1/python_matter_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

