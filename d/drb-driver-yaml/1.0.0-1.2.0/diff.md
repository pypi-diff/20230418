# Comparing `tmp/drb-driver-yaml-1.0.0.tar.gz` & `tmp/drb-driver-yaml-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drb-driver-yaml-1.0.0.tar", last modified: Fri Dec 16 14:05:14 2022, max compression
+gzip compressed data, was "drb-driver-yaml-1.2.0.tar", last modified: Tue Apr 18 08:26:34 2023, max compression
```

## Comparing `drb-driver-yaml-1.0.0.tar` & `drb-driver-yaml-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.264845 drb-driver-yaml-1.0.0/
--rw-r--r--   0 root         (0) root         (0)     2366 2022-12-16 14:05:14.264845 drb-driver-yaml-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1780 2022-12-15 20:33:07.000000 drb-driver-yaml-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.260845 drb-driver-yaml-1.0.0/drb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.260845 drb-driver-yaml-1.0.0/drb/drivers/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.268845 drb-driver-yaml-1.0.0/drb/drivers/yaml/
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-12-15 20:33:07.000000 drb-driver-yaml-1.0.0/drb/drivers/yaml/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2022-12-16 14:05:14.268845 drb-driver-yaml-1.0.0/drb/drivers/yaml/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     7298 2022-12-15 20:55:09.000000 drb-driver-yaml-1.0.0/drb/drivers/yaml/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.260845 drb-driver-yaml-1.0.0/drb/topics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.260845 drb-driver-yaml-1.0.0/drb/topics/yaml/
--rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 20:33:07.000000 drb-driver-yaml-1.0.0/drb/topics/yaml/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      219 2022-12-15 20:33:07.000000 drb-driver-yaml-1.0.0/drb/topics/yaml/cortex.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-16 14:05:14.264845 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2366 2022-12-16 14:05:14.000000 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      433 2022-12-16 14:05:14.000000 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-16 14:05:14.000000 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       90 2022-12-16 14:05:14.000000 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       18 2022-12-16 14:05:14.000000 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2022-12-16 14:05:14.000000 drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       17 2022-12-16 12:32:13.000000 drb-driver-yaml-1.0.0/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)      210 2022-12-16 14:05:14.264845 drb-driver-yaml-1.0.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1302 2022-12-15 20:33:07.000000 drb-driver-yaml-1.0.0/setup.py
--rw-rw-rw-   0 root         (0) root         (0)    83607 2022-12-15 20:33:07.000000 drb-driver-yaml-1.0.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.887769 drb-driver-yaml-1.2.0/
+-rw-rw-rw-   0 root         (0) root         (0)     7651 2023-01-19 13:36:02.000000 drb-driver-yaml-1.2.0/LICENCE.txt
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-04-18 08:26:34.887769 drb-driver-yaml-1.2.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2022-12-15 20:33:07.000000 drb-driver-yaml-1.2.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.843768 drb-driver-yaml-1.2.0/drb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.843768 drb-driver-yaml-1.2.0/drb/drivers/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.891769 drb-driver-yaml-1.2.0/drb/drivers/yaml/
+-rw-rw-rw-   0 root         (0) root         (0)      219 2022-12-15 20:33:07.000000 drb-driver-yaml-1.2.0/drb/drivers/yaml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-04-18 08:26:34.891769 drb-driver-yaml-1.2.0/drb/drivers/yaml/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     6487 2023-04-14 07:57:10.000000 drb-driver-yaml-1.2.0/drb/drivers/yaml/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.843768 drb-driver-yaml-1.2.0/drb/topics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.879768 drb-driver-yaml-1.2.0/drb/topics/yaml/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2022-12-15 20:33:07.000000 drb-driver-yaml-1.2.0/drb/topics/yaml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.883769 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2322 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      599 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       89 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       18 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-04-18 08:26:34.000000 drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      104 2023-04-05 06:57:16.000000 drb-driver-yaml-1.2.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       17 2023-04-05 06:57:16.000000 drb-driver-yaml-1.2.0/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1092 2023-04-18 08:26:34.891769 drb-driver-yaml-1.2.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      134 2023-04-05 06:57:16.000000 drb-driver-yaml-1.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 08:26:34.887769 drb-driver-yaml-1.2.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     2379 2023-04-05 06:57:17.000000 drb-driver-yaml-1.2.0/tests/test_base_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1325 2023-04-05 06:57:17.000000 drb-driver-yaml-1.2.0/tests/test_yaml_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)     4248 2023-04-14 07:57:55.000000 drb-driver-yaml-1.2.0/tests/test_yaml_node.py
+-rw-rw-rw-   0 root         (0) root         (0)     1447 2023-04-05 06:57:17.000000 drb-driver-yaml-1.2.0/tests/test_yaml_signature.py
+-rw-rw-rw-   0 root         (0) root         (0)      600 2022-12-15 20:33:07.000000 drb-driver-yaml-1.2.0/tests/test_yaml_user.py
+-rw-rw-rw-   0 root         (0) root         (0)    83607 2022-12-15 20:33:07.000000 drb-driver-yaml-1.2.0/versioneer.py
```

### Comparing `drb-driver-yaml-1.0.0/PKG-INFO` & `drb-driver-yaml-1.2.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-yaml
-Version: 1.0.0
-Summary: DRB Yaml implementation
-Home-page: https://gitlab.com/drb-python/impl/yaml
+Version: 1.2.0
+Summary: DRB yaml driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/yaml
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/yaml
 Project-URL: Source, https://gitlab.com/drb-python/impl/yaml
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # YamlNode Implementation
 
 This `drb-driver-yaml` module implements yaml format access with DRB data
 model. It is able to navigates among the yaml contents.
 
 ## Yaml Factory and Yaml Node
