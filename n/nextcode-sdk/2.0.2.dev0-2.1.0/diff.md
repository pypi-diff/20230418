# Comparing `tmp/nextcode_sdk-2.0.2.dev0.tar.gz` & `tmp/nextcode_sdk-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextcode_sdk-2.0.2.dev0.tar", max compression
+gzip compressed data, was "nextcode_sdk-2.1.0.tar", max compression
```

## Comparing `nextcode_sdk-2.0.2.dev0.tar` & `nextcode_sdk-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,48 @@
--rw-r--r--   0        0        0     1070 2022-10-24 15:18:50.761869 nextcode_sdk-2.0.2.dev0/LICENSE
--rw-r--r--   0        0        0     2393 2022-10-24 15:18:50.761869 nextcode_sdk-2.0.2.dev0/README.md
--rw-r--r--   0        0        0      647 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/__init__.py
--rw-r--r--   0        0        0     8552 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/client.py
--rw-r--r--   0        0        0     6482 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/config.py
--rw-r--r--   0        0        0     3327 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/credentials.py
--rw-r--r--   0        0        0     6746 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/csa.py
--rw-r--r--   0        0        0     1302 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/exceptions.py
--rw-r--r--   0        0        0    15309 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/keycloak.py
--rw-r--r--   0        0        0      516 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/nextcode.py
--rw-r--r--   0        0        0     4292 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/packagelocal.py
--rw-r--r--   0        0        0     3081 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/__init__.py
--rw-r--r--   0        0        0      134 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenoteke/__init__.py
--rw-r--r--   0        0        0     1895 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenoteke/service.py
--rw-r--r--   0        0        0      167 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/__init__.py
--rw-r--r--   0        0        0     1789 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/analysis_catalog.py
--rw-r--r--   0        0        0     1554 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/analysis_catalog_run.py
--rw-r--r--   0        0        0      127 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/exceptions.py
--rw-r--r--   0        0        0     8034 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/phenotype.py
--rw-r--r--   0        0        0     3604 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/phenotype_matrix.py
--rw-r--r--   0        0        0     3803 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/playlist.py
--rw-r--r--   0        0        0    30337 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/service.py
--rw-r--r--   0        0        0      669 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/__init__.py
--rw-r--r--   0        0        0      224 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/exceptions.py
--rw-r--r--   0        0        0     5881 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/job.py
--rw-r--r--   0        0        0     3838 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/service.py
--rw-r--r--   0        0        0      214 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/project/__init__.py
--rw-r--r--   0        0        0      227 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/project/exceptions.py
--rw-r--r--   0        0        0    12632 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/project/service.py
--rw-r--r--   0        0        0      154 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/query/__init__.py
--rw-r--r--   0        0        0      481 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/query/exceptions.py
--rw-r--r--   0        0        0    16226 2022-10-24 15:18:50.765869 nextcode_sdk-2.0.2.dev0/nextcode/services/query/jupyter.py
--rw-r--r--   0        0        0    12819 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/query/query.py
--rw-r--r--   0        0        0    15851 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/query/service.py
--rw-r--r--   0        0        0     2142 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/query/utils.py
--rw-r--r--   0        0        0      135 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/queryserver/__init__.py
--rw-r--r--   0        0        0     6151 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/queryserver/result.py
--rw-r--r--   0        0        0     3842 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/queryserver/service.py
--rw-r--r--   0        0        0      310 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/__init__.py
--rw-r--r--   0        0        0      223 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/exceptions.py
--rw-r--r--   0        0        0    10501 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/job.py
--rw-r--r--   0        0        0     9159 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/pytest_plugin.py
--rw-r--r--   0        0        0    12238 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/service.py
--rw-r--r--   0        0        0     1574 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/weblog.py
--rw-r--r--   0        0        0     8172 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/session.py
--rw-r--r--   0        0        0     4350 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/nextcode/utils.py
--rw-r--r--   0        0        0     2200 2022-10-24 15:18:50.769869 nextcode_sdk-2.0.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     3883 1970-01-01 00:00:00.000000 nextcode_sdk-2.0.2.dev0/setup.py
--rw-r--r--   0        0        0     4559 1970-01-01 00:00:00.000000 nextcode_sdk-2.0.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-18 15:04:38.684354 nextcode_sdk-2.1.0/LICENSE
+-rw-r--r--   0        0        0     2393 2023-04-18 15:04:38.684354 nextcode_sdk-2.1.0/README.md
+-rw-r--r--   0        0        0      647 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/__init__.py
+-rw-r--r--   0        0        0     8570 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/client.py
+-rw-r--r--   0        0        0     6482 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/config.py
+-rw-r--r--   0        0        0     3327 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/credentials.py
+-rw-r--r--   0        0        0     6746 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/csa.py
+-rw-r--r--   0        0        0     1302 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/exceptions.py
+-rw-r--r--   0        0        0    15309 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/keycloak.py
+-rw-r--r--   0        0        0     1150 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/nextcode.py
+-rw-r--r--   0        0        0     4292 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/packagelocal.py
+-rw-r--r--   0        0        0     3081 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/__init__.py
+-rw-r--r--   0        0        0      134 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenoteke/__init__.py
+-rw-r--r--   0        0        0     1895 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenoteke/service.py
+-rw-r--r--   0        0        0      167 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/__init__.py
+-rw-r--r--   0        0        0     1789 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog.py
+-rw-r--r--   0        0        0     1554 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog_run.py
+-rw-r--r--   0        0        0      127 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/exceptions.py
+-rw-r--r--   0        0        0     8034 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype.py
+-rw-r--r--   0        0        0     3604 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype_matrix.py
+-rw-r--r--   0        0        0     3803 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/playlist.py
+-rw-r--r--   0        0        0    30337 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/phenotype/service.py
+-rw-r--r--   0        0        0      669 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/__init__.py
+-rw-r--r--   0        0        0      224 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/exceptions.py
+-rw-r--r--   0        0        0     5881 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/job.py
+-rw-r--r--   0        0        0     3838 2023-04-18 15:04:38.688354 nextcode_sdk-2.1.0/nextcode/services/pipelines/service.py
+-rw-r--r--   0        0        0      214 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/project/__init__.py
+-rw-r--r--   0        0        0      227 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/project/exceptions.py
+-rw-r--r--   0        0        0    12632 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/project/service.py
+-rw-r--r--   0        0        0      154 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/__init__.py
+-rw-r--r--   0        0        0      481 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/exceptions.py
+-rw-r--r--   0        0        0    16226 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/jupyter.py
+-rw-r--r--   0        0        0    12837 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/query.py
+-rw-r--r--   0        0        0    15851 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/service.py
+-rw-r--r--   0        0        0     2142 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/query/utils.py
+-rw-r--r--   0        0        0      135 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/queryserver/__init__.py
+-rw-r--r--   0        0        0     6151 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/queryserver/result.py
+-rw-r--r--   0        0        0     3842 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/queryserver/service.py
+-rw-r--r--   0        0        0      310 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/__init__.py
+-rw-r--r--   0        0        0      223 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/exceptions.py
+-rw-r--r--   0        0        0    10501 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/job.py
+-rw-r--r--   0        0        0     9159 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/pytest_plugin.py
+-rw-r--r--   0        0        0    12238 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/service.py
+-rw-r--r--   0        0        0     1574 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/services/workflow/weblog.py
+-rw-r--r--   0        0        0     8172 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/session.py
+-rw-r--r--   0        0        0     4350 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/nextcode/utils.py
+-rw-r--r--   0        0        0     2199 2023-04-18 15:04:38.692354 nextcode_sdk-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4562 1970-01-01 00:00:00.000000 nextcode_sdk-2.1.0/PKG-INFO
```

### Comparing `nextcode_sdk-2.0.2.dev0/LICENSE` & `nextcode_sdk-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/README.md` & `nextcode_sdk-2.1.0/README.md`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/__init__.py` & `nextcode_sdk-2.1.0/nextcode/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/client.py` & `nextcode_sdk-2.1.0/nextcode/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """
 client
 ~~~~~~~~~~
 
-This is the basic entrypoint to interact with services.
+This is the client used by the Service class to communicate with the API.
 """
 
 import os
 import pkgutil
 from importlib import import_module
 from pathlib import Path
 import logging
```

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/config.py` & `nextcode_sdk-2.1.0/nextcode/config.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/credentials.py` & `nextcode_sdk-2.1.0/nextcode/credentials.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/csa.py` & `nextcode_sdk-2.1.0/nextcode/csa.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/exceptions.py` & `nextcode_sdk-2.1.0/nextcode/exceptions.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/keycloak.py` & `nextcode_sdk-2.1.0/nextcode/keycloak.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/packagelocal.py` & `nextcode_sdk-2.1.0/nextcode/packagelocal.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/__init__.py` & `nextcode_sdk-2.1.0/nextcode/services/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenoteke/service.py` & `nextcode_sdk-2.1.0/nextcode/services/phenoteke/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/analysis_catalog.py` & `nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/analysis_catalog_run.py` & `nextcode_sdk-2.1.0/nextcode/services/phenotype/analysis_catalog_run.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/phenotype.py` & `nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/phenotype_matrix.py` & `nextcode_sdk-2.1.0/nextcode/services/phenotype/phenotype_matrix.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/playlist.py` & `nextcode_sdk-2.1.0/nextcode/services/phenotype/playlist.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/phenotype/service.py` & `nextcode_sdk-2.1.0/nextcode/services/phenotype/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/__init__.py` & `nextcode_sdk-2.1.0/nextcode/services/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/job.py` & `nextcode_sdk-2.1.0/nextcode/services/pipelines/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/pipelines/service.py` & `nextcode_sdk-2.1.0/nextcode/services/pipelines/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/project/service.py` & `nextcode_sdk-2.1.0/nextcode/services/project/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/query/jupyter.py` & `nextcode_sdk-2.1.0/nextcode/services/query/jupyter.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/query/query.py` & `nextcode_sdk-2.1.0/nextcode/services/query/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,16 +58,17 @@
     This object is returned from query methods in the 'query' service.
 
     :param service: query service handle
     :param resp: json response from query api endpoint
 
     Example usage:
 
