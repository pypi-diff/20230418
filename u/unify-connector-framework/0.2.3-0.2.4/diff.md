# Comparing `tmp/unify-connector-framework-0.2.3.tar.gz` & `tmp/unify-connector-framework-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-connector-framework-0.2.3.tar", last modified: Tue Oct  4 19:05:12 2022, max compression
+gzip compressed data, was "dist/unify-connector-framework-0.2.4.tar", last modified: Tue Apr 18 16:45:51 2023, max compression
```

## Comparing `unify-connector-framework-0.2.3.tar` & `unify-connector-framework-0.2.4.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unify_connector_framework.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unify_connector_framework.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)      468 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unify_connector_framework.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unify_connector_framework.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unify_connector_framework.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unify_connector_framework.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-10-04 19:05:12.000000 unify-connector-framework-0.2.3/unifyconnectorframework/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/unifyconnectorframework/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    15041 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/unifyconnectorframework/connector.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/unifyconnectorframework/connector_handler.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    17842 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/unifyconnectorframework/organization_client.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2022-10-04 19:05:05.000000 unify-connector-framework-0.2.3/unifyconnectorframework/utils.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/LICENSE
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2477 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/README.md
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/setup.cfg
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1690 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/setup.py
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     2969 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      503 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       35 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/requires.txt
+-rw-r--r--   0 circleci  (3434) circleci  (3434)       24 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unify_connector_framework.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-04-18 16:45:51.000000 unify-connector-framework-0.2.4/unifyconnectorframework/
+-rw-r--r--   0 circleci  (3434) circleci  (3434)      799 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/__init__.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    15890 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/connector.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    10771 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/connector_handler.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1691 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/logging.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)    17872 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/organization_client.py
+-rw-r--r--   0 circleci  (3434) circleci  (3434)     1373 2023-04-18 16:45:45.000000 unify-connector-framework-0.2.4/unifyconnectorframework/utils.py
```

### Comparing `unify-connector-framework-0.2.3/LICENSE` & `unify-connector-framework-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.3/PKG-INFO` & `unify-connector-framework-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 0.2.3
+Version: 0.2.4
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-0.2.3/README.md` & `unify-connector-framework-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.3/setup.py` & `unify-connector-framework-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.3/unify_connector_framework.egg-info/PKG-INFO` & `unify-connector-framework-0.2.4/unify_connector_framework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unify-connector-framework
-Version: 0.2.3
+Version: 0.2.4
 Summary: Develop connectors for Element Unify with the Connector Framework
 Home-page: https://github.com/ElementAnalytics/unify-python-agents-common
 Author: Element Analytics
 Author-email: platform@ean.io
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `unify-connector-framework-0.2.3/unifyconnectorframework/__init__.py` & `unify-connector-framework-0.2.4/unifyconnectorframework/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 """
 Defines package information
 """
 from .organization_client import DatasetOperation, OrganizationClient
 from .connector_handler import ConnectorHandler
 from .connector import Connector
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
```

### Comparing `unify-connector-framework-0.2.3/unifyconnectorframework/connector.py` & `unify-connector-framework-0.2.4/unifyconnectorframework/connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,40 +12,65 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 A connector class includes methods needed for connectors.
 """
 import csv
+import logging
 from unify.connectors import ArtifactType, LogType
+from unifyconnectorframework.logging import UnifyHandler
 from unifyconnectorframework.organization_client import OrganizationClient, DatasetOperation
 
 class Connector:
     """
     Common connector class
     """
-    def __init__(self, account_id, password, org_id, hostname, id="", labels=None, version="0.0.0"):
+    def __init__(
+            self,
+            account_id,
+            password,
+            org_id,
+            hostname,
+            id="",
+            labels=None,
+            version="0.0.0",
+            logger = None,
+        ):
         """
         Initiate a new connector
 
         :type account_id: string
         :param account_id: Service account identifier
         :type password: string
         :param password: Content to upload
         :type org_id: string
         :param org_id: Content to upload
         :type hostname: string
         :param hostname: Content to upload
         :type id: GUID
         :param id: Connector identifier
-        :type label: dict
-        :param label: Labels associated to connector, in format {"category": "[connector_category]"}
+        :type labels: dict
+        :param labels: Labels related to connector, in format {"category": "[connector_category]"}
         :type version: string
         :param version: Connector version
+        :type logger: logging.Logger
+        :param logger: instance of logger to be used
         """
+
+        if logger is None:
+            self.log = logging.getLogger("unifyconnectorframework")
+            self.log.setLevel(logging.INFO)
+            fmt = logging.Formatter('%(asctime)s - [%(levelname)s] %(message)s')
+            hdl = logging.StreamHandler()
+            hdl.setFormatter(fmt)
+            self.log.addHandler(hdl)
+        else:
+            self.log = logger
+
         self.id = id
         self.labels = labels
         # Note that the default value for labels is set to None rather than a default dictionary.
         # The "default" dictionary gets created as a persistent object so every invocation of a
         # Connector that does not specify an extra param will use the same dictionary.
         if labels is None:
             self.labels = {"category": ""}
@@ -58,15 +83,22 @@
             "version": self.version
         }
         self.organization_client = OrganizationClient(
             user_name=self.account_id,
             password=password,
             org_id=org_id,
             cluster=hostname,
-            connector_params=self.connector_params)
+            connector_params=self.connector_params,
+            logger=self.log
+        )
+
+        if logger is None:
+            hdl = UnifyHandler(self)
+            hdl.setFormatter(fmt)
+            self.log.addHandler(hdl)
 
     def list_datasets(self):
         """
         Retrieve all datasets.
         """
         return self.organization_client.list_datasets()
 
@@ -174,15 +206,15 @@
         """
         dataset_id_str = self.organization_client.resolve_dataset_id(dataset_id)
         if isinstance(labels, str):
             result = self.organization_client.update_dataset_labels(dataset_id_str, [labels])
         elif isinstance(labels, list):
             result = self.organization_client.update_dataset_labels(dataset_id_str, labels)
         else:
