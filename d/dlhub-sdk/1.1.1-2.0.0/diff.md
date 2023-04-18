# Comparing `tmp/dlhub_sdk-1.1.1.tar.gz` & `tmp/dlhub_sdk-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dlhub_sdk-1.1.1.tar", last modified: Mon Oct 24 17:00:26 2022, max compression
+gzip compressed data, was "dlhub_sdk-2.0.0.tar", last modified: Tue Apr 18 14:51:01 2023, max compression
```

## Comparing `dlhub_sdk-1.1.1.tar` & `dlhub_sdk-2.0.0.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:26.102929 dlhub_sdk-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-24 17:00:26.102929 dlhub_sdk-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6661 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:26.094929 dlhub_sdk-1.1.1/dlhub_sdk/
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27920 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (121)      195 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:26.094929 dlhub_sdk-1.1.1/dlhub_sdk/models/
--rw-r--r--   0 runner    (1001) docker     (121)    18602 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    19302 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/datacite.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:26.098929 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/
--rw-r--r--   0 runner    (1001) docker     (121)     4649 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6976 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/keras.py
--rw-r--r--   0 runner    (1001) docker     (121)     9905 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/python.py
--rw-r--r--   0 runner    (1001) docker     (121)     2923 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (121)     7090 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/sklearn.py
--rw-r--r--   0 runner    (1001) docker     (121)     7703 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/models/servables/tensorflow.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:26.102929 dlhub_sdk-1.1.1/dlhub_sdk/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (121)     1505 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/funcx_login_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     3211 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/futures.py
--rw-r--r--   0 runner    (1001) docker     (121)     4546 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/inspect.py
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)     7071 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/search.py
--rw-r--r--   0 runner    (1001) docker     (121)     3931 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (121)    11358 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/utils/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/dlhub_sdk/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-24 17:00:26.094929 dlhub_sdk-1.1.1/dlhub_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      986 2022-10-24 17:00:26.000000 dlhub_sdk-1.1.1/dlhub_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      824 2022-10-24 17:00:26.000000 dlhub_sdk-1.1.1/dlhub_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-24 17:00:26.000000 dlhub_sdk-1.1.1/dlhub_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-10-24 17:00:26.000000 dlhub_sdk-1.1.1/dlhub_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-24 17:00:26.000000 dlhub_sdk-1.1.1/dlhub_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-10-24 17:00:26.102929 dlhub_sdk-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1637 2022-10-24 17:00:16.000000 dlhub_sdk-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:51:01.763718 dlhub_sdk-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 14:51:01.763718 dlhub_sdk-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6661 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:51:01.759718 dlhub_sdk-2.0.0/dlhub_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33939 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:51:01.759718 dlhub_sdk-2.0.0/dlhub_sdk/models/
+-rw-r--r--   0 runner    (1001) docker     (123)    18602 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19337 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/datacite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:51:01.763718 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9905 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/python.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/sklearn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/models/servables/tensorflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:51:01.763718 dlhub_sdk-2.0.0/dlhub_sdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/funcx_login_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3211 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/futures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7849 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/publish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/utils/validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/dlhub_sdk/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 14:51:01.759718 dlhub_sdk-2.0.0/dlhub_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 14:51:01.000000 dlhub_sdk-2.0.0/dlhub_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-04-18 14:51:01.000000 dlhub_sdk-2.0.0/dlhub_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 14:51:01.000000 dlhub_sdk-2.0.0/dlhub_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-18 14:51:01.000000 dlhub_sdk-2.0.0/dlhub_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 14:51:01.000000 dlhub_sdk-2.0.0/dlhub_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-18 14:51:01.763718 dlhub_sdk-2.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-04-18 14:50:52.000000 dlhub_sdk-2.0.0/setup.py
```

### Comparing `dlhub_sdk-1.1.1/LICENSE` & `dlhub_sdk-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/PKG-INFO` & `dlhub_sdk-2.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlhub_sdk
-Version: 1.1.1
+Version: 2.0.0
 Summary: Python interface and utilities for DLHub
 Home-page: https://github.com/DLHub-Argonne/dlhub_sdk
 Author: Ben Blaiszik
 Author-email: bblaiszik@anl.gov
 License: Apache License, Version 2.0
 Keywords: DLHub,Data and Learning Hub for Science,machine learning,data publication,reproducibility
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dlhub_sdk-1.1.1/README.md` & `dlhub_sdk-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/client.py` & `dlhub_sdk-2.0.0/dlhub_sdk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,33 @@
 import importlib
 import logging
