# Comparing `tmp/pymodelio-1.0.0-py3-none-any.whl.zip` & `tmp/pymodelio-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,37 +1,42 @@
-Zip file size: 21881 bytes, number of entries: 35
--rw-r--r--  2.0 unx      614 b- defN 23-Apr-13 14:32 pymodelio/__init__.py
--rw-r--r--  2.0 unx     1744 b- defN 23-Apr-13 15:15 pymodelio/attribute.py
--rw-r--r--  2.0 unx     8979 b- defN 23-Apr-13 15:04 pymodelio/base_model.py
+Zip file size: 26885 bytes, number of entries: 40
+-rw-r--r--  2.0 unx      374 b- defN 23-Apr-18 16:32 pymodelio/__init__.py
+-rw-r--r--  2.0 unx     1882 b- defN 23-Apr-18 12:32 pymodelio/attribute.py
 -rw-r--r--  2.0 unx       67 b- defN 22-Sep-06 22:04 pymodelio/constants.py
--rw-r--r--  2.0 unx     1489 b- defN 23-Apr-12 22:31 pymodelio/model_serializer.py
--rw-r--r--  2.0 unx      115 b- defN 23-Apr-13 11:20 pymodelio/shared_vars.py
+-rw-r--r--  2.0 unx      845 b- defN 23-Apr-18 13:35 pymodelio/model_serializer.py
+-rw-r--r--  2.0 unx      408 b- defN 23-Apr-17 16:04 pymodelio/pymodelio_cache.py
+-rw-r--r--  2.0 unx    11024 b- defN 23-Apr-18 15:26 pymodelio/pymodelio_model.py
+-rw-r--r--  2.0 unx       44 b- defN 23-Apr-18 14:09 pymodelio/shared_vars.py
 -rw-r--r--  2.0 unx       88 b- defN 23-Apr-13 15:15 pymodelio/undefined.py
+-rw-r--r--  2.0 unx      399 b- defN 23-Apr-18 16:31 pymodelio/utils.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 11:20 pymodelio/decorators/__init__.py
 -rw-r--r--  2.0 unx      495 b- defN 23-Apr-12 22:33 pymodelio/decorators/do_not_serialize.py
--rw-r--r--  2.0 unx     1315 b- defN 23-Apr-13 13:39 pymodelio/decorators/model.py
--rw-r--r--  2.0 unx      206 b- defN 23-Apr-13 11:21 pymodelio/decorators/overrides_child_always.py
--rw-r--r--  2.0 unx      230 b- defN 23-Apr-13 11:22 pymodelio/decorators/overrides_child_if_not_implemented.py
--rw-r--r--  2.0 unx       80 b- defN 22-Sep-06 22:04 pymodelio/exceptions/__init__.py
+-rw-r--r--  2.0 unx      761 b- defN 23-Apr-18 14:51 pymodelio/decorators/pymodelio_cached.py
+-rw-r--r--  2.0 unx      158 b- defN 23-Apr-17 15:04 pymodelio/exceptions/__init__.py
+-rw-r--r--  2.0 unx       58 b- defN 23-Apr-17 15:04 pymodelio/exceptions/auto_validator_creation_exception.py
 -rw-r--r--  2.0 unx       52 b- defN 22-Sep-06 22:04 pymodelio/exceptions/model_validation_exception.py
 -rw-r--r--  2.0 unx        0 b- defN 23-Apr-13 14:15 pymodelio/settings/__init__.py
--rw-r--r--  2.0 unx      194 b- defN 23-Apr-13 14:14 pymodelio/settings/pymodelio_setting.py
--rw-r--r--  2.0 unx      854 b- defN 23-Apr-13 15:08 pymodelio/settings/pymodelio_settings.py
--rw-r--r--  2.0 unx      496 b- defN 22-Sep-06 22:04 pymodelio/validators/__init__.py
+-rw-r--r--  2.0 unx      398 b- defN 23-Apr-15 22:13 pymodelio/settings/pymodelio_setting.py
+-rw-r--r--  2.0 unx     1040 b- defN 23-Apr-15 22:13 pymodelio/settings/pymodelio_settings.py
+-rw-r--r--  2.0 unx      635 b- defN 23-Apr-18 14:19 pymodelio/validators/__init__.py
 -rw-r--r--  2.0 unx      285 b- defN 22-Sep-06 22:04 pymodelio/validators/bool_validator.py
 -rw-r--r--  2.0 unx      323 b- defN 22-Sep-06 22:04 pymodelio/validators/datetime_validator.py
+-rw-r--r--  2.0 unx     5503 b- defN 23-Apr-18 14:12 pymodelio/validators/default_validators_builder.py
 -rw-r--r--  2.0 unx      285 b- defN 22-Sep-06 22:04 pymodelio/validators/dict_validator.py
 -rw-r--r--  2.0 unx      752 b- defN 22-Sep-06 22:04 pymodelio/validators/email_validator.py
 -rw-r--r--  2.0 unx      463 b- defN 22-Sep-06 22:04 pymodelio/validators/float_validator.py
+-rw-r--r--  2.0 unx      961 b- defN 23-Apr-18 16:31 pymodelio/validators/forward_ref_validator.py
 -rw-r--r--  2.0 unx      455 b- defN 22-Sep-06 22:04 pymodelio/validators/int_validator.py
--rw-r--r--  2.0 unx     1324 b- defN 22-Sep-06 22:04 pymodelio/validators/iterable_validator.py
+-rw-r--r--  2.0 unx     1327 b- defN 23-Apr-15 15:12 pymodelio/validators/iterable_validator.py
 -rw-r--r--  2.0 unx      473 b- defN 22-Sep-06 22:04 pymodelio/validators/list_validator.py
--rw-r--r--  2.0 unx     1007 b- defN 22-Sep-06 22:04 pymodelio/validators/numeric_validator.py
--rw-r--r--  2.0 unx     1335 b- defN 22-Sep-06 22:04 pymodelio/validators/string_validator.py
+-rw-r--r--  2.0 unx     1010 b- defN 23-Apr-15 15:13 pymodelio/validators/numeric_validator.py
+-rw-r--r--  2.0 unx      471 b- defN 23-Apr-16 21:48 pymodelio/validators/set_validator.py
+-rw-r--r--  2.0 unx     1341 b- defN 23-Apr-15 15:14 pymodelio/validators/string_validator.py
+-rw-r--r--  2.0 unx      475 b- defN 23-Apr-16 21:48 pymodelio/validators/tuple_validator.py
 -rw-r--r--  2.0 unx      274 b- defN 22-Sep-06 22:04 pymodelio/validators/validation_patterns.py
