# Comparing `tmp/drb-driver-s3-1.1.0.tar.gz` & `tmp/drb-driver-s3-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-s3-1.1.0.tar", last modified: Wed Dec 28 09:45:46 2022, max compression
+gzip compressed data, was "drb-driver-s3-1.2.0.tar", last modified: Tue Apr 18 13:12:27 2023, max compression
```

## Comparing `drb-driver-s3-1.1.0.tar` & `drb-driver-s3-1.2.0.tar`

### file list

```diff
@@ -1,25 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.644251 drb-driver-s3-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-28 09:14:39.000000 drb-driver-s3-1.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2346 2022-12-28 09:45:46.644251 drb-driver-s3-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1761 2022-12-28 09:14:39.000000 drb-driver-s3-1.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.628251 drb-driver-s3-1.1.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.628251 drb-driver-s3-1.1.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.644251 drb-driver-s3-1.1.0/drb/drivers/aws3/
--rw-rw-rw-   0 root         (0) root         (0)      290 2022-12-27 17:52:39.000000 drb-driver-s3-1.1.0/drb/drivers/aws3/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-28 09:45:46.644251 drb-driver-s3-1.1.0/drb/drivers/aws3/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    17386 2022-12-28 09:14:39.000000 drb-driver-s3-1.1.0/drb/drivers/aws3/aws3.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.628251 drb-driver-s3-1.1.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.640251 drb-driver-s3-1.1.0/drb/topics/aws3/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 18:52:20.000000 drb-driver-s3-1.1.0/drb/topics/aws3/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      184 2022-12-28 09:14:39.000000 drb-driver-s3-1.1.0/drb/topics/aws3/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-28 09:45:46.644251 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2346 2022-12-28 09:45:46.000000 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2022-12-28 09:45:46.000000 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-28 09:45:46.000000 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2022-12-28 09:45:46.000000 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       79 2022-12-28 09:45:46.000000 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-28 09:45:46.000000 drb-driver-s3-1.1.0/drb_driver_s3.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       79 2022-12-28 09:14:39.000000 drb-driver-s3-1.1.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-28 09:45:46.644251 drb-driver-s3-1.1.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1300 2022-12-28 09:14:39.000000 drb-driver-s3-1.1.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-20 18:52:20.000000 drb-driver-s3-1.1.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.053690 drb-driver-s3-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-18 14:31:00.000000 drb-driver-s3-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       59 2022-12-28 09:14:39.000000 drb-driver-s3-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-18 13:12:27.053690 drb-driver-s3-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2022-12-28 09:14:39.000000 drb-driver-s3-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.025690 drb-driver-s3-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.025690 drb-driver-s3-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.057690 drb-driver-s3-1.2.0/drb/drivers/aws3/
+-rw-rw-rw-   0 root         (0) root         (0)      290 2022-12-27 17:52:39.000000 drb-driver-s3-1.2.0/drb/drivers/aws3/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-18 13:12:27.057690 drb-driver-s3-1.2.0/drb/drivers/aws3/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    15310 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/drb/drivers/aws3/aws3.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.025690 drb-driver-s3-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.045690 drb-driver-s3-1.2.0/drb/topics/aws3/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-20 18:52:20.000000 drb-driver-s3-1.2.0/drb/topics/aws3/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-04-18 13:11:28.000000 drb-driver-s3-1.2.0/drb/topics/aws3/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.045690 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-18 13:12:27.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      606 2023-04-18 13:12:27.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:12:27.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       87 2023-04-18 13:12:27.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 13:12:26.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       79 2023-04-18 13:12:27.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 13:12:27.000000 drb-driver-s3-1.2.0/drb_driver_s3.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       79 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1087 2023-04-18 13:12:27.053690 drb-driver-s3-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 13:12:27.053690 drb-driver-s3-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     3213 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/tests/test_bucket.py
+-rw-rw-rw-   0 root         (0) root         (0)      887 2022-12-28 09:14:39.000000 drb-driver-s3-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3719 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/tests/test_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1858 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/tests/test_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1624 2023-04-18 09:10:08.000000 drb-driver-s3-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    83021 2022-12-20 18:52:20.000000 drb-driver-s3-1.2.0/versioneer.py
```

### Comparing `drb-driver-s3-1.1.0/PKG-INFO` & `drb-driver-s3-1.2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-s3
-Version: 1.1.0
-Summary: DRB aws3 implementation
-Home-page: https://gitlab.com/drb-python/impl/aws3
+Version: 1.2.0
+Summary: DRB aws3 driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/aws3/
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/aws3
 Project-URL: Source, https://gitlab.com/drb-python/impl/aws3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Amazon simple storage service driver
 
 This drb-driver-s3 module implements S3 protocol access with DRB data model.
 
 ## S3 Factory and S3 Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
