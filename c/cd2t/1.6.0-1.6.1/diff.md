# Comparing `tmp/cd2t-1.6.0.tar.gz` & `tmp/cd2t-1.6.1.tar.gz`

## Comparing `cd2t-1.6.0.tar` & `cd2t-1.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/DataParser.py
--rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/References.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/RunTimeEnv.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/__init__.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/results.py
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/schema.py
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/utils.py
--rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/List.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/NoneDataType.py
--rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/__init__.py
--rw-r--r--   0        0        0     7993 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/base.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/bool.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/datatype.py
--rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/enum.py
--rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/float.py
--rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/idlist.py
--rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/integer.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/multitype.py
--rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/object.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/schema.py
--rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 cd2t-1.6.0/cd2t/types/string.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.6.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.6.0/LICENSE
--rw-r--r--   0        0        0    17972 2020-02-02 00:00:00.000000 cd2t-1.6.0/README.md
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.6.0/pyproject.toml
--rw-r--r--   0        0        0    18619 2020-02-02 00:00:00.000000 cd2t-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/DataParser.py
+-rw-r--r--   0        0        0     9345 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/References.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/RunTimeEnv.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/__init__.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/results.py
+-rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/schema.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/utils.py
+-rw-r--r--   0        0        0     3215 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/List.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/NoneDataType.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/__init__.py
+-rw-r--r--   0        0        0     7874 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/base.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/bool.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/datatype.py
+-rw-r--r--   0        0        0     1404 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/enum.py
+-rw-r--r--   0        0        0     8595 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/float.py
+-rw-r--r--   0        0        0     7198 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/idlist.py
+-rw-r--r--   0        0        0     6919 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/integer.py
+-rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/multitype.py
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/object.py
+-rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/schema.py
+-rw-r--r--   0        0        0     5269 2020-02-02 00:00:00.000000 cd2t-1.6.1/cd2t/types/string.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cd2t-1.6.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 cd2t-1.6.1/LICENSE
+-rw-r--r--   0        0        0    18056 2020-02-02 00:00:00.000000 cd2t-1.6.1/README.md
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 cd2t-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0    18703 2020-02-02 00:00:00.000000 cd2t-1.6.1/PKG-INFO
```

### Comparing `cd2t-1.6.0/cd2t/DataParser.py` & `cd2t-1.6.1/cd2t/DataParser.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/References.py` & `cd2t-1.6.1/cd2t/References.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/RunTimeEnv.py` & `cd2t-1.6.1/cd2t/RunTimeEnv.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/results.py` & `cd2t-1.6.1/cd2t/results.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/schema.py` & `cd2t-1.6.1/cd2t/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/utils.py` & `cd2t-1.6.1/cd2t/utils.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/List.py` & `cd2t-1.6.1/cd2t/types/List.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/base.py` & `cd2t-1.6.1/cd2t/types/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,26 +38,25 @@
         self.load_reference_option(schema, path)
         self.load_schema_options(schema, path)
         self.verify_options(path=path)
         return self
     
     def _get_data_type(self, option :str, path :str) -> DataType:
         schema = self.__dict__[option]
-        if (self.RTE.allow_shortcuts and (not isinstance(schema, str) or isinstance(schema, dict))) or \
-                (not self.RTE.allow_shortcuts and not isinstance(schema, dict)):
-            raise SchemaError("Wrong value type", path)
         if isinstance(schema, dict):
             if len(schema) == 0:
                 return BaseDataType(RTE=self.RTE)
             if not 'type' in schema.keys():
                 raise SchemaError("Needs to have a key 'type'", path)
             data_type_name = schema['type']
-        else:
+        elif self.RTE.allow_shortcuts and isinstance(schema, str):
             data_type_name = schema
             self.__dict__[option] = dict()
+        else:
+            raise SchemaError("Wrong value type", path)
         
         try:
             data_type = self.RTE.get_data_type_class(data_type_name)(RTE=self.RTE)
         except SchemaError:
             raise SchemaError("Data type '%s' not found" % data_type_name, path)
         return data_type
```

### Comparing `cd2t-1.6.0/cd2t/types/bool.py` & `cd2t-1.6.1/cd2t/types/bool.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/enum.py` & `cd2t-1.6.1/cd2t/types/enum.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/float.py` & `cd2t-1.6.1/cd2t/types/float.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/idlist.py` & `cd2t-1.6.1/cd2t/types/idlist.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/integer.py` & `cd2t-1.6.1/cd2t/types/integer.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/multitype.py` & `cd2t-1.6.1/cd2t/types/multitype.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/object.py` & `cd2t-1.6.1/cd2t/types/object.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/schema.py` & `cd2t-1.6.1/cd2t/types/schema.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/cd2t/types/string.py` & `cd2t-1.6.1/cd2t/types/string.py`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/LICENSE` & `cd2t-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cd2t-1.6.0/README.md` & `cd2t-1.6.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.6.1**:
+- *Fix*: Data Type shortcut mode with classic dictionary schema
+
 **Version 1.6.0**:
 - *Changed*: Python 3.9 or higher required
 - *New*: Data Type Shortcuts - Specify data type with defaults as string only
 - *Add*: Validator API - Method to get reference findings
 - *Changed*: Multitype Data Type - Enhanced data type support
 
 **Version 1.5.0**:
```

### Comparing `cd2t-1.6.0/pyproject.toml` & `cd2t-1.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.hatch.build]
 include = [
   "/cd2t",
 ]
 
 [project]
 name = "cd2t"
-version = "1.6.0"
+version = "1.6.1"
 authors = [
   { name="Korte Noack", email="korte@8lacht.de" },
 ]
 description = "cd2t validates data structure, data types and values with templates"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `cd2t-1.6.0/PKG-INFO` & `cd2t-1.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cd2t
-Version: 1.6.0
+Version: 1.6.1
 Summary: cd2t validates data structure, data types and values with templates
 Project-URL: Homepage, https://gitlab.com/ko.no/cd2t
 Project-URL: Bug Tracker, https://gitlab.com/ko.no/cd2t/-/issues
 Author-email: Korte Noack <korte@8lacht.de>
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -33,14 +33,17 @@
 - **Referencing**: Referencing can check the **uniqueness** of values at different positions in the data structure (i.e. lists of objects with ID attribute). It also can enforce a **consumer/producer modell**. In example, strings at some positions can be collected as *producers*. Strings at other positions must match one of those *produced* string. Scope of references can be limited to namespace.
 - **Value Autogeneration**: Some data types support creation of non-existing values. I.e. unique IDs can be added to the data structure.
 Uniqueness can be limited to namespaces.
 - **Multi Data Support**: Multiple data sources can be check with one schema or many schemas. You can switch schemas during iterating over data sources. Referencing or Autogeneration works across schemas and data sources - but can also be limited to current data.
 - **Schema Validation**: Typos, syntax mistakes or missing required options are reported as SchemaErrors (Exception) during schema loading. Reason and path through schema structured are provided.
 
 ## Change Log
+**Version 1.6.1**:
+- *Fix*: Data Type shortcut mode with classic dictionary schema
+
 **Version 1.6.0**:
 - *Changed*: Python 3.9 or higher required
 - *New*: Data Type Shortcuts - Specify data type with defaults as string only
 - *Add*: Validator API - Method to get reference findings
 - *Changed*: Multitype Data Type - Enhanced data type support
 
 **Version 1.5.0**:
```