--rw-r--r--  2.0 unx     1368 b- defN 22-Sep-06 22:04 pymodelio/validators/validator.py
--rw-r--r--  2.0 unx     1070 b- defN 23-Apr-13 15:22 pymodelio-1.0.0.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx    19679 b- defN 23-Apr-13 15:22 pymodelio-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-13 15:22 pymodelio-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-Apr-13 15:22 pymodelio-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3142 b- defN 23-Apr-13 15:22 pymodelio-1.0.0.dist-info/RECORD
-35 files, 49355 bytes uncompressed, 16731 bytes compressed:  66.1%
+-rw-r--r--  2.0 unx     1368 b- defN 23-Apr-17 19:50 pymodelio/validators/validator.py
+-rw-r--r--  2.0 unx     1070 b- defN 23-Apr-18 16:40 pymodelio-1.0.1.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx    24463 b- defN 23-Apr-18 16:40 pymodelio-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Apr-18 16:40 pymodelio-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-Apr-18 16:40 pymodelio-1.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3608 b- defN 23-Apr-18 16:40 pymodelio-1.0.1.dist-info/RECORD
+40 files, 63737 bytes uncompressed, 20983 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,44 +1,47 @@
 Filename: pymodelio/__init__.py
 Comment: 
 
 Filename: pymodelio/attribute.py
 Comment: 
 
-Filename: pymodelio/base_model.py
-Comment: 
-
 Filename: pymodelio/constants.py
 Comment: 
 
 Filename: pymodelio/model_serializer.py
 Comment: 
 
+Filename: pymodelio/pymodelio_cache.py
+Comment: 
+
+Filename: pymodelio/pymodelio_model.py
+Comment: 
+
 Filename: pymodelio/shared_vars.py
 Comment: 
 
 Filename: pymodelio/undefined.py
 Comment: 
 
-Filename: pymodelio/decorators/__init__.py
+Filename: pymodelio/utils.py
 Comment: 
 
-Filename: pymodelio/decorators/do_not_serialize.py
+Filename: pymodelio/decorators/__init__.py
 Comment: 
 
-Filename: pymodelio/decorators/model.py
+Filename: pymodelio/decorators/do_not_serialize.py
 Comment: 
 
-Filename: pymodelio/decorators/overrides_child_always.py
+Filename: pymodelio/decorators/pymodelio_cached.py
 Comment: 
 
-Filename: pymodelio/decorators/overrides_child_if_not_implemented.py
+Filename: pymodelio/exceptions/__init__.py
 Comment: 
 
-Filename: pymodelio/exceptions/__init__.py
+Filename: pymodelio/exceptions/auto_validator_creation_exception.py
 Comment: 
 
 Filename: pymodelio/exceptions/model_validation_exception.py
 Comment: 
 
 Filename: pymodelio/settings/__init__.py
 Comment: 
@@ -54,53 +57,65 @@
 
 Filename: pymodelio/validators/bool_validator.py
 Comment: 
 
 Filename: pymodelio/validators/datetime_validator.py
 Comment: 
 
+Filename: pymodelio/validators/default_validators_builder.py
+Comment: 
+
 Filename: pymodelio/validators/dict_validator.py
 Comment: 
 
 Filename: pymodelio/validators/email_validator.py
 Comment: 
 
 Filename: pymodelio/validators/float_validator.py
 Comment: 
 
+Filename: pymodelio/validators/forward_ref_validator.py
+Comment: 
+
 Filename: pymodelio/validators/int_validator.py
 Comment: 
 
 Filename: pymodelio/validators/iterable_validator.py
 Comment: 
 
 Filename: pymodelio/validators/list_validator.py
 Comment: 
 
 Filename: pymodelio/validators/numeric_validator.py
 Comment: 
 
+Filename: pymodelio/validators/set_validator.py
+Comment: 
+
 Filename: pymodelio/validators/string_validator.py
 Comment: 
 
+Filename: pymodelio/validators/tuple_validator.py
+Comment: 
+
 Filename: pymodelio/validators/validation_patterns.py
 Comment: 
 
 Filename: pymodelio/validators/validator.py
 Comment: 
 
-Filename: pymodelio-1.0.0.dist-info/LICENSE.txt
+Filename: pymodelio-1.0.1.dist-info/LICENSE.txt
 Comment: 
 
-Filename: pymodelio-1.0.0.dist-info/METADATA
+Filename: pymodelio-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: pymodelio-1.0.0.dist-info/WHEEL
+Filename: pymodelio-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: pymodelio-1.0.0.dist-info/top_level.txt
+Filename: pymodelio-1.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pymodelio-1.0.0.dist-info/RECORD
+Filename: pymodelio-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymodelio/__init__.py

```diff
@@ -1,26 +1,17 @@
 # flake8: noqa
 
-__version__ = '1.0.0'
+__version__ = '1.0.1'
 
 # constants
 from .constants import UNDEFINED
 
 # Settings
 from .settings.pymodelio_setting import PymodelioSetting
 from .settings.pymodelio_settings import PymodelioSettings
 
-# BaseModel for those who don't like the decorators :'(
-from .base_model import BaseModel
-
-# pymodelio_model decorator
-from .decorators.model import model
-
-pymodelio_model = model
+from .pymodelio_model import PymodelioModel
 
 # Attribute with all aliases
-from .attribute import Attribute
 from .attribute import Attr
-from .attribute import ModelAttribute
-from .attribute import ModelAttr
 
 from .decorators.do_not_serialize import do_not_serialize
```

## pymodelio/attribute.py