@@ -59,8 +58,7 @@
 This driver doesn't allow to write, modify, delete file on a s3 bucket,
 or it doesn't allow to delete or upload a file.
 This driver doesn't allow to download directly a bucket.
 
 ## Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/aws3
-
```

### Comparing `drb-driver-s3-1.1.0/README.md` & `drb-driver-s3-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-s3-1.1.0/drb/drivers/aws3/aws3.py` & `drb-driver-s3-1.2.0/drb/drivers/aws3/aws3.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
-import os
 from abc import ABC
-from typing import Optional, Any, List, Dict, Tuple
+from typing import Any, List
 
 import boto3
 from botocore.client import BaseClient
-from drb.core import DrbNode, ParsedPath, DrbFactory
+from deprecated.classic import deprecated
+from drb.core import DrbNode, DrbFactory
 from drb.drivers.http import DrbHttpNode
 from drb.exceptions.core import DrbException
 from drb.nodes.abstract_node import AbstractNode
 from requests.auth import HTTPBasicAuth
 
 
 class Auth:
@@ -216,15 +216,14 @@
         if self.__res is None or self._iter is None:
             if self._iter is not None:
                 self._iter.close()
                 self._iter = None
             self._buff = bytearray(0)
 
             if self._headers is not None:
-                print(heads)
                 pos_start = pos_start + self._headers[0]
                 if len(self._headers) > 1:
                     end = pos_start + self._headers[1]
                     heads = {
                         "range":
                             f"bytes={pos_start}"
                             f"-{end}"
@@ -311,83 +310,63 @@
     """
 
     def __init__(self, auth: Auth):
         super(DrbS3Node, self).__init__()
         self._auth = auth
         self._conn = None
 
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
     def close(self) -> None:
         """
         Close The s3 connection
         """
         if self._conn is not None:
             self._conn.close()
 
     def get_auth(self) -> Auth:
         """
         Return the Auth object created to access the service.
         """
         return self._auth
 
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
     def __eq__(self, other):
         return isinstance(other, DrbS3Node) and \
             self._auth == other._auth
 
     def __hash__(self):
-        return hash(self.auth)
+        return hash(self._auth)
 
 
 class DrbS3Object(DrbS3Node):
     def __init__(self, obj, parent: DrbS3Node):
         super().__init__(auth=parent.get_auth())
         self.req = Requests(parent.get_auth())
         self._obj = obj
-        self._name = obj.key
-        self._path = os.path.join(parent.path.original_path, self._name)
-        self._attributes = obj.get_available_subresources()
-        self._children = None
-        self._parent = parent
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None:
-            if name in self.attributes:
-                return self._obj.name
-        raise DrbException(f'No attribute found: ({name}, {namespace_uri})')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(self._path)
+        self.name = obj.key
+        self.parent = parent
+        self._available_impl.append(io.BytesIO)
+        self._init_attrs()
+
+    def _init_attrs(self):
+        for e in self._obj.get_available_subresources():
+            name = e
+            value = self._obj.name
+            self @= (name, value)
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
         return []
 
-    def has_impl(self, impl: type) -> bool:
-        return issubclass(io.BytesIO, impl)
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         """
         These class allow the download of object in a bucket.
 
         Parameters:
             impl (type): The type supported by this implementation,
                          here only subclass of io.BytesIO are supported.
@@ -407,129 +386,76 @@
                 return Download(self.req.get_obj(
                     self.parent.name,
                     self.name), kwargs.get('chunk_size', 4 * 1048576),
                     headers=headers)
         raise DrbException(
             f"SwiftService doesn't support {impl} implementation")
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        return False
-
 
 class DrbS3Bucket(DrbS3Node):
 
     def __init__(self, obj, parent: DrbS3Node):
         super().__init__(auth=parent.get_auth())
         self.req = Requests(parent.get_auth())
         self._bucket = obj
-        self._name = obj.name
-        self._path = os.path.join(parent.path.path, self._name)
-        self._attributes = obj.get_available_subresources()
+        self.name = obj.name
         self._children = None
-        self._parent = parent
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        if namespace_uri is None:
-            if name in self.attributes:
-                return self._bucket.name
-        raise DrbException(f'No attribute found: ({name}, {namespace_uri})')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(self._path)
+        self.parent = parent
+        self._available_impl = []
+        self._init_attrs()
+
+    def _init_attrs(self):
+        for e in self._bucket.get_available_subresources():
+            name = e
+            value = self._bucket.name
+            self @= (name, value)
 
     @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
         self._conn = Connection(self._auth)
         if self._children is None:
             objects = self.req.list_objects(self.name)
             self._children = [
                 DrbS3Object(obj, self)
                 for obj in objects
             ]
         return self._children
 
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbException(
             f"SwiftService doesn't support {impl} implementation")
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace is None:
-            if name is not None:
-                return name in [x.name for x in self.children]
-            return len(self.children) > 0
-        return False
-
 
 class DrbS3Service(DrbS3Node):
     def __init__(self, auth: Auth):
         super().__init__(auth=auth)
         self.req = Requests(auth)
-        self._attributes = {}
         self._children = None
+        self.name = self._auth.service_name
+        self._available_impl = []
 
     @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        raise DrbException(f'No attribute found: ({name}, {namespace_uri})')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return None
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(os.path.sep)
-
-    @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
         self._conn = Connection(self._auth)
         if self._children is None:
             buckets = self.req.list_buckets()
             self._children = [
                 DrbS3Bucket(bucket, self)
                 for bucket in buckets
             ]
         return self._children
 
-    @property
-    def name(self) -> str:
-        return self._auth.service_name
-
-    def has_impl(self, impl: type) -> bool:
-        return False
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         raise DrbException(
             f"SwiftService doesn't support {impl} implementation")
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace is None:
-            if name is not None:
-                return name in [x.name for x in self.children]
-            return len(self.children) > 0
-        return False
-
 
 class S3NodeFactory(DrbFactory):
 
     def _create(self, node: DrbNode) -> DrbNode:
         if isinstance(node, DrbS3Node):
             return node
         if isinstance(node, DrbHttpNode):
```

### Comparing `drb-driver-s3-1.1.0/drb_driver_s3.egg-info/PKG-INFO` & `drb-driver-s3-1.2.0/drb_driver_s3.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-s3
-Version: 1.1.0
-Summary: DRB aws3 implementation
-Home-page: https://gitlab.com/drb-python/impl/aws3
+Version: 1.2.0
+Summary: DRB aws3 driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/aws3/
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/aws3
 Project-URL: Source, https://gitlab.com/drb-python/impl/aws3
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Amazon simple storage service driver
 
 This drb-driver-s3 module implements S3 protocol access with DRB data model.
 
 ## S3 Factory and S3 Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
@@ -59,8 +58,7 @@
 This driver doesn't allow to write, modify, delete file on a s3 bucket,
 or it doesn't allow to delete or upload a file.
 This driver doesn't allow to download directly a bucket.
 
 ## Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/aws3
-
```

### Comparing `drb-driver-s3-1.1.0/versioneer.py` & `drb-driver-s3-1.2.0/versioneer.py`

 * *Files identical despite different names*

