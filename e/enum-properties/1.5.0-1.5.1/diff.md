# Comparing `tmp/enum_properties-1.5.0.tar.gz` & `tmp/enum_properties-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "enum_properties-1.5.0.tar", max compression
+gzip compressed data, was "enum_properties-1.5.1.tar", max compression
```

## Comparing `enum_properties-1.5.0.tar` & `enum_properties-1.5.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.5.0/LICENSE
--rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.5.0/README.rst
--rw-r--r--   0        0        0    22832 2023-04-16 00:18:17.368670 enum_properties-1.5.0/enum_properties/__init__.py
--rw-r--r--   0        0        0     1878 2023-04-15 23:04:18.596595 enum_properties-1.5.0/pyproject.toml
--rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 enum_properties-1.5.0/setup.py
--rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-02-16 05:48:06.639467 enum_properties-1.5.1/LICENSE
+-rw-r--r--   0        0        0     4345 2023-04-08 09:04:38.023115 enum_properties-1.5.1/README.rst
+-rw-r--r--   0        0        0    22922 2023-04-18 06:27:52.684685 enum_properties-1.5.1/enum_properties/__init__.py
+-rw-r--r--   0        0        0     1878 2023-04-18 06:27:52.693441 enum_properties-1.5.1/pyproject.toml
+-rw-r--r--   0        0        0     5804 1970-01-01 00:00:00.000000 enum_properties-1.5.1/PKG-INFO
```

### Comparing `enum_properties-1.5.0/LICENSE` & `enum_properties-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `enum_properties-1.5.0/README.rst` & `enum_properties-1.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `enum_properties-1.5.0/enum_properties/__init__.py` & `enum_properties-1.5.1/enum_properties/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 try:
     from functools import cached_property
 except ImportError:  # pragma: no cover
     # todo remove when python 3.7 support is dropped
     cached_property = property  # pylint: disable=C0103
 
 
-VERSION = (1, 5, 0)
+VERSION = (1, 5, 1)
 
 __title__ = 'Enum Properties'
 __version__ = '.'.join(str(i) for i in VERSION)
 __author__ = 'Brian Kohan'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2022-2023 Brian Kohan'
 
@@ -214,32 +214,33 @@
 
         if isinstance(value, str):
             try:
                 return cls._ep_isymmetric_map_[_do_casenorm(value)]
             except KeyError:
                 pass
 
-        for coerce_to in cls._ep_coerce_types_:
-            try:
-                val = coerce_to(value)
+        if value is not None:
+            for coerce_to in cls._ep_coerce_types_:
                 try:
-                    return cls._value2member_map_[val]
-                except KeyError:
-                    pass
+                    val = coerce_to(value)
+                    try:
+                        return cls._value2member_map_[val]
+                    except KeyError:
+                        pass
+
+                    try:
+                        return cls._ep_symmetric_map_[val]
+                    except KeyError:
+                        pass
 
-                try:
-                    return cls._ep_symmetric_map_[val]
-                except KeyError:
-                    pass
+                    if isinstance(val, str):
+                        return cls._ep_isymmetric_map_[_do_casenorm(val)]
 
-                if isinstance(val, str):
-                    return cls._ep_isymmetric_map_[_do_casenorm(val)]
-
-            except (KeyError, TypeError, ValueError):
-                pass
+                except (KeyError, TypeError, ValueError):
+                    pass
 
         return super()._missing_(value)
 
 
 class EnumPropertiesMeta(enum.EnumMeta):
     """
     A metaclass for creating enum choices with additional named properties for
```

### Comparing `enum_properties-1.5.0/pyproject.toml` & `enum_properties-1.5.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "enum-properties"
-version = "1.5.0"
+version = "1.5.1"
 description = "Add properties and method specializations to Python enumeration values with a simple declarative syntax."
 authors = ["Brian Kohan <bckohan@gmail.com>"]
 license = "MIT"
 repository = "https://github.com/bckohan/enum-properties"
 homepage = "https://enum-properties.readthedocs.io"
 readme = "README.rst"
 keywords = ["enum",  "properties", "defines", "field"]
```

### Comparing `enum_properties-1.5.0/PKG-INFO` & `enum_properties-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: enum-properties
-Version: 1.5.0
+Version: 1.5.1
 Summary: Add properties and method specializations to Python enumeration values with a simple declarative syntax.
 Home-page: https://enum-properties.readthedocs.io
 License: MIT
 Keywords: enum,properties,defines,field
 Author: Brian Kohan
 Author-email: bckohan@gmail.com
 Requires-Python: >=3.7,<4.0
```