```diff
@@ -1,59 +1,52 @@
-from typing import Generic, Callable, Optional, Any, TypeVar, Type
+from typing import Callable, Optional, Any, TypeVar, Union
 
+from pymodelio import UNDEFINED, PymodelioSettings, PymodelioSetting
+from pymodelio.undefined import Undefined
+from pymodelio.validators.default_validators_builder import DefaultValidatorsBuilder
 from pymodelio.validators.validator import Validator
 
 T = TypeVar('T')
 
 
-class GenericAttribute(Generic[T]):
-
-    def __init__(self, validator: Optional[Validator] = None, initable: bool = True,
+class PymodelioAttr:
+    def __init__(self, attr_type: T, validator: Optional[Validator] = UNDEFINED, initable: bool = True,
                  default_factory: Callable = None) -> None:
-        self._validator = validator
+        self._attr_type = attr_type
         self._initable = initable
         self._default_factory = default_factory or (lambda: None)
+        self._init_validator(validator)
+
+    def _init_validator(self, validator: Union[Validator, None, Undefined]) -> None:
+        if validator == UNDEFINED:
+            if PymodelioSettings.get(PymodelioSetting.USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED):
+                self._validator = DefaultValidatorsBuilder.build(self.attr_type)
+            else:
+                self._validator = None
+        else:
+            self._validator = validator
 
     def validate(self, value: Optional[Any], path: str) -> None:
         if self.validator is not None:
             self.validator.validate(value, path)
 
     @property
-    def validator(self) -> Validator:
+    def validator(self) -> Optional[Validator]:
         return self._validator
 
     @property
     def initable(self) -> bool:
         return self._initable
 
     @property
     def default_factory(self) -> Callable:
         return self._default_factory
 
     @property
-    def attr_type(self) -> Type:
-        return self.__orig_class__.__args__[0]
-
-    def __getitem__(self, attr_type: T) -> Callable[..., T]:
-        # Only declared for type hinting
-        raise NotImplementedError()
-
-
-# Indirections for type hinting
-class _AttributeRetriever(GenericAttribute):
-    def __getitem__(self, attr_type: T) -> Callable[..., T]:
-        return GenericAttribute[attr_type]
-
-
-PymodelioAttribute = _AttributeRetriever()
-
-# Exposed Attribute and aliases
-"""
-Any of these exposed attributes can be called using this signature:
+    def attr_type(self) -> T:
+        return self._attr_type
 
-Attribute(validator: Optional[Validator] = None, initable: bool = True, default_factory: Callable = None)
 
-"""
-Attribute: GenericAttribute = PymodelioAttribute
-Attr: GenericAttribute = PymodelioAttribute
-ModelAttribute: GenericAttribute = PymodelioAttribute
-ModelAttr: GenericAttribute = PymodelioAttribute
+def Attr(attr_type: T, validator: Optional[Validator] = UNDEFINED, initable: bool = True,
+         default_factory: Callable = None) -> T:
+    return PymodelioAttr(attr_type=attr_type, validator=validator, initable=initable,
+                         default_factory=default_factory)
```

## pymodelio/model_serializer.py

```diff
@@ -1,42 +1,26 @@
+from datetime import datetime
 from typing import Any
 
-from pymodelio import shared_vars
-
 
 class ModelSerializer:
 
     @classmethod
     def serialize(cls, value: Any) -> Any:
         if cls._is_model(value):
             return cls._serialize_model(value)
         if isinstance(value, (list, tuple, set)):
             return [cls.serialize(x) for x in value]
+        if isinstance(value, datetime):
+            return value.isoformat()
         return value
 
     @classmethod
     def _serialize_model(cls, model: Any) -> dict:
         serialized = {}
-        for attr_name in cls._get_model_attrs(model):
-            if cls._is_marked_as_do_not_serialize(model, attr_name):
-                continue
-            attr_value = getattr(model, attr_name)
-            # If it is a function, we ignore it
-            if callable(attr_value):
-                continue
+        for attr_name, attr_value in model._get_serializable_attrs():
             serialized[attr_name] = cls.serialize(attr_value)
         return serialized
 
     @classmethod
-    def _is_marked_as_do_not_serialize(cls, model: Any, attr_name: str) -> bool:
-        class_qualname = model.__class__.__qualname__
-        if class_qualname not in shared_vars.to_do_not_serialize:
-            return False
-        return attr_name in shared_vars.to_do_not_serialize[class_qualname]
-
-    @classmethod
-    def _get_model_attrs(cls, model: Any) -> dict:
-        return [attr_name for attr_name in dir(model) if not attr_name.startswith('_')]
-
-    @classmethod
     def _is_model(cls, attr_value: Any) -> bool:
         return hasattr(attr_value, '_is_pymodelio_model') and getattr(attr_value, '_is_pymodelio_model')()
```

## pymodelio/shared_vars.py

```diff
@@ -1,3 +1,2 @@
-base_model_overrides_child_always = []
-base_model_overrides_child_if_not_implemented = []
 to_do_not_serialize = {}
+model_globals = {}
```

## pymodelio/exceptions/__init__.py

```diff
@@ -1,2 +1,3 @@
 # flake8: noqa
 from .model_validation_exception import ModelValidationException
+from .auto_validator_creation_exception import AutoValidatorCreationException
```

## pymodelio/settings/pymodelio_setting.py

```diff
@@ -1,6 +1,9 @@
 from enum import Enum
 
 
 class PymodelioSetting(Enum):
     INIT_PROTECTED_ATTRS_BY_DEFAULT = 'INIT_PROTECTED_ATTRS_BY_DEFAULT'
     INIT_PRIVATE_ATTRS_BY_DEFAULT = 'INIT_PRIVATE_ATTRS_BY_DEFAULT'
+    USE_CACHE_OPTIMIZATIONS = 'USE_CACHE_OPTIMIZATIONS'
+    AUTO_PARSE_DATES_AS_UTC = 'AUTO_PARSE_DATES_AS_UTC'
+    USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED = 'USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED'
```

## pymodelio/settings/pymodelio_settings.py

```diff
@@ -3,15 +3,18 @@
 
 from pymodelio.settings.pymodelio_setting import PymodelioSetting
 
 
 class PymodelioSettings:
     __initial_settings = {
         PymodelioSetting.INIT_PROTECTED_ATTRS_BY_DEFAULT: True,
-        PymodelioSetting.INIT_PRIVATE_ATTRS_BY_DEFAULT: True
+        PymodelioSetting.INIT_PRIVATE_ATTRS_BY_DEFAULT: True,
+        PymodelioSetting.USE_CACHE_OPTIMIZATIONS: True,
+        PymodelioSetting.AUTO_PARSE_DATES_AS_UTC: True,
+        PymodelioSetting.USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED: True
     }
 
     __settings = deepcopy(__initial_settings)
 
     @classmethod
     def set(cls, setting: PymodelioSetting, value: Any) -> None:
         expected_type = cls.__settings[setting].__class__
```

## pymodelio/validators/__init__.py

