# Comparing `tmp/sqlmodel_repository-2.0.0.tar.gz` & `tmp/sqlmodel_repository-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_repository-2.0.0.tar", max compression
+gzip compressed data, was "sqlmodel_repository-2.0.1.tar", max compression
```

## Comparing `sqlmodel_repository-2.0.0.tar` & `sqlmodel_repository-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/LICENSE
--rw-r--r--   0        0        0     5752 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/README.md
--rw-r--r--   0        0        0     1524 2023-04-16 09:29:18.660712 sqlmodel_repository-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      199 2023-04-16 09:29:18.656712 sqlmodel_repository-2.0.0/sqlmodel_repository/__init__.py
--rw-r--r--   0        0        0    13925 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/base_repository.py
--rw-r--r--   0        0        0      167 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/entity.py
--rw-r--r--   0        0        0      589 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/exceptions.py
--rw-r--r--   0        0        0      543 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/logger.py
--rw-r--r--   0        0        0     2640 2023-04-16 09:29:08.992709 sqlmodel_repository-2.0.0/sqlmodel_repository/repository.py
--rw-r--r--   0        0        0     6364 1970-01-01 00:00:00.000000 sqlmodel_repository-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5752 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/README.md
+-rw-r--r--   0        0        0     1524 2023-04-18 18:26:49.130169 sqlmodel_repository-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-04-18 18:26:49.126169 sqlmodel_repository-2.0.1/sqlmodel_repository/__init__.py
+-rw-r--r--   0        0        0    14839 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/sqlmodel_repository/base_repository.py
+-rw-r--r--   0        0        0      167 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/sqlmodel_repository/entity.py
+-rw-r--r--   0        0        0      589 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/sqlmodel_repository/exceptions.py
+-rw-r--r--   0        0        0      543 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/sqlmodel_repository/logger.py
+-rw-r--r--   0        0        0     2640 2023-04-18 18:26:37.637777 sqlmodel_repository-2.0.1/sqlmodel_repository/repository.py
+-rw-r--r--   0        0        0     6364 1970-01-01 00:00:00.000000 sqlmodel_repository-2.0.1/PKG-INFO
```

### Comparing `sqlmodel_repository-2.0.0/LICENSE` & `sqlmodel_repository-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-2.0.0/README.md` & `sqlmodel_repository-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-2.0.0/pyproject.toml` & `sqlmodel_repository-2.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.poetry]
 authors = ["Jonas Scholl <jonas@code-specialist.com>", "Yannic Schröer <yannic@code-specialist.com>"]
 description = "Repository pattern implementation for SQLModel (SQLAlchemy)"
 license = "MIT"
 name = "sqlmodel-repository"
 readme = "README.md"
-version = "2.0.0"
+version = "2.0.1"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 sqlmodel = "^0.0.8"
 structlog = "^23.1.0"
 
 [tool.poetry.dev-dependencies]
```

### Comparing `sqlmodel_repository-2.0.0/sqlmodel_repository/base_repository.py` & `sqlmodel_repository-2.0.1/sqlmodel_repository/base_repository.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from abc import ABC, abstractmethod
 from functools import lru_cache
 from typing import Generic, List, Optional, Type, TypeVar, get_args
 
 from sqlalchemy.orm import Session
+from sqlalchemy.sql.elements import ColumnClause
 from sqlmodel import col
 from structlog import WriteLogger
 
 from sqlmodel_repository.entity import SQLModelEntity
 from sqlmodel_repository.exceptions import CouldNotCreateEntityException, CouldNotDeleteEntityException, EntityDoesNotPossessAttributeException, EntityNotFoundException
 from sqlmodel_repository.logger import sqlmodel_repository_logger
 
 GenericEntity = TypeVar("GenericEntity", bound=SQLModelEntity)
 
 
 class BaseRepository(Generic[GenericEntity], ABC):
     """Abstract base class for all repositories"""
