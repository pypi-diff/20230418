# Comparing `tmp/python_property_based_testing-0.3.0.tar.gz` & `tmp/python_property_based_testing-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_property_based_testing-0.3.0.tar", max compression
+gzip compressed data, was "python_property_based_testing-0.4.0.tar", max compression
```

## Comparing `python_property_based_testing-0.3.0.tar` & `python_property_based_testing-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/LICENSE
--rw-r--r--   0        0        0     8292 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/README.md
--rw-r--r--   0        0        0        0 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/core/__init__.py
--rw-r--r--   0        0        0     6720 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/core/core.py
--rw-r--r--   0        0        0     3195 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/core/util.py
--rw-r--r--   0        0        0        0 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/tests/__init__.py
--rw-r--r--   0        0        0      575 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/tests/simple_nonclass_test.py
--rw-r--r--   0        0        0      628 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pybt/tests/simple_unit_test.py
--rw-r--r--   0        0        0      425 2023-04-17 10:35:01.900560 python_property_based_testing-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     8634 1970-01-01 00:00:00.000000 python_property_based_testing-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/core/__init__.py
+-rw-r--r--   0        0        0     6635 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/core/core.py
+-rw-r--r--   0        0        0     3195 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/core/util.py
+-rw-r--r--   0        0        0        0 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/tests/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/tests/simple_nonclass_test.py
+-rw-r--r--   0        0        0      628 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pybt/tests/simple_unit_test.py
+-rw-r--r--   0        0        0      425 2023-04-18 14:34:14.769258 python_property_based_testing-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8634 1970-01-01 00:00:00.000000 python_property_based_testing-0.4.0/PKG-INFO
```

### Comparing `python_property_based_testing-0.3.0/LICENSE` & `python_property_based_testing-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.3.0/README.md` & `python_property_based_testing-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.3.0/pybt/core/core.py` & `python_property_based_testing-0.4.0/pybt/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,17 +30,14 @@
 DATA_STRUCT_TYPE_MAP = {
     dict: lambda s, d: partial(gen_dict, s, d),
     list: lambda s, l: partial(gen_list, s, l),
 }
 
 
 def _validate_args(f, type_hints):
-    if not len(type_hints):
-        raise Exception("No type annotations provided")
-
     all_vars = set(f.__code__.co_varnames).difference(set(["self", "f"]))
 
     if not len(type_hints) == len(all_vars):
         raise Exception("Please provide type hints for all variables")
 
 
 def _get_complex_args_helper(
```

### Comparing `python_property_based_testing-0.3.0/pybt/core/util.py` & `python_property_based_testing-0.4.0/pybt/core/util.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.3.0/pybt/tests/simple_nonclass_test.py` & `python_property_based_testing-0.4.0/pybt/tests/simple_nonclass_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.3.0/pybt/tests/simple_unit_test.py` & `python_property_based_testing-0.4.0/pybt/tests/simple_unit_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.3.0/PKG-INFO` & `python_property_based_testing-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-property-based-testing
-Version: 0.3.0
+Version: 0.4.0
 Summary: Property Based Testing in Python
 Author: vrindisbacher
 Author-email: vrindisbacher77@gmail.com
 Requires-Python: >=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