```diff
@@ -6,7 +6,10 @@
 from .string_validator import StringValidator
 from .email_validator import EmailValidator
 from .numeric_validator import NumericValidator
 from .float_validator import FloatValidator
 from .int_validator import IntValidator
 from .iterable_validator import IterableValidator
 from .list_validator import ListValidator
+from .set_validator import SetValidator
+from .tuple_validator import TupleValidator
+from .forward_ref_validator import ForwardRefValidator
```

## pymodelio/validators/iterable_validator.py

```diff
@@ -14,15 +14,15 @@
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         if len(value) == 0 and not self.allow_empty:
             self.raise_validation_error(path, 'must not be empty')
         for i, x in enumerate(value):
-            sub_path = f'{path}[{i}]'
-
+            sub_path = '%s[%s]' % (path, i)
             if self.elements_type != (None,) and not isinstance(x, self.elements_type):
-                self.raise_validation_error(sub_path,
-                                            f'is not a valid {" or ".join([t.__name__ for t in self.elements_type])}')
+                self.raise_validation_error(
+                    sub_path, 'is not a valid %s' % (' or '.join([t.__name__ for t in self.elements_type]))
+                )
             # If it is a model
             if hasattr(x, 'validate'):
                 x.validate(sub_path)
```

## pymodelio/validators/numeric_validator.py

```diff
@@ -14,10 +14,10 @@
         self.max_value = max_value
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         if self.min_value is not None and value < self.min_value:
-            self.raise_validation_error(path, f'is lower than {self.min_value}')
+            self.raise_validation_error(path, 'is less than %s' % self.min_value)
         if self.max_value is not None and value > self.max_value:
-            self.raise_validation_error(path, f'is greater than {self.max_value}')
+            self.raise_validation_error(path, 'is greater than %s' % self.max_value)
```

## pymodelio/validators/string_validator.py

```diff
@@ -15,14 +15,14 @@
         self.regex = regex
 
     def validate(self, value: Any, path: str = None) -> None:
         super().validate(value, path)
         if value is None:
             return
         if self.min_len is not None and len(value) < self.min_len:
-            self.raise_validation_error(path, f'is shorter than {self.min_len}')
+            self.raise_validation_error(path, 'is shorter than %s' % self.min_len)
         if self.max_len is not None and len(value) > self.max_len:
-            self.raise_validation_error(path, f'is longer than {self.max_len}')
+            self.raise_validation_error(path, 'is longer than %s' % self.max_len)
         if self.fixed_len is not None and len(value) != self.fixed_len:
-            self.raise_validation_error(path, f'length is different than {self.fixed_len}')
+            self.raise_validation_error(path, 'length is different than %s' % self.fixed_len)
         if self.regex is not None and re.compile(self.regex).match(value) is None:
             self.raise_validation_error(path, 'does not match configured regex')
```

## pymodelio/validators/validator.py

```diff
@@ -17,16 +17,17 @@
 
     def validate(self, value: Any, path: str = None) -> None:
         if value is None:
             if not self.nullable:
                 self.raise_validation_error(path, 'must not be None')
             return
         if self._expected_types is not None and not isinstance(value, self._expected_types):
-            self.raise_validation_error(path,
-                                        f'is not a valid {" or ".join([t.__name__ for t in self._expected_types])}')
+            self.raise_validation_error(
+                path, 'is not a valid %s' % (' or '.join([t.__name__ for t in self._expected_types]))
+            )
         # If it is a model
         if hasattr(value, 'validate'):
             value.validate(path)
 
     def raise_validation_error(self, path: str, message: str) -> None:
         _message = message if self.message is None else self.message
-        raise ModelValidationException(f'{path} {_message}')
+        raise ModelValidationException('%s %s' % (path, _message))
```

## Comparing `pymodelio-1.0.0.dist-info/LICENSE.txt` & `pymodelio-1.0.1.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `pymodelio-1.0.0.dist-info/METADATA` & `pymodelio-1.0.1.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pymodelio
-Version: 1.0.0
+Version: 1.0.1
 Summary: A simple Python module for defining domain models, serializing, deserializing and validating them
 Home-page: https://github.com/GabrielMartinMoran/pymodelio
 Author: Gabriel Martín Moran
 Author-email: moran.gabriel.95@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
+Requires-Dist: ciso8601
 
