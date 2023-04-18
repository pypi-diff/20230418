# Comparing `tmp/pypendency-0.2.0.tar.gz` & `tmp/pypendency-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypendency-0.2.0.tar", last modified: Wed Apr 12 09:34:22 2023, max compression
+gzip compressed data, was "dist/pypendency-0.3.0.tar", last modified: Tue Apr 18 15:56:01 2023, max compression
```

## Comparing `pypendency-0.2.0.tar` & `pypendency-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-12 09:34:22.000000 pypendency-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-12 09:34:09.000000 pypendency-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 09:34:22.000000 pypendency-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-12 09:34:09.000000 pypendency-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/argument.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/py_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/loaders/yaml_loader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency/types/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-12 09:34:09.000000 pypendency-0.2.0/src/pypendency/types/python_loadable_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-12 09:34:22.000000 pypendency-0.2.0/src/pypendency.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-12 09:34:21.000000 pypendency-0.2.0/src/pypendency.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 15:56:01.000000 pypendency-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-18 15:55:47.000000 pypendency-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:56:01.000000 pypendency-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-18 15:55:47.000000 pypendency-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/argument.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/py_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/loaders/yaml_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/tag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency/types/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-18 15:55:47.000000 pypendency-0.3.0/src/pypendency/types/python_loadable_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-18 15:56:01.000000 pypendency-0.3.0/src/pypendency.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 15:56:00.000000 pypendency-0.3.0/src/pypendency.egg-info/top_level.txt
```

### Comparing `pypendency-0.2.0/PKG-INFO` & `pypendency-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.2.0
+Version: 0.3.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
-Author: Marcos Hernandez Juarez
-Author-email: marcos.hernandezjuarez@gmail.com
+Author: Fever - Platform Squad
+Author-email: platform@feverup.com
 License: MIT License
 Description: # Pypendency
         Pypendency is a dependency injection library for python >=3.7.
         
         ## Installation
         ```bash
         pip install pypendency
```

