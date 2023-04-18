# Comparing `tmp/fractal-specifications-3.0.1.tar.gz` & `tmp/fractal-specifications-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-specifications-3.0.1.tar", last modified: Tue Apr 18 08:30:38 2023, max compression
+gzip compressed data, was "fractal-specifications-3.1.0.tar", last modified: Tue Apr 18 09:34:12 2023, max compression
```

## Comparing `fractal-specifications-3.0.1.tar` & `fractal-specifications-3.1.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      187 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.coveragerc
--rw-r--r--   0        0        0      100 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.flake8
--rw-r--r--   0        0        0      965 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.gitignore
--rw-r--r--   0        0        0      161 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.isort.cfg
--rw-r--r--   0        0        0     1716 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/LICENSE
--rw-r--r--   0        0        0     1436 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/Makefile
--rw-r--r--   0        0        0    14107 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/README.md
--rw-r--r--   0        0        0      780 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/align_version.py
--rw-r--r--   0        0        0      157 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/django/__init__.py
--rw-r--r--   0        0        0     2679 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/django/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     3167 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/elasticsearch/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     2381 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/google_firestore/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/mongo/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4014 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/pandas/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1599 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/sqlalchemy/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/collections.py
--rw-r--r--   0        0        0     4863 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/dsl_parser.py
--rw-r--r--   0        0        0     4069 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/operators.py
--rw-r--r--   0        0        0     6543 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/specification.py
--rw-r--r--   0        0        0     1713 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/setup.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0     2761 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/django/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2447 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/elasticsearch/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     1724 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/google_firestore/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2205 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/mongo/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4709 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/pandas/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/sqlalchemy/test_specifications.py
--rw-r--r--   0        0        0       52 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     4254 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/fixtures/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/__init__.py
--rw-r--r--   0        0        0     3730 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_collections.py
--rw-r--r--   0        0        0     3435 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_operators.py
--rw-r--r--   0        0        0     5601 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_serialization.py
--rw-r--r--   0        0        0     3854 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_specification.py
--rw-r--r--   0        0        0      705 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tox.ini
--rw-r--r--   0        0        0    14999 1970-01-01 00:00:00.000000 fractal-specifications-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-18 09:33:53.827102 fractal-specifications-3.1.0/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-18 09:33:53.827102 fractal-specifications-3.1.0/.flake8
+-rw-r--r--   0        0        0      965 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.isort.cfg
+-rw-r--r--   0        0        0     1716 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/LICENSE
+-rw-r--r--   0        0        0     1436 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/Makefile
+-rw-r--r--   0        0        0    14107 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/README.md
+-rw-r--r--   0        0        0      780 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/align_version.py
+-rw-r--r--   0        0        0      157 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2679 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/django/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     3167 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/elasticsearch/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/google_firestore/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/mongo/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4014 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/pandas/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1599 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/sqlalchemy/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/collections.py
+-rw-r--r--   0        0        0     4863 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/dsl_parser.py
+-rw-r--r--   0        0        0     4222 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/operators.py
+-rw-r--r--   0        0        0     6543 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/specification.py
+-rw-r--r--   0        0        0     1713 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/setup.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2761 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/django/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2447 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/elasticsearch/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     1724 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/google_firestore/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2205 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/mongo/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4709 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/pandas/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/sqlalchemy/test_specifications.py
+-rw-r--r--   0        0        0       52 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/fixtures/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/__init__.py
+-rw-r--r--   0        0        0     3730 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_collections.py
+-rw-r--r--   0        0        0     3669 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_operators.py
+-rw-r--r--   0        0        0     5601 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_serialization.py
+-rw-r--r--   0        0        0     3854 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_specification.py
+-rw-r--r--   0        0        0      705 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tox.ini
+-rw-r--r--   0        0        0    14999 1970-01-01 00:00:00.000000 fractal-specifications-3.1.0/PKG-INFO
```

### Comparing `fractal-specifications-3.0.1/.github/workflows/build.yml` & `fractal-specifications-3.1.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/.github/workflows/publish.yml` & `fractal-specifications-3.1.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/.gitignore` & `fractal-specifications-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/.pre-commit-config.yaml` & `fractal-specifications-3.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/LICENSE` & `fractal-specifications-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/Makefile` & `fractal-specifications-3.1.0/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/README.md` & `fractal-specifications-3.1.0/README.md`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/align_version.py` & `fractal-specifications-3.1.0/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/contrib/django/specifications.py` & `fractal-specifications-3.1.0/fractal_specifications/contrib/django/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/contrib/elasticsearch/specifications.py` & `fractal-specifications-3.1.0/fractal_specifications/contrib/elasticsearch/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/contrib/google_firestore/specifications.py` & `fractal-specifications-3.1.0/fractal_specifications/contrib/google_firestore/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/contrib/mongo/specifications.py` & `fractal-specifications-3.1.0/fractal_specifications/contrib/mongo/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/contrib/pandas/specifications.py` & `fractal-specifications-3.1.0/fractal_specifications/contrib/pandas/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/contrib/sqlalchemy/specifications.py` & `fractal-specifications-3.1.0/fractal_specifications/contrib/sqlalchemy/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/generic/collections.py` & `fractal-specifications-3.1.0/fractal_specifications/generic/collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/generic/dsl_parser.py` & `fractal-specifications-3.1.0/fractal_specifications/generic/dsl_parser.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/fractal_specifications/generic/operators.py` & `fractal-specifications-3.1.0/fractal_specifications/generic/operators.py`

 * *Files 20% similar despite different names*