+[![Python v3.8+](https://img.shields.io/badge/Python-v3.8%2B-blue)](https://www.python.org/downloads)
 [![Python tests](https://github.com/GabrielMartinMoran/pymodelio/actions/workflows/python.yml/badge.svg?branch=main)](https://github.com/GabrielMartinMoran/pymodelio/actions/workflows/python.yml)
 [![codecov](https://codecov.io/gh/GabrielMartinMoran/pymodelio/branch/main/graph/badge.svg?token=VVKW3GDMLD)](https://codecov.io/gh/GabrielMartinMoran/pymodelio)
 
 # pymodelio
 
 A simple Python module for defining domain models, serializing, deserializing and validating them.
 
@@ -25,108 +25,176 @@
 restrictions.
 
 ## How to install the module
 
 Installing the module is simple as running the following script on your terminal:
 
 ```shell
-pip install pymodelio
+pip install -U pymodelio
 ```
 
 ## How to use the module
 
 ### Declaring the models
 
-Models can be declared using the `pymodelio_model` decorator or by inheriting from `BaseModel`. In the example below,
-the decorator way it's used for not complicating the inheritance tree, but it would be the same if instead of using the
-decorator in each model, we just declare `Component` class as `class Component(BaseModel)`.
+Pymodelio models are declared by inheriting from `PymodelioModel` class. When instantiating a model, all _initable_
+declared attributes should be provided (if not, default generated from _default_factory_ builders will be used instead).
+
+**Let's begin with a simple example**
+
+```py
+from datetime import datetime
+from pymodelio import Attr, PymodelioModel
+
+class Person(PymodelioModel):
+    name: Attr(str)
+    created_at: Attr(datetime)
+    age: Attr(int)
+
+    def describe(self) -> str:
+        return f'{self.name} is {self.age} years old, and it was created on {self.created_at}'
+
+
+person = Person(name='Rick Sánchez', created_at=datetime.now(), age=70)
+
+print(person)
+# > Person(age=70, created_at=datetime(2023, 4, 18, 11, 46, 25, 978204, None), name='Rick Sánchez')
+
+print(person.describe())
+# > Rick Sánchez is 70 years old, and it was created on 2023-04-18 13:16:01.838463
+```
+*IMPORTANT NOTE:* Note that pymodelio attributes are defined by using Python type annotations, so we are not setting dafault values to static class attributes. Also, when you interact with these attibutes, the code autocompletion engine is going to autocomplete with the methods and properties of attribute type you specified as the first parameter of `Attr` (because on runtime you will be really working with that attribute type). For instance when interacting with `name` inside of the class, that prop will we considered as a `str`.
+
+**What about using models from other models?**
+
+```py
+from datetime import datetime
+from typing import Optional
+from pymodelio import Attr, PymodelioModel
+
+class Pet(PymodelioModel):
+    name: Attr(str)
+
+
+class Person(PymodelioModel):
+    name: Attr(str)
+    created_at: Attr(datetime)
+    age: Attr(int)
+    pet: Attr(Pet)
+
+
+person = Person(name='Morty Smith', created_at=datetime.now(), age=14, pet=Pet(name='Snuffles'))
+
+print(person)
+# > Person(age=14, created_at=datetime(2023, 4, 18, 12, 13, 0, 852099, None), name='Morty Smith',
+#       pet=Pet(name='Snuffles'))
+```
+
+**What about using a model within the same model?**
+
+For doing this, we need to use [forward references](https://peps.python.org/pep-0484/#forward-references) when using the `Person` model, because it was not yet initialized during the attribute declaration.
+
+```py
+from datetime import datetime
+from typing import Optional
+from pymodelio import Attr, PymodelioModel
+
+class Person(PymodelioModel):
+    name: Attr(str)
+    created_at: Attr(datetime)
+    age: Attr(int)
+    grandchild: Attr(Optional['Person'])
+
+
+person = Person(
+    name='Rick Sánchez', created_at=datetime.now(), age=70,
+    grandchild=Person(
+        name='Morty Smith', created_at=datetime.now(), age=14
+    )
+)
+
+print(person)
+# > Person(age=70, created_at=datetime(2023, 4, 18, 12, 14, 40, 841897, None), grandchild=Person(age=14,
+#       created_at=datetime(2023, 4, 18, 12, 14, 40, 841900, None), grandchild=None, name='Morty Smith'),
+#       name='Rick Sánchez')
+```
+
+**Let's continue with a more complex example?**
 
 ```py
 import uuid
 from typing import List
-
-import pymodelio
-from pymodelio import Attribute
+from pymodelio import Attr, PymodelioModel
 from pymodelio.validators import ListValidator, StringValidator
 from pymodelio.validators.int_validator import IntValidator
 from pymodelio.validators.validator import Validator
 
 
-@pymodelio.model
-class Component:
-    __serial_no: Attribute[str](
+
+class Component(PymodelioModel):
+    __serial_no: Attr(str,
         validator=StringValidator(fixed_len=36, regex=r'^[a-z0-9-]+$'),
         default_factory=lambda: uuid.uuid4().__str__()
     )
 
     @property
     def serial_no(self) -> str:
         return self.__serial_no
 
 
-@pymodelio.model
 class CPU(Component):
-    _frequency: Attribute[int](validator=IntValidator(min_value=0))
-    cores: Attribute[int](validator=IntValidator(min_value=0))
+    _frequency: Attr(int, validator=IntValidator(min_value=0))
+    cores: Attr(int, validator=IntValidator(min_value=0))
 
     @property
     def frequency(self) -> int:
         return self._frequency
 
 
-@pymodelio.model
 class RAM(Component):
-    frequency: Attribute[int](validator=IntValidator(min_value=0))
-    size: Attribute[int](validator=IntValidator(min_value=0))
+    frequency: Attr(int, validator=IntValidator(min_value=0))
+    size: Attr(int, validator=IntValidator(min_value=0))
 
 
-@pymodelio.model
 class Disk(Component):
-    size: Attribute[int](validator=IntValidator(min_value=0))
+    size: Attr(int, validator=IntValidator(min_value=0))
 
 
-@pymodelio.model
 class Computer(Component):
-    _cpu: Attribute[CPU](validator=Validator(expected_type=CPU))
-    _rams: Attribute[List[RAM]](validator=ListValidator(elements_type=RAM, allow_empty=False))
-    _disks: Attribute[List[Disk]](validator=ListValidator(elements_type=Disk))
+    _cpu: Attr(CPU, validator=Validator(expected_type=CPU))
+    _rams: Attr(List[RAM], validator=ListValidator(elements_type=RAM, allow_empty=False))
+    _disks: Attr(List[Disk], validator=ListValidator(elements_type=Disk))
 
     @property
     def cpu(self) -> CPU:
         return self._cpu
 
     @property
     def rams(self) -> List[RAM]:
         return self._rams
 
     @property
     def disks(self) -> List[Disk]:
         return self._disks
-```
-
-### Let's use these models
-
-You can do it by using the class constructors
 
-```py
 computer = Computer(
     serial_no='123e4567-e89b-12d3-a456-426614174000',
     cpu=CPU(frequency=3500, cores=8),
     rams=[
         RAM(frequency=1600, size=8),
         RAM(frequency=1800, size=16)
     ],
     disks=[
         Disk(size=1024),
         Disk(size=512)
     ]
 )
 ```
 
-Or you can call `from_dict` factory constructor for instantiating the models by deserializing a python dictionary
+Also, instead of initializing a models using their constructors, we can deserialize them from python dictionaries by calling `from_dict` factory constructor.
 
 ```py
 computer = Computer.from_dict({
     'serial_no': '123e4567-e89b-12d3-a456-426614174000',
     'cpu': {
         'frequency': 3500,
         'cores': 8
@@ -148,15 +216,15 @@
         {
             'size': 512
         }
     ]
 })
 ```
 
-### Wait a second, what is happening here?
+**Wait a second, what is happening here?**
 
 You probably noticed that in the example above, there are some protected and private attributes that are being set by
 providing their names without underscores.
 
 **Why is it doing that?**
 
 Some known Python modules that do similar things like pymodelio forces you to specify the protected or private
@@ -225,76 +293,70 @@
 }, auto_validate=False)
 ```
 
 Other thing that differentiates pymodelio from other modules that have a similar job, is that when you use pymodelio,
 you have available a lot of already implementing validators that simplifies most cases like validating an email, the
 length of a string, the range of a number, the emptiness of a list, etc. Even if a validator is not already implemented,
 you can do it in a very easy way by inheriting from `Validator` class or using some exposed middleware model
-initialization methods. If you are interested on this, please scroll down until you find the *validation* section.
+initialization methods. If you are interested on this, please scroll down until you find the _validation_ section.
 
 ### Customizing the model's initialization workflow
 
 ```py
-@pymodelio_model
-class Model:
-    model_attr: Attribute[str]()
-
-    @classmethod
-    def __before_init__(cls, *args, **kwargs) -> None:
-        # This method is called before everything when the model constructor is called
+class Model(PymodelioModel):
+    model_attr: Attr(str)
+
+    def __before_init__(self, *args, **kwargs) -> None:
+        # This method is called before any other method when the model constructor is called
         # It receives the same parameters the constructor gets
         pass
 
-    @classmethod
-    def __before_validate__(cls) -> None:
+    def __before_validate__(self) -> None:
         # This method is called after initializing the model attributes but just before
-        # performing the model validations (it will be executed even if 
+        # performing the model validations (it will be executed even if
         # auto_validate = False)
         pass
 
-    @classmethod
-    def __once_validated__(cls) -> None:
+    def __once_validated__(self) -> None:
         # This method is called just after performing the model validations initializing
         # the model attributes but before performing the model validations (it will be
         # executed even if auto_validate = False)
         pass
 ```
 
 ### Non initable attributes
 
 ```py
-@pymodelio_model
-class Model:
-    non_initable_model_attr: Attribute[str](initable=False, default_factory=lambda: 'Non initable default value')
+class Model(PymodelioModel):
+    non_initable_model_attr: Attr(str, initable=False, default_factory=lambda: 'Non initable default value')
 
 
 # WARNING: This will raise a NameError('non_initable_model_attr attribute is not
 #          initable for class Model')
 Model(non_initable_model_attr='custom value')
 
 
 ```
 
 ## Considerations
 
 When instantiating a model specifying `auto_validate = False`, the model won't be automatically validated during
 initialization.
 
-When a class attribute has the annotation `Attribute[<type>]`, it will be transformed into an instance attribute during
+When a class attribute has the annotation `Attr(<type>)`, it will be transformed into an instance attribute during
 the model initialization.
 
 When defining a protected or private model attribute with underscore or double underscore respectively, if that property
 can be set by the model constructor, it's value will be obtained from an attribute with the same name but without
 underscores. For instance:
 
 ```py
-@pymodelio_model
-class Component:
-    __serial_no: Attribute[str]()
-    _model_name: Attribute[str]()
+class Component(PymodelioModel):
+    __serial_no: Attr(str)
+    _model_name: Attr(str)
 
     @property
     def serial_no(self) -> str:
         return self.__serial_no
 
     @property
     def model_name(self) -> str:
@@ -303,26 +365,28 @@
 
 component = Component(serial_no='123e4567-e89b-12d3-a456-426614174000', model_name='ABC123')
 
 print(component.serial_no)  # It will print '123e4567-e89b-12d3-a456-426614174000'
 print(component.model_name)  # It will print 'ABC123'
 ```
 
+As we mentioned before, this default behavior can be disabled by configuring `PymodelioSettings`.
+
 ## Validation
 
 ### Customizing the validation process
 
 Custom validators can be implemented by inheriting from the `Validator` class. Even that, there is also other way of
 performing custom validations that consists on implementing `_when_validating_attr` method in the defined model. This
 method is called after the attribute validator is called (if the attribute does not have a validator, this method is
 called anyway).
 
 ```py
 def _when_validating_attr(self, internal_attr_name: str, exposed_attr_name: str, attr_value: Any, attr_path: str,
-                          parent_path: str, pymodel_attribute: Attribute) -> None:
+                          parent_path: str, attr: PymodelioAttr) -> None:
     pass
 ```
 
 ## Available validators
 
 ### Validator
 
@@ -394,26 +458,52 @@
 A subclass of IterableValidator specific for lists.
 
 ```py
 ListValidator(elements_type: Union[type, List[type]] = None, allow_empty: bool = True, nullable: bool = False, message:
 Optional[str] = None)
 ```
 
+### SetValidator
+
+A subclass of IterableValidator specific for sets.
+
+```py
+SetValidator(elements_type: Union[type, List[type]] = None, allow_empty: bool = True, nullable: bool = False, message:
+Optional[str] = None)
+```
+
+### TupleValidator
+
+A subclass of IterableValidator specific for tuples.
+
+```py
+TupleValidator(elements_type: Union[type, List[type]] = None, allow_empty: bool = True, nullable: bool = False, message:
+Optional[str] = None)
+```
+
 ### EmailValidator
 
 ```py
 EmailValidator(nullable: bool = False, message: Optional[str] = None)
 ```
 
 ### BoolValidator
 
 ```py
 BoolValidator(nullable: bool = False, message: Optional[str] = None)
 ```
 
+### ForwardRefValidator
+
+A validator used for forwarded references (see `typing.ForwardRef` for more info in `typing` module documentation). The expected type of the validator is intended to be always a _PymodelioModel_ and it's obtained when validating the attribute the first time.
+
+```py
+ForwardRefValidator(ref: ForwardRef, nullable: bool = False, message: Optional[str] = None)
+```
+
 ## Serialization and de-serialization
 
 For serialization, pymodelio models implement a `to_dict()` method that serializes the public attributes and
 properties (defined using the `property` decorator). For the example at the beginning of this documentation,
 calling `to_dict()` method in a computer's instance returns something like:
 
 ```py
@@ -458,17 +548,16 @@
 
 ```
 
 In case of properties (defined using the `property` decorator) that you don't want to serialize, you can use the
 `@do_not_serialize` decorator like this:
 
 ```py
-@pymodelio.model
-class Person:
-    _name: Attribute[str]()
+class Person(PymodelioModel):
+    _name: Attr(str)
 
     @property
     def name(self) -> str:
         return self._name
 
     @property
     @pymodelio.do_not_serialize
@@ -485,14 +574,42 @@
 
 ```py
 @classmethod
 def from_dict(cls, data: dict, auto_validate: bool = True) -> CustomModel:
     return CustomModel(**data)  # Replace CustomModel with your model and call the constructor as you need
 ```
 
+## Configuring Pymodelio settings
+
+As we mentioned before, there are some settings that can be configured by calling the `PymodelioSettings` class. These settigs and their expected types are:
+
+- **PymodelioSetting.INIT_PROTECTED_ATTRS_BY_DEFAULT** (`bool`): If `True`, all initable protected attributes will be exposed in the constructor on their public form. For instance: `_name` will be exposed as `name`.
+- **PymodelioSetting.INIT_PRIVATE_ATTRS_BY_DEFAULT** (`bool`): If `True`, all initable private attributes will be exposed in the constructor on their public form. For instance: `__id` will be exposed as `id`.
+- **PymodelioSetting.USE_CACHE_OPTIMIZATIONS** (`bool`): If `True`, pymodelio will use a cache for some performance tweaks. Disable it if you want to re-define model classes using the same under the same scope.
+- **PymodelioSetting.AUTO_PARSE_DATES_AS_UTC** (`bool`): If `True`, deserialized dates will be considered `UTC`.
+- **PymodelioSetting.USE_DEFAULT_ATTR_VALIDATOR_IF_NOT_DEFINED** (`bool`): If a validator is not provided when defining a model attribute (like `Attr(str)`) an automatically inferred validator will be used instead. If disabled, the attribute won't have any validator at all unless you manually specified one.
+
+Updating a setting it's as simple as doing:
+
+```py
+PymodelioSettings.set(PymodelioSetting.<setting_name>, <value>)
+```
+
+For getting the value of a setting, you can call:
+
+```py
+PymodelioSettings.get(PymodelioSetting.<setting_name>)
+```
+
+Settings can also be resseted by calling:
+
+```py
+PymodelioSettings.reset()
+```
+
 ## Let's compare the same code using raw python against using pymodelio
 
 For this comparison, we are not implementing serialization and de-serialization in the raw Python models (pymodelio
 handles this automatically for its models).
 
 ### Using raw python
 
@@ -555,24 +672,21 @@
 
 ### Using pymodelio
 
 pymodelio model validation errors also give more information about the full path of nested structures. In case of lists,
 including the index of the list element where the error occurred.
 
 ```py
-@pymodelio_model
-class PymodelioChildModel:
-    public_child_attr: Attribute[int](validator=IntValidator())
+class PymodelioChildModel(PymodelioModel):
+    public_child_attr: Attr(int)
 
 
-@pymodelio_model
-class PymodelioModel:
-    public_attr: Attribute[int](validator=IntValidator(min_value=0, max_value=10))
-    _protected_attr: Attribute[str](validator=StringValidator(fixed_len=5, regex='^[A-Z]+$'))  # Only capitalized chars
-    __private_attr: Attribute[datetime](validator=DatetimeValidator())
-    child_model_attr: Attribute[PymodelioChildModel](validator=Validator(expected_type=PymodelioChildModel))
-    children_model_attr: Attribute[List[PymodelioChildModel]](
-        validator=ListValidator(elements_type=PymodelioChildModel))
-    optional_attr: Attribute[dict](validator=DictValidator())
-    non_initable_attr: Attribute[List[str]](initable=False, default_factory=list)
-```
+class PymodelioParentModel(PymodelioModel):
+    public_attr: Attr(int, validator=IntValidator(min_value=0, max_value=10))
+    _protected_attr: Attr(str, validator=StringValidator(fixed_len=5, regex='^[A-Z]+$'))  # Only capitalized chars
+    __private_attr: Attr(datetime)
+    child_model_attr: Attr(PymodelioChildModel)
+    children_model_attr: Attr(List[PymodelioChildModel])
+    optional_attr: Attr(dict, default_factory=dict)
+    non_initable_attr: Attr(List[str], initable=False, default_factory=list)
 
+```
```

## Comparing `pymodelio-1.0.0.dist-info/RECORD` & `pymodelio-1.0.1.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-pymodelio/__init__.py,sha256=vncU2bJl2eB5Vj6V0MdzKJVVZX18ckvHxqtG1y3Q4H0,614
-pymodelio/attribute.py,sha256=thQZtwQYC0fbw5RaTUTONzE8iLLwfURTpyJx_6wpQIw,1744
-pymodelio/base_model.py,sha256=TzaK3bo7ptBFKClxggkJUb1WYybq3TKDb6AepObxB3o,8979
+pymodelio/__init__.py,sha256=7HQ1Ty_lJH5YwuVS0180GrWFXe2xkwm2JnPtfhnEg6E,374
+pymodelio/attribute.py,sha256=W9z_mZg6892XqqQ_t1fvwHJG-cJ7UyrGNUHdvcSwlQU,1882
 pymodelio/constants.py,sha256=qDMrr5LAO8nm9yVfWJbCJ6MV9WenSypNm4GBVopNgwY,67
-pymodelio/model_serializer.py,sha256=iRXVXfDCMJlKjsCKBemXwlciLheE6Ojsu0VDU0my4tE,1489
-pymodelio/shared_vars.py,sha256=wRZmgVx1Y49mcwOLdIdkLCfpDlLsk4WhKflTDqlvH8o,115
+pymodelio/model_serializer.py,sha256=S3Ywak4tdorwSYsI4mvUMRXlA7d8H0_fC6wvHOl5YU0,845
+pymodelio/pymodelio_cache.py,sha256=BQ9tWj8oIcTBIqlwI_-XR3Nm4DAadLy6OVZSgmr-W84,408
+pymodelio/pymodelio_model.py,sha256=F108FflmfmH0K01tpstG-gOeYaBHj6vz4IIQ0ymL1Ho,11024
+pymodelio/shared_vars.py,sha256=grXRCAaGUhOG1-tENkcZgJEndtZJSQvF_QU7qbRjycc,44
 pymodelio/undefined.py,sha256=dvmNY7_3EmfidEGomJNzWXkOdbg8VfJski1t05mniH0,88
+pymodelio/utils.py,sha256=tjtv8aFhsqu3XKorq6UtJDx541L4stPJOgGla6tINWU,399
 pymodelio/decorators/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pymodelio/decorators/do_not_serialize.py,sha256=4XoufTgS3g0HYSPVc-8_oYKMMf3d1XYIJgF5Bz3-kp8,495
-pymodelio/decorators/model.py,sha256=vY29pSXx-GbUS1RZjy5mSR6juxyGoGMRjrWf0mbbo1k,1315
-pymodelio/decorators/overrides_child_always.py,sha256=GluQ3E40hLvjDoE0zmbhV7CI1raGD2J-sBmlyOPpXps,206
-pymodelio/decorators/overrides_child_if_not_implemented.py,sha256=Pc2wNurXWgFxGgQZsFoNhhiRl9iFHbP73TXmiUaViMk,230
-pymodelio/exceptions/__init__.py,sha256=n6flrcyGG9PMIpEzrmV9DdHd4-H4-P-Zmlr__HeYnQM,80
+pymodelio/decorators/pymodelio_cached.py,sha256=C2tz_A1omw_meDO7QZmZLnj8V_yYbkQd9FD3VRQgW_A,761
+pymodelio/exceptions/__init__.py,sha256=xufuLIo1wPqOVDrYisHdUOl51-GPe_bWKesAb89FFAo,158
+pymodelio/exceptions/auto_validator_creation_exception.py,sha256=gAlViH6kPTq8hWE6uCGHmImhXM16eAmXUGDpy1Z0jMk,58
 pymodelio/exceptions/model_validation_exception.py,sha256=JfxWxtfdT3Y6ruigYs8X8usBIJC4dwSte3r7oPGUxb8,52
 pymodelio/settings/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pymodelio/settings/pymodelio_setting.py,sha256=YpbyfSTT2T1kDUdc55OYtGe5WJMEbSIXP-297jBQ0jE,194
-pymodelio/settings/pymodelio_settings.py,sha256=F21ezhmXJAy7RgxeSnJk76qUy_-fYcvChJm-gJQHx_M,854
-pymodelio/validators/__init__.py,sha256=0pv7D0MoxYiiWjfPt0-g7ydUFhmIjXnJSJagZXkrO5g,496
+pymodelio/settings/pymodelio_setting.py,sha256=iaG5QqJHLqWJcbV2KPVOnu40qU8pmrRJ2pOGTpn6_p0,398
+pymodelio/settings/pymodelio_settings.py,sha256=4BqMNG9Rx9PNRk1aOV2G4aWKyHH5eVPtFUEfblKjXXE,1040
+pymodelio/validators/__init__.py,sha256=D2ACgRBgX97IRmKurhDZNegxtW_6ZYnUioqocYMRQkc,635
 pymodelio/validators/bool_validator.py,sha256=KHTd2I0QRUX-8Lcrxvtg1wqLZvsMotlwv1VpCiZi-cc,285
 pymodelio/validators/datetime_validator.py,sha256=TZ9Pt_zJZT49OIhAZyf7U37bKWesHQXpJoy6bg6mCjc,323
+pymodelio/validators/default_validators_builder.py,sha256=9Zgu19bYtPtqbEZvxdINWGDa3d9p9WeDJWapO-tNkA0,5503
 pymodelio/validators/dict_validator.py,sha256=Y_NmLEFdySBbuDcEdbPCVRF3Sf_mrnyUbdROA8zwSTk,285
 pymodelio/validators/email_validator.py,sha256=xFHPHRNoznLWnd8QVuEbH9BSJxnoszR1RgdkOVCXwN0,752
 pymodelio/validators/float_validator.py,sha256=LOy0OEYn7_7FxILFVngYd24gYEeUF6D5IFJCc44PVXI,463
+pymodelio/validators/forward_ref_validator.py,sha256=8uk-vdrX9TPmg7CnNEhAxPm_mlt1D3o8SCqymddoJyo,961
 pymodelio/validators/int_validator.py,sha256=_3TJIKZN9G8wprtizbV4JgBiNX2rvsiZmugHjRcno54,455
-pymodelio/validators/iterable_validator.py,sha256=tiOeDhC_mOFQuFAW9NvA5UgapKRnINIzJI6LeGMcvfQ,1324
+pymodelio/validators/iterable_validator.py,sha256=3wvudiIEc1g6EPwcdSvhsngERooFmtv-DkvZKawJK-4,1327
 pymodelio/validators/list_validator.py,sha256=T5-7KDGyLsg8o7WFAO7djOkKLGrmqzb9Q8Pv2TcvuvY,473
-pymodelio/validators/numeric_validator.py,sha256=74YJ2cYT-EGMEnk1_1NAmU1dCB-e1QTObEtz2eGfoVM,1007
-pymodelio/validators/string_validator.py,sha256=b3g0H9Z8kaVql2KPzs0JRG2-NDmzvJeCijFfzb9A8G8,1335
+pymodelio/validators/numeric_validator.py,sha256=M6TpOVg69P460AvBPeu32_sGv9xE_TedmC9nXl7peaA,1010
+pymodelio/validators/set_validator.py,sha256=X7XcbS6Az4E9snK4g_Vr6jXEnGJTY4qGBOQ8HC8ycUQ,471
+pymodelio/validators/string_validator.py,sha256=HidLUkuIYmDhDIZuWa5LYVX6w1rm2XupYhzQY_G9rZM,1341
+pymodelio/validators/tuple_validator.py,sha256=GLva3HKUmGWTfohgfC1mW2q7DfPl_qIQ5RAH6V8KWt4,475
 pymodelio/validators/validation_patterns.py,sha256=-gSYH0dt_J-K2A10VeAv6bEIi4TRV8x8OWLkYuLZrk4,274
-pymodelio/validators/validator.py,sha256=kxX8w7nhSf1K460ypwyeEqmPEsHwrxTGax_SRDqgFu8,1368
-pymodelio-1.0.0.dist-info/LICENSE.txt,sha256=sL92kzk5LocRUegJuJvjbS-U5nceM2IAKHEUIavtJ90,1070
-pymodelio-1.0.0.dist-info/METADATA,sha256=KPwCGL-saUOtFigwMI3TrmFR94W0_5fXe1HQeEYdqes,19679
-pymodelio-1.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pymodelio-1.0.0.dist-info/top_level.txt,sha256=XrPsEjrAMkBQoxcrC6tFQs-EiY6TbHuDV5I68o5ZZyE,10
-pymodelio-1.0.0.dist-info/RECORD,,
+pymodelio/validators/validator.py,sha256=nASHjjGKtPqkN1ClaHnoIkipG7Lmo24fmtJl0tkyLUE,1368
+pymodelio-1.0.1.dist-info/LICENSE.txt,sha256=sL92kzk5LocRUegJuJvjbS-U5nceM2IAKHEUIavtJ90,1070
+pymodelio-1.0.1.dist-info/METADATA,sha256=oIplWhDSyD7xK_gt1K_Il2B7kHE2yN9WyLt48YA-Uvo,24463
+pymodelio-1.0.1.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+pymodelio-1.0.1.dist-info/top_level.txt,sha256=XrPsEjrAMkBQoxcrC6tFQs-EiY6TbHuDV5I68o5ZZyE,10
+pymodelio-1.0.1.dist-info/RECORD,,
```

