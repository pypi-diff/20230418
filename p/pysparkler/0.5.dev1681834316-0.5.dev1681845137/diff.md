# Comparing `tmp/pysparkler-0.5.dev1681834316.tar.gz` & `tmp/pysparkler-0.5.dev1681845137.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.5.dev1681834316.tar", max compression
+gzip compressed data, was "pysparkler-0.5.dev1681845137.tar", max compression
```

## Comparing `pysparkler-0.5.dev1681834316.tar` & `pysparkler-0.5.dev1681845137.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9111 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/README.md
--rw-r--r--   0        0        0     1203 2023-04-18 16:11:57.004204 pysparkler-0.5.dev1681834316/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/__init__.py
--rw-r--r--   0        0        0     4490 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/api.py
--rw-r--r--   0        0        0     6057 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/cli.py
--rw-r--r--   0        0        0     6077 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2204 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10438 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4263 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.5.dev1681834316/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/README.md
+-rw-r--r--   0        0        0     1203 2023-04-18 19:12:18.141053 pysparkler-0.5.dev1681845137/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4490 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/api.py
+-rw-r--r--   0        0        0     6212 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2206 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10450 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3969 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4550 2023-04-18 19:12:11.453007 pysparkler-0.5.dev1681845137/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.5.dev1681845137/PKG-INFO
```

### Comparing `pysparkler-0.5.dev1681834316/README.md` & `pysparkler-0.5.dev1681845137/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681834316/pyproject.toml` & `pysparkler-0.5.dev1681845137/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.5.dev1681834316"
+version = "0.5.dev1681845137"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/__init__.py` & `pysparkler-0.5.dev1681845137/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/api.py` & `pysparkler-0.5.dev1681845137/pysparkler/api.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/base.py` & `pysparkler-0.5.dev1681845137/pysparkler/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import libcst.matchers as m
 
 
 class BaseTransformer(m.MatcherDecoratableTransformer):
     """Base class for all transformers.
 
     Attributes:
-        transformer_id: A unique identifier for the transformer rule. Follows the format PY<From-Major-Version>-<To-Major-Version>-<Rule-Number>
+        transformer_id: A unique identifier for the transformer rule. Follows the format
+            PY<From-Major-Version>-<To-Major-Version>-<Rule-Number>
             Important for idempotency checks and debugging.
 
     """
 
     def __init__(self, transformer_id: str):
         super().__init__()
         self.transformer_id = transformer_id
