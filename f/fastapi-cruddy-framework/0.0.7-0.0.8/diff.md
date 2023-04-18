# Comparing `tmp/fastapi_cruddy_framework-0.0.7.tar.gz` & `tmp/fastapi_cruddy_framework-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cruddy_framework-0.0.7.tar", max compression
+gzip compressed data, was "fastapi_cruddy_framework-0.0.8.tar", max compression
```

## Comparing `fastapi_cruddy_framework-0.0.7.tar` & `fastapi_cruddy_framework-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/LICENSE
--rw-r--r--   0        0        0    29689 2023-04-16 00:33:35.866892 fastapi_cruddy_framework-0.0.7/README.md
--rw-r--r--   0        0        0      979 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/__init__.py
--rw-r--r--   0        0        0     4533 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/adapters.py
--rw-r--r--   0        0        0    17466 2023-04-16 00:39:33.654484 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/controller.py
--rw-r--r--   0        0        0       46 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/inflector.py
--rw-r--r--   0        0        0    24682 2023-04-16 00:38:48.250535 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/repository.py
--rw-r--r--   0        0        0    19346 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/resource.py
--rw-r--r--   0        0        0     2282 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/router.py
--rw-r--r--   0        0        0     2633 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/schemas.py
--rw-r--r--   0        0        0      468 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/util.py
--rw-r--r--   0        0        0     4840 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/uuid.py
--rw-r--r--   0        0        0     1895 2023-04-16 00:12:37.160738 fastapi_cruddy_framework-0.0.7/pyproject.toml
--rw-r--r--   0        0        0    31056 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/LICENSE
+-rw-r--r--   0        0        0    29689 2023-04-16 00:33:35.866892 fastapi_cruddy_framework-0.0.8/README.md
+-rw-r--r--   0        0        0      979 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/__init__.py
+-rw-r--r--   0        0        0     4533 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/adapters.py
+-rw-r--r--   0        0        0    17772 2023-04-18 15:27:38.582224 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/controller.py
+-rw-r--r--   0        0        0       46 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/inflector.py
+-rw-r--r--   0        0        0    24682 2023-04-16 00:38:48.250535 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/repository.py
+-rw-r--r--   0        0        0    19346 2023-04-15 22:07:32.387542 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/resource.py
+-rw-r--r--   0        0        0     2282 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/router.py
+-rw-r--r--   0        0        0     2633 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/schemas.py
+-rw-r--r--   0        0        0      468 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/util.py
+-rw-r--r--   0        0        0     4840 2023-04-15 22:07:32.391543 fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/uuid.py
+-rw-r--r--   0        0        0     1895 2023-04-18 15:28:22.744103 fastapi_cruddy_framework-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0    31056 1970-01-01 00:00:00.000000 fastapi_cruddy_framework-0.0.8/PKG-INFO
```

### Comparing `fastapi_cruddy_framework-0.0.7/LICENSE` & `fastapi_cruddy_framework-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/README.md` & `fastapi_cruddy_framework-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/__init__.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/adapters.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/adapters.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/controller.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from asyncio import gather
 from fastapi import APIRouter, Path, Query, Depends
 from sqlalchemy.sql.schema import Column, ForeignKey
 from sqlalchemy.orm import (
     ONETOMANY,
     MANYTOMANY,
     MANYTOONE,
 )
@@ -334,26 +335,35 @@
     id: possible_id_types = ...,
     record: CruddyModel = ...,
     relation_config_map: Dict[str, RelationshipConfig] = ...,
     repository: "AbstractRepository" = ...,
 ):
     relationship_lists = GetRelationships(record, relation_config_map)
     modified_records = 0
+    awaitables = []
     for k, v in relationship_lists.items():
         name: str = k
         new_relations: List[possible_id_types] = v
         config: RelationshipConfig = relation_config_map[name]
         if config.orm_relationship.direction == MANYTOMANY:
-            modified_records += await repository.set_many_many_relations(
-                id=id, relation=name, relations=new_relations
+            awaitables.append(
+                repository.set_many_many_relations(
+                    id=id, relation=name, relations=new_relations
+                )
             )
         elif config.orm_relationship.direction == ONETOMANY:
-            modified_records += await repository.set_one_many_relations(
-                id=id, relation=name, relations=new_relations
+            awaitables.append(
+                repository.set_one_many_relations(
+                    id=id, relation=name, relations=new_relations
+                )
             )
+    results = await gather(*awaitables, return_exceptions=True)
+    for result_or_exc in results:
+        if not isinstance(result_or_exc, Exception):
+            modified_records += result_or_exc
     return modified_records
 
 
 def ControllerCongifurator(
     controller: APIRouter = ...,
     repository: "AbstractRepository" = ...,
     id_type: possible_id_types = int,
```

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/repository.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/repository.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/resource.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/resource.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/router.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/router.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/schemas.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/schemas.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/fastapi_cruddy_framework/uuid.py` & `fastapi_cruddy_framework-0.0.8/fastapi_cruddy_framework/uuid.py`

 * *Files identical despite different names*

### Comparing `fastapi_cruddy_framework-0.0.7/pyproject.toml` & `fastapi_cruddy_framework-0.0.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-cruddy-framework"
-version = "0.0.7"
+version = "0.0.8"
 description = "A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships"
 authors = ["mdconaway <mdconaway@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{include = "fastapi_cruddy_framework"}]
 homepage = "https://github.com/mdconaway/fastapi-cruddy-framework"
 repository = "https://github.com/mdconaway/fastapi-cruddy-framework"
 keywords = ["fastapi", "crud", "mvc", "orm", "ember", "sails", "json"]
```

### Comparing `fastapi_cruddy_framework-0.0.7/PKG-INFO` & `fastapi_cruddy_framework-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cruddy-framework
-Version: 0.0.7
+Version: 0.0.8
 Summary: A holistic CRUD/MVC framework for FastAPI, with endpoint policies and relationships
 Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json
 Author: mdconaway
 Author-email: mdconaway@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 0.0.7 Summary: A
+Metadata-Version: 2.1 Name: fastapi-cruddy-framework Version: 0.0.8 Summary: A
 holistic CRUD/MVC framework for FastAPI, with endpoint policies and
 relationships Home-page: https://github.com/mdconaway/fastapi-cruddy-framework
 Keywords: fastapi,crud,mvc,orm,ember,sails,json Author: mdconaway Author-email:
 mdconaway@users.noreply.github.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 4 - Beta Classifier: Environment :: Web Environment
 Classifier: Framework :: FastAPI Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
```

