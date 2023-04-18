# Comparing `tmp/schemey-6.0.0.tar.gz` & `tmp/schemey-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/schemey-6.0.0.tar", last modified: Tue Apr 18 21:24:36 2023, max compression
+gzip compressed data, was "dist/schemey-6.0.1.tar", last modified: Tue Apr 18 21:32:51 2023, max compression
```

## Comparing `schemey-6.0.0.tar` & `schemey-6.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/
--rw-r--r--   0 tofarr     (501) staff       (20)     3879 2023-04-18 21:24:36.000000 schemey-6.0.0/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     3441 2023-01-15 16:34:55.000000 schemey-6.0.0/README.md
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/marshy_config_schemey/
--rw-r--r--   0 tofarr     (501) staff       (20)      225 2022-07-28 13:03:35.000000 schemey-6.0.0/marshy_config_schemey/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey/
--rw-r--r--   0 tofarr     (501) staff       (20)     1414 2022-07-28 21:35:38.000000 schemey-6.0.0/schemey/__init__.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey/factory/
--rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-27 21:59:06.000000 schemey-6.0.0/schemey/factory/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1398 2023-01-15 15:35:44.000000 schemey-6.0.0/schemey/factory/any_of_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2926 2023-01-15 15:27:56.000000 schemey-6.0.0/schemey/factory/array_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     5118 2023-01-15 15:35:53.000000 schemey-6.0.0/schemey/factory/dataclass_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1036 2023-01-15 15:27:52.000000 schemey-6.0.0/schemey/factory/datetime_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1260 2023-04-18 21:19:24.000000 schemey-6.0.0/schemey/factory/enum_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1216 2023-01-15 15:28:00.000000 schemey-6.0.0/schemey/factory/external_type_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      874 2022-12-23 00:16:46.000000 schemey-6.0.0/schemey/factory/factory_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     2695 2023-01-15 15:27:40.000000 schemey-6.0.0/schemey/factory/impl_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)      767 2022-12-23 00:16:46.000000 schemey-6.0.0/schemey/factory/ref_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1052 2022-12-22 23:47:30.000000 schemey-6.0.0/schemey/factory/schema_factory_abc.py
--rw-r--r--   0 tofarr     (501) staff       (20)      960 2023-01-15 15:27:44.000000 schemey-6.0.0/schemey/factory/simple_type_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1744 2023-01-15 15:27:47.000000 schemey-6.0.0/schemey/factory/tuple_schema_factory.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1003 2023-01-15 15:27:49.000000 schemey-6.0.0/schemey/factory/uuid_factory.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey/json_schema/
--rw-r--r--   0 tofarr     (501) staff       (20)      291 2023-01-15 15:42:18.000000 schemey-6.0.0/schemey/json_schema/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1185 2023-01-15 16:41:29.000000 schemey-6.0.0/schemey/json_schema/ranges.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1943 2023-01-15 17:25:49.000000 schemey-6.0.0/schemey/json_schema/timestamp.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3707 2023-03-11 00:43:10.000000 schemey-6.0.0/schemey/schema.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1831 2023-01-15 15:13:45.000000 schemey-6.0.0/schemey/schema_context.py
--rw-r--r--   0 tofarr     (501) staff       (20)      653 2022-07-29 12:27:06.000000 schemey-6.0.0/schemey/schema_marshaller.py
--rw-r--r--   0 tofarr     (501) staff       (20)      459 2022-11-30 22:21:30.000000 schemey-6.0.0/schemey/schemey_format_checker.py
--rw-r--r--   0 tofarr     (501) staff       (20)      230 2022-07-15 12:34:09.000000 schemey-6.0.0/schemey/string_format.py
--rw-r--r--   0 tofarr     (501) staff       (20)      109 2022-07-28 13:07:38.000000 schemey-6.0.0/schemey/util.py
--rw-r--r--   0 tofarr     (501) staff       (20)     3016 2022-12-23 00:16:46.000000 schemey-6.0.0/schemey/validated.py
--rw-r--r--   0 tofarr     (501) staff       (20)     1755 2022-07-28 21:44:55.000000 schemey-6.0.0/schemey/validator.py
--rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:18:18.000000 schemey-6.0.0/schemey/version.py
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey.egg-info/
--rw-r--r--   0 tofarr     (501) staff       (20)     3879 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey.egg-info/PKG-INFO
--rw-r--r--   0 tofarr     (501) staff       (20)     1102 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey.egg-info/SOURCES.txt
--rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey.egg-info/dependency_links.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       28 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey.egg-info/requires.txt
--rw-r--r--   0 tofarr     (501) staff       (20)       53 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey.egg-info/top_level.txt
-drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:24:36.000000 schemey-6.0.0/schemey_config_default/
--rw-r--r--   0 tofarr     (501) staff       (20)     2079 2023-01-15 15:58:18.000000 schemey-6.0.0/schemey_config_default/__init__.py
--rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:24:36.000000 schemey-6.0.0/setup.cfg
--rw-r--r--   0 tofarr     (501) staff       (20)      763 2022-11-30 22:16:28.000000 schemey-6.0.0/setup.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/
+-rw-r--r--   0 tofarr     (501) staff       (20)     3879 2023-04-18 21:32:51.000000 schemey-6.0.1/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     3441 2023-01-15 16:34:55.000000 schemey-6.0.1/README.md
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/marshy_config_schemey/
+-rw-r--r--   0 tofarr     (501) staff       (20)      225 2022-07-28 13:03:35.000000 schemey-6.0.1/marshy_config_schemey/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey/
+-rw-r--r--   0 tofarr     (501) staff       (20)     1414 2022-07-28 21:35:38.000000 schemey-6.0.1/schemey/__init__.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey/factory/
+-rw-r--r--   0 tofarr     (501) staff       (20)        0 2022-07-27 21:59:06.000000 schemey-6.0.1/schemey/factory/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1398 2023-01-15 15:35:44.000000 schemey-6.0.1/schemey/factory/any_of_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2926 2023-01-15 15:27:56.000000 schemey-6.0.1/schemey/factory/array_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     5118 2023-01-15 15:35:53.000000 schemey-6.0.1/schemey/factory/dataclass_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1036 2023-01-15 15:27:52.000000 schemey-6.0.1/schemey/factory/datetime_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1260 2023-04-18 21:19:24.000000 schemey-6.0.1/schemey/factory/enum_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1216 2023-01-15 15:28:00.000000 schemey-6.0.1/schemey/factory/external_type_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      874 2022-12-23 00:16:46.000000 schemey-6.0.1/schemey/factory/factory_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     2695 2023-01-15 15:27:40.000000 schemey-6.0.1/schemey/factory/impl_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      767 2022-12-23 00:16:46.000000 schemey-6.0.1/schemey/factory/ref_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1052 2022-12-22 23:47:30.000000 schemey-6.0.1/schemey/factory/schema_factory_abc.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      960 2023-01-15 15:27:44.000000 schemey-6.0.1/schemey/factory/simple_type_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1744 2023-01-15 15:27:47.000000 schemey-6.0.1/schemey/factory/tuple_schema_factory.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1003 2023-01-15 15:27:49.000000 schemey-6.0.1/schemey/factory/uuid_factory.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey/json_schema/
+-rw-r--r--   0 tofarr     (501) staff       (20)      291 2023-01-15 15:42:18.000000 schemey-6.0.1/schemey/json_schema/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1185 2023-01-15 16:41:29.000000 schemey-6.0.1/schemey/json_schema/ranges.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1943 2023-01-15 17:25:49.000000 schemey-6.0.1/schemey/json_schema/timestamp.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3707 2023-03-11 00:43:10.000000 schemey-6.0.1/schemey/schema.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1831 2023-01-15 15:13:45.000000 schemey-6.0.1/schemey/schema_context.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      653 2022-07-29 12:27:06.000000 schemey-6.0.1/schemey/schema_marshaller.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      459 2022-11-30 22:21:30.000000 schemey-6.0.1/schemey/schemey_format_checker.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      230 2022-07-15 12:34:09.000000 schemey-6.0.1/schemey/string_format.py
+-rw-r--r--   0 tofarr     (501) staff       (20)      109 2022-07-28 13:07:38.000000 schemey-6.0.1/schemey/util.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     3016 2022-12-23 00:16:46.000000 schemey-6.0.1/schemey/validated.py
+-rw-r--r--   0 tofarr     (501) staff       (20)     1755 2022-07-28 21:44:55.000000 schemey-6.0.1/schemey/validator.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       22 2023-04-18 21:32:19.000000 schemey-6.0.1/schemey/version.py
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/
+-rw-r--r--   0 tofarr     (501) staff       (20)     3879 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/PKG-INFO
+-rw-r--r--   0 tofarr     (501) staff       (20)     1102 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/SOURCES.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)        1 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/dependency_links.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       28 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/requires.txt
+-rw-r--r--   0 tofarr     (501) staff       (20)       53 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey.egg-info/top_level.txt
+drwxr-xr-x   0 tofarr     (501) staff       (20)        0 2023-04-18 21:32:51.000000 schemey-6.0.1/schemey_config_default/
+-rw-r--r--   0 tofarr     (501) staff       (20)     2079 2023-01-15 15:58:18.000000 schemey-6.0.1/schemey_config_default/__init__.py
+-rw-r--r--   0 tofarr     (501) staff       (20)       38 2023-04-18 21:32:51.000000 schemey-6.0.1/setup.cfg
+-rw-r--r--   0 tofarr     (501) staff       (20)      763 2023-04-18 21:32:19.000000 schemey-6.0.1/setup.py
```

### Comparing `schemey-6.0.0/PKG-INFO` & `schemey-6.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemey
-Version: 6.0.0
+Version: 6.0.1
 Summary: Convention over configuration Object Schemas for python
 Home-page: https://github.com/tofarr/schemey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schemey-6.0.0/README.md` & `schemey-6.0.1/README.md`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/__init__.py` & `schemey-6.0.1/schemey/__init__.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/any_of_schema_factory.py` & `schemey-6.0.1/schemey/factory/any_of_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/array_schema_factory.py` & `schemey-6.0.1/schemey/factory/array_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/dataclass_schema_factory.py` & `schemey-6.0.1/schemey/factory/dataclass_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/datetime_factory.py` & `schemey-6.0.1/schemey/factory/datetime_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/enum_schema_factory.py` & `schemey-6.0.1/schemey/factory/enum_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/external_type_factory.py` & `schemey-6.0.1/schemey/factory/external_type_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/factory_schema_factory.py` & `schemey-6.0.1/schemey/factory/factory_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/impl_schema_factory.py` & `schemey-6.0.1/schemey/factory/impl_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/ref_schema_factory.py` & `schemey-6.0.1/schemey/factory/ref_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/schema_factory_abc.py` & `schemey-6.0.1/schemey/factory/schema_factory_abc.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/simple_type_factory.py` & `schemey-6.0.1/schemey/factory/simple_type_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/tuple_schema_factory.py` & `schemey-6.0.1/schemey/factory/tuple_schema_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/factory/uuid_factory.py` & `schemey-6.0.1/schemey/factory/uuid_factory.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/json_schema/ranges.py` & `schemey-6.0.1/schemey/json_schema/ranges.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/json_schema/timestamp.py` & `schemey-6.0.1/schemey/json_schema/timestamp.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/schema.py` & `schemey-6.0.1/schemey/schema.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/schema_context.py` & `schemey-6.0.1/schemey/schema_context.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/schema_marshaller.py` & `schemey-6.0.1/schemey/schema_marshaller.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/validated.py` & `schemey-6.0.1/schemey/validated.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey/validator.py` & `schemey-6.0.1/schemey/validator.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey.egg-info/PKG-INFO` & `schemey-6.0.1/schemey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemey
-Version: 6.0.0
+Version: 6.0.1
 Summary: Convention over configuration Object Schemas for python
 Home-page: https://github.com/tofarr/schemey
 Author: Tim O'Farrell
 Author-email: tofarr@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schemey-6.0.0/schemey.egg-info/SOURCES.txt` & `schemey-6.0.1/schemey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/schemey_config_default/__init__.py` & `schemey-6.0.1/schemey_config_default/__init__.py`

 * *Files identical despite different names*

### Comparing `schemey-6.0.0/setup.py` & `schemey-6.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,14 @@
     author="Tim O'Farrell",
     author_email="tofarr@gmail.com",
     description="Convention over configuration Object Schemas for python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/tofarr/schemey",
     packages=setuptools.find_packages(exclude=("tests", "tests.*")),
-    install_requires=["marshy~=3.0", "jsonschema~=4.8"],
+    install_requires=["marshy~=4.0", "jsonschema~=4.8"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

