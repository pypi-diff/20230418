# Comparing `tmp/django-typomatic-2.2.0.tar.gz` & `tmp/django-typomatic-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-typomatic-2.2.0.tar", last modified: Thu Apr 13 04:03:06 2023, max compression
+gzip compressed data, was "django-typomatic-2.3.0.tar", last modified: Tue Apr 18 06:10:52 2023, max compression
```

## Comparing `django-typomatic-2.2.0.tar` & `django-typomatic-2.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic/
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/management/commands/generate_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/django_typomatic/test__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/django_typomatic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-13 04:03:06.000000 django-typomatic-2.2.0/django_typomatic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 04:03:06.127905 django-typomatic-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-13 04:02:50.000000 django-typomatic-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:52.978016 django-typomatic-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-18 06:10:52.974017 django-typomatic-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:52.974017 django-typomatic-2.3.0/django_typomatic/
+-rw-r--r--   0 runner    (1001) docker     (123)    17190 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/django_typomatic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:52.974017 django-typomatic-2.3.0/django_typomatic/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/django_typomatic/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:52.974017 django-typomatic-2.3.0/django_typomatic/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/django_typomatic/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5058 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/django_typomatic/management/commands/generate_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/django_typomatic/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8100 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/django_typomatic/test__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:10:52.974017 django-typomatic-2.3.0/django_typomatic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-04-18 06:10:52.000000 django-typomatic-2.3.0/django_typomatic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-18 06:10:52.000000 django-typomatic-2.3.0/django_typomatic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:10:52.000000 django-typomatic-2.3.0/django_typomatic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:10:52.000000 django-typomatic-2.3.0/django_typomatic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 06:10:52.000000 django-typomatic-2.3.0/django_typomatic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 06:10:52.000000 django-typomatic-2.3.0/django_typomatic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:10:52.978016 django-typomatic-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-18 06:10:31.000000 django-typomatic-2.3.0/setup.py
```

### Comparing `django-typomatic-2.2.0/LICENSE` & `django-typomatic-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.2.0/PKG-INFO` & `django-typomatic-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.2.0
+Version: 2.3.0
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.2.0/README.md` & `django-typomatic-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.2.0/django_typomatic/__init__.py` & `django-typomatic-2.3.0/django_typomatic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from pathlib import Path
 
 from .mappings import mappings
 
 from rest_framework import serializers
+from rest_framework.serializers import BaseSerializer
 from rest_framework.fields import empty
 
 from django.db.models.enums import Choices
 import inspect
 
 from typing import get_type_hints, get_origin, get_args
 
@@ -77,14 +78,22 @@
                 if cls not in __mapping_overrides[context]:
                     __mapping_overrides[context][cls] = mapping_overrides
         return cls
 
     return decorator
 
 
