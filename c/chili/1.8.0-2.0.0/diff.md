# Comparing `tmp/chili-1.8.0.tar.gz` & `tmp/chili-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chili-1.8.0.tar", max compression
+gzip compressed data, was "chili-2.0.0.tar", max compression
```

## Comparing `chili-1.8.0.tar` & `chili-2.0.0.tar`

### file list

```diff
@@ -1,13 +1,16 @@
--rw-r--r--   0        0        0    19882 2022-09-26 05:17:23.730178 chili-1.8.0/README.md
--rw-r--r--   0        0        0      452 2022-09-26 05:17:23.730178 chili-1.8.0/chili/__init__.py
--rw-r--r--   0        0        0       22 2022-09-26 05:17:23.730178 chili-1.8.0/chili/__version__.py
--rw-r--r--   0        0        0      577 2022-09-26 05:17:23.730178 chili-1.8.0/chili/dataclasses.py
--rw-r--r--   0        0        0     1218 2022-09-26 05:17:23.730178 chili-1.8.0/chili/error.py
--rw-r--r--   0        0        0    22142 2022-09-26 05:17:23.730178 chili-1.8.0/chili/hydration.py
--rw-r--r--   0        0        0     5740 2022-09-26 05:17:23.730178 chili-1.8.0/chili/iso_datetime.py
--rw-r--r--   0        0        0     2418 2022-09-26 05:17:23.730178 chili-1.8.0/chili/mapping.py
--rw-r--r--   0        0        0        0 2022-09-26 05:17:23.730178 chili-1.8.0/chili/py.typed
--rw-r--r--   0        0        0     1968 2022-09-26 05:17:23.730178 chili-1.8.0/chili/typing.py
--rw-r--r--   0        0        0     1290 2022-09-26 05:17:23.730178 chili-1.8.0/pyproject.toml
--rw-r--r--   0        0        0    21421 1970-01-01 00:00:00.000000 chili-1.8.0/setup.py
--rw-r--r--   0        0        0    21252 1970-01-01 00:00:00.000000 chili-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-04-18 05:11:12.568292 chili-2.0.0/LICENSE
+-rw-r--r--   0        0        0    11664 2023-04-18 05:11:12.568292 chili-2.0.0/README.md
+-rw-r--r--   0        0        0      614 2023-04-18 05:11:12.568292 chili-2.0.0/chili/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-18 05:11:12.568292 chili-2.0.0/chili/__version__.py
+-rw-r--r--   0        0        0    16042 2023-04-18 05:11:12.568292 chili-2.0.0/chili/decoder.py
+-rw-r--r--   0        0        0    13956 2023-04-18 05:11:12.568292 chili-2.0.0/chili/encoder.py
+-rw-r--r--   0        0        0      411 2023-04-18 05:11:12.568292 chili-2.0.0/chili/error.py
+-rw-r--r--   0        0        0     5741 2023-04-18 05:11:12.568292 chili-2.0.0/chili/iso_datetime.py
+-rw-r--r--   0        0        0     1093 2023-04-18 05:11:12.568292 chili-2.0.0/chili/json_support.py
+-rw-r--r--   0        0        0     3155 2023-04-18 05:11:12.568292 chili-2.0.0/chili/mapper.py
+-rw-r--r--   0        0        0        0 2023-04-18 05:11:12.568292 chili-2.0.0/chili/py.typed
+-rw-r--r--   0        0        0     1513 2023-04-18 05:11:12.568292 chili-2.0.0/chili/serializer.py
+-rw-r--r--   0        0        0      260 2023-04-18 05:11:12.568292 chili-2.0.0/chili/state.py
+-rw-r--r--   0        0        0     6043 2023-04-18 05:11:12.568292 chili-2.0.0/chili/typing.py
+-rw-r--r--   0        0        0     1228 2023-04-18 05:11:12.568292 chili-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13059 1970-01-01 00:00:00.000000 chili-2.0.0/PKG-INFO
```

### Comparing `chili-1.8.0/chili/iso_datetime.py` & `chili-2.0.0/chili/iso_datetime.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 import re
 from datetime import date, datetime, time, timedelta, timezone
 