@@ -71,8 +70,7 @@
 FILE_NODE = DrbFileNode(PATH_TO_YOUR_YAML)
 NODE = FACTORY.create(FILE_NODE)
 ```
 
 ### Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/yaml
-
```

### Comparing `drb-driver-yaml-1.0.0/README.md` & `drb-driver-yaml-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `drb-driver-yaml-1.0.0/drb/drivers/yaml/yaml.py` & `drb-driver-yaml-1.2.0/drb/drivers/yaml/yaml.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,143 +1,103 @@
-import os
-
+from pathlib import Path
 import yaml
+from deprecated.classic import deprecated
 from drb.core import DrbFactory, DrbNode, ParsedPath
 
 from io import BufferedIOBase, BytesIO, RawIOBase
 from typing import Union, Optional, Any, Dict, Tuple, IO, List
 
-from drb.exceptions.core import DrbNotImplementationException, DrbException
+from drb.exceptions.core import DrbNotImplementationException
 from drb.nodes.abstract_node import AbstractNode
 
 
 class YamlNode(AbstractNode):
     """
     This class represents a single node of a tree
     of data. When a node has one or several children he has no value.
 
     Parameters:
             path (str): The path to the yaml file.
             parent (DrbNode): The parent of this node (default: None).
             data : The yaml data (default: None).
     """
 
-    supported_impl = [dict, str]
-
     def __init__(self, path: str,
                  parent: DrbNode = None, data=None):
         super().__init__()
         if data is not None:
             self._data = data
-            self._name = os.path.basename(path)
-            self._path = ParsedPath(path)
         else:
             with open(path) as yamlFile:
                 data = list(yaml.safe_load_all(yamlFile))
                 if len(data) == 1:
                     self._data = data[0]
                 else:
                     self._data = data
                 yamlFile.close()
-            self._name = os.path.basename(path)
-            self._path = ParsedPath(path)
-
-        self._parent = parent
+        self._path = ParsedPath(path)
+        self._available_impl += [dict, str]
+        self.name = Path(path).name
+        self.value = self._data
+        self.parent = parent
         self._children = None
 
-    @property
-    def name(self) -> str:
-        return self._name
-
-    @property
-    def namespace_uri(self) -> Optional[str]:
-        return None
-
-    @property
-    def value(self) -> Optional[Any]:
-        return self._data
-
-    @property
-    def attributes(self) -> Dict[Tuple[str, str], Any]:
-        return {}
+    def __setitem__(self, key, value):
+        raise NotImplementedError
 
-    def get_attribute(self, name: str, namespace_uri: str = None) -> Any:
-        raise DrbException(f'No attribute ({name}:{namespace_uri}) found!')
-
-    @property
-    def parent(self) -> Optional[DrbNode]:
-        return self._parent
+    def __delitem__(self, key):
+        raise NotImplementedError
 
     @property
     def path(self) -> ParsedPath:
         return self._path
 
-    def has_impl(self, impl: type) -> bool:
-        return impl in self.supported_impl
-
     def get_impl(self, impl: type, **kwargs) -> Any:
         if self.has_impl(impl):
             if impl == dict:
                 return self._data
-            else:
+            elif impl == str:
                 return yaml.dump(self._data)
+            else:
+                return BytesIO(bytes(yaml.dump(self._data), 'utf-8'))
 
         raise DrbNotImplementationException(
             f"YamlNode doesn't implement {impl}")
 
