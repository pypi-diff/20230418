# Comparing `tmp/drb-driver-ftp-1.1.1.tar.gz` & `tmp/drb-driver-ftp-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-ftp-1.1.1.tar", last modified: Mon Dec 19 14:41:18 2022, max compression
+gzip compressed data, was "drb-driver-ftp-1.2.0.tar", last modified: Tue Apr 18 08:23:52 2023, max compression
```

## Comparing `drb-driver-ftp-1.1.1.tar` & `drb-driver-ftp-1.2.0.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.851335 drb-driver-ftp-1.1.1/
--rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-19 10:38:34.000000 drb-driver-ftp-1.1.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2407 2022-12-19 14:41:18.851335 drb-driver-ftp-1.1.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1952 2022-12-19 08:05:07.000000 drb-driver-ftp-1.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.847335 drb-driver-ftp-1.1.1/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.847335 drb-driver-ftp-1.1.1/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.855335 drb-driver-ftp-1.1.1/drb/drivers/ftp/
--rw-rw-rw-   0 root         (0) root         (0)      241 2022-12-19 08:05:07.000000 drb-driver-ftp-1.1.1/drb/drivers/ftp/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-19 14:41:18.855335 drb-driver-ftp-1.1.1/drb/drivers/ftp/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     8002 2022-12-19 13:23:27.000000 drb-driver-ftp-1.1.1/drb/drivers/ftp/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.851335 drb-driver-ftp-1.1.1/drb/exceptions/
--rw-rw-rw-   0 root         (0) root         (0)      184 2022-12-19 13:23:27.000000 drb-driver-ftp-1.1.1/drb/exceptions/ftp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.847335 drb-driver-ftp-1.1.1/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.851335 drb-driver-ftp-1.1.1/drb/topics/ftp/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 08:05:07.000000 drb-driver-ftp-1.1.1/drb/topics/ftp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2022-12-19 08:05:07.000000 drb-driver-ftp-1.1.1/drb/topics/ftp/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-19 14:41:18.851335 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2407 2022-12-19 14:41:18.000000 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      455 2022-12-19 14:41:18.000000 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-19 14:41:18.000000 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       84 2022-12-19 14:41:18.000000 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       11 2022-12-19 14:41:18.000000 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-19 14:41:18.000000 drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       11 2022-12-19 08:05:07.000000 drb-driver-ftp-1.1.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      208 2022-12-19 14:41:18.855335 drb-driver-ftp-1.1.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1181 2022-12-19 08:05:07.000000 drb-driver-ftp-1.1.1/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    80044 2022-09-28 15:53:34.000000 drb-driver-ftp-1.1.1/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.105058 drb-driver-ftp-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 14:03:09.000000 drb-driver-ftp-1.2.0/LICENCE.txt
+-rw-rw-rw-   0 root         (0) root         (0)       58 2022-12-19 10:38:34.000000 drb-driver-ftp-1.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-18 08:23:52.105058 drb-driver-ftp-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1952 2022-12-19 08:05:07.000000 drb-driver-ftp-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.041057 drb-driver-ftp-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.041057 drb-driver-ftp-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.109058 drb-driver-ftp-1.2.0/drb/drivers/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)      185 2023-04-04 20:51:12.000000 drb-driver-ftp-1.2.0/drb/drivers/ftp/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-18 08:23:52.109058 drb-driver-ftp-1.2.0/drb/drivers/ftp/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     7460 2023-04-14 09:26:40.000000 drb-driver-ftp-1.2.0/drb/drivers/ftp/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.077058 drb-driver-ftp-1.2.0/drb/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2022-12-19 13:23:27.000000 drb-driver-ftp-1.2.0/drb/exceptions/ftp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.045057 drb-driver-ftp-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.085058 drb-driver-ftp-1.2.0/drb/topics/ftp/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-19 08:05:07.000000 drb-driver-ftp-1.2.0/drb/topics/ftp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-18 08:23:02.000000 drb-driver-ftp-1.2.0/drb/topics/ftp/cortex.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.089058 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-04-18 08:23:52.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      583 2023-04-18 08:23:52.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:23:52.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-18 08:23:52.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:23:51.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-18 08:23:52.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 08:23:52.000000 drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-04 15:02:49.000000 drb-driver-ftp-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       11 2023-04-04 15:02:49.000000 drb-driver-ftp-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2023-04-18 08:23:52.109058 drb-driver-ftp-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-04 15:02:49.000000 drb-driver-ftp-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:23:52.093058 drb-driver-ftp-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      525 2023-04-04 20:51:12.000000 drb-driver-ftp-1.2.0/tests/test_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2913 2023-04-14 08:34:11.000000 drb-driver-ftp-1.2.0/tests/test_ftp.py
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-04-04 15:02:49.000000 drb-driver-ftp-1.2.0/tests/test_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)    80044 2022-09-28 15:53:34.000000 drb-driver-ftp-1.2.0/versioneer.py
```

### Comparing `drb-driver-ftp-1.1.1/PKG-INFO` & `drb-driver-ftp-1.2.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-ftp
-Version: 1.1.1
-Summary: DRB Ftp implementation
-Home-page: https://gitlab.com/drb-python/impl/ftp
+Version: 1.2.0
+Summary: DRB Ftp driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/ftp
+Project-URL: Source, https://gitlab.com/drb-python/impl/ftp
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Ftp driver
 This drb-driver-ftp module implements ftp protocol access with DRB data model.
 
 ## Ftp Factory and Ftp Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -57,8 +58,7 @@
 ## Limitations
 
 None
 
 ## Documentation
 
 The documentation of this driver can be found here https://drb-python.gitlab.io/impl/ftp