-    >>> svc = nextcode.Client(profile_name='test').service('query', project='myproject')
-    >>> query = svc.get_queries(limit=1)[0]
+    >>> from nextcode import Nextcode
+    >>> nc = Nextcode(profile_name='test', project='myproject')
+    >>> query = nc.query.get_queries(limit=1)[0]
     >>> query.status
     'DONE'
     """
 
     raw: Dict = {}
     query_id = None
     url = None
```

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/query/service.py` & `nextcode_sdk-2.1.0/nextcode/services/query/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/query/utils.py` & `nextcode_sdk-2.1.0/nextcode/services/query/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/queryserver/result.py` & `nextcode_sdk-2.1.0/nextcode/services/queryserver/result.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/queryserver/service.py` & `nextcode_sdk-2.1.0/nextcode/services/queryserver/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/job.py` & `nextcode_sdk-2.1.0/nextcode/services/workflow/job.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/pytest_plugin.py` & `nextcode_sdk-2.1.0/nextcode/services/workflow/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/service.py` & `nextcode_sdk-2.1.0/nextcode/services/workflow/service.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/services/workflow/weblog.py` & `nextcode_sdk-2.1.0/nextcode/services/workflow/weblog.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/session.py` & `nextcode_sdk-2.1.0/nextcode/session.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/nextcode/utils.py` & `nextcode_sdk-2.1.0/nextcode/utils.py`

 * *Files identical despite different names*

### Comparing `nextcode_sdk-2.0.2.dev0/pyproject.toml` & `nextcode_sdk-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nextcode-sdk"
-version = "2.0.2-dev"
+version = "2.1.0"
 description = "Python SDK for Genuity Science Services"
 license = "MIT"
 authors = ["WUXI NextCODE <support@wuxinextcode.com>"]
 maintainers = ["Genuity Science Software Development <sdev@genuitysci.com>"]
 readme = "README.md"
 homepage = "https://www.github.com/wuxi-nextcode/nextcode-python-sdk"
 repository = "https://www.github.com/wuxi-nextcode/nextcode-python-sdk"
@@ -28,40 +28,40 @@
 ]
 packages = [{include = "nextcode"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 python-dateutil = "^2.8.2"
 PyYAML = "^6.0"
-requests = "^2.28.1"
+requests = "^2.28.2"
 hjson = "^3.1.0"
-boto3 = "^1.24.93"
-pandas = {version = "^1.5.1", optional = true}
-ipython = {version = "^8.5.0", optional = true}
-termcolor = {version = "^2.0.1", optional = true}
-tqdm = {version = "^4.64.1", optional = true}
-ipywidgets = {version = "^8.0.2", optional = true}
-plotly = {version = "^5.10.0", optional = true}
-PyJWT = "^2.5.0"
+boto3 = "^1.26.115"
+pandas = {version = "^2.0.0", optional = true}
+ipython = {version = "^8.12.0", optional = true}
+termcolor = {version = "^2.2.0", optional = true}
+tqdm = {version = "^4.65.0", optional = true}
+ipywidgets = {version = "^8.0.6", optional = true}
+plotly = {version = "^5.14.0", optional = true}
+PyJWT = "^2.6.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.1.3"
-responses = "^0.22.0"
+pytest = "^7.2.2"
+responses = "^0.23.1"
 pytest-cov = "^4.0.0"
 asserts = "^0.12.0"
 
 [tool.poetry.group.docs.dependencies]
-Sphinx = "^5.3.0"
+Sphinx = "^6.1.3"
 sphinx-bootstrap-theme = "^0.8.1"
-sphinx-rtd-theme = "^1.0.0"
-sphinx-autodoc-typehints = "^1.19.4"
-nbsphinx = "^0.8.9"
+sphinx-rtd-theme = "^1.2.0"
+sphinx-autodoc-typehints = "^1.19.5"
+nbsphinx = "^0.9.1"
 
 [tool.poetry.group.dev.dependencies]
-ipython = "^8.5.0"
+ipython = "^8.12.0"
 
 [tool.poetry.extras]
 jupyter = ["pandas", "ipython", "termcolor", "tqdm", "ipywidgets", "plotly"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nextcode_sdk-2.0.2.dev0/PKG-INFO` & `nextcode_sdk-2.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextcode-sdk
-Version: 2.0.2.dev0
+Version: 2.1.0
 Summary: Python SDK for Genuity Science Services
 Home-page: https://www.github.com/wuxi-nextcode/nextcode-python-sdk
 License: MIT
 Author: WUXI NextCODE
 Author-email: support@wuxinextcode.com
 Maintainer: Genuity Science Software Development
 Maintainer-email: sdev@genuitysci.com
@@ -25,26 +25,26 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: jupyter
-Requires-Dist: PyJWT (>=2.5.0,<3.0.0)
+Requires-Dist: PyJWT (>=2.6.0,<3.0.0)
 Requires-Dist: PyYAML (>=6.0,<7.0)
-Requires-Dist: boto3 (>=1.24.93,<2.0.0)
+Requires-Dist: boto3 (>=1.26.115,<2.0.0)
 Requires-Dist: hjson (>=3.1.0,<4.0.0)
-Requires-Dist: ipython (>=8.5.0,<9.0.0); extra == "jupyter"
-Requires-Dist: ipywidgets (>=8.0.2,<9.0.0); extra == "jupyter"
-Requires-Dist: pandas (>=1.5.1,<2.0.0); extra == "jupyter"
-Requires-Dist: plotly (>=5.10.0,<6.0.0); extra == "jupyter"
+Requires-Dist: ipython (>=8.12.0,<9.0.0) ; extra == "jupyter"
+Requires-Dist: ipywidgets (>=8.0.6,<9.0.0) ; extra == "jupyter"
+Requires-Dist: pandas (>=2.0.0,<3.0.0) ; extra == "jupyter"
+Requires-Dist: plotly (>=5.14.0,<6.0.0) ; extra == "jupyter"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: termcolor (>=2.0.1,<3.0.0); extra == "jupyter"
-Requires-Dist: tqdm (>=4.64.1,<5.0.0); extra == "jupyter"
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: termcolor (>=2.2.0,<3.0.0) ; extra == "jupyter"
+Requires-Dist: tqdm (>=4.65.0,<5.0.0) ; extra == "jupyter"
 Project-URL: Documentation, https://wuxi-nextcode.github.io/nextcode-python-sdk/
 Project-URL: Repository, https://www.github.com/wuxi-nextcode/nextcode-python-sdk
 Description-Content-Type: text/markdown
 
 [![Latest version on
 PyPi](https://badge.fury.io/py/nextcode-sdk.svg)](https://badge.fury.io/py/nextcode-sdk)
 [![Build Status](https://api.travis-ci.org/wuxi-nextcode/nextcode-python-sdk.svg?branch=master)](https://travis-ci.org/wuxi-nextcode/nextcode-python-sdk)
```