+
+__all__ = [
+    "parse_iso_datetime",
+    "parse_iso_date",
+    "parse_iso_duration",
+    "parse_iso_time",
+    "timedelta_to_iso_duration",
+]
+
+
 ISO_8601_DATETIME_REGEX = re.compile(
     r"^(\d{4})-?([0-1]\d)-?([0-3]\d)[t\s]?([0-2]\d:?[0-5]\d:?[0-5]\d|23:59:60|235960)(\.\d+)?(z|[+-]\d{2}:\d{2})?$",
     re.I,
 )
 ISO_8601_DATE_REGEX = re.compile(r"^(\d{4})-?([0-1]\d)-?([0-3]\d)$", re.I)
 ISO_8601_TIME_REGEX = re.compile(
     r"^(?P<time>[0-2]\d:?[0-5]\d:?[0-5]\d|23:59:60|235960)(?P<microseconds>\.\d+)?(?P<tzpart>z|[+-]\d{2}:\d{2})?$",
@@ -155,16 +165,7 @@
     if seconds:
         if seconds.is_integer():
             iso_8601_time += f"{int(seconds)}S"
         else:
             iso_8601_time += f"{seconds}S"
 
     return f"{iso_8601}{iso_8601_date}" + (f"T{iso_8601_time}" if iso_8601_time else "")
-
-
-__all__ = [
-    "parse_iso_datetime",
-    "parse_iso_date",
-    "parse_iso_duration",
-    "parse_iso_time",
-    "timedelta_to_iso_duration",
-]
```

### Comparing `chili-1.8.0/chili/mapping.py` & `chili-2.0.0/chili/mapper.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,80 @@
 from collections import namedtuple
 from collections.abc import Iterable
 from typing import Any, Callable, Dict, Union
 
-KeyMapper = namedtuple("KeyMapper", "key scheme")
-MappingScheme = Dict[str, Union[Dict, str, Callable]]
+from chili.error import MapperError
+
+KeyScheme = namedtuple("KeyScheme", "key scheme")
+MappingScheme = Dict[str, Union[Dict, str, Callable, KeyScheme]]
 
 
 class Mapper:
-    def __init__(self, scheme: MappingScheme):
+    def __init__(self, scheme: Union[MappingScheme]):
         self.scheme = scheme
 
-    def map(self, data) -> Any:
-        return self._map(data, self.scheme)
+    def map(self, data: Dict[str, Any], skip_keys: bool = False, default_value: Any = None) -> Dict[str, Any]:
+        return self._map(data, self.scheme, skip_keys, default_value)
 
-    def _map(self, data: Dict, scheme: MappingScheme) -> Any:
+    def _map(self, data: Dict, scheme: MappingScheme, skip_keys: bool, default_value: Any = None) -> Any:
         result = {}
+        evaluated_keys = set()
         for new_key, old_key in scheme.items():
-            if isinstance(old_key, int):
-                if old_key:
-                    result[new_key] = data.get(new_key, None)
+            k_type = type(old_key)
+
+            if new_key is Ellipsis:
+                map_key = callable(old_key)
+                if k_type not in (int, bool) and not map_key:
+                    raise MapperError.invalid_schema
+
+                for key, value in data.items():
+                    if key in evaluated_keys:
+                        continue
+                    evaluated_keys.add(key)
+
+                    if map_key:
+                        key, value = old_key(key, value)  # type: ignore
+                    result[key] = value
                 continue
-            elif isinstance(old_key, str):
-                result[new_key] = data.get(old_key, None)
+            elif k_type is int or k_type is bool:
+                if old_key:
+                    evaluated_keys.add(old_key)
+                    if skip_keys and old_key not in data:
+                        continue
+                    result[new_key] = data.get(new_key, default_value)
+                continue
+            elif k_type is str:
+                evaluated_keys.add(old_key)
+                if skip_keys and old_key not in data:
+                    continue
+                result[new_key] = data.get(old_key, default_value)
                 continue
-            elif isinstance(old_key, KeyMapper):
-                if old_key.key not in data:
-                    result[new_key] = None
-                value = data[old_key.key]
-                item_scheme = old_key.scheme
-            elif isinstance(old_key, dict):
-                if new_key not in data:
-                    result[new_key] = None
+            elif k_type is KeyScheme:
+                if skip_keys and old_key.key not in data:  # type: ignore
+                    continue
+                value = data.get(old_key.key, default_value)  # type: ignore
+                item_scheme = old_key.scheme  # type: ignore
+            elif k_type is dict:
+                if skip_keys and new_key not in data:
                     continue
-                value = data[new_key]
+                value = data.get(new_key, default_value)
                 item_scheme = old_key
             elif callable(old_key):
+                evaluated_keys.add(old_key)
                 result[new_key] = old_key(data)
                 continue
             else:
-                raise ValueError(
-                    f"Unexpected mapping schema passed in `{new_key}`, "
-                    f"expected string, callable, bool or instance of KeyMapper."
-                )
+                raise MapperError.invalid_schema
 
             if callable(item_scheme):
                 result[new_key] = item_scheme(value)
                 continue
             elif isinstance(value, dict):
-                result[new_key] = self._map(value, item_scheme)
+                result[new_key] = self._map(value, item_scheme, skip_keys, default_value)
                 continue
             elif isinstance(value, Iterable):
-                result[new_key] = [self._map(item, item_scheme) for item in iter(value)]
+                result[new_key] = [self._map(item, item_scheme, skip_keys, default_value) for item in iter(value)]
                 continue
             else:
-                raise ValueError(f"Could not map value {value} with provided scheme {item_scheme}")
+                raise MapperError.invalid_value
 
         return result
-
-
-class PersistentMapper(Mapper):
-    def _map(self, data: Dict, scheme: MappingScheme) -> Any:
-        results = super()._map(data, scheme)
-        for key, value in data.items():
-            if key not in results:
-                results[key] = value
-        return results
```

### Comparing `chili-1.8.0/pyproject.toml` & `chili-2.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -10,30 +10,30 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: Software Development :: Code Generators",
     "Topic :: Utilities",
 ]
-description = "Chili is a dataclass support library. It is providing simple and fast hydration and extraction interfaces for dataclasses."
+description = "Chili is serialisation library. It can serialise/deserialise almost any object."
 documentation = "https://github.com/kodemore/chili"
 homepage = "https://github.com/kodemore/chili"
-keywords = ["dataclasses", "dataclass", "library", "mapping", "dto", "hydration", "extraction"]
+keywords = ["serialise", "deserialise", "encode", "decode", "object", "class"]
 license = "MIT"
 name = "chili"
 readme = "README.md"
 repository = "https://github.com/kodemore/chili"
-version = "1.8.0"
+version = "2.0.0"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 typing-extensions = "^4.2"
+gaffe = "0.2.0"
 
 [tool.poetry.dev-dependencies]
-bandit = "^1.7.4"
 black = "22.3"
 flake8 = "^5.0.4"
 isort = "^5.6.4"
 mypy = "^0.961"
 pylint = "^2.7.2"
 pytest = "^7.1"
 pytest-cov = "^3.0"
```