+
     _default_excluded_keys = ["_sa_instance_state"]
 
     def __init__(self, logger: Optional[WriteLogger] = None, sensitive_attribute_keys: Optional[list[str]] = None):
         """Initializes the repository
 
         Args:
             logger (Logger, optional): The logger to use. Defaults to None and will use the default logger.
@@ -41,28 +43,39 @@
         """Get multiple entities with one query by filters
 
         Args:
             **kwargs: The filters to apply
 
         Returns:
             List[GenericEntity]: The entities that were found in the repository for the given filters
-            
+
         Notes:
             - Success log is covered by get_batch
         """
         filters = []
         self._emit_operation_begin_log("Finding", **kwargs)
-
-        for key, value in kwargs.items():
-            try:
-                filters.append(col(getattr(self.entity, key)) == value)
-            except AttributeError as attribute_error:
-                raise EntityDoesNotPossessAttributeException(f"Entity {self.entity} does not have the attribute {key}") from attribute_error
+        filters = self._create_filters(**kwargs)
         return self.get_batch(filters=filters)
 
+    def find_one(self, **kwargs) -> GenericEntity:
+        """Get a single entity with one query by filters
+
+        Args:
+            **kwargs: The filters to apply
+
+        Returns:
+            GenericEntity: The entity that was found in the repository for the given filters
+        """
+        session = self.get_session()
+        self._emit_operation_begin_log("Finding one", **kwargs)
+        filters = self._create_filters(**kwargs)
+        result = session.query(self.entity).filter(*filters).one()
+        self._emit_operation_success_log("Finding one", entities=[result])
+        return result
+
     def update(self, entity: GenericEntity, **kwargs) -> GenericEntity:
         """Updates an entity with the given attributes (keyword arguments) if they are not None
 
         Args:
             entity (Entity): The entity to update
             **kwargs: The attributes to update with their new values
 
@@ -85,15 +98,15 @@
                 try:
                     setattr(entity, key, value)
                 except Exception as exception:
                     raise EntityDoesNotPossessAttributeException(f"Could not set attribute {key} to {value} on entity {entity}") from exception
 
         session.commit()
         session.refresh(entity)
-        
+
         self._emit_operation_success_log("Updating", entities=[entity])
         return entity
 
     def update_batch(self, entities: list[GenericEntity], **kwargs) -> list[GenericEntity]:
         """Updates a list of entities with the given attributes (keyword arguments) if they are not None
 
         Args:
@@ -137,15 +150,15 @@
         """
         session = self.get_session()
         self._emit_operation_begin_log("Getting", id=entity_id)
 
         result = session.query(self.entity).filter(self.entity.id == entity_id).one_or_none()
         if result is None:
             raise EntityNotFoundException(f"Entity {GenericEntity.__name__} with ID {entity_id} not found")
-        
+
         self._emit_operation_success_log("Getting", entities=[result])
         return result
 
     # pylint: disable=dangerous-default-value
     def get_batch(self, filters: Optional[list] = None) -> list[GenericEntity]:
         """Retrieves a list of entities from the database that match the specified filters.
 
@@ -158,15 +171,15 @@
         session = self.get_session()
         filters = filters if filters is not None else []
 
         # TODO: Add (MEANINGFUL!) filters to log. This is a bit tricky because filters is a list of ColumnClause objects and the type is not correctly defined within SQLModel.
         self._emit_operation_begin_log("Batch get")
 
         result = session.query(self.entity).filter(*filters).all()
-        
+
         self._emit_operation_success_log("Batch get", entities=result)
         return result
 
     def create(self, entity: GenericEntity) -> GenericEntity:
         """Adds a new entity to the database.
 
         Args:
@@ -181,16 +194,16 @@
         session = self.get_session()
         self._emit_operation_begin_log("Creating", entities=[entity])
 
         try:
             session.add(entity)
             session.commit()
             session.refresh(entity)