-import json
 import os
 from tempfile import mkstemp
 from typing import Sequence, Union, Any, Optional, Tuple, Dict, List
 import requests
 import globus_sdk
+import uuid
 
 from globus_sdk import BaseClient
-from globus_sdk.utils import slash_join
 from globus_sdk.authorizers import GlobusAuthorizer
 from mdf_toolbox import login, logout
 from mdf_toolbox.globus_search.search_helper import SEARCH_LIMIT
 from funcx.sdk.client import FuncXClient
 from globus_sdk.scopes import AuthScopes, SearchScopes
 
-from dlhub_sdk.config import DLHUB_SERVICE_ADDRESS, CLIENT_ID
+from dlhub_sdk.config import DLHUB_SERVICE_ADDRESS, CLIENT_ID, GLOBUS_SEARCH_LAMBDA_SCOPE
 from dlhub_sdk.utils.futures import DLHubFuture
 from dlhub_sdk.utils.schemas import validate_against_dlhub_schema
 from dlhub_sdk.utils.search import DLHubSearchHelper, get_method_details, filter_latest
 from dlhub_sdk.utils.validation import validate
 from dlhub_sdk.utils.funcx_login_manager import FuncXLoginManager
+# from dlhub_sdk.utils.publish import *
+from dlhub_sdk.utils.publish import create_container_spec, search_ingest, get_dlhub_file, register_funcx, check_container_build_status
+from dlhub_sdk.utils.publish import update_servable_zip_with_metadata
+from time import time
 
 # Directory for authentication tokens
 _token_dir = os.path.expanduser("~/.dlhub/credentials")
 logger = logging.getLogger(__name__)
 
 
 class HelpMessage(Exception):
@@ -53,14 +56,15 @@
     # service name is a class attribute in Globus SDK 3
     service_name = "DLHub"
 
     def __init__(self, dlh_authorizer: Optional[GlobusAuthorizer] = None,
                  search_authorizer: Optional[GlobusAuthorizer] = None,
                  fx_authorizer: Optional[GlobusAuthorizer] = None,
                  openid_authorizer: Optional[GlobusAuthorizer] = None,
+                 sl_authorizer: Optional[GlobusAuthorizer] = None,
                  http_timeout: Optional[int] = None,
                  force_login: bool = False, **kwargs):
         """Initialize the client
 
         Args:
             http_timeout (int): Timeout for any call to service in seconds. (default is no timeout)
             force_login (bool): Whether to force a login to get new credentials.
@@ -83,58 +87,77 @@
             fx_authorizer (:class:`GlobusAuthorizer
                             <globus_sdk.authorizers.base.GlobusAuthorizer>`):
                 An authorizer instance used to communicate with funcX.
                 If ``None``, will be created from your account's credentials.
             openid_authorizer (:class:`GlobusAuthorizer
                             <globus_sdk.authorizers.base.GlobusAuthorizer>`):
                 An authorizer instance used to communicate with OpenID.
+            sl_authorizer (:class:`GlobusAuthorizer
+                            <globus_sdk.authorizers.base.GlobusAuthorizer>`):
+                An authorizer instance used to communicate with the search lambda..
                 If ``None``, will be created from your account's credentials.
         Keyword arguments are the same as for :class:`BaseClient <globus_sdk.base.BaseClient>`.
         """
 
-        authorizers = [dlh_authorizer, search_authorizer, openid_authorizer, fx_authorizer]
+        authorizers = [dlh_authorizer, search_authorizer, openid_authorizer, fx_authorizer, sl_authorizer]
         # Get authorizers through Globus login if any are not provided
         if not all(a is not None for a in authorizers):
             # If some but not all were provided, warn the user they could be making a mistake
             if any(a is not None for a in authorizers):
                 logger.warning('You have defined some of the authorizers but not all. DLHub is falling back to login. '
                                'You must provide authorizers for DLHub, Search, OpenID, FuncX.')
 
             auth_res = login(services=["search", "dlhub",
-                                       FuncXClient.FUNCX_SCOPE, "openid"],
+                                       FuncXClient.FUNCX_SCOPE,
+                                       "openid",
+                                       "email",
+                                       "profile",
+                                       GLOBUS_SEARCH_LAMBDA_SCOPE],
                              app_name="DLHub_Client",
                              make_clients=False,
                              client_id=CLIENT_ID,
                              clear_old_tokens=force_login,
                              token_dir=_token_dir,
                              no_local_server=kwargs.get("no_local_server", True),
                              no_browser=kwargs.get("no_browser", True))
 
             # Unpack the authorizers
             dlh_authorizer = auth_res["dlhub"]
             fx_authorizer = auth_res[FuncXClient.FUNCX_SCOPE]
             openid_authorizer = auth_res['openid']
             search_authorizer = auth_res['search']
