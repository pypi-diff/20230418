# Comparing `tmp/easycheck_doiteasy-0.0.2.tar.gz` & `tmp/easycheck_doiteasy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycheck_doiteasy-0.0.2.tar", last modified: Tue Apr 18 14:06:14 2023, max compression
+gzip compressed data, was "easycheck_doiteasy-0.0.3.tar", last modified: Tue Apr 18 15:31:36 2023, max compression
```

## Comparing `easycheck_doiteasy-0.0.2.tar` & `easycheck_doiteasy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.2/LICENSE.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.2/README.md
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/easycheck_doiteasy/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       40 2023-04-12 17:08:43.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy/__init__.py
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2999 2023-04-18 13:45:18.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy/easycheck_doiteasy.py
-drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/PKG-INFO
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/SOURCES.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/dependency_links.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-18 14:06:14.000000 easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/top_level.txt
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.2/pyproject.toml
--rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-18 14:06:14.518424 easycheck_doiteasy-0.0.2/setup.cfg
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:31:36.571897 easycheck_doiteasy-0.0.3/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1061 2023-04-11 19:56:22.000000 easycheck_doiteasy-0.0.3/LICENSE.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-18 15:31:36.571897 easycheck_doiteasy-0.0.3/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     1292 2023-04-11 17:30:51.000000 easycheck_doiteasy-0.0.3/README.md
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:31:36.571897 easycheck_doiteasy-0.0.3/easycheck_doiteasy/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:17:56.000000 easycheck_doiteasy-0.0.3/easycheck_doiteasy/__init__.py
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     3293 2023-04-18 15:21:44.000000 easycheck_doiteasy-0.0.3/easycheck_doiteasy/easycheck_doiteasy.py
+drwxrwxr-x   0 jrojas    (1000) jrojas    (1000)        0 2023-04-18 15:31:36.571897 easycheck_doiteasy-0.0.3/easycheck_doiteasy.egg-info/
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)     2897 2023-04-18 15:31:36.000000 easycheck_doiteasy-0.0.3/easycheck_doiteasy.egg-info/PKG-INFO
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      286 2023-04-18 15:31:36.000000 easycheck_doiteasy-0.0.3/easycheck_doiteasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)        1 2023-04-18 15:31:36.000000 easycheck_doiteasy-0.0.3/easycheck_doiteasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       19 2023-04-18 15:31:36.000000 easycheck_doiteasy-0.0.3/easycheck_doiteasy.egg-info/top_level.txt
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)       84 2023-04-12 16:58:48.000000 easycheck_doiteasy-0.0.3/pyproject.toml
+-rw-rw-r--   0 jrojas    (1000) jrojas    (1000)      670 2023-04-18 15:31:36.571897 easycheck_doiteasy-0.0.3/setup.cfg
```

### Comparing `easycheck_doiteasy-0.0.2/LICENSE.txt` & `easycheck_doiteasy-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.2/PKG-INFO` & `easycheck_doiteasy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck_doiteasy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.2/README.md` & `easycheck_doiteasy-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `easycheck_doiteasy-0.0.2/easycheck_doiteasy/easycheck_doiteasy.py` & `easycheck_doiteasy-0.0.3/easycheck_doiteasy/easycheck_doiteasy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import requests
 import os
 import logging
 logging = logging.getLogger(__name__)
 
 
 
-class Easycheck():
+class MainMonitror():
 
     def __init__(self, token):
+        """
+        Constructor for the Monitor class.
+        Parameters:
+        token (str): The authentication token for the ETLCheck API.
+        Attributes:
+        token (str): The provided authentication token.
+        domain (str): The default domain URL for API calls.
+        """
         self.token = token
         self.domain = 'https://etlcheck.com'
 
 
     def send_ejecution(self, name, duration, start_datetime, end_datetime, destination, total_register, successful):
         """
         Sends execution data to a specified API endpoint.
```

### Comparing `easycheck_doiteasy-0.0.2/easycheck_doiteasy.egg-info/PKG-INFO` & `easycheck_doiteasy-0.0.3/easycheck_doiteasy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycheck-doiteasy
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple Python package example
 Home-page: https://etlcheck.com/
 Author: Jesus Rojas
 Author-email: jora2415@gmailc.om
 Project-URL: Bug Tracker, https://github.com/kamicase24/easycheck/-/issues
 Project-URL: repository, https://github.com/kamicase24/easycheck
 Classifier: Programming Language :: Python :: 3
```

### Comparing `easycheck_doiteasy-0.0.2/setup.cfg` & `easycheck_doiteasy-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = easycheck_doiteasy
-version = 0.0.2
+version = 0.0.3
 author = Jesus Rojas
 author_email = jora2415@gmailc.om
 description = A simple Python package example
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://etlcheck.com/
 project_urls =
```