-            
-            self._emit_operation_success_log("Creating", entities=[entity])            
+
+            self._emit_operation_success_log("Creating", entities=[entity])
             return entity
         except Exception as exception:
             session.rollback()
             raise CouldNotCreateEntityException from exception
 
     def create_batch(self, entities: list[GenericEntity]) -> list[GenericEntity]:
         """Adds a batch of new entities to the database.
@@ -211,15 +224,15 @@
             session.commit()
         except Exception as exception:
             session.rollback()
             raise CouldNotCreateEntityException from exception
 
         for entity in entities:
             session.refresh(entity)
-            
+
         self._emit_operation_success_log("Batch creating", entities=entities)
         return entities
 
     def delete(self, entity: GenericEntity) -> GenericEntity:
         """Deletes an entity from the database.
 
         Args:
@@ -233,15 +246,15 @@
         """
         session = self.get_session()
         self._emit_operation_begin_log("Deleting", entities=[entity])
 
         try:
             session.delete(entity)
             session.commit()
-            
+
             self._emit_operation_success_log("Deleting", entities=[entity])
             return entity
         except Exception as exception:
             session.rollback()
             raise CouldNotDeleteEntityException from exception
 
     def delete_batch(self, entities: list[GenericEntity]) -> None:
@@ -262,14 +275,31 @@
 
             self._emit_operation_success_log("Batch deleting", entities=entities)
             session.commit()
         except Exception as exception:
             session.rollback()
             raise CouldNotDeleteEntityException from exception
 
+    def _create_filters(self, **kwargs) -> list[ColumnClause]:
+        """Creates a list of filters for a query
+
+        Args:
+            **kwargs: The filters to build
+
+        Returns:
+            list: The filters to apply to a query
+        """
+        filters = []
+        for key, value in kwargs.items():
+            try:
+                filters.append(col(getattr(self.entity, key)) == value)
+            except AttributeError as attribute_error:
+                raise EntityDoesNotPossessAttributeException(f"Entity {self.entity} does not have the attribute {key}") from attribute_error
+        return filters
+
     def _safe_kwargs(self, prefix: str = "", **kwargs) -> dict[str, str]:
         """Filters out sensitive attributes from the log kwargs
 
         Args:
             **kwargs: The key-value pairs to filter
 
         Returns:
@@ -286,15 +316,15 @@
             entities (Optional[list[GenericEntity]]): A list of entities to include in the log message. Default is None.
         """
         entities = entities or []
         try:
             entity_ids = [entity.id for entity in entities]
             entity_log: dict = {"entity_ids": entity_ids}
             self.logger.debug(f"{operation} {self.entity.__name__} succeeded", **entity_log)
-        except Exception as exception: # pylint: disable=broad-except:
+        except Exception as exception:  # pylint: disable=broad-except:
             # We want to catch all exceptions here. Logs must be written by all means. It's no silent passing and thereby acceptable.
             self.logger.exception(f"Could not emit log for concluding {operation} {self.entity.__name__}", exception=exception)  # type: ignore TODO: fix this
 
     def _emit_operation_begin_log(self, operation: str, entities: Optional[list[GenericEntity]] = None, **kwargs) -> None:
         """Emits a log message for the specified event
 
         Args:
```

### Comparing `sqlmodel_repository-2.0.0/sqlmodel_repository/exceptions.py` & `sqlmodel_repository-2.0.1/sqlmodel_repository/exceptions.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-2.0.0/sqlmodel_repository/logger.py` & `sqlmodel_repository-2.0.1/sqlmodel_repository/logger.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-2.0.0/sqlmodel_repository/repository.py` & `sqlmodel_repository-2.0.1/sqlmodel_repository/repository.py`

 * *Files identical despite different names*

### Comparing `sqlmodel_repository-2.0.0/PKG-INFO` & `sqlmodel_repository-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-repository
-Version: 2.0.0
+Version: 2.0.1
 Summary: Repository pattern implementation for SQLModel (SQLAlchemy)
 License: MIT
 Author: Jonas Scholl
 Author-email: jonas@code-specialist.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

