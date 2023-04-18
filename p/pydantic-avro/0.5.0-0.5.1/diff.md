# Comparing `tmp/pydantic_avro-0.5.0.tar.gz` & `tmp/pydantic_avro-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_avro-0.5.0.tar", max compression
+gzip compressed data, was "pydantic_avro-0.5.1.tar", max compression
```

## Comparing `pydantic_avro-0.5.0.tar` & `pydantic_avro-0.5.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-17 12:54:48.752535 pydantic_avro-0.5.0/LICENSE
--rw-r--r--   0        0        0     1863 2023-04-17 12:54:48.752535 pydantic_avro-0.5.0/README.md
--rw-r--r--   0        0        0     1515 2023-04-17 12:55:06.793082 pydantic_avro-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 12:54:48.752535 pydantic_avro-0.5.0/src/pydantic_avro/__init__.py
--rw-r--r--   0        0        0      685 2023-04-17 12:54:48.752535 pydantic_avro-0.5.0/src/pydantic_avro/__main__.py
--rw-r--r--   0        0        0     4473 2023-04-17 12:54:48.752535 pydantic_avro-0.5.0/src/pydantic_avro/avro_to_pydantic.py
--rw-r--r--   0        0        0     6286 2023-04-17 12:54:48.752535 pydantic_avro-0.5.0/src/pydantic_avro/base.py
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.5.0/setup.py
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2021-12-17 10:39:19.013474 pydantic_avro-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1863 2021-12-30 18:43:33.078382 pydantic_avro-0.5.1/README.md
+-rw-r--r--   0        0        0     1515 2023-04-18 11:57:54.151329 pydantic_avro-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2021-12-17 10:46:42.844382 pydantic_avro-0.5.1/src/pydantic_avro/__init__.py
+-rw-r--r--   0        0        0      685 2021-12-17 15:30:57.013907 pydantic_avro-0.5.1/src/pydantic_avro/__main__.py
+-rw-r--r--   0        0        0     5180 2023-04-18 11:57:37.546545 pydantic_avro-0.5.1/src/pydantic_avro/avro_to_pydantic.py
+-rw-r--r--   0        0        0     6987 2023-04-18 11:57:37.547329 pydantic_avro-0.5.1/src/pydantic_avro/base.py
+-rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.5.1/setup.py
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.5.1/PKG-INFO
```

### Comparing `pydantic_avro-0.5.0/LICENSE` & `pydantic_avro-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.0/README.md` & `pydantic_avro-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.0/pyproject.toml` & `pydantic_avro-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-avro"
-version = "0.5.0"
+version = "0.5.1"
 description = "Converting pydantic classes to avro schemas"
 authors = ["Peter van 't Hof' <peter.vanthof@godatadriven.com>"]
 
 keywords = ["pydantic", "avro"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/godatadriven/pydantic-avro"
```

### Comparing `pydantic_avro-0.5.0/src/pydantic_avro/__main__.py` & `pydantic_avro-0.5.1/src/pydantic_avro/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.0/src/pydantic_avro/avro_to_pydantic.py` & `pydantic_avro-0.5.1/src/pydantic_avro/avro_to_pydantic.py`

 * *Files 21% similar despite different names*

```diff
@@ -15,34 +15,39 @@
 
     def get_python_type(t: Union[str, dict]) -> str:
         """Returns python type for given avro type"""
         optional = False
         if isinstance(t, str):
             if t == "string":
                 py_type = "str"
-            elif t == "long" or t == "int":
+            elif t == "int":
+                py_type = "int"
+            elif t == "long":
                 py_type = "int"
             elif t == "boolean":
                 py_type = "bool"
             elif t == "double" or t == "float":
                 py_type = "float"
             elif t == "bytes":
                 py_type = "bytes"
             elif t in classes:
                 py_type = t
             else:
                 raise NotImplementedError(f"Type {t} not supported yet")
         elif isinstance(t, list):
-            if "null" in t:
+            if "null" in t and len(t) == 2:
                 optional = True
-            if len(t) > 2 or (not optional and len(t) > 1):
-                raise NotImplementedError("Only a single type ia supported yet")
-            c = t.copy()
-            c.remove("null")
-            py_type = get_python_type(c[0])
+                c = t.copy()
+                c.remove("null")
+                py_type = get_python_type(c[0])
+            else:
+                if "null" in t:
+                    py_type = f"Optional[Union[{','.join([ get_python_type(e) for e in t if e != 'null'])}]]"
+                else:
+                    py_type = f"Union[{','.join([ get_python_type(e) for e in t])}]"
         elif t.get("logicalType") == "uuid":
             py_type = "UUID"
         elif t.get("logicalType") == "decimal":
             py_type = "Decimal"
         elif t.get("logicalType") == "timestamp-millis" or t.get("logicalType") == "timestamp-micros":
             py_type = "datetime"
         elif t.get("logicalType") == "time-millis" or t.get("logicalType") == "time-micros":
@@ -83,15 +88,21 @@
         name = schema["name"]
         current = f"class {name}(BaseModel):\n"
 
         for field in schema["fields"]:
             n = field["name"]
             t = get_python_type(field["type"])
             default = field.get("default")
-            if "default" not in field:
+            if field["type"] == "int" and "default" in field and isinstance(default, (bool, type(None))):
+                current += f"    {n}: {t} = Field({default}, ge=-2**31, le=(2**31 - 1))\n"
+            elif field["type"] == "int" and "default" in field:
+                current += f"    {n}: {t} = Field({json.dumps(default)}, ge=-2**31, le=(2**31 - 1))\n"
+            elif field["type"] == "int":
+                current += f"    {n}: {t} = Field(..., ge=-2**31, le=(2**31 - 1))\n"
+            elif "default" not in field:
                 current += f"    {n}: {t}\n"
             elif isinstance(default, (bool, type(None))):
                 current += f"    {n}: {t} = {default}\n"
             else:
                 current += f"    {n}: {t} = {json.dumps(default)}\n"
         if len(schema["fields"]) == 0:
             current += "    pass\n"
@@ -100,18 +111,18 @@
 
     record_type_to_pydantic(schema)
 
     file_content = """
 from datetime import date, datetime, time
 from decimal import Decimal
 from enum import Enum
-from typing import List, Optional, Dict
+from typing import List, Optional, Dict, Union
 from uuid import UUID
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Field
 
 
 """
     file_content += "\n\n".join(classes.values())
 
     return file_content
```

### Comparing `pydantic_avro-0.5.0/src/pydantic_avro/base.py` & `pydantic_avro-0.5.1/src/pydantic_avro/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -39,22 +39,29 @@
 
         def get_type(value: dict) -> dict:
             """Returns a type of a single field"""
             t = value.get("type")
             f = value.get("format")
             r = value.get("$ref")
             a = value.get("additionalProperties")
+            u = value.get("anyOf")
+            minimum = value.get("minimum")
+            maximum = value.get("maximum")
             avro_type_dict: Dict[str, Any] = {}
             if "default" in value:
                 avro_type_dict["default"] = value.get("default")
             if "description" in value:
                 avro_type_dict["doc"] = value.get("description")
             if "allOf" in value and len(value["allOf"]) == 1:
                 r = value["allOf"][0]["$ref"]
-            if r is not None:
+            if u is not None:
+                avro_type_dict["type"] = []
+                for union_element in u:
+                    avro_type_dict["type"].append(get_type(union_element)["type"])
+            elif r is not None:
                 class_name = r.replace("#/definitions/", "")
                 if class_name in classes_seen:
                     avro_type_dict["type"] = class_name
                 else:
                     d = get_definition(r, schema)
                     if "enum" in d:
                         avro_type_dict["type"] = {
@@ -66,14 +73,15 @@
                         avro_type_dict["type"] = {
                             "type": "record",
                             "fields": get_fields(d),
                             # Name of the struct should be unique true the complete schema
                             # Because of this the path in the schema is tracked and used as name for a nested struct/array
                             "name": class_name,
                         }
+
                     classes_seen.add(class_name)
             elif t == "array":
                 items = value.get("items")
                 tn = get_type(items)
                 # If items in array are a object:
                 if "$ref" in items:
                     tn = tn["type"]
@@ -108,16 +116,19 @@
             elif t == "string" and f == "binary":
                 avro_type_dict["type"] = "bytes"
             elif t == "string":
                 avro_type_dict["type"] = "string"
             elif t == "number":
                 avro_type_dict["type"] = "double"
             elif t == "integer":
-                # integer in python can be a long
-                avro_type_dict["type"] = "long"
+                # integer in python can be a long, only if minimum and maximum value is set a int can be used
+                if minimum is not None and minimum >= -(2**31) and maximum is not None and maximum <= (2**31 - 1):
+                    avro_type_dict["type"] = "int"
+                else:
+                    avro_type_dict["type"] = "long"
             elif t == "boolean":
                 avro_type_dict["type"] = "boolean"
             elif t == "object":
                 if a is None:
                     value_type = "string"
                 else:
                     value_type = get_type(a)
@@ -137,15 +148,17 @@
 
             required = s.get("required", [])
             for key, value in s.get("properties", {}).items():
                 avro_type_dict = get_type(value)
                 avro_type_dict["name"] = key
 
                 if key not in required:
-                    if avro_type_dict.get("default") is None:
+                    if type(avro_type_dict["type"]) is list:
+                        avro_type_dict["type"].insert(0, "null")
+                    elif avro_type_dict.get("default") is None:
                         avro_type_dict["type"] = ["null", avro_type_dict["type"]]
                         avro_type_dict["default"] = None
 
                 fields.append(avro_type_dict)
             return fields
 
         fields = get_fields(schema)
```

### Comparing `pydantic_avro-0.5.0/setup.py` & `pydantic_avro-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['pydantic>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pydantic-avro = pydantic_avro.__main__:root_main']}
 
 setup_kwargs = {
     'name': 'pydantic-avro',
-    'version': '0.5.0',
+    'version': '0.5.1',
     'description': 'Converting pydantic classes to avro schemas',
     'long_description': '[![Python package](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml)\n[![codecov](https://codecov.io/gh/godatadriven/pydantic-avro/branch/main/graph/badge.svg?token=5L08GOERAW)](https://codecov.io/gh/godatadriven/pydantic-avro)\n[![PyPI version](https://badge.fury.io/py/pydantic-avro.svg)](https://badge.fury.io/py/pydantic-avro)\n[![CodeQL](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml)\n\n# pydantic-avro\n\nThis library can convert a pydantic class to a avro schema or generate python code from a avro schema.\n\n### Install\n\n```bash\npip install pydantic-avro\n```\n\n### Pydantic class to avro schema\n\n```python\nimport json\nfrom typing import Optional\n\nfrom pydantic_avro.base import AvroBase\n\nclass TestModel(AvroBase):\n    key1: str\n    key2: int\n    key2: Optional[str]\n\nschema_dict: dict = TestModel.avro_schema()\nprint(json.dumps(schema_dict))\n\n```\n\n### Avro schema to pydantic\n\n```shell\n# Print to stdout\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc\n\n# Save it to a file\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc --output /path/to/output.py\n```\n\n\n### Install for developers\n\n###### Install package\n\n- Requirement: Poetry 1.*\n\n```shell\npoetry install\n```\n\n###### Run unit tests\n```shell\npytest\ncoverage run -m pytest  # with coverage\n# or (depends on your local env) \npoetry run pytest\npoetry run coverage run -m pytest  # with coverage\n```\n\n##### Run linting\n\nThe linting is checked in the github workflow. To fix and review issues run this:\n```shell\nblack .   # Auto fix all issues\nisort .   # Auto fix all issues\npflake .  # Only display issues, fixing is manual\n```\n',
     'author': "Peter van 't Hof'",
     'author_email': 'peter.vanthof@godatadriven.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/godatadriven/pydantic-avro',
```

### Comparing `pydantic_avro-0.5.0/PKG-INFO` & `pydantic_avro-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-avro
-Version: 0.5.0
+Version: 0.5.1
 Summary: Converting pydantic classes to avro schemas
 Home-page: https://github.com/godatadriven/pydantic-avro
 License: MIT
 Keywords: pydantic,avro
 Author: Peter van 't Hof'
 Author-email: peter.vanthof@godatadriven.com
 Requires-Python: >=3.7,<4.0
```

