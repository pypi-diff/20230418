# Comparing `tmp/pysparkler-0.5.dev1681764938.tar.gz` & `tmp/pysparkler-0.5.dev1681834316.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysparkler-0.5.dev1681764938.tar", max compression
+gzip compressed data, was "pysparkler-0.5.dev1681834316.tar", max compression
```

## Comparing `pysparkler-0.5.dev1681764938.tar` & `pysparkler-0.5.dev1681834316.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     9111 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/README.md
--rw-r--r--   0        0        0     1203 2023-04-17 20:55:38.407690 pysparkler-0.5.dev1681764938/pyproject.toml
--rw-r--r--   0        0        0      807 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/__init__.py
--rw-r--r--   0        0        0     4490 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/api.py
--rw-r--r--   0        0        0     6057 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/base.py
--rw-r--r--   0        0        0     5734 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/cli.py
--rw-r--r--   0        0        0     4556 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_22_to_23.py
--rw-r--r--   0        0        0     2204 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_23_to_24.py
--rw-r--r--   0        0        0    10438 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_24_to_30.py
--rw-r--r--   0        0        0     3967 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_31_to_32.py
--rw-r--r--   0        0        0     4263 2023-04-17 20:55:30.939604 pysparkler-0.5.dev1681764938/pysparkler/pyspark_32_to_33.py
--rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.5.dev1681764938/PKG-INFO
+-rw-r--r--   0        0        0     9111 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/README.md
+-rw-r--r--   0        0        0     1203 2023-04-18 16:11:57.004204 pysparkler-0.5.dev1681834316/pyproject.toml
+-rw-r--r--   0        0        0      807 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/__init__.py
+-rw-r--r--   0        0        0     4490 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/api.py
+-rw-r--r--   0        0        0     6057 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/base.py
+-rw-r--r--   0        0        0     5734 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/cli.py
+-rw-r--r--   0        0        0     6077 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_22_to_23.py
+-rw-r--r--   0        0        0     2204 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_23_to_24.py
+-rw-r--r--   0        0        0    10438 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_24_to_30.py
+-rw-r--r--   0        0        0     3967 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_31_to_32.py
+-rw-r--r--   0        0        0     4263 2023-04-18 16:11:48.492282 pysparkler-0.5.dev1681834316/pysparkler/pyspark_32_to_33.py
+-rw-r--r--   0        0        0     9990 1970-01-01 00:00:00.000000 pysparkler-0.5.dev1681834316/PKG-INFO
```

### Comparing `pysparkler-0.5.dev1681764938/README.md` & `pysparkler-0.5.dev1681834316/README.md`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pyproject.toml` & `pysparkler-0.5.dev1681834316/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pysparkler"
-version = "0.5.dev1681764938"
+version = "0.5.dev1681834316"
 description = "A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline"
 authors = ["Dhruv Pratap <dhruv.pratap@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/holdenk/spark-upgrade"
 repository = "https://github.com/holdenk/spark-upgrade"
 maintainers = [
```

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/__init__.py` & `pysparkler-0.5.dev1681834316/pysparkler/__init__.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/api.py` & `pysparkler-0.5.dev1681834316/pysparkler/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from pysparkler.pyspark_32_to_33 import pyspark_32_to_33_transformers
 
 
 class PySparkler:
     """Main class for PySparkler"""
 
     def __init__(
-        self, from_pyspark: str = "2.4", to_pyspark: str = "3.0", dry_run: bool = False
+        self, from_pyspark: str = "2.2", to_pyspark: str = "3.3", dry_run: bool = False
     ):
         self.from_pyspark = from_pyspark
         self.to_pyspark = to_pyspark
         self.dry_run = dry_run
 
     @property
     def transformers(self):
```

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/base.py` & `pysparkler-0.5.dev1681834316/pysparkler/base.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/cli.py` & `pysparkler-0.5.dev1681834316/pysparkler/cli.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/pyspark_22_to_23.py` & `pysparkler-0.5.dev1681834316/pysparkler/pyspark_22_to_23.py`

 * *Files 17% similar despite different names*

