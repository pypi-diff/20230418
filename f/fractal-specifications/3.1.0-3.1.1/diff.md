# Comparing `tmp/fractal-specifications-3.1.0.tar.gz` & `tmp/fractal-specifications-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-specifications-3.1.0.tar", last modified: Tue Apr 18 09:34:12 2023, max compression
+gzip compressed data, was "fractal-specifications-3.1.1.tar", last modified: Tue Apr 18 11:58:37 2023, max compression
```

## Comparing `fractal-specifications-3.1.0.tar` & `fractal-specifications-3.1.1.tar`

### file list

```diff
@@ -1,56 +1,56 @@
--rw-r--r--   0        0        0      187 2023-04-18 09:33:53.827102 fractal-specifications-3.1.0/.coveragerc
--rw-r--r--   0        0        0      100 2023-04-18 09:33:53.827102 fractal-specifications-3.1.0/.flake8
--rw-r--r--   0        0        0      965 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.gitignore
--rw-r--r--   0        0        0      161 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.isort.cfg
--rw-r--r--   0        0        0     1716 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/LICENSE
--rw-r--r--   0        0        0     1436 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/Makefile
--rw-r--r--   0        0        0    14107 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/README.md
--rw-r--r--   0        0        0      780 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/align_version.py
--rw-r--r--   0        0        0      157 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/django/__init__.py
--rw-r--r--   0        0        0     2679 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/django/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     3167 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/elasticsearch/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     2381 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/google_firestore/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/mongo/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4014 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/pandas/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1599 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/contrib/sqlalchemy/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/__init__.py
--rw-r--r--   0        0        0     1968 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/collections.py
--rw-r--r--   0        0        0     4863 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/dsl_parser.py
--rw-r--r--   0        0        0     4222 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/operators.py
--rw-r--r--   0        0        0     6543 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/fractal_specifications/generic/specification.py
--rw-r--r--   0        0        0     1713 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/pyproject.toml
--rw-r--r--   0        0        0       69 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/setup.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0     2761 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/django/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2447 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/elasticsearch/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     1724 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/google_firestore/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2205 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/mongo/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4709 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/pandas/test_specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1153 2023-04-18 09:33:53.831102 fractal-specifications-3.1.0/tests/contrib/sqlalchemy/test_specifications.py
--rw-r--r--   0        0        0       52 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     4254 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/fixtures/specifications.py
--rw-r--r--   0        0        0        0 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/__init__.py
--rw-r--r--   0        0        0     3730 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_collections.py
--rw-r--r--   0        0        0     3669 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_operators.py
--rw-r--r--   0        0        0     5601 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_serialization.py
--rw-r--r--   0        0        0     3854 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tests/generic/test_specification.py
--rw-r--r--   0        0        0      705 2023-04-18 09:33:53.835103 fractal-specifications-3.1.0/tox.ini
--rw-r--r--   0        0        0    14999 1970-01-01 00:00:00.000000 fractal-specifications-3.1.0/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-04-18 11:58:22.063182 fractal-specifications-3.1.1/.coveragerc
+-rw-r--r--   0        0        0      100 2023-04-18 11:58:22.063182 fractal-specifications-3.1.1/.flake8
+-rw-r--r--   0        0        0      965 2023-04-18 11:58:22.063182 fractal-specifications-3.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/.gitignore
+-rw-r--r--   0        0        0      161 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/.isort.cfg
+-rw-r--r--   0        0        0     1716 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/LICENSE
+-rw-r--r--   0        0        0     1436 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/Makefile
+-rw-r--r--   0        0        0    14207 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/README.md
+-rw-r--r--   0        0        0      780 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/align_version.py
+-rw-r--r--   0        0        0      157 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2679 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/django/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     3167 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/elasticsearch/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     2381 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/google_firestore/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/mongo/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4014 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/pandas/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1599 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/contrib/sqlalchemy/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/generic/__init__.py
+-rw-r--r--   0        0        0     1968 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/generic/collections.py
+-rw-r--r--   0        0        0     4878 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/generic/dsl_parser.py
+-rw-r--r--   0        0        0     4222 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/generic/operators.py
+-rw-r--r--   0        0        0     6610 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/fractal_specifications/generic/specification.py
+-rw-r--r--   0        0        0     1713 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/setup.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2761 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/django/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2447 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/elasticsearch/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     1724 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/google_firestore/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2205 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/mongo/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4709 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/pandas/test_specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1153 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/contrib/sqlalchemy/test_specifications.py
+-rw-r--r--   0        0        0       52 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     4254 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/fixtures/specifications.py
+-rw-r--r--   0        0        0        0 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/generic/__init__.py
+-rw-r--r--   0        0        0     3730 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/generic/test_collections.py
+-rw-r--r--   0        0        0     3807 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/generic/test_operators.py
+-rw-r--r--   0        0        0     5624 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/generic/test_serialization.py
+-rw-r--r--   0        0        0     3936 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tests/generic/test_specification.py
+-rw-r--r--   0        0        0      705 2023-04-18 11:58:22.067182 fractal-specifications-3.1.1/tox.ini
+-rw-r--r--   0        0        0    15099 1970-01-01 00:00:00.000000 fractal-specifications-3.1.1/PKG-INFO
```

### Comparing `fractal-specifications-3.1.0/.github/workflows/build.yml` & `fractal-specifications-3.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/.github/workflows/publish.yml` & `fractal-specifications-3.1.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/.gitignore` & `fractal-specifications-3.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/.pre-commit-config.yaml` & `fractal-specifications-3.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/LICENSE` & `fractal-specifications-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/Makefile` & `fractal-specifications-3.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/README.md` & `fractal-specifications-3.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -128,14 +128,16 @@
 
 Apart from basic JSON serialization, Fractal Specifications also comes with a DSL.
 
 Example specifications DSL strings:
 
 - `field_name == 10`
   - This is a simple comparison expression with a numerical value.