-            raise Exception('Labels should be an instance of str or list')
+            raise ValueError('Labels should be an instance of str or list')
         dataset_name = [x['name'] for x in self.list_datasets() if x['id']['id']==dataset_id_str][0]
         self.check_or_set_artifact(dataset_id_str, ArtifactType.DATASET, dataset_name)
         return result
 
     def operate_dataset(
         self,
         dataset_csv,
```

### Comparing `unify-connector-framework-0.2.3/unifyconnectorframework/connector_handler.py` & `unify-connector-framework-0.2.4/unifyconnectorframework/connector_handler.py`

 * *Files identical despite different names*

### Comparing `unify-connector-framework-0.2.3/unifyconnectorframework/organization_client.py` & `unify-connector-framework-0.2.4/unifyconnectorframework/organization_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 A organization client includes methods needed for connectors.
 """
-import logging
 from enum import Enum
 from unify.properties import Properties, ClusterSetting
 from unify.orgadmin import OrgAdmin
 from unify.sources import Sources
 from unify.templates import Templates
 from unify.graph import Graph
 from unify.connectors import LogType, Connectors
@@ -32,15 +31,18 @@
     APPEND = 2
 
 class OrganizationClient:
     """
     Common connector class
     """
 
-    def __init__(self, user_name, password, org_id, cluster, connector_params):
+    def __init__(self, user_name, password, org_id, cluster, connector_params, logger):
+
+        self.log = logger
+
         self.user_name = user_name
         self.password = password
         self.org_id = org_id
         self.cluster = cluster
         self.connector_params = connector_params
 
         self.app_name = 'imc'
@@ -52,39 +54,39 @@
                 query_params=connector_params
             )
             self.props.set_auth_token(
                 token=token,
                 cluster=self.app_name
             )
         except Exception as error:
-            logging.error('Failed to login. %s', error)
+            self.log.error('Failed to login. %s', error)
             raise error
 
         try:
             self.connectors = Connectors(self.app_name, self.props, self.org_id)
         except Exception as error:
-            logging.error('Failed to get organization connectors client.')
+            self.log.error('Failed to get organization connectors client.')
             raise error
 
         try:
             self.sources = Sources(self.app_name, self.props, self.org_id)
         except Exception as error:
-            logging.error('Failed to get organization sources client.')
+            self.log.error('Failed to get organization sources client.')
             raise error
 
         try:
             self.templates = Templates(self.app_name, self.props, self.org_id)
         except Exception as error:
-            logging.error('Failed to get organization templates client.')
+            self.log.error('Failed to get organization templates client.')
             raise error
 
         try:
             self.graph = Graph(self.app_name, self.props, self.org_id)
         except Exception as error:
-            logging.error('Failed to get organization graph client.')
+            self.log.error('Failed to get organization graph client.')
             raise error
 
     def list_datasets(self):
         """
         Retrieve all datasets.
         """
         return self.sources.get_sources(org_id=self.org_id)
@@ -235,31 +237,31 @@
         :param dataset_id: Existing dataset id
         :type operation: Enum
         :param operation: Operation on dataset, update or append
         """
         dataset_id_str = self.resolve_dataset_id(dataset_id)
         if dataset_id_str is None:
             dataset_id_str = self.create_dataset(dataset_name, dataset_csv)['data_set_id']
-            logging.info('create dataset %s id %s to cluster: %s, organization: %d',
+            self.log.info('create dataset %s id %s to cluster: %s, organization: %d',
                 dataset_name, dataset_id_str, self.cluster, self.org_id)
         else:
             # validate dataset_id
             existing_datasets = [
                 dataset.get("id", {}).get('id') for dataset in self.list_datasets()
             ]
             if dataset_id_str not in existing_datasets:
-                raise Exception(f'Given dataset id {dataset_id_str} does not exists.')
+                raise ValueError(f'Given dataset id {dataset_id_str} does not exists.')
             if operation is DatasetOperation.UPDATE:
                 self.truncate_dataset(dataset_id=dataset_id_str)
                 self.append_dataset(dataset_id=dataset_id_str, dataset_csv=dataset_csv)
-                logging.info('update dataset %s  to cluster: %s, organization: %d',
+                self.log.info('update dataset %s  to cluster: %s, organization: %d',
                     dataset_id_str, self.cluster, self.org_id)
             elif operation is DatasetOperation.APPEND:
                 self.append_dataset(dataset_id_str, dataset_csv)
-                logging.info('append dataset %s to cluster: %s, organization: %d',
+                self.log.info('append dataset %s to cluster: %s, organization: %d',
                     dataset_id_str, self.cluster, self.org_id)
         return dataset_id_str
 
     def get_datastream_info(self, datastream_id, sequence_nr=0):
         """
         Returns the information of the events starting in the event sequene number provided
```

### Comparing `unify-connector-framework-0.2.3/unifyconnectorframework/utils.py` & `unify-connector-framework-0.2.4/unifyconnectorframework/utils.py`

 * *Files identical despite different names*

