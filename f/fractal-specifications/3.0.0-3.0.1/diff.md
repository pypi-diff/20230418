# Comparing `tmp/fractal-specifications-3.0.0.tar.gz` & `tmp/fractal-specifications-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-specifications-3.0.0.tar", last modified: Tue Apr 11 07:19:26 2023, max compression
+gzip compressed data, was "fractal-specifications-3.0.1.tar", last modified: Tue Apr 18 08:30:38 2023, max compression
```

## Comparing `fractal-specifications-3.0.0.tar` & `fractal-specifications-3.0.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      187 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.coveragerc
--rw-r--r--   0        0        0      100 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.flake8
--rw-r--r--   0        0        0      965 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.gitignore
--rw-r--r--   0        0        0      161 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.isort.cfg
--rw-r--r--   0        0        0     1716 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/LICENSE
--rw-r--r--   0        0        0     1436 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/Makefile
--rw-r--r--   0        0        0    14107 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/README.md
--rw-r--r--   0        0        0      780 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/align_version.py
--rw-r--r--   0        0        0      157 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/django/__init__.py
--rw-r--r--   0        0        0     2679 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/django/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     3167 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/elasticsearch/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     2381 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/google_firestore/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/mongo/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4014 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/pandas/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1599 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/contrib/sqlalchemy/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/collections.py
--rw-r--r--   0        0        0     4863 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/dsl_parser.py
--rw-r--r--   0        0        0     4069 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/operators.py
--rw-r--r--   0        0        0     6528 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/fractal_specifications/generic/specification.py
--rw-r--r--   0        0        0     1713 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/setup.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0     2761 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/django/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2447 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/elasticsearch/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     1724 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/google_firestore/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2205 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/mongo/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4709 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/pandas/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/contrib/sqlalchemy/test_specifications.py
--rw-r--r--   0        0        0       52 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     4254 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/fixtures/specifications.py
--rw-r--r--   0        0        0        0 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/generic/__init__.py
--rw-r--r--   0        0        0     3730 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/generic/test_collections.py
--rw-r--r--   0        0        0     3435 2023-04-11 07:19:07.825229 fractal-specifications-3.0.0/tests/generic/test_operators.py
--rw-r--r--   0        0        0     5601 2023-04-11 07:19:07.829229 fractal-specifications-3.0.0/tests/generic/test_serialization.py
--rw-r--r--   0        0        0     3854 2023-04-11 07:19:07.829229 fractal-specifications-3.0.0/tests/generic/test_specification.py
--rw-r--r--   0        0        0      705 2023-04-11 07:19:07.829229 fractal-specifications-3.0.0/tox.ini
--rw-r--r--   0        0        0    14999 1970-01-01 00:00:00.000000 fractal-specifications-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.flake8
+-rw-r--r--   0        0        0      965 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.isort.cfg
+-rw-r--r--   0        0        0     1716 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/LICENSE
+-rw-r--r--   0        0        0     1436 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/Makefile
+-rw-r--r--   0        0        0    14107 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/README.md
+-rw-r--r--   0        0        0      780 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/align_version.py
+-rw-r--r--   0        0        0      157 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2679 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/django/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     3167 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/elasticsearch/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/google_firestore/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/mongo/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4014 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/pandas/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1599 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/contrib/sqlalchemy/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/collections.py
+-rw-r--r--   0        0        0     4863 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/dsl_parser.py
+-rw-r--r--   0        0        0     4069 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/operators.py
+-rw-r--r--   0        0        0     6543 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/fractal_specifications/generic/specification.py
+-rw-r--r--   0        0        0     1713 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/setup.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2761 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/django/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2447 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/elasticsearch/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     1724 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/google_firestore/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2205 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/mongo/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4709 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/pandas/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-18 08:30:20.785545 fractal-specifications-3.0.1/tests/contrib/sqlalchemy/test_specifications.py
+-rw-r--r--   0        0        0       52 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/fixtures/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/__init__.py
+-rw-r--r--   0        0        0     3730 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_collections.py
+-rw-r--r--   0        0        0     3435 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_operators.py
+-rw-r--r--   0        0        0     5601 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_serialization.py
+-rw-r--r--   0        0        0     3854 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tests/generic/test_specification.py
+-rw-r--r--   0        0        0      705 2023-04-18 08:30:20.789545 fractal-specifications-3.0.1/tox.ini
+-rw-r--r--   0        0        0    14999 1970-01-01 00:00:00.000000 fractal-specifications-3.0.1/PKG-INFO
```

### Comparing `fractal-specifications-3.0.0/.github/workflows/build.yml` & `fractal-specifications-3.0.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/.github/workflows/publish.yml` & `fractal-specifications-3.0.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/.gitignore` & `fractal-specifications-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/.pre-commit-config.yaml` & `fractal-specifications-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/LICENSE` & `fractal-specifications-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/Makefile` & `fractal-specifications-3.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/README.md` & `fractal-specifications-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/align_version.py` & `fractal-specifications-3.0.1/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/contrib/django/specifications.py` & `fractal-specifications-3.0.1/fractal_specifications/contrib/django/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/contrib/elasticsearch/specifications.py` & `fractal-specifications-3.0.1/fractal_specifications/contrib/elasticsearch/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/contrib/google_firestore/specifications.py` & `fractal-specifications-3.0.1/fractal_specifications/contrib/google_firestore/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/contrib/mongo/specifications.py` & `fractal-specifications-3.0.1/fractal_specifications/contrib/mongo/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/contrib/pandas/specifications.py` & `fractal-specifications-3.0.1/fractal_specifications/contrib/pandas/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/contrib/sqlalchemy/specifications.py` & `fractal-specifications-3.0.1/fractal_specifications/contrib/sqlalchemy/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/generic/collections.py` & `fractal-specifications-3.0.1/fractal_specifications/generic/collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/generic/dsl_parser.py` & `fractal-specifications-3.0.1/fractal_specifications/generic/dsl_parser.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/generic/operators.py` & `fractal-specifications-3.0.1/fractal_specifications/generic/operators.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/fractal_specifications/generic/specification.py` & `fractal-specifications-3.0.1/fractal_specifications/generic/specification.py`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,15 @@
             if child_strings:
                 return f"({op.join(child_strings)})"
         elif isinstance(self, EmptySpecification):
             return "#"
         raise ValueError(f"Unsupported specification type: {type(self)}")
 
     @staticmethod
+    @lru_cache
     def load_dsl(dsl_string) -> Specification:
         from lark import Lark
 
         from fractal_specifications.generic.dsl_parser import DSLTransformer, grammar
 
         dsl_parser = Lark(grammar, start="start", parser="lalr")
         transformer = DSLTransformer()
```

