# Comparing `tmp/ctor-0.3.3.tar.gz` & `tmp/ctor-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\ctor-0.3.3.tar", last modified: Sat Dec  3 09:48:32 2022, max compression
+gzip compressed data, was "dist\ctor-0.3.4.tar", last modified: Tue Apr 18 03:55:08 2023, max compression
```

## Comparing `ctor-0.3.3.tar` & `ctor-0.3.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-12-03 09:48:32.822016 ctor-0.3.3/
--rw-rw-rw-   0        0        0     1091 2021-12-19 17:16:50.000000 ctor-0.3.3/LICENSE
--rw-rw-rw-   0        0        0     5218 2022-12-03 09:48:32.821016 ctor-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0     4358 2021-12-19 20:02:17.000000 ctor-0.3.3/README.md
--rw-rw-rw-   0        0        0       42 2022-12-03 09:48:32.822016 ctor-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1381 2022-12-03 09:42:59.000000 ctor-0.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-12-03 09:48:32.797016 ctor-0.3.3/src/
-drwxrwxrwx   0        0        0        0 2022-12-03 09:48:32.810017 ctor-0.3.3/src/ctor/
--rw-rw-rw-   0        0        0      118 2022-04-25 20:58:16.000000 ctor-0.3.3/src/ctor/__init__.py
--rw-rw-rw-   0        0        0     2120 2022-04-26 22:21:21.000000 ctor-0.3.3/src/ctor/common.py
--rw-rw-rw-   0        0        0    38147 2022-12-03 09:45:11.000000 ctor-0.3.3/src/ctor/conversion.py
--rw-rw-rw-   0        0        0     2430 2022-04-25 20:48:01.000000 ctor-0.3.3/src/ctor/errors.py
--rw-rw-rw-   0        0        0        0 2022-04-25 20:39:25.000000 ctor-0.3.3/src/ctor/py.typed
--rw-rw-rw-   0        0        0     5799 2022-04-26 22:01:27.000000 ctor-0.3.3/src/ctor/typing_utils.py
-drwxrwxrwx   0        0        0        0 2022-12-03 09:48:32.819016 ctor-0.3.3/src/ctor.egg-info/
--rw-rw-rw-   0        0        0     5218 2022-12-03 09:48:32.000000 ctor-0.3.3/src/ctor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2022-12-03 09:48:32.000000 ctor-0.3.3/src/ctor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-03 09:48:32.000000 ctor-0.3.3/src/ctor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2022-12-03 09:48:32.000000 ctor-0.3.3/src/ctor.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2022-12-03 09:48:32.000000 ctor-0.3.3/src/ctor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 03:55:08.402097 ctor-0.3.4/
+-rw-rw-rw-   0        0        0     1091 2021-12-19 17:16:50.000000 ctor-0.3.4/LICENSE
+-rw-rw-rw-   0        0        0     5218 2023-04-18 03:55:08.402097 ctor-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4358 2021-12-19 20:02:17.000000 ctor-0.3.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 03:55:08.403097 ctor-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1381 2023-04-18 03:42:28.000000 ctor-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:55:08.378097 ctor-0.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-04-18 03:55:08.390097 ctor-0.3.4/src/ctor/
+-rw-rw-rw-   0        0        0      118 2022-04-25 20:58:16.000000 ctor-0.3.4/src/ctor/__init__.py
+-rw-rw-rw-   0        0        0     2120 2022-04-26 22:21:21.000000 ctor-0.3.4/src/ctor/common.py
+-rw-rw-rw-   0        0        0    38169 2023-04-18 03:46:22.000000 ctor-0.3.4/src/ctor/conversion.py
+-rw-rw-rw-   0        0        0     2430 2022-04-25 20:48:01.000000 ctor-0.3.4/src/ctor/errors.py
+-rw-rw-rw-   0        0        0        0 2022-04-25 20:39:25.000000 ctor-0.3.4/src/ctor/py.typed
+-rw-rw-rw-   0        0        0     5799 2022-04-26 22:01:27.000000 ctor-0.3.4/src/ctor/typing_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 03:55:08.400097 ctor-0.3.4/src/ctor.egg-info/
+-rw-rw-rw-   0        0        0     5218 2023-04-18 03:55:08.000000 ctor-0.3.4/src/ctor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      310 2023-04-18 03:55:08.000000 ctor-0.3.4/src/ctor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 03:55:08.000000 ctor-0.3.4/src/ctor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-04-18 03:55:08.000000 ctor-0.3.4/src/ctor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-04-18 03:55:08.000000 ctor-0.3.4/src/ctor.egg-info/top_level.txt
```

### Comparing `ctor-0.3.3/LICENSE` & `ctor-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ctor-0.3.3/PKG-INFO` & `ctor-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctor
-Version: 0.3.3
+Version: 0.3.4
 Summary: Object tree serialization library for python
 Home-page: https://github.com/bshishov/ctor
 Author: Boris Shishov
 Author-email: borisshishov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `ctor-0.3.3/README.md` & `ctor-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `ctor-0.3.3/setup.py` & `ctor-0.3.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ctor",