```diff
@@ -91,25 +91,65 @@
             transformer_id="PY22-23-003",
             comment=f"As of PySpark {pyspark_version}, df.replace does not allow to omit value when to_replace is not \
 a dictionary. Previously, value could be omitted in the other cases and had None by default, which is counterintuitive \
 and error-prone.",
         )
 
     def visit_Call(self, node: cst.Call) -> None:
-        """Check if replace is being called on a DataFrame with only one argument that is not a dictionary"""
+        """Check if df.na.replace is being called on a DataFrame with only one argument that is not a dictionary"""
         if m.matches(
             node,
             m.Call(
-                func=m.Attribute(attr=m.Name("replace")),
+                func=m.Attribute(
+                    value=m.Attribute(attr=m.Name("na")), attr=m.Name("replace")
+                ),
                 args=[m.AtMostN(n=1, matcher=m.DoesNotMatch(m.Arg(m.Dict())))],
             ),
         ):
             self.match_found = True
 
 
+class FillNaReplacesBooleanWithNulls(StatementLineCommentWriter):
+    """In PySpark 2.3, na.fill() or fillna also accepts boolean and replaces nulls with booleans. In prior Spark
+    versions, PySpark just ignores it and returns the original Dataset/DataFrame.
+    """
+
+    def __init__(
+        self,
+        pyspark_version: str = "2.3",
+    ):
+        super().__init__(
+            transformer_id="PY22-23-004",
+            comment=f"As of PySpark {pyspark_version}, na.fill() or fillna also accepts boolean and replaces nulls \
+with booleans. In prior Spark versions, PySpark just ignores it and returns the original Dataset/DataFrame.",
+        )
+
+    def visit_Call(self, node: cst.Call) -> None:
+        """Check if df.na.fill or fillna is being called on a DataFrame with only one argument that is a boolean"""
+        if m.matches(
+            node,
+            m.Call(
+                func=m.OneOf(
+                    m.Attribute(
+                        value=m.Attribute(attr=m.Name("na")), attr=m.Name("fill")
+                    ),
+                    m.Attribute(attr=m.Name("fillna")),
+                ),
+                args=[
+                    m.AtMostN(
+                        n=1,
+                        matcher=m.Arg(value=m.OneOf(m.Name("True"), m.Name("False"))),
+                    )
+                ],
+            ),
+        ):
+            self.match_found = True
+
+
 def pyspark_22_to_23_transformers() -> list[cst.CSTTransformer]:
     """Return a list of transformers for PySpark 2.2 to 2.3 migration guide"""
     return [
         RequiredPandasVersionCommentWriter(),
         PandasRespectSessionTimeZone(),
         DataFrameReplaceWithoutUsingDictionary(),
+        FillNaReplacesBooleanWithNulls(),
     ]
```

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/pyspark_23_to_24.py` & `pysparkler-0.5.dev1681834316/pysparkler/pyspark_23_to_24.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/pyspark_24_to_30.py` & `pysparkler-0.5.dev1681834316/pysparkler/pyspark_24_to_30.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/pyspark_31_to_32.py` & `pysparkler-0.5.dev1681834316/pysparkler/pyspark_31_to_32.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/pysparkler/pyspark_32_to_33.py` & `pysparkler-0.5.dev1681834316/pysparkler/pyspark_32_to_33.py`

 * *Files identical despite different names*

### Comparing `pysparkler-0.5.dev1681764938/PKG-INFO` & `pysparkler-0.5.dev1681834316/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pysparkler
-Version: 0.5.dev1681764938
+Version: 0.5.dev1681834316
 Summary: A tool that upgrades your PySpark scripts to the latest Spark version as per Spark migration Guideline
 Home-page: https://github.com/holdenk/spark-upgrade
 License: Apache-2.0
 Author: Dhruv Pratap
 Author-email: dhruv.pratap@gmail.com
 Maintainer: Holden Karau
 Maintainer-email: holden@pigscanfly.ca
```