-    def has_child(self, name: str = None, namespace: str = None) -> bool:
-        if namespace:
-            return False
-        if name:
-            if isinstance(self._data, dict):
-                for e in self._data.keys():
-                    if e == name:
-                        return True
-                    return False
-            if isinstance(self._data, list):
-                for e in self._data:
-                    if e == name:
-                        return True
-                    return False
-        return isinstance(self._data, dict) or isinstance(self._data, list)
-
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def children(self) -> List[DrbNode]:
         if self._children is None:
             self._children = []
-            if self.has_child():
-                if isinstance(self._data, list):
-                    self._children = [
-                        YamlNode(path=self.path.path,
-                                 parent=self,
-                                 data=e)
-                        for e in self._data]
-                else:
-                    for e in self._data.keys():
-                        if isinstance(self._data[e], list):
-                            for x in self._data[e]:
-                                self._children.append(
-                                    YamlNode(path=os.path.join(
-                                        self.path.path, e),
-                                        parent=self,
-                                        data=x)
-                                )
-                        else:
+            if isinstance(self._data, list):
+                self._children = [
+                    YamlNode(path=self.path.path,
+                             parent=self,
+                             data=e)
+                    for e in self._data]
+            elif isinstance(self._data, dict):
+                for e in self._data.keys():
+                    if isinstance(self._data[e], list):
+                        for x in self._data[e]:
                             self._children.append(
-                                YamlNode(path=os.path.join(self.path.path, e),
-                                         parent=self,
-                                         data=self._data[e])
+                                YamlNode(
+                                    path=Path(self.path.path).
+                                    joinpath(e).as_posix(),
+                                    parent=self,
+                                    data=x)
                             )
-            else:
-                self._children = []
+                    elif isinstance(self._data, dict):
+                        self._children.append(
+                            YamlNode(path=Path(self.path.path).
+                                     joinpath(e).as_posix(),
+                                     parent=self,
+                                     data=self._data[e])
+                        )
         return self._children
 
-    def close(self) -> None:
-        pass
-
 
 class YamlBaseNode(AbstractNode):
     """
         This class represents a single node of a tree
         of data. When the data came from another implementation.
 
         Parameters:
@@ -171,28 +131,31 @@
         return self.base_node.path
 
     @property
     def parent(self) -> Optional[DrbNode]:
         return self.base_node.parent
 
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def attributes(self) -> Dict[Tuple[str, str], Any]:
         return self.base_node.attributes
 
     @property
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def children(self) -> List[DrbNode]:
         return [self.yaml_node]
 
     def has_child(self, name: str = None, namespace: str = None) -> bool:
         if name and self.yaml_node.name == name:
             return True
         elif namespace:
             return False
         return True
 
+    @deprecated(version="1.2.0", reason="drb core deprecation since 2.1.0")
     def get_attribute(self, name: str) -> Any:
         return self.base_node.get_attribute(name)
 
     def has_impl(self, impl: type) -> bool:
         return self.base_node.has_impl(impl)
 
     def get_impl(self, impl: type, **kwargs) -> Any:
```

### Comparing `drb-driver-yaml-1.0.0/drb_driver_yaml.egg-info/PKG-INFO` & `drb-driver-yaml-1.2.0/drb_driver_yaml.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: drb-driver-yaml
-Version: 1.0.0
-Summary: DRB Yaml implementation
-Home-page: https://gitlab.com/drb-python/impl/yaml
+Version: 1.2.0
+Summary: DRB yaml driver
 Author: GAEL Systems
 Author-email: drb-python@gael.fr
-License: UNKNOWN
-Project-URL: Documentation, https://drb-python.gitlab.io/impl/yaml
+License: LGPLv3
+Project-URL: Documentation, http://drb-python.gitlab.io/impl/yaml
 Project-URL: Source, https://gitlab.com/drb-python/impl/yaml
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
+Classifier: Environment :: Plugins
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+License-File: LICENCE.txt
 
 # YamlNode Implementation
 
 This `drb-driver-yaml` module implements yaml format access with DRB data
 model. It is able to navigates among the yaml contents.
 
 ## Yaml Factory and Yaml Node
@@ -71,8 +70,7 @@
 FILE_NODE = DrbFileNode(PATH_TO_YOUR_YAML)
 NODE = FACTORY.create(FILE_NODE)
 ```
 
 ### Documentation
 
 The documentation of this implementation can be found here https://drb-python.gitlab.io/impl/yaml
-
```

### Comparing `drb-driver-yaml-1.0.0/versioneer.py` & `drb-driver-yaml-1.2.0/versioneer.py`

 * *Files identical despite different names*