+def ts_format(format):
+    def decorator(f):
+        f.format = format
+        return f
+
+    return decorator
+
+
 def __get_trimmed_name(name, trim_serializer_output):
     key = "Serializer"
     return name[:-len(key)] if trim_serializer_output and name.endswith(key) else name
 
 
 def __map_choices_to_union(field_type, choices):
     '''
@@ -133,15 +142,15 @@
             return None
     choices_enum = choices_enum + "}\n"
 
     return choices_enum
 
 
 def __process_field(field_name, field, context, serializer, trim_serializer_output, camelize,
-                    enum_choices, enum_values):
+                    enum_choices, enum_values, annotations):
     '''
     Generates and returns a tuple representing the Typescript field name and Type.
     '''
     ts_enum = None
     ts_enum_value = None
     if hasattr(field, 'child'):
         is_many = True
@@ -171,14 +180,15 @@
     elif hasattr(field, 'choices'):
         ts_type = __map_choices_to_union(field_type, field.choices)
     elif field_type == serializers.SerializerMethodField:
         types = []
         field_function = getattr(serializer, f'get_{field_name}')
         return_type = get_type_hints(field_function).get('return')
         is_generic_type = hasattr(return_type, '__origin__')
+        is_serializer_type = False
         many = False
 
         # TODO type pass recursively to represent something like a list from a list e.g. List[List[int]]
         if is_generic_type:
             return_type, many = __process_generic_type(return_type)
 
         if isinstance(return_type, list) or isinstance(return_type, tuple) or isinstance(return_type, set):
@@ -191,20 +201,48 @@
                 if is_generic_type:
                     return_type, many = __process_generic_type(return_type)
 
                 ts_type, ts_enum, ts_enum_value = __process_method_field(
                     field_name, field_type, return_type, enum_choices, enum_values, many
                 )
                 types.append(ts_type)
+        elif return_type:
+            ts_type, ts_enum, ts_enum_value = __process_method_field(
+                field_name, field_type, return_type, enum_choices, enum_values, many
+            )
+
+            if isinstance(return_type, BaseSerializer):
+                many = return_type.many
+                return_type = return_type.child.__class__
+
+            if issubclass(return_type, BaseSerializer):
+                is_external_serializer = not return_type.__module__.replace('.serializers', '') == context
+                is_serializer_type = True
+
+                if is_external_serializer and return_type not in __serializers.get(context, []):
+                    # TODO import external interface, not duplicate
+                    # Include external Interface
+                    ts_interface(context=context)(return_type)
+                    # For duplicate interface, set not exported
+                    setattr(return_type, '__exported__', False)
+
+            if is_serializer_type:
+                ts_type = __get_trimmed_name(return_type.__name__, trim_serializer_output)
+                is_many = many
+
+            types.append(ts_type)
         else:
             ts_type, ts_enum, ts_enum_value = __process_method_field(
                 field_name, field_type, return_type, enum_choices, enum_values, many
             )
             types.append(ts_type)
 
+        if hasattr(field_function, 'format'):
+            field.format = field_function.format
+
         # Clear duplicate types
         types = list(dict.fromkeys(types))
         ts_type = " | ".join(types)
     else:
         ts_type = mappings.get(field_type, 'any')
     if is_many:
         ts_type += '[]'
@@ -279,15 +317,15 @@
         fields = instance.get_fields().items()
     else:
         fields = serializer._declared_fields.items()
     ts_fields = []
     enums = []
     for key, value in fields:
         ts_property, ts_type, ts_enum, ts_enum_value = __process_field(
-            key, value, context, serializer, trim_serializer_output, camelize, enum_choices, enum_values)
+            key, value, context, serializer, trim_serializer_output, camelize, enum_choices, enum_values, annotations)
 
         if ts_enum_value is not None:
             enums.append(ts_enum_value)
 
         if ts_enum is not None:
             enums.append(ts_enum)
 
@@ -300,15 +338,16 @@
         if annotations:
             annotations_list = __get_annotations(value, ts_type)
             if annotations_list:
                 ts_fields.append('\n'.join(annotations_list))
 
         ts_fields.append(f"    {ts_property}: {ts_type};")
     collapsed_fields = '\n'.join(ts_fields)
-    return f'export interface {name} {{\n{collapsed_fields}\n}}\n\n', enums
+    exported = getattr(serializer, '__exported__', True)
+    return f'{"export " if exported else ""}interface {name} {{\n{collapsed_fields}\n}}\n\n', enums
 
 
 def __generate_interfaces_and_enums(context, trim_serializer_output, camelize, enum_choices, enum_values, annotations):
     if context not in __serializers:
         return []
     return [__get_ts_interface_and_enums(serializer, context, trim_serializer_output, camelize,
                                          enum_choices, enum_values, annotations) for serializer in
@@ -357,14 +396,16 @@
         if default is not None:
             annotations.append(f'    * @default {default}')
 
     field_type = type(field)
 
     if field_type in format_mappings:
         annotations.append(f'    * @format {format_mappings[field_type]}')
+    elif hasattr(field, 'format'):
+        annotations.append(f'    * @format {field.format}')
 
     annotations.append('    */')
 
     # Clear annotations header and footer if nothing to include
     if len(annotations) == 2:
         annotations = []
```

### Comparing `django-typomatic-2.2.0/django_typomatic/management/commands/generate_ts.py` & `django-typomatic-2.3.0/django_typomatic/management/commands/generate_ts.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.2.0/django_typomatic/mappings.py` & `django-typomatic-2.3.0/django_typomatic/mappings.py`

 * *Files identical despite different names*

### Comparing `django-typomatic-2.2.0/django_typomatic/test__init__.py` & `django-typomatic-2.3.0/django_typomatic/test__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,13 @@
-import io
 import random
 from typing import List
 
-import pytest
 from rest_framework import serializers
 from django.db import models
-from unittest.mock import patch, mock_open, MagicMock
-from . import ts_interface, generate_ts, get_ts
+from . import ts_interface, get_ts, ts_format
 
 
 @ts_interface(context='internal')
 class FooSerializer(serializers.Serializer):
     some_field = serializers.ListField(child=serializers.IntegerField())
     another_field = serializers.CharField()
     null_field = serializers.CharField(allow_null=True)
@@ -41,14 +38,19 @@
     date_field = serializers.DateField()
     datetime_field = serializers.DateTimeField()
     time_field = serializers.TimeField()
     uuid_field = serializers.UUIDField()
     url_field = serializers.URLField(default='https://google.com')
     float_field = serializers.FloatField()
     empty_annotation = serializers.CharField()
+    custom_format = serializers.SerializerMethodField()
+
+    @ts_format('email')
+    def get_custom_format(self, instance) -> str:
+        return 'test@email.com'
 
 
 class ActionType(models.TextChoices):
     ACTION1 = "Action1", ("Action1")
     ACTION2 = "Action2", ("Action2")
     ACTION3 = "Action3", ("Action3")
 
@@ -74,21 +76,28 @@
 @ts_interface('files')
 class FileSerializer(serializers.Serializer):
     image = serializers.ImageField()
     file = serializers.FileField()
 
 
 @ts_interface('methodFields')
+class MethodFieldsNestedSerializer(serializers.Serializer):
+    name = serializers.CharField(max_length=15)
+    description = serializers.CharField(max_length=100)
+
+
+@ts_interface('methodFields')
 class MethodFieldsSerializer(serializers.Serializer):
     integer_field = serializers.SerializerMethodField()
     string_field = serializers.SerializerMethodField()
     float_field = serializers.SerializerMethodField()
     choice_field = serializers.SerializerMethodField()
     multiple_return = serializers.SerializerMethodField()
     various_type_return = serializers.SerializerMethodField()
+    serializer_type_return = serializers.SerializerMethodField()
 
     def get_integer_field(self) -> int:
         return 5
 
     def get_string_field(self) -> str:
         return 'test'
 
@@ -100,14 +109,17 @@
 
     def get_multiple_return(self) -> List[int]:
         return [1, 2]
 
     def get_various_type_return(self) -> [int, str]:
         return random.choice([1, 'test'])
 
+    def get_serializer_type_return(self) -> MethodFieldsNestedSerializer:
+        return MethodFieldsNestedSerializer(name='test', description='Test')
+
 
 def test_get_ts():
     expected = """export interface FooSerializer {
     some_field: number[];
     another_field: string;
     null_field: string | null;
 }
@@ -263,14 +275,18 @@
     */
     url_field?: string;
     /**
     * @format double
     */
     float_field: number;
     empty_annotation: string;
+    /**
+    * @format email
+    */
+    custom_format?: string;
 }
 
 """
     interfaces = get_ts('annotations', annotations=True)
     assert interfaces == expected
 
 
@@ -307,19 +323,25 @@
     expected = """export enum ChoiceFieldChoiceEnum {
     ACTION1 = 'Action1',
     ACTION2 = 'Action2',
     ACTION3 = 'Action3',
 }
 
 
+export interface MethodFieldsNestedSerializer {
+    name: string;
+    description: string;
+}
+
 export interface MethodFieldsSerializer {
     integer_field?: number;
     string_field?: string;
     float_field?: number;
     choice_field?: ChoiceFieldChoiceEnum;
     multiple_return?: number[];
     various_type_return?: number | string;
+    serializer_type_return?: MethodFieldsNestedSerializer;
 }
 
 """
     interfaces = get_ts('methodFields', enum_choices=True)
     assert interfaces == expected
```

### Comparing `django-typomatic-2.2.0/django_typomatic.egg-info/PKG-INFO` & `django-typomatic-2.3.0/django_typomatic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-typomatic
-Version: 2.2.0
+Version: 2.3.0
 Summary: A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.
 Home-page: https://github.com/adenh93/django-typomatic
 Author: Aden Herold
 Author-email: aden.herold1@gmail.com
 Keywords: Django,Django Rest Framework,DRF,Typescript,Python
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `django-typomatic-2.2.0/setup.py` & `django-typomatic-2.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open('README.md') as file:
     long_description = file.read()
 
 setuptools.setup(
     name="django-typomatic",
-    version="2.2.0",
+    version="2.3.0",
     url="https://github.com/adenh93/django-typomatic",
 
     author="Aden Herold",
     author_email="aden.herold1@gmail.com",
 
     description="A simple solution for generating Typescript interfaces from your Django Rest Framework Serializers.",
     long_description=long_description,
```