### Comparing `pypendency-0.2.0/README.md` & `pypendency-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pypendency-0.2.0/setup.py` & `pypendency-0.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 with open('README.md', 'r') as readme:
     README = readme.read()
 
 
 setup(
     name='pypendency',
-    version='0.2.0',
+    version='0.3.0',
     packages=find_packages('src'),
     package_dir={'': 'src'},
-    author='Marcos Hernandez Juarez',
-    author_email='marcos.hernandezjuarez@gmail.com',
+    author='Fever - Platform Squad',
+    author_email='platform@feverup.com',
     description='A dependency injection tool for python',
     long_description=README,
     long_description_content_type='text/markdown',
     license='MIT License',
     url='https://github.com/Feverup/pypendency',
     classifiers=[
         'Intended Audience :: Developers',
```

### Comparing `pypendency-0.2.0/src/pypendency/builder.py` & `pypendency-0.3.0/src/pypendency/builder.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Optional, List
 
 from pypendency import exceptions
-from pypendency.definition import Definition
 from pypendency.container import Container
+from pypendency.definition import Definition
 
 
 class ContainerBuilder(Container):
     _instance: Optional["ContainerBuilder"] = None
 
     def __init__(self, definitions: List[Definition]):
         ContainerBuilder._instance = self
```

### Comparing `pypendency-0.2.0/src/pypendency/container.py` & `pypendency-0.3.0/src/pypendency/container.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from abc import ABC, abstractmethod
 from pydoc import locate
-from typing import Any, Dict, List, Optional, Union
+from typing import Any, Dict, List, Optional, Union, Set, Tuple
 
 from pypendency import exceptions
 from pypendency.argument import Argument
 from pypendency.definition import Definition
+from pypendency.tag import Tag
 
 
 class AbstractContainer(ABC):
     @abstractmethod
     def set(self, identifier: str, service: object) -> None: pass
 
     @abstractmethod
@@ -21,39 +22,81 @@
 class Container(AbstractContainer):
     def __init__(self, definitions: List[Definition]):
         self._resolved = False
         self._service_mapping: Dict[str, Union[None, object, Definition]] = {
             definition.identifier: definition
             for definition in definitions
         }
+        self._tags_mapping: Dict[Tag, List[str]] = {}
 
     def resolve(self) -> None:
         if self.is_resolved():
             raise exceptions.ContainerAlreadyResolved()
 
+        self.__populate_tags_map()
         self._resolved = True
 
     def is_resolved(self) -> bool:
         return self._resolved
 
-    def set(self, identifier: str, service: object) -> None:
+    def __populate_tags_map(self) -> None:
+        for service in self._service_mapping.values():
+            if not isinstance(service, Definition):
+                continue
+            for tag in service.tags:
+                self.__add_service_to_tag_group(tag, service.identifier)
+
+    def __add_service_to_tag_group(self, tag: Tag, service_identifier: str) -> None:
+        self._tags_mapping.setdefault(tag, set()).add(service_identifier)
+
+    def set(self, identifier: str, service: object, tags: Optional[Set[Tag]] = None) -> None:
         if self.is_resolved():
             raise exceptions.ForbiddenChangeOnResolvedContainer()
 
         if self.has(identifier):
             raise exceptions.ServiceAlreadyDefined(identifier)
 
         self._service_mapping.update({identifier: service})
+        if tags is not None:
+            for tag in tags:
+                self.__add_service_to_tag_group(tag, identifier)
 
     def get(self, identifier: str) -> Optional[object]:
         if self.is_resolved() is False:
             self.resolve()
 
         return self._do_get(identifier)
 
+    def get_by_tag(self, tag: Tag) -> Set[object]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        if tag not in self._tags_mapping:
+            raise exceptions.TagNotFoundInContainer(tag.identifier)
+
+        return set([self._do_get(service) for service in self._tags_mapping[tag]])
+
+    def get_by_tag_name(self, tag_identifier: str, tag_value: Optional[object] = Tag.UNSET_VALUE) -> Set[object]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        services = set()
+        for tag, tagged_services in self._tags_mapping.items():
+            if tag.identifier == tag_identifier and (tag_value == Tag.UNSET_VALUE or tag.value == tag_value):
+                for tagged_service in tagged_services:
+                    services.add(self._do_get(tagged_service))
+
+        return services
+
+    def get_service_tags(self, service_identifier: str) -> Set[Tag]:
+        if self.is_resolved() is False:
+            self.resolve()
+
+        return {tag for tag, services in self._tags_mapping.items() if service_identifier in services}
+
     def _do_get(self, identifier: str) -> Optional[object]:
         empty = object()
 
         service = self._service_mapping.get(identifier, empty)
 
         if service is empty:
             raise exceptions.ServiceNotFoundInContainer(identifier)
```

### Comparing `pypendency-0.2.0/src/pypendency/exceptions.py` & `pypendency-0.3.0/src/pypendency/exceptions.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+from pypendency.tag import Tag
+
+
 class ContainerAlreadyResolved(Exception):
     def __init__(self):
         super().__init__("Container already resolved can't be resolved again")
 
 
 class ForbiddenChangeOnResolvedContainer(Exception):
     def __init__(self):
@@ -32,7 +35,13 @@
         )
 
 
 class ServiceInstantiationFailed(Exception):
     def __init__(self, service_fqn: str) -> None:
         self.service_fqn = service_fqn
         super().__init__(f"Type {service_fqn} cannot be instantiated by the container")
+
+
+class TagNotFoundInContainer(Exception):
+    def __init__(self, tag_identifier: str) -> None:
+        self.tag_identifier = tag_identifier
+        super().__init__(f"The tag '{tag_identifier}' does not exist in the container")
```

### Comparing `pypendency-0.2.0/src/pypendency/loaders/exceptions.py` & `pypendency-0.3.0/src/pypendency/loaders/exceptions.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.2.0/src/pypendency/loaders/py_loader.py` & `pypendency-0.3.0/src/pypendency/loaders/py_loader.py`

 * *Files identical despite different names*

### Comparing `pypendency-0.2.0/src/pypendency/loaders/yaml_loader.py` & `pypendency-0.3.0/src/pypendency/loaders/yaml_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import glob
-
 import yaml
 
 from pypendency.argument import Argument
 from pypendency.builder import ContainerBuilder
 from pypendency.definition import Definition
 from pypendency.loaders import exceptions
 from pypendency.loaders.loader import Loader
+from pypendency.tag import Tag
 
 
 class YamlLoader(Loader):
     def __init__(self, container: ContainerBuilder):
         self.__container = container
 
     def load(self, resource: str) -> None:
@@ -32,19 +32,25 @@
             ]
 
             arguments += [
                 Argument(arg_name, arg_value)
                 for arg_name, arg_value in definition_content.get('kwargs', {}).items()
             ]
 
+            tags = {
+                Tag(identifier=identifier, value=value)
+                for identifier, value in definition_content.get('tags', {}).items()
+            }
+
             self.__container.set_definition(
                 Definition(
                     identifier,
                     definition_content['fqn'],
                     arguments,
+                    tags,
                 )
             )
 
     def __resource_loaded(self, resource: str) -> dict:
         with open(resource, 'r') as stream:
             return yaml.safe_load(stream)
```

### Comparing `pypendency-0.2.0/src/pypendency.egg-info/PKG-INFO` & `pypendency-0.3.0/src/pypendency.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: pypendency
-Version: 0.2.0
+Version: 0.3.0
 Summary: A dependency injection tool for python
 Home-page: https://github.com/Feverup/pypendency
-Author: Marcos Hernandez Juarez
-Author-email: marcos.hernandezjuarez@gmail.com
+Author: Fever - Platform Squad
+Author-email: platform@feverup.com
 License: MIT License
 Description: # Pypendency
         Pypendency is a dependency injection library for python >=3.7.
         
         ## Installation
         ```bash
         pip install pypendency
```

### Comparing `pypendency-0.2.0/src/pypendency.egg-info/SOURCES.txt` & `pypendency-0.3.0/src/pypendency.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 setup.py
 src/pypendency/__init__.py
 src/pypendency/argument.py
 src/pypendency/builder.py
 src/pypendency/container.py
 src/pypendency/definition.py
 src/pypendency/exceptions.py
+src/pypendency/tag.py
 src/pypendency.egg-info/PKG-INFO
 src/pypendency.egg-info/SOURCES.txt
 src/pypendency.egg-info/dependency_links.txt
 src/pypendency.egg-info/requires.txt
 src/pypendency.egg-info/top_level.txt
 src/pypendency/loaders/__init__.py
 src/pypendency/loaders/exceptions.py
```

