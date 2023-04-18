# Comparing `tmp/saagieapi-2.4.0.tar.gz` & `tmp/saagieapi-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saagieapi-2.4.0.tar", max compression
+gzip compressed data, was "saagieapi-2.4.1.tar", max compression
```

## Comparing `saagieapi-2.4.0.tar` & `saagieapi-2.4.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11357 2023-04-12 13:06:35.221221 saagieapi-2.4.0/LICENSE
--rw-r--r--   0        0        0     4379 2023-04-12 13:06:35.221221 saagieapi-2.4.0/README.md
--rw-r--r--   0        0        0     1562 2023-04-12 13:07:06.465411 saagieapi-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      502 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/__init__.py
--rw-r--r--   0        0        0       43 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/apps/__init__.py
--rw-r--r--   0        0        0    33369 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/apps/apps.py
--rw-r--r--   0        0        0     7591 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/apps/gql_queries.py
--rw-r--r--   0        0        0       83 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/docker_credentials/__init__.py
--rw-r--r--   0        0        0     8465 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/docker_credentials/docker_credentials.py
--rw-r--r--   0        0        0     1657 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/docker_credentials/gql_queries.py
--rw-r--r--   0        0        0       53 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/env_vars/__init__.py
--rw-r--r--   0        0        0    27280 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/env_vars/env_vars.py
--rw-r--r--   0        0        0     2671 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/env_vars/gql_queries.py
--rw-r--r--   0        0        0     2414 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/gql_queries.py
--rw-r--r--   0        0        0       43 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/jobs/__init__.py
--rw-r--r--   0        0        0     9510 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/jobs/gql_queries.py
--rw-r--r--   0        0        0    36314 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/jobs/jobs.py
--rw-r--r--   0        0        0      141 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/pipelines/__init__.py
--rw-r--r--   0        0        0     7785 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/pipelines/gql_queries.py
--rw-r--r--   0        0        0     2384 2023-04-12 13:06:35.225221 saagieapi-2.4.0/saagieapi/pipelines/graph_pipeline.py
--rw-r--r--   0        0        0    29262 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/pipelines/pipelines.py
--rw-r--r--   0        0        0       55 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/projects/__init__.py
--rw-r--r--   0        0        0     2962 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/projects/gql_queries.py
--rw-r--r--   0        0        0    24403 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/projects/projects.py
--rw-r--r--   0        0        0       67 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/repositories/__init__.py
--rw-r--r--   0        0        0     8443 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/repositories/gql_queries.py
--rw-r--r--   0        0        0    10534 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/repositories/repositories.py
--rw-r--r--   0        0        0    14653 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/saagie_api.py
--rw-r--r--   0        0        0       55 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/storages/__init__.py
--rw-r--r--   0        0        0     1384 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/storages/gql_queries.py
--rw-r--r--   0        0        0     6561 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/storages/storages.py
--rw-r--r--   0        0        0        0 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/__init__.py
--rw-r--r--   0        0        0     1725 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/bearer_auth.py
--rw-r--r--   0        0        0     3969 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/folder_functions.py
--rw-r--r--   0        0        0     3113 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/gql_client.py
--rw-r--r--   0        0        0       54 2023-04-12 13:06:35.229221 saagieapi-2.4.0/saagieapi/utils/rich_console.py
--rw-r--r--   0        0        0     5328 1970-01-01 00:00:00.000000 saagieapi-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-18 13:00:45.947220 saagieapi-2.4.1/LICENSE
+-rw-r--r--   0        0        0     4555 2023-04-18 13:00:45.947220 saagieapi-2.4.1/README.md
+-rw-r--r--   0        0        0     1562 2023-04-18 13:01:22.735811 saagieapi-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      502 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/__init__.py
+-rw-r--r--   0        0        0       43 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/apps/__init__.py
+-rw-r--r--   0        0        0    33369 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/apps/apps.py
+-rw-r--r--   0        0        0     7591 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/apps/gql_queries.py
+-rw-r--r--   0        0        0       83 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/docker_credentials/__init__.py
+-rw-r--r--   0        0        0     8465 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/docker_credentials/docker_credentials.py
+-rw-r--r--   0        0        0     1657 2023-04-18 13:00:45.951220 saagieapi-2.4.1/saagieapi/docker_credentials/gql_queries.py
+-rw-r--r--   0        0        0       53 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/env_vars/__init__.py
+-rw-r--r--   0        0        0    27280 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/env_vars/env_vars.py
+-rw-r--r--   0        0        0     2671 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/env_vars/gql_queries.py
+-rw-r--r--   0        0        0     2414 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/gql_queries.py
+-rw-r--r--   0        0        0       43 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/jobs/__init__.py
+-rw-r--r--   0        0        0     9510 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/jobs/gql_queries.py
+-rw-r--r--   0        0        0    36314 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/jobs/jobs.py
+-rw-r--r--   0        0        0      141 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/__init__.py
+-rw-r--r--   0        0        0     7785 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/gql_queries.py
+-rw-r--r--   0        0        0     2384 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/graph_pipeline.py
+-rw-r--r--   0        0        0    29262 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/pipelines/pipelines.py
+-rw-r--r--   0        0        0       55 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/projects/__init__.py
+-rw-r--r--   0        0        0     2962 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/projects/gql_queries.py
+-rw-r--r--   0        0        0    24404 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/projects/projects.py
+-rw-r--r--   0        0        0       67 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/repositories/__init__.py
+-rw-r--r--   0        0        0     8443 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/repositories/gql_queries.py
+-rw-r--r--   0        0        0    10534 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/repositories/repositories.py
+-rw-r--r--   0        0        0    14653 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/saagie_api.py
+-rw-r--r--   0        0        0       55 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/storages/__init__.py
+-rw-r--r--   0        0        0     1384 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/storages/gql_queries.py
+-rw-r--r--   0        0        0     6561 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/storages/storages.py
+-rw-r--r--   0        0        0        0 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/__init__.py
+-rw-r--r--   0        0        0     1725 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/bearer_auth.py
+-rw-r--r--   0        0        0     3969 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/folder_functions.py
+-rw-r--r--   0        0        0     3113 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/gql_client.py
+-rw-r--r--   0        0        0       54 2023-04-18 13:00:45.955220 saagieapi-2.4.1/saagieapi/utils/rich_console.py
+-rw-r--r--   0        0        0     5504 1970-01-01 00:00:00.000000 saagieapi-2.4.1/PKG-INFO
```

### Comparing `saagieapi-2.4.0/LICENSE` & `saagieapi-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/README.md` & `saagieapi-2.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,26 +17,31 @@
 - [Usage](#usage)
 - [Contributing](#contributing)
 
 ## Presentation
 
 The `saagieapi` python package implements python API wrappers to easily interact with the Saagie platform in python.
 
+## Documentation
+
+You can find the documentation of this package [here](https://saagieapi.readthedocs.io/en/latest/).
+
 ## Installing
 
 ```bash
 pip install saagieapi==<version>
 ```
 
 ### Compatibility with your Saagie platform
 
 | **Saagie platform version** | **saagie-api release** |
 |-----------------------------|------------------------|
 | < 2.2.0                     | < 0.6.0                |
 | >= 2.2.0                    | >= 0.6.0               |
+| >= 2023.01                  | >= 2.4.0               |
 
 ## Usage
 
 All the implemented features are documented in the [Wiki](https://github.com/saagie/api-saagie/wiki)
 
 Here's a full example of how to use the API:
```

### Comparing `saagieapi-2.4.0/pyproject.toml` & `saagieapi-2.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saagieapi"
-version = "2.4.0"
+version = "2.4.1"
 description = "Python API to interact with Saagie"
 authors = ["Saagie"]
 license = "GLWTPL"
 readme = "README.md"
 repository = "https://github.com/saagie/api-saagie"
 
 [tool.poetry.dependencies]
```

### Comparing `saagieapi-2.4.0/saagieapi/apps/apps.py` & `saagieapi-2.4.1/saagieapi/apps/apps.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/apps/gql_queries.py` & `saagieapi-2.4.1/saagieapi/apps/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/docker_credentials/docker_credentials.py` & `saagieapi-2.4.1/saagieapi/docker_credentials/docker_credentials.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/docker_credentials/gql_queries.py` & `saagieapi-2.4.1/saagieapi/docker_credentials/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/env_vars/env_vars.py` & `saagieapi-2.4.1/saagieapi/env_vars/env_vars.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/env_vars/gql_queries.py` & `saagieapi-2.4.1/saagieapi/env_vars/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/gql_queries.py` & `saagieapi-2.4.1/saagieapi/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/jobs/gql_queries.py` & `saagieapi-2.4.1/saagieapi/jobs/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/jobs/jobs.py` & `saagieapi-2.4.1/saagieapi/jobs/jobs.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/pipelines/gql_queries.py` & `saagieapi-2.4.1/saagieapi/pipelines/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/pipelines/graph_pipeline.py` & `saagieapi-2.4.1/saagieapi/pipelines/graph_pipeline.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/pipelines/pipelines.py` & `saagieapi-2.4.1/saagieapi/pipelines/pipelines.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/projects/gql_queries.py` & `saagieapi-2.4.1/saagieapi/projects/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/projects/projects.py` & `saagieapi-2.4.1/saagieapi/projects/projects.py`

 * *Files 0% similar despite different names*

```diff
@@ -528,15 +528,15 @@
             logging.info("✅ Project [%s] successfully exported", project_id)
         return result
 
     def import_from_json(
         self,
         path_to_folder: str = None,
     ) -> bool:
-        """Import a job from JSON format
+        """Import a project from a folder
 
         Parameters
         ----------
         path_to_folder : str, optional
             Path to the folder of the project to import
         Returns
         -------
```

### Comparing `saagieapi-2.4.0/saagieapi/repositories/gql_queries.py` & `saagieapi-2.4.1/saagieapi/repositories/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/repositories/repositories.py` & `saagieapi-2.4.1/saagieapi/repositories/repositories.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/saagie_api.py` & `saagieapi-2.4.1/saagieapi/saagie_api.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/storages/gql_queries.py` & `saagieapi-2.4.1/saagieapi/storages/gql_queries.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/storages/storages.py` & `saagieapi-2.4.1/saagieapi/storages/storages.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/utils/bearer_auth.py` & `saagieapi-2.4.1/saagieapi/utils/bearer_auth.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/utils/folder_functions.py` & `saagieapi-2.4.1/saagieapi/utils/folder_functions.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/saagieapi/utils/gql_client.py` & `saagieapi-2.4.1/saagieapi/utils/gql_client.py`

 * *Files identical despite different names*

### Comparing `saagieapi-2.4.0/PKG-INFO` & `saagieapi-2.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saagieapi
-Version: 2.4.0
+Version: 2.4.1
 Summary: Python API to interact with Saagie
 Home-page: https://github.com/saagie/api-saagie
 License: GLWTPL
 Author: Saagie
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -42,26 +42,31 @@
 - [Usage](#usage)
 - [Contributing](#contributing)
 
 ## Presentation
 
 The `saagieapi` python package implements python API wrappers to easily interact with the Saagie platform in python.
 
+## Documentation
+
+You can find the documentation of this package [here](https://saagieapi.readthedocs.io/en/latest/).
+
 ## Installing
 
 ```bash
 pip install saagieapi==<version>
 ```
 
 ### Compatibility with your Saagie platform
 
 | **Saagie platform version** | **saagie-api release** |
 |-----------------------------|------------------------|
 | < 2.2.0                     | < 0.6.0                |
 | >= 2.2.0                    | >= 0.6.0               |
+| >= 2023.01                  | >= 2.4.0               |
 
 ## Usage
 
 All the implemented features are documented in the [Wiki](https://github.com/saagie/api-saagie/wiki)
 
 Here's a full example of how to use the API:
```