-
```

### Comparing `drb-driver-ftp-1.1.1/README.md` & `drb-driver-ftp-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-ftp-1.1.1/drb/drivers/ftp/ftp.py` & `drb-driver-ftp-1.2.0/drb/drivers/ftp/ftp.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,21 @@
+import ftplib
 import io
-import enum
-import os
+from urllib.parse import urljoin
 import ssl
 from urllib.parse import urlparse
 from ftplib import FTP, error_perm, FTP_TLS
-from typing import Any, List, Dict, Optional, Tuple
+from typing import Any, List
 
+import keyring
+from deprecated.classic import deprecated
 from drb.core import DrbNode, ParsedPath, DrbFactory
-from drb.exceptions.core import DrbException, DrbNotImplementationException
+from drb.exceptions.core import DrbNotImplementationException
 from drb.nodes.abstract_node import AbstractNode
+from keyring.errors import NoKeyringError
 
 from requests.auth import HTTPBasicAuth
 
 from drb.exceptions.ftp import DrbFtpNodeException
 
 
 def check_args(*args):
@@ -96,146 +99,122 @@
                 cls.ftp = FTP(host)
                 cls.ftp.connect(tmp[0], int(tmp[1]))
             if auth is not None:
                 cls.ftp.login(auth.username, auth.password)
         return cls.ftp
 
 
-class DrbFtpAttributeNames(enum.Enum):
-    """
-    This Enum class provide us the different
-    attribute of a file.
-    """
-    DIRECTORY = 'directory'
-    SIZE = 'size'
-    MODIFIED = 'modified'
-
-
 class DrbFtpNode(AbstractNode):
     ftp = None
+    __attributes = [
+        'directory', 'size', 'modified']
 
     def __init__(self, path, host: str = '',
                  parent: DrbNode = None,
                  auth: HTTPBasicAuth = None, protocol=None):
         super().__init__()
         self._original_path = path
-        self._path = path
+        self.name = urlparse(self._original_path).path.split('/')[-1]
         self._host = host
-        self._parent: DrbNode = parent
+        self.parent = parent
         self._protocol = protocol
+        self._available_impl.append(io.BytesIO)
         if parent:
             self.ftp = parent.ftp
-        self._attributes: Dict[Tuple[str, str], Any] = None
         self._children: List[DrbNode] = None
         self._auth = auth
+        self._init_attr()
+
+    def _init_attr(self):
+        try:
+            self @= (self.__attributes[0], not self.is_file(self.path.path))
+
+            if self.is_file(self.path.path):
+                self.ftp.voidcmd('TYPE I')
+                self @= (self.__attributes[1],
+                         self.ftp.size(self.path.path))
+            else:
+                self @= (self.__attributes[1], 0)
+
+            self @= (self.__attributes[2],
+                     self.get_modification_date(self.path.path))
+        except (ftplib.Error, AttributeError) as e:
+            raise DrbFtpNodeException(
+                f'Error occurred when retrieving attributes: {e}')
+
+    def __setitem__(self, key, value):
+        raise NotImplementedError
+
+    def __delitem__(self, key):
+        raise NotImplementedError
+
+    @property
+    def auth(self) -> HTTPBasicAuth:
+        if self._auth is None:
+            credential = keyring.get_credential(
+                self.path.path
+            )
+            if credential is not None:
+                self._auth = HTTPBasicAuth(
+                    credential.username,
+                    credential.password
+                )
+        return self._auth
+
+    @property
+    def path(self) -> ParsedPath:
+        return ParsedPath(self._original_path)
 
     def is_file(self, filename):
         """
         Check if the file given in argument is not a folder.
         :param filename: str
         :return: True if the filename given in argument is a file
         False otherwise
         """