+            sl_authorizer = auth_res[GLOBUS_SEARCH_LAMBDA_SCOPE]
 
         # Define the subclients needed by the service
 
         auth_dict = {
             FuncXClient.FUNCX_SCOPE: fx_authorizer,
             AuthScopes.openid: openid_authorizer,
             SearchScopes.all: search_authorizer,
             'dlhub': dlh_authorizer,
         }
 
         login_manager = FuncXLoginManager(authorizers=auth_dict)
+        # Dev funcx_service_address="https://api.dev.funcx.org/v2"
+        # self._fx_client = FuncXClient(funcx_service_address="https://api.dev.funcx.org/v2", login_manager=login_manager)
         self._fx_client = FuncXClient(login_manager=login_manager)
 
         self._search_client = globus_sdk.SearchClient(authorizer=search_authorizer,
                                                       transport_params={"http_timeout": http_timeout})
 
+        self._openid_client = globus_sdk.AuthClient(authorizer=openid_authorizer,
+                                                    transport_params={"http_timeout": http_timeout})
+
+        self.userinfo = self._openid_client.oauth2_userinfo()
+        self.sl_authorizer = sl_authorizer
+
         # funcX endpoint to use
+        # Production endpoint is '86a47061-f3d9-44f0-90dc-56ddc642c000'
+        # Dev endpoint is '2238617a-8756-4030-a8ab-44ffb1446092'
+        # self.fx_endpoint = '2238617a-8756-4030-a8ab-44ffb1446092'
         self.fx_endpoint = '86a47061-f3d9-44f0-90dc-56ddc642c000'
         self.fx_cache = {}
 
         super(DLHubClient, self).__init__(environment='dlhub',
                                           authorizer=dlh_authorizer,
                                           transport_params={"http_timeout": http_timeout},
                                           base_url=DLHUB_SERVICE_ADDRESS,
@@ -250,15 +273,15 @@
     def run(self, name: str, inputs: Any, parameters: Optional[Dict[str, Any]] = None,
             asynchronous: bool = False, debug: bool = False, validate_input: bool = False,
             async_wait: float = 5, timeout: Optional[float] = None) \
             -> Union[
                 DLHubFuture,
                 Tuple[Any, Dict[str, Any]],
                 Any
-            ]:
+    ]:
         """Invoke a DLHub servable
 
         Args:
             name: DLHub name of the servable of the form <user>/<servable_name>
             inputs: Data to be used as input to the function. Can be a string of file paths or URLs
             parameters: Any optional parameters to pass to the function.
             asynchronous: Whether to return from the function immediately or wait for the execution to finish.
@@ -407,92 +430,121 @@
         model_info.set_creators(creators, affiliations or [])  # affiliations if provided, else empty list
         model_info.set_name(short_name)
 
         if paper_doi is not None:
             model_info.add_related_resource(paper_doi, "DOI", "IsDescribedBy")
 
         # perform the publish
-        task_id = self.publish_servable(model_info)
+        container_id = self.publish_servable(model_info)
 
         # return the id of the publish task
-        return task_id
+        return container_id
 
     def publish_servable(self, model):
         """Submit a servable to DLHub
 
         If this servable has not been published before, it will be assigned a unique identifier.
 
         If it has been published before (DLHub detects if it has an identifier), then DLHub
         will update the servable to the new version.
 
         Args:
             model (BaseMetadataModel): Servable to be submitted
         Returns:
-            (string): Task ID of this submission, used for checking for success
+            (string): Container ID of this submission, as returned from the Container Service
         """
 
         # Get the metadata
         metadata = model.to_dict(simplify_paths=True)
 
         # Mark the method used to submit the model
-        metadata['dlhub']['transfer_method'] = {'POST': 'file'}
+        # We're using signed_urls so it is S3
+        metadata['dlhub']['transfer_method'] = {'S3': 's3://'}
 
         # Validate against the servable schema
         validate_against_dlhub_schema(metadata, 'servable')
 
+        # Add username, etc. to metadata
+        self._prepare_metadata(metadata)
+
         # Wipe the fx cache so we don't keep reusing an old servable
         self.clear_funcx_cache()
 
         # Get the data to be submitted as a ZIP file
         fp, zip_filename = mkstemp('.zip')
         os.close(fp)
         os.unlink(zip_filename)
         try:
             model.get_zip_file(zip_filename)
 
+            # Add dlhub.json to zipfile
+            update_servable_zip_with_metadata(zip_filename, metadata)
+
             # Get the authorization header token (string for the headers dict)
-            header = self.authorizer.get_authorization_header()
+            # header = self.authorizer.get_authorization_header()
+
+            # Use signed URL to upload zip file
+            SIGNED_URL_ENDPOINT = "https://api.dlhub.org/api/v1/publish/signed_url"
+            S3_DOWNLOAD_PREFIX = "https://dlhub-anl.s3.us-east-1.amazonaws.com/"
+            reply = requests.get(
+                SIGNED_URL_ENDPOINT)
+            signed_url = reply.json()
+            logger.debug(f'signed_url["url"] is {signed_url["url"]}')
 
-            # Submit data to DLHub service
             with open(zip_filename, 'rb') as zf:
-                reply = requests.post(
-                    slash_join(self.base_url, 'publish'),
-                    headers={"Authorization": header},
+                http_response = requests.post(
+                    signed_url['url'],
+                    data=signed_url['fields'],
                     files={
-                        'json': ('dlhub.json', json.dumps(metadata), 'application/json'),
-                        'file': ('servable.zip', zf, 'application/octet-stream')
+                        'file': (signed_url['fields']['key'], zf, 'application/octet-stream')
                     }
                 )
 
+            # Per https://docs.aws.amazon.com/AmazonS3/latest/API/RESTObjectPOST.html
+            # default success returns a 204, but it could be set to return 200
+            # response on success.  We'll accept either
+            if not (http_response.status_code == 204 or http_response.status_code == 200):
+                raise Exception(http_response.text)
+            metadata['dlhub']['transfer_method']['S3'] = S3_DOWNLOAD_PREFIX + signed_url['fields']['key']
+
+            # Ingest Model to DLHub
+            task = self._ingest(metadata)
+
             # Return the task id
-            if reply.status_code != 200:
-                raise Exception(reply.text)
-            return reply.json()['task_id']
+            return task['container_id']
         finally:
             os.unlink(zip_filename)
 
     def publish_repository(self, repository):
         """Submit a repository to DLHub for publication
 
         Args:
             repository (string): Repository to publish
         Returns:
-            (string): Task ID of this submission, used for checking for success
+            (string): Container ID of this submission, as returned from the Container Service
         """
+        # Get dlhub.json from github repo
+        try:
+            metadata = get_dlhub_file(repository)
+        except Exception as e:
+            help_err = HelpMessage(f"No dlhub.json file could be retrieved from repository: {e}")
+            raise help_err from e
 
-        # Publish to DLHub
-        metadata = {"repository": repository}
+        # Set repository location in metadata
+        metadata['repository'] = repository
+
+        self._prepare_metadata(metadata)
 
         # Wipe the fx cache so we don't keep reusing an old servable
         self.clear_funcx_cache()
 
-        response = self.post('publish_repo', json_body=metadata)
+        # Ingest Model to DLHub
+        task = self._ingest(metadata)
 
-        task_id = response.data['task_id']
-        return task_id
+        return task['container_id']
 
     def search(self, query, advanced=False, limit=None, only_latest=True):
         """Query the DLHub servable library
 
         By default, the query is used as a simple plaintext search of all model metadata.
         Optionally, you can provided an advanced query on any of the indexed fields in
         the DLHub model metadata by setting :code:`advanced=True` and following the guide for
@@ -604,7 +656,89 @@
 
         if servable:
             del (self.fx_cache[servable])
         else:
             self.fx_cache = {}
 
         return self.fx_cache