+- `obj.id == 10`
+  - This is a comparison expression on an object attribute with a numerical value.
 - `name != 'John'`
   - This is another comparison expression with a string value.
 - `age >= 18 && is_student == True`
   - This is a logical AND operation between two comparison expressions and a boolean value.
 - `roles contains "admin" || roles contains "editor"`
   - This is a logical OR operation between two values of a list field.
 - `!(active == True)`
```

### Comparing `fractal-specifications-3.1.0/align_version.py` & `fractal-specifications-3.1.1/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/contrib/django/specifications.py` & `fractal-specifications-3.1.1/fractal_specifications/contrib/django/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/contrib/elasticsearch/specifications.py` & `fractal-specifications-3.1.1/fractal_specifications/contrib/elasticsearch/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/contrib/google_firestore/specifications.py` & `fractal-specifications-3.1.1/fractal_specifications/contrib/google_firestore/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/contrib/mongo/specifications.py` & `fractal-specifications-3.1.1/fractal_specifications/contrib/mongo/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/contrib/pandas/specifications.py` & `fractal-specifications-3.1.1/fractal_specifications/contrib/pandas/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/contrib/sqlalchemy/specifications.py` & `fractal-specifications-3.1.1/fractal_specifications/contrib/sqlalchemy/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/generic/collections.py` & `fractal-specifications-3.1.1/fractal_specifications/generic/collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/generic/dsl_parser.py` & `fractal-specifications-3.1.1/fractal_specifications/generic/dsl_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     field_value: string_value | number_value | boolean_value | none_value
     comparison_operator: "==" -> eq_op
         | "!=" -> neq_op
         | "<" -> lt_op
         | "<=" -> lte_op
         | ">" -> gt_op
         | ">="-> gte_op
-    field_name: CNAME
+    field_name: CNAME ("." CNAME)*
     string_value: ESCAPED_STRING | DOUBLE_QUOTED_STRING | SINGLE_QUOTED_STRING
     number_value: SIGNED_FLOAT | SIGNED_INT
     boolean_value: "True" -> true | "False" -> false
     none_value: "None" -> none
     DOUBLE_QUOTED_STRING  : /"[^"]*"/
     SINGLE_QUOTED_STRING  : /'[^']*'/
     %import common.ESCAPED_STRING
@@ -121,15 +121,15 @@
         return RegexStringMatchSpecification(field_name, value)
 
     def contains_expression(self, items):
         field_name, value = items
         return ContainsSpecification(field_name, value)
 
     def field_name(self, items):
-        return str(items[0])
+        return ".".join(items)
 
     def is_none_expression(self, items):
         return IsNoneSpecification(items[0])
 
     def field_values(self, tokens):
         return tokens
```

### Comparing `fractal-specifications-3.1.0/fractal_specifications/generic/operators.py` & `fractal-specifications-3.1.1/fractal_specifications/generic/operators.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/fractal_specifications/generic/specification.py` & `fractal-specifications-3.1.1/fractal_specifications/generic/specification.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,20 +30,21 @@
             "|": collections.OrSpecification,
         },
     }
 
 
 def _parse_specification_item(field_op: str, value: Any) -> Optional[Specification]:
     if "__" not in field_op:
-        return all_specifications()["eq"](field_op, value)
+        return all_specifications()["=="](field_op, value)
 
-    field, operator = field_op.split("__")
-    for op, spec in all_specifications().items():
-        if op == operator:
-            return spec(field, value)
+    parts = field_op.split("__")
+    field = ".".join(parts[:-1])
+    op = parts[-1]
+    if spec := all_specifications().get(op, None):
+        return spec(field, value)
     return None
 
 
 def parse_specification(**kwargs) -> Iterator[Specification]:
     for field_op, value in kwargs.items():
         if spec := _parse_specification_item(field_op, value):
             yield spec