### Comparing `fractal-specifications-3.0.0/pyproject.toml` & `fractal-specifications-3.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-specifications"
-version = "3.0.0"
+version = "3.0.1"
 description = "Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [tool.poetry.dependencies]
 lark = "*"
 
 [build-system]
```

### Comparing `fractal-specifications-3.0.0/tests/contrib/django/test_specifications.py` & `fractal-specifications-3.0.1/tests/contrib/django/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/contrib/elasticsearch/test_specifications.py` & `fractal-specifications-3.0.1/tests/contrib/elasticsearch/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/contrib/google_firestore/test_specifications.py` & `fractal-specifications-3.0.1/tests/contrib/google_firestore/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/contrib/mongo/test_specifications.py` & `fractal-specifications-3.0.1/tests/contrib/mongo/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/contrib/pandas/test_specifications.py` & `fractal-specifications-3.0.1/tests/contrib/pandas/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/contrib/sqlalchemy/test_specifications.py` & `fractal-specifications-3.0.1/tests/contrib/sqlalchemy/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/fixtures/specifications.py` & `fractal-specifications-3.0.1/tests/fixtures/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/generic/test_collections.py` & `fractal-specifications-3.0.1/tests/generic/test_collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/generic/test_operators.py` & `fractal-specifications-3.0.1/tests/generic/test_operators.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/generic/test_serialization.py` & `fractal-specifications-3.0.1/tests/generic/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tests/generic/test_specification.py` & `fractal-specifications-3.0.1/tests/generic/test_specification.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/tox.ini` & `fractal-specifications-3.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.0.0/PKG-INFO` & `fractal-specifications-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-specifications
-Version: 3.0.0
+Version: 3.0.1
 Summary: Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-specifications
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