```diff
@@ -51,102 +51,108 @@
     def is_satisfied_by(self, obj: Any) -> bool:
         raise NotImplementedError
 
     def to_collection(self) -> Collection:
         return {self.field, self.value}
 
 
+def _get_value(obj: Any, field: str) -> Any:
+    for f in field.split("."):
+        obj = getattr(obj, f)
+    return obj
+
+
 class InSpecification(FieldValueSpecification):
     def __init__(self, field: str, values: List[Any]):
         super(InSpecification, self).__init__(field, values)
 
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) in self.value
+        return _get_value(obj, self.field) in self.value
 
     @classmethod
     def _from_dict(cls, d: dict):
         return cls(field=d["field"], values=d["value"])
 
 
 class EqualsSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) == self.value
+        return _get_value(obj, self.field) == self.value
 
     @classmethod
     def name(cls):
         return "eq"
 
 
 class NotEqualsSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) != self.value
+        return _get_value(obj, self.field) != self.value
 
     @classmethod
     def name(cls):
         return "neq"
 
 
 class LessThanSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) < self.value
+        return _get_value(obj, self.field) < self.value
 
     @classmethod
     def name(cls):
         return "lt"
 
 
 class LessThanEqualSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) <= self.value
+        return _get_value(obj, self.field) <= self.value
 
     @classmethod
     def name(cls):
         return "lte"
 
 
 class GreaterThanSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) > self.value
+        return _get_value(obj, self.field) > self.value
 
     @classmethod
     def name(cls):
         return "gt"
 
 
 class GreaterThanEqualSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) >= self.value
+        return _get_value(obj, self.field) >= self.value
 
     @classmethod
     def name(cls):
         return "gte"
 
 
 class ContainsSpecification(FieldValueSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
-        return self.value in getattr(obj, self.field)
+        return self.value in _get_value(obj, self.field)
 
 
 class RegexStringMatchSpecification(ContainsSpecification):
     def is_satisfied_by(self, obj: Any) -> bool:
         import re
 
-        return bool(re.match(self.value, getattr(obj, self.field)))
+        return bool(re.match(self.value, _get_value(obj, self.field)))
 
     @classmethod
     def name(cls):
         return "matches"
 
 
 class IsNoneSpecification(FieldValueSpecification):
     def __init__(self, field: str):
         super(IsNoneSpecification, self).__init__(field, None)
 
     def __str__(self):
         return f"{self.__class__.__name__}({self.field})"
 
     def is_satisfied_by(self, obj: Any) -> bool:
-        return getattr(obj, self.field) is None
+        return _get_value(obj, self.field) is None
 
     @classmethod
     def _from_dict(cls, d: dict):
         return cls(field=d["field"])
```

### Comparing `fractal-specifications-3.0.1/fractal_specifications/generic/specification.py` & `fractal-specifications-3.1.0/fractal_specifications/generic/specification.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/pyproject.toml` & `fractal-specifications-3.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-specifications"
-version = "3.0.1"
+version = "3.1.0"
 description = "Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [tool.poetry.dependencies]
 lark = "*"
 
 [build-system]
```

### Comparing `fractal-specifications-3.0.1/tests/contrib/django/test_specifications.py` & `fractal-specifications-3.1.0/tests/contrib/django/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/contrib/elasticsearch/test_specifications.py` & `fractal-specifications-3.1.0/tests/contrib/elasticsearch/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/contrib/google_firestore/test_specifications.py` & `fractal-specifications-3.1.0/tests/contrib/google_firestore/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/contrib/mongo/test_specifications.py` & `fractal-specifications-3.1.0/tests/contrib/mongo/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/contrib/pandas/test_specifications.py` & `fractal-specifications-3.1.0/tests/contrib/pandas/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/contrib/sqlalchemy/test_specifications.py` & `fractal-specifications-3.1.0/tests/contrib/sqlalchemy/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/fixtures/specifications.py` & `fractal-specifications-3.1.0/tests/fixtures/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/generic/test_collections.py` & `fractal-specifications-3.1.0/tests/generic/test_collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/generic/test_operators.py` & `fractal-specifications-3.1.0/tests/generic/test_operators.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,14 +51,21 @@
 
 def test_equals_specification():
     spec = EqualsSpecification("id", 1)
     DC = make_dataclass("DC", [("id", int)])
     assert spec.is_satisfied_by(DC(**dict(id=1)))
 
 
+def test_equals_specification_dot():
+    spec = EqualsSpecification("obj.id", 1)
+    DC1 = make_dataclass("DC1", [("id", int)])
+    DC2 = make_dataclass("DC2", [("obj", DC1)])
+    assert spec.is_satisfied_by(DC2(DC1(**dict(id=1))))
+
+
 def test_not_equals_specification():
     spec = NotEqualsSpecification("id", 1)
     DC = make_dataclass("DC", [("id", int)])
     assert spec.is_satisfied_by(DC(**dict(id=2)))
 
 
 def test_less_than_specification():
```

### Comparing `fractal-specifications-3.0.1/tests/generic/test_serialization.py` & `fractal-specifications-3.1.0/tests/generic/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tests/generic/test_specification.py` & `fractal-specifications-3.1.0/tests/generic/test_specification.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/tox.ini` & `fractal-specifications-3.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.1/PKG-INFO` & `fractal-specifications-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-specifications
-Version: 3.0.1
+Version: 3.1.0
 Summary: Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-specifications
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