+
+    def _prepare_metadata(self, metadata):
+        """Insert owner name, time-stamp, repository ID, and servable_uuid into metadata."""
+
+        # Insert owner name and time-stamp into metadata
+        # We get user name from the OIDC userinfo from Globus Auth
+        if "preferred_username" in self.userinfo:
+            user_name = self.userinfo['preferred_username']
+        else:
+            user_name = self.userinfo['sub']
+        if '@' in user_name:
+            short_name = "{name}_{org}".format(name=user_name.split(
+                "@")[0], org=user_name.split("@")[1].split(".")[0])
+        else:
+            short_name = user_name
+        metadata['dlhub']['owner'] = short_name
+        metadata['dlhub']['publication_date'] = int(round(time() * 1000))
+        metadata['dlhub']['user_id'] = self.userinfo['sub']
+
+        # Make name from repository ID
+        model_name = metadata['dlhub']['name']
+        shorthand_name = "{name}/{model}".format(name=short_name, model=model_name.replace(" ", "_"))
+        metadata['dlhub']['shorthand_name'] = shorthand_name
+
+        servable_uuid = str(uuid.uuid4())
+        metadata['dlhub']['id'] = servable_uuid
+
+    def _ingest(self, metadata):
+        """Ingest the model: build container using container service, and ingest metadata into search index.
+
+        Args:
+            Metadata: dict
+                The metadata of the model to build/ingest.
+        Returns:
+            dict: The metadata of the ingested model
+        """
+
+        logger.debug("Starting ingest")
+        if 'dlhub' not in metadata:
+            metadata['dlhub'] = {}
+        if 'test' not in metadata['dlhub']:
+            metadata['dlhub']['test'] = False
+
+        fxc = self._fx_client
+
+        container_spec = create_container_spec(metadata)
+
+        try:
+            container_uuid = fxc.build_container(container_spec)
+        except Exception as e:
+            help_err = HelpMessage(f"Container build failed with exception: {e}")
+            raise help_err from e
+
+        # Putting container_uuid in metadata instead of task_id, as we don't
+        # have a task to monitor, just a container
+        metadata['container_id'] = container_uuid
+
+        # check_container_build_status will block until container builds,
+        # or build fails, or timeout after 30 minutes (same timeout as the
+        # build itself)
+        status = check_container_build_status(fxc, container_uuid)
+
+        if status == "failed":
+            raise Exception("ContainerService build failed")
+        # print(f"Container uuid: {container_uuid} status: {status}")
+        # print(fxc.get_container(container_uuid, container_type="docker"))
+
+        funcx_id = register_funcx(metadata, container_uuid, fxc)
+        if 'funcx_token' in metadata['dlhub']:
+            del (metadata['dlhub']['funcx_token'])
+
+        metadata['dlhub']['funcx_id'] = funcx_id
+
+        # Ingest metadata to search
+        # Get header from the search lambda authorizer
+        header = self.sl_authorizer.get_authorization_header()
+        try:
+            search_ingest(metadata, header)
+        except Exception as e:
+            raise Exception("Failed to ingest to search. {}".format(e))
+
+        return metadata
```

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/__init__.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/datacite.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/datacite.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
         family_name, given_name = name.split(",", 1)
         return DataciteCreator(familyName=family_name.strip(), givenName=given_name.strip(),
                                affiliations=affiliations)
 
 
 class DataciteTitle(BaseModel):
-    class DataciteTitleType(Enum):
+    class DataciteTitleType(str, Enum):
         AlternativeTitle = "AlternativeTitle"
         Subtitle = "Subtitle"
         TranslatedTitle = "TranslatedTitle"
         Other = "Other"
 
     title: str = Field(...)
     type: Optional[DataciteTitleType]
@@ -62,15 +62,15 @@
     subject: str = ""
     subjectScheme: Optional[str] = ""
     schemeURI: Optional[AnyUrl] = ""
     valueURI: Optional[AnyUrl] = ""
     lang: str = ""
 
 
-class DataciteResourceTypeGeneral(Enum):
+class DataciteResourceTypeGeneral(str, Enum):
     Audiovisual = "Audiovisual"
     Collection = "Collection"
     Dataset = "Dataset"
     Event = "Event"
     Image = "Image"
     InteractiveResource = "InteractiveResource"
     Model = "Model"
@@ -85,15 +85,15 @@
 
 class DataciteResourceType(BaseModel):
     resourceType: Optional[str] = ""
     resourceTypeGeneral: DataciteResourceTypeGeneral = None
 
 
 class DataciteContributor(BaseModel):
-    class DataciteContributorType(Enum):
+    class DataciteContributorType(str, Enum):
         ContactPerson = "ContactPerson"
         DataCollector = "DataCollector"
         DataCurator = "DataCurator"
         DataManager = "DataManager"
         Editor = "Editor"
         HostingInstitution = "HostingInstitution"
         Other = "Other"
@@ -124,15 +124,15 @@
      This may be any alphanumeric string which is unique within its domain of issue. May be used for local identifiers.
     AlternateIdentifier should be used for another identifier of the same instance (same location, same file)."""
 
     alternateIdentifier: str
     alternateIdentifierType: str
 
 
-class DataciteRelatedIdentifierType(Enum):
+class DataciteRelatedIdentifierType(str, Enum):
     """Types of identifiers for different objects"""
     ARK = "ARK"
     arXiv = "arXiv"
     bibcode = "bibcode"
     DOI = "DOI"
     EAN13 = "EAN13"
     EISSN = "EISSN"
@@ -146,15 +146,15 @@
     PMID = "PMID"
     PURL = "PURL"
     UPC = "UPC"
     URL = "URL"
     URN = "URN"
 
 
-class DataciteRelationType(Enum):
+class DataciteRelationType(str, Enum):
     """Ways another object is related to the object describe by our DataCite record"""
     IsCitedBy = "IsCitedBy"
     Cites = "Cites"
     IsSupplementTo = "IsSupplementTo"
     IsSupplementedBy = "IsSupplementedBy"
     IsContinuedBy = "IsContinuedBy"
     Continues = "Continues"
@@ -189,15 +189,15 @@
 
 
 class DataciteDescription(BaseModel):
     """Additional information that does not fit in any of the other categories.
 
     May be used for technical information. It is a best practice to supply a description."""
 
-    class DataciteDescriptionType(Enum):
+    class DataciteDescriptionType(str, Enum):
         abstract = "Abstract"
         methods = "Methods"
         seriesInformation = "SeriesInformation"
         tableOfContents = "TableOfContents"
         technicalInfo = "TechnicalInfo"
         other = "Other"
 
@@ -216,15 +216,15 @@
 
 class DataciteFundingReference(BaseModel):
     """Information about financial support (funding) for the resource being registered."""
 
     class FunderIdentifier(BaseModel):
         """Uniquely identifies a funding entity, according to various types."""
 
-        class FunderIdentifierType(Enum):
+        class FunderIdentifierType(str, Enum):
             ISNI = "ISNI"
             GRID = "GRID"
             CrossRef = "Crossref Funder ID"
             Other = "Other"
 
         funderIdentifier: str
         funderIdentifierType: FunderIdentifierType
```

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/servables/__init__.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/servables/__init__.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/servables/keras.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/servables/keras.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/servables/python.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/servables/python.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/servables/pytorch.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/servables/pytorch.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/servables/sklearn.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/servables/sklearn.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/models/servables/tensorflow.py` & `dlhub_sdk-2.0.0/dlhub_sdk/models/servables/tensorflow.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/__init__.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/funcx_login_manager.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/funcx_login_manager.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/futures.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/futures.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/inspect.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/inspect.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/schemas.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/search.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/search.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/types.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/types.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk/utils/validation.py` & `dlhub_sdk-2.0.0/dlhub_sdk/utils/validation.py`

 * *Files identical despite different names*

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk.egg-info/PKG-INFO` & `dlhub_sdk-2.0.0/dlhub_sdk.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dlhub-sdk
-Version: 1.1.1
+Version: 2.0.0
 Summary: Python interface and utilities for DLHub
 Home-page: https://github.com/DLHub-Argonne/dlhub_sdk
 Author: Ben Blaiszik
 Author-email: bblaiszik@anl.gov
 License: Apache License, Version 2.0
 Keywords: DLHub,Data and Learning Hub for Science,machine learning,data publication,reproducibility
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `dlhub_sdk-1.1.1/dlhub_sdk.egg-info/SOURCES.txt` & `dlhub_sdk-2.0.0/dlhub_sdk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -20,11 +20,12 @@
 dlhub_sdk/models/servables/sklearn.py
 dlhub_sdk/models/servables/tensorflow.py
 dlhub_sdk/utils/__init__.py
 dlhub_sdk/utils/files.py
 dlhub_sdk/utils/funcx_login_manager.py
 dlhub_sdk/utils/futures.py
 dlhub_sdk/utils/inspect.py
+dlhub_sdk/utils/publish.py
 dlhub_sdk/utils/schemas.py
 dlhub_sdk/utils/search.py
 dlhub_sdk/utils/types.py
 dlhub_sdk/utils/validation.py
```

### Comparing `dlhub_sdk-1.1.1/setup.py` & `dlhub_sdk-2.0.0/setup.py`

 * *Files identical despite different names*