-        self.ftp = FtpConnection(self._auth, self._original_path, self._host)
+        self.ftp = FtpConnection(self.auth, self._original_path, self._host)
         current = self.ftp.pwd()
         try:
             self.ftp.cwd(filename)
         except error_perm:
             self.ftp.cwd(current)
             return True
         self.ftp.cwd(current)
         return False
 
     def check_file_exist(self, filename):
-        self.ftp = FtpConnection(self._auth, self._original_path, self._host)
+        self.ftp = FtpConnection(self.auth, self._original_path, self._host)
         return filename in self.ftp.nlst()
 
     def get_modification_date(self, file_name):
-        self.ftp = FtpConnection(self._auth, self._original_path, self._host)
+        self.ftp = FtpConnection(self.auth, self._original_path, self._host)
         line = []
         self.ftp.dir(file_name, line.append)
         tokens = line[0].split(maxsplit=9)
         return tokens[5] + " " + tokens[6] + " " + tokens[7]
 
     @property
-    def name(self) -> str:
-        parsed_uri = urlparse(self._path)
-        return parsed_uri.path.split('/')[-1]
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return None
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
-
-    @property
-    def path(self) -> ParsedPath:
-        return ParsedPath(self._path)
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        if self._attributes is None:
-            self._attributes = {}
-            name = DrbFtpAttributeNames.DIRECTORY.value
-            self._attributes[(name, None)] = not self.is_file(self.path.path)
-
-            name = DrbFtpAttributeNames.SIZE.value
-            if self.is_file(self.path.path):
-                self.ftp.voidcmd('TYPE I')
-                self._attributes[(name, None)] = self.ftp.size(self.path.path)
-            else:
-                self._attributes[(name, None)] = None
-
-            name = DrbFtpAttributeNames.MODIFIED.value
-            self._attributes[(name, None)] = \
-                self.get_modification_date(self.path.path)
-
-        return self._attributes
-
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        key = (name, namespace_uri)
-        if key in self.attributes.keys():
-            return self.attributes[key]
-        raise DrbException(f'Attribute not found name: {name}, '
-                           f'namespace: {namespace_uri}')
-
-    @property
+    @deprecated(version='1.2.0',
+                reason='Usage of the bracket is recommended')
     def children(self) -> List[DrbNode]:
-        self.ftp = FtpConnection(self._auth, self._original_path, self._host)
+        self.ftp = FtpConnection(self.auth, self._original_path, self._host)
         if self._children is None:
             self._children = []
             if not self.is_file(self.path.path):
                 sorted_child_names = sorted(self.ftp.nlst(self.path.path))
                 for filename in sorted_child_names:
-                    child = DrbFtpNode(os.path.join(
-                        self._original_path, filename),
+                    child = DrbFtpNode(
+                        urljoin(self._original_path + "/", filename),
                         parent=self,
-                        auth=self._auth)
+                        auth=self.auth)
                     self._children.append(child)
         return self._children
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace is None:
-            if name is None:
-                return len(self.children) > 0
-            return name in list(map(lambda x: x.name, self.children))
-
-        return False
-
-    def has_impl(self, impl: type) -> bool:
-        return issubclass(io.BytesIO, impl)
-
     def get_impl(self, impl: type, **kwargs) -> Any:
-        self.ftp = FtpConnection(self._auth, self._original_path, self._host)
+        self.ftp = FtpConnection(self.auth, self._original_path, self._host)
         if self.has_impl(impl):
             return Download(self.path.path, kwargs.get('chunk_size', 12000),
                             self.ftp)
         raise DrbNotImplementationException(
             f'no {impl} implementation found')
 
     def close(self) -> None:
```

### Comparing `drb-driver-ftp-1.1.1/drb_driver_ftp.egg-info/PKG-INFO` & `drb-driver-ftp-1.2.0/drb_driver_ftp.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-ftp
-Version: 1.1.1
-Summary: DRB Ftp implementation
-Home-page: https://gitlab.com/drb-python/impl/ftp
+Version: 1.2.0
+Summary: DRB Ftp driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Platform: UNKNOWN
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/ftp
+Project-URL: Source, https://gitlab.com/drb-python/impl/ftp
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # Ftp driver
 This drb-driver-ftp module implements ftp protocol access with DRB data model.
 
 ## Ftp Factory and Ftp Node
 The module implements the factory model defined in DRB in its node resolver. Based on the python entry point mechanism, this module can be dynamically imported into applications.
 
@@ -57,8 +58,7 @@
 ## Limitations
 
 None
 
 ## Documentation
 
 The documentation of this driver can be found here https://drb-python.gitlab.io/impl/ftp
-
```

### Comparing `drb-driver-ftp-1.1.1/versioneer.py` & `drb-driver-ftp-1.2.0/versioneer.py`

 * *Files identical despite different names*

