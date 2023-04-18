# Comparing `tmp/python_property_based_testing-0.5.0.tar.gz` & `tmp/python_property_based_testing-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_property_based_testing-0.5.0.tar", max compression
+gzip compressed data, was "python_property_based_testing-0.6.0.tar", max compression
```

## Comparing `python_property_based_testing-0.5.0.tar` & `python_property_based_testing-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/LICENSE
--rw-r--r--   0        0        0     8292 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/core/__init__.py
--rw-r--r--   0        0        0     6635 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/core/core.py
--rw-r--r--   0        0        0     3195 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/core/util.py
--rw-r--r--   0        0        0        0 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/tests/__init__.py
--rw-r--r--   0        0        0      575 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/tests/simple_nonclass_test.py
--rw-r--r--   0        0        0      628 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pybt/tests/simple_unit_test.py
--rw-r--r--   0        0        0      432 2023-04-18 14:42:56.584120 python_property_based_testing-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 python_property_based_testing-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/core/__init__.py
+-rw-r--r--   0        0        0     6755 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/core/core.py
+-rw-r--r--   0        0        0     3195 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/core/util.py
+-rw-r--r--   0        0        0        0 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/tests/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/tests/simple_nonclass_test.py
+-rw-r--r--   0        0        0      628 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pybt/tests/simple_unit_test.py
+-rw-r--r--   0        0        0      432 2023-04-18 15:11:48.852521 python_property_based_testing-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 python_property_based_testing-0.6.0/PKG-INFO
```

### Comparing `python_property_based_testing-0.5.0/LICENSE` & `python_property_based_testing-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.5.0/README.md` & `python_property_based_testing-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.5.0/pybt/core/core.py` & `python_property_based_testing-0.6.0/pybt/core/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,16 +31,15 @@
     dict: lambda s, d: partial(gen_dict, s, d),
     list: lambda s, l: partial(gen_list, s, l),
 }
 
 
 def _validate_args(f, type_hints):
     all_vars = set(f.__code__.co_varnames).difference(set(["self", "f"]))
-
-    if not len(type_hints) == len(all_vars):
+    if not set(type_hints.keys()).difference(all_vars) == set():
         raise Exception("Please provide type hints for all variables")
 
 
 def _get_complex_args_helper(
     arg_type, arg_struct, max_basic_arg_size, max_complex_arg_size
 ):
     base_type = typing.get_origin(arg_type)
@@ -114,22 +113,25 @@
     arg_to_generator_map,
     type_hints,
     generators,
     max_basic_arg_size,
     max_complex_arg_size,
 ):
     for arg_name, arg_type in type_hints.items():
-        if is_base_type(arg_type) or (generators and (gen := generators.get(arg_name))):
-            if gen:
+        found = False
+        if is_base_type(arg_type) or generators:
+            if gen := generators.get(arg_name):
                 arg_to_generator_map[arg_name] = gen
-            else:
+                found = True
+            elif is_base_type(arg_type):
                 arg_to_generator_map[arg_name] = BASIC_TYPE_MAP[arg_type](
                     max_basic_arg_size
                 )
-        else:
+                found = True
+        elif not found:
             complex_generator_map = _get_complex_args(
                 arg_type, max_basic_arg_size, max_complex_arg_size
             )
             arg_to_generator_map[arg_name] = complex_generator_map
 
 
 def _drive_tests(arg_to_generator_map, f, type_hints, n, hypotheses, self_=None):
```

### Comparing `python_property_based_testing-0.5.0/pybt/core/util.py` & `python_property_based_testing-0.6.0/pybt/core/util.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.5.0/pybt/tests/simple_nonclass_test.py` & `python_property_based_testing-0.6.0/pybt/tests/simple_nonclass_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.5.0/pybt/tests/simple_unit_test.py` & `python_property_based_testing-0.6.0/pybt/tests/simple_unit_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.5.0/PKG-INFO` & `python_property_based_testing-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-property-based-testing
-Version: 0.5.0
+Version: 0.6.0
 Summary: Property Based Testing in Python
 Author: vrindisbacher
 Author-email: vrindisbacher77@gmail.com
 Requires-Python: >=3.10,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