-    version="0.3.3",
+    version="0.3.4",
     description="Object tree serialization library for python",
     url="https://github.com/bshishov/ctor",
     author="Boris Shishov",
     author_email="borisshishov@gmail.com",
     long_description=long_description,
     long_description_content_type="text/markdown",
     package_dir={"": "src"},
```

### Comparing `ctor-0.3.3/src/ctor/common.py` & `ctor-0.3.4/src/ctor/common.py`

 * *Files identical despite different names*

### Comparing `ctor-0.3.3/src/ctor/conversion.py` & `ctor-0.3.4/src/ctor/conversion.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     Tuple,
     Any,
     Union,
     Generic,
     TypeVar,
     Type,
     overload,
+    Iterable,
 )
 
 from ctor.typing_utils import (
     ForwardRef,
     get_args,
     get_origin,
     eval_type,
@@ -407,15 +408,15 @@
         getter=getter,
     )
 
 
 class DiscriminatedConverter(Generic[_T], IConverter[_T]):
     def __init__(
         self,
-        converters: List[Tuple[str, TypeOrCallable[_T], IConverter[_T]]],
+        converters: Iterable[Tuple[str, TypeOrCallable[_T], IConverter[_T]]],
         discriminator_key: str = "type",
     ):
         self.discriminator_key = discriminator_key
         self.load_map = {}
         self.dump_map = {}
 
         for discriminator_value, typ, converter in converters:
@@ -510,15 +511,15 @@
 
 
 class DiscriminatedConverterFactory(IConverterFactory[_T]):
     __slots__ = "discriminator_type_map", "converter_factory", "discriminator_key"
 
     def __init__(
         self,
-        discriminator_type_map: Dict[str, TypeOrCallable[_T]],
+        discriminator_type_map: Mapping[str, TypeOrCallable[_T]],
         converter_factory: IConverterFactory[_T],
         discriminator_key: str = "type",
     ):
         self.discriminator_type_map = discriminator_type_map
         self.converter_factory = converter_factory
         self.discriminator_key = discriminator_key
```

### Comparing `ctor-0.3.3/src/ctor/errors.py` & `ctor-0.3.4/src/ctor/errors.py`

 * *Files identical despite different names*

### Comparing `ctor-0.3.3/src/ctor/typing_utils.py` & `ctor-0.3.4/src/ctor/typing_utils.py`

 * *Files identical despite different names*

### Comparing `ctor-0.3.3/src/ctor.egg-info/PKG-INFO` & `ctor-0.3.4/src/ctor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctor
-Version: 0.3.3
+Version: 0.3.4
 Summary: Object tree serialization library for python
 Home-page: https://github.com/bshishov/ctor
 Author: Boris Shishov
 Author-email: borisshishov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