@@ -75,15 +76,16 @@
         pyspark_version: str,
         required_dependency_name: str,
         required_dependency_version: str,
         import_name: str | None = None,
     ):
         super().__init__(
             transformer_id=transformer_id,
-            comment=f"PySpark {pyspark_version} requires {required_dependency_name} version {required_dependency_version} or higher",
+            comment=f"PySpark {pyspark_version} requires {required_dependency_name} version \
+{required_dependency_version} or higher",
         )
         self.required_dependency_name = required_dependency_name
         self._import_name = import_name
 
     @property
     def import_name(self):
         return (
@@ -121,38 +123,39 @@
 
 
 def add_comment_to_end_of_a_simple_statement_line(
     node: cst.SimpleStatementLine, transformer_id: str, comment: str
 ) -> cst.SimpleStatementLine:
     """Adds a comment to the end of a statement line"""
 
+    ignore_line_too_long = "# noqa: E501"
     if node.trailing_whitespace.comment:
         # If there is already a comment
-        if transformer_id in node.trailing_whitespace.comment.value:
+        original_comment = node.trailing_whitespace.comment.value
+        if transformer_id in original_comment:
             # If the comment is already added by this transformer, do nothing
             return node
         else:
             # Add the comment to the end of the comments
+            new_cm = f"{original_comment.replace(ignore_line_too_long, '').rstrip()}  {comment}  {ignore_line_too_long}"
             return node.with_changes(
                 trailing_whitespace=cst.TrailingWhitespace(
                     whitespace=node.trailing_whitespace.whitespace,
-                    comment=node.trailing_whitespace.comment.with_changes(
-                        value=f"{node.trailing_whitespace.comment.value}  {comment}",
-                    ),
+                    comment=node.trailing_whitespace.comment.with_changes(value=new_cm),
                     newline=node.trailing_whitespace.newline,
                 )
             )
     else:
         # If there is no comment, add a comment to the trailing whitespace
         return node.with_changes(
             trailing_whitespace=cst.TrailingWhitespace(
                 whitespace=cst.SimpleWhitespace(
                     value="  ",
                 ),
-                comment=cst.Comment(value=comment),
+                comment=cst.Comment(value=f"{comment}  {ignore_line_too_long}"),
                 newline=cst.Newline(
                     value=None,
                 ),
             )
         )
```

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/cli.py` & `pysparkler-0.5.dev1681845137/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.5.dev1681845137/pysparkler/pyspark_22_to_23.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.5.dev1681845137/pysparkler/pyspark_23_to_24.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,16 @@
 
     def __init__(
         self,
         pyspark_version: str = "2.4",
     ):
         super().__init__(
             transformer_id="PY23-24-001",
-            comment=f"As of PySpark {pyspark_version} toPandas() allows fallback to non-optimization by default when Arrow optimization is unable to be used. This can be switched off by spark.sql.execution.arrow.fallback.enabled",
+            comment=f"As of PySpark {pyspark_version} toPandas() allows fallback to non-optimization by default when \
+Arrow optimization is unable to be used. This can be switched off by spark.sql.execution.arrow.fallback.enabled",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
         """Check if toPandas is being called"""
         if m.matches(node, m.Call(func=m.Attribute(attr=m.Name("toPandas")))):
             self.match_found = True
```

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.5.dev1681845137/pysparkler/pyspark_24_to_30.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         self,
         pyspark_version: str = "3.0",
         required_dependency_name: str = "pandas",
         required_dependency_version: str = "0.23.2",
     ):
         super().__init__(
             transformer_id="PY24-30-002",
-            comment=f"PySpark {pyspark_version} requires a {required_dependency_name} version of {required_dependency_version} or higher to use toPandas()",
+            comment=f"PySpark {pyspark_version} requires a {required_dependency_name} version of \
+{required_dependency_version} or higher to use toPandas()",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
         """Check if toPandas is being called"""
         if m.matches(node, m.Call(func=m.Attribute(attr=m.Name("toPandas")))):
             self.match_found = True
 
@@ -97,15 +98,16 @@
         self,
         pyspark_version: str = "3.0",
         required_dependency_name: str = "PyArrow",
         required_dependency_version: str = "0.12.1",
     ):
         super().__init__(
             transformer_id="PY24-30-004",
-            comment=f"PySpark {pyspark_version} requires {required_dependency_name} version {required_dependency_version} or higher when spark.sql.execution.arrow.enabled is set to true",
+            comment=f"PySpark {pyspark_version} requires {required_dependency_name} version \
+{required_dependency_version} or higher when spark.sql.execution.arrow.enabled is set to true",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
         """Check if spark_session.conf.set("spark.sql.execution.arrow.enabled", "true")"""
         if m.matches(
             node,
             m.Call(
@@ -136,30 +138,32 @@
 
     def __init__(self):
         super().__init__()
         self.transformer_id = "PY24-30-005"
 
     @property
     def comment(self):
-        return "Consider setting spark.sql.execution.pandas.convertToArrowArraySafely to true to raise errors in case of Integer overflow or Floating point truncation, instead of silent allows."
+        return "Consider setting spark.sql.execution.pandas.convertToArrowArraySafely to true to raise errors in case \
+of Integer overflow or Floating point truncation, instead of silent allows."
 
 
 class CreateDataFrameVerifySchemaCommentWriter(StatementLineCommentWriter):
     """In Spark 3.0, createDataFrame(..., verifySchema=True) validates LongType as well in PySpark. Previously, LongType
     was not verified and resulted in None in case the value overflows. To restore this behavior, verifySchema can be set
     to `False` to disable the validation.
     """
 
     def __init__(
         self,
         pyspark_version: str = "3.0",
     ):
         super().__init__(
             transformer_id="PY24-30-006",
-            comment=f"Setting verifySchema to True validates LongType as well in PySpark {pyspark_version}. Previously, LongType was not verified and resulted in None in case the value overflows.",
+            comment=f"Setting verifySchema to True validates LongType as well in PySpark {pyspark_version}. \
+Previously, LongType was not verified and resulted in None in case the value overflows.",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
         """Check if createDataFrame(..., verifySchema=True) is being called"""
         if m.matches(
             node,
             m.Call(
@@ -182,15 +186,16 @@
 
     def __init__(
         self,
         pyspark_version: str = "3.0",
     ):
         super().__init__(
             transformer_id="PY24-30-007",
-            comment=f"Sorting Row fields by name alphabetically since as of Spark {pyspark_version}, they are no longer when constructed with named arguments.",
+            comment=f"Sorting Row fields by name alphabetically since as of Spark {pyspark_version}, they are no \
+longer when constructed with named arguments.",
         )
 
     def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
         """Check if Row(...) is being called with named arguments and sort Dataframe Row fields by name alphabetically
         when constructed with named arguments for backwards compatibility"""
         if m.matches(
             original_node,
@@ -220,15 +225,16 @@
 
     def __init__(
         self,
         pyspark_version: str = "3.0",
     ):
         super().__init__(
             transformer_id="PY24-30-008",
-            comment=f"In Spark {pyspark_version}, pyspark.ml.param.shared.Has* mixins do not provide any set*(self, value) setter methods anymore, use the respective self.set(self.*, value) instead.",
+            comment=f"In Spark {pyspark_version}, pyspark.ml.param.shared.Has* mixins do not provide any \
+set*(self, value) setter methods anymore, use the respective self.set(self.*, value) instead.",
         )
 
     def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
         """Check if pyspark.ml.param.shared is being used in a from import statement"""
         if m.matches(
             node,
             m.ImportFrom(
```

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.5.dev1681845137/pysparkler/pyspark_31_to_32.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 
     def __init__(
         self,
         pyspark_version: str = "3.2",
     ):
         super().__init__(
             transformer_id="PY31-32-001",
-            comment=f"As of PySpark {pyspark_version}, the methods from sql, ml, spark_on_pandas modules raise the TypeError instead of ValueError when are applied to a param of inappropriate type.",
+            comment=f"As of PySpark {pyspark_version}, the methods from sql, ml, spark_on_pandas modules raise the \
+TypeError instead of ValueError when are applied to a param of inappropriate type.",
         )
         self._has_sql_or_ml_import = False
 
     def visit_ImportFrom(self, node: cst.ImportFrom) -> None:
         """Check if pyspark.sql.* or pyspark.ml.* is being used in a from import statement"""
         if m.matches(
             node,
```

### Comparing `pysparkler-0.5.dev1681834316/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.5.dev1681845137/pysparkler/pyspark_32_to_33.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,26 +20,27 @@
 
 from pysparkler.base import (
     RequiredDependencyVersionCommentWriter,
     StatementLineCommentWriter,
 )
 
 
-class DataframeDropAxisIndexByDefaultCommentWriter(StatementLineCommentWriter):
+class DataframeDropAxisIndexByDefault(StatementLineCommentWriter):
     """In Spark 3.3, the drop method of pandas API on Spark DataFrame supports dropping rows by index, and sets dropping
     by index instead of column by default.
     """
 
     def __init__(
         self,
         pyspark_version: str = "3.3",
     ):
         super().__init__(
             transformer_id="PY32-33-001",
-            comment=f"As of PySpark {pyspark_version}, the drop method of pandas API on Spark DataFrame supports dropping rows by index, and sets dropping by index instead of column by default.",
+            comment=f"Explicitly setting axis to 1 to drop by column, since as of PySpark {pyspark_version} the drop \
+method of pandas API on Spark DataFrame sets drop by index as default, instead of drop by column.",
         )
         self.inside_drop_call = False
 
     def leave_Call(self, original_node: cst.Call, updated_node: cst.Call) -> cst.Call:
         """Specify the axis argument to 1 if it is not specified to maintain the behavior of dropping columns"""
         if m.matches(
             original_node,
@@ -55,15 +56,22 @@
                 ],
             ),
         ):
             self.match_found = True
             return updated_node.with_changes(
                 args=[
                     *updated_node.args,
-                    cst.Arg(keyword=cst.Name("axis"), value=cst.Integer("1")),
+                    cst.Arg(
+                        keyword=cst.Name("axis"),
+                        value=cst.Integer("1"),
+                        equal=cst.AssignEqual(
+                            whitespace_before=cst.SimpleWhitespace(""),
+                            whitespace_after=cst.SimpleWhitespace(""),
+                        ),
+                    ),
                 ]
             )
         else:
             return updated_node
 
 
 class RequiredPandasVersionCommentWriter(RequiredDependencyVersionCommentWriter):
@@ -90,26 +98,27 @@
 
     def __init__(
         self,
         pyspark_version: str = "3.3",
     ):
         super().__init__(
             transformer_id="PY32-33-003",
-            comment=f"As of PySpark {pyspark_version}, the repr return values of SQL DataTypes have been changed to yield an object with the same value when passed to eval.",
+            comment=f"As of PySpark {pyspark_version}, the repr return values of SQL DataTypes have been changed to \
+yield an object with the same value when passed to eval.",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
         """Check if the repr method of SQL DataTypes is called"""
         if m.matches(
             node,
             m.Call(func=m.Name("repr")),
         ):
             self.match_found = True
 
 
 def pyspark_32_to_33_transformers() -> list[cst.CSTTransformer]:
     """Return a list of transformers for PySpark 3.2 to 3.3 migration guide"""
     return [
-        DataframeDropAxisIndexByDefaultCommentWriter(),
+        DataframeDropAxisIndexByDefault(),
         RequiredPandasVersionCommentWriter(),
         SQLDataTypesReprReturnsObjectCommentWriter(),
     ]
```

### Comparing `pysparkler-0.5.dev1681834316/PKG-INFO` & `pysparkler-0.5.dev1681845137/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.5.dev1681834316
+Version: 0.5.dev1681845137
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