@@ -80,14 +81,17 @@
 
     def __or__(self, other):
         return self.Or(other)
 
     def __str__(self):
         raise NotImplementedError
 
+    def __repr__(self):
+        return self.__str__()
+
     @staticmethod
     def Not(specification: "Specification") -> "Specification":
         from fractal_specifications.generic.operators import NotSpecification
 
         return NotSpecification(specification)
 
     @staticmethod
```

### Comparing `fractal-specifications-3.1.0/pyproject.toml` & `fractal-specifications-3.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-specifications"
-version = "3.1.0"
+version = "3.1.1"
 description = "Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [tool.poetry.dependencies]
 lark = "*"
 
 [build-system]
```

### Comparing `fractal-specifications-3.1.0/tests/contrib/django/test_specifications.py` & `fractal-specifications-3.1.1/tests/contrib/django/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/contrib/elasticsearch/test_specifications.py` & `fractal-specifications-3.1.1/tests/contrib/elasticsearch/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/contrib/google_firestore/test_specifications.py` & `fractal-specifications-3.1.1/tests/contrib/google_firestore/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/contrib/mongo/test_specifications.py` & `fractal-specifications-3.1.1/tests/contrib/mongo/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/contrib/pandas/test_specifications.py` & `fractal-specifications-3.1.1/tests/contrib/pandas/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/contrib/sqlalchemy/test_specifications.py` & `fractal-specifications-3.1.1/tests/contrib/sqlalchemy/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/fixtures/specifications.py` & `fractal-specifications-3.1.1/tests/fixtures/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/generic/test_collections.py` & `fractal-specifications-3.1.1/tests/generic/test_collections.py`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/tests/generic/test_operators.py` & `fractal-specifications-3.1.1/tests/generic/test_operators.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,7 +115,12 @@
     DC = make_dataclass("DC", [("name", str)])
     assert spec.is_satisfied_by(DC(**dict(name=None)))
 
 
 def test_is_none_specification_str():
     spec = IsNoneSpecification("name")
     assert spec.__str__() == "IsNoneSpecification(name)"
+
+
+def test_is_none_specification_repr():
+    spec = IsNoneSpecification("name")
+    assert spec.__repr__() == "IsNoneSpecification(name)"
```

### Comparing `fractal-specifications-3.1.0/tests/generic/test_serialization.py` & `fractal-specifications-3.1.1/tests/generic/test_serialization.py`

 * *Files 0% similar despite different names*

```diff
@@ -159,10 +159,11 @@
         'roles contains "admin" || roles contains "editor"',
         "!(active == True)",
         "name in['John', 'Jane']",
         'email matches "[a-zA-Z0-9._%+-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}"',
         'address contains "123 Main St"',
         "#",
         "salary is None",
+        "obj.id == 1",
     ]:
         spec = Specification.load_dsl(s)
         assert spec == Specification.load_dsl(spec.dump_dsl())
```

### Comparing `fractal-specifications-3.1.0/tests/generic/test_specification.py` & `fractal-specifications-3.1.1/tests/generic/test_specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 
 
 def test_parse():
     assert Specification.parse(id=1) == EqualsSpecification("id", 1)
     assert Specification.parse(id_x=1) == EqualsSpecification("id_x", 1)
     assert not Specification.parse(id__x=1)
     assert Specification.parse(id__eq=1) == EqualsSpecification("id", 1)
+    assert Specification.parse(obj__id__eq=1) == EqualsSpecification("obj.id", 1)
     assert Specification.parse(id__in=[1]) == InSpecification("id", [1])
     assert Specification.parse(id__contains="a") == ContainsSpecification("id", "a")
     assert Specification.parse(name__matches=r"^.*$") == RegexStringMatchSpecification(
         "name", r"^.*$"
     )
     assert Specification.parse(id__lt=1) == LessThanSpecification("id", 1)
     assert Specification.parse(id__lte=1) == LessThanEqualSpecification("id", 1)
```

### Comparing `fractal-specifications-3.1.0/tox.ini` & `fractal-specifications-3.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-specifications-3.1.0/PKG-INFO` & `fractal-specifications-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-specifications
-Version: 3.1.0
+Version: 3.1.1
 Summary: Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-specifications
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
@@ -150,14 +150,16 @@
 
 Apart from basic JSON serialization, Fractal Specifications also comes with a DSL.
 
 Example specifications DSL strings:
 
 - `field_name == 10`
   - This is a simple comparison expression with a numerical value.
+- `obj.id == 10`
+  - This is a comparison expression on an object attribute with a numerical value.
 - `name != 'John'`
   - This is another comparison expression with a string value.
 - `age >= 18 && is_student == True`
   - This is a logical AND operation between two comparison expressions and a boolean value.
 - `roles contains "admin" || roles contains "editor"`
   - This is a logical OR operation between two values of a list field.
 - `!(active == True)`
```

