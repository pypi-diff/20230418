# Comparing `tmp/python_property_based_testing-0.8.0.tar.gz` & `tmp/python_property_based_testing-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_property_based_testing-0.8.0.tar", max compression
+gzip compressed data, was "python_property_based_testing-0.9.0.tar", max compression
```

## Comparing `python_property_based_testing-0.8.0.tar` & `python_property_based_testing-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-04-18 16:10:09.783503 python_property_based_testing-0.8.0/LICENSE
--rw-r--r--   0        0        0     8292 2023-04-18 16:10:09.783503 python_property_based_testing-0.8.0/README.md
--rw-r--r--   0        0        0        0 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/core/__init__.py
--rw-r--r--   0        0        0     7507 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/core/core.py
--rw-r--r--   0        0        0     3195 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/core/util.py
--rw-r--r--   0        0        0        0 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/tests/__init__.py
--rw-r--r--   0        0        0      575 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/tests/simple_nonclass_test.py
--rw-r--r--   0        0        0      628 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pybt/tests/simple_unit_test.py
--rw-r--r--   0        0        0      432 2023-04-18 16:10:09.787503 python_property_based_testing-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 python_property_based_testing-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/core/__init__.py
+-rw-r--r--   0        0        0     7511 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/core/core.py
+-rw-r--r--   0        0        0     3195 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/core/util.py
+-rw-r--r--   0        0        0        0 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/tests/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/tests/simple_nonclass_test.py
+-rw-r--r--   0        0        0      628 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pybt/tests/simple_unit_test.py
+-rw-r--r--   0        0        0      432 2023-04-18 16:17:16.833580 python_property_based_testing-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 python_property_based_testing-0.9.0/PKG-INFO
```

### Comparing `python_property_based_testing-0.8.0/LICENSE` & `python_property_based_testing-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.8.0/README.md` & `python_property_based_testing-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.8.0/pybt/core/core.py` & `python_property_based_testing-0.9.0/pybt/core/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,15 +185,15 @@
     parameter max_complex_arg_size : maximum size to use for all structures (list, dicts)
     """
     
     if n <= 0:
         raise Exception("You should run more than 0 iterations! Please set n > 0.")
     if generators and type(generators) != dict:
         raise Exception("Invalid generators! Please try again with a dict of argument name to function") 
-    if hypotheses type(hypotheses) != dict:
+    if hypotheses and type(hypotheses) != dict:
         raise Exception("Invalid hypotheses! Please try again with a dict of argument name to function that returns a boolean") 
     if max_basic_arg_size <= 0:
         raise Exception("Please set a max basic arg size greater than 0") 
     if max_complex_arg_size <= 0:
         raise Exception("Please set a max complex arg size greater than 0") 
     
     if f is None:
```

### Comparing `python_property_based_testing-0.8.0/pybt/core/util.py` & `python_property_based_testing-0.9.0/pybt/core/util.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.8.0/pybt/tests/simple_nonclass_test.py` & `python_property_based_testing-0.9.0/pybt/tests/simple_nonclass_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.8.0/pybt/tests/simple_unit_test.py` & `python_property_based_testing-0.9.0/pybt/tests/simple_unit_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.8.0/PKG-INFO` & `python_property_based_testing-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-property-based-testing
-Version: 0.8.0
+Version: 0.9.0
 Summary: Property Based Testing in Python
 Author: vrindisbacher
 Author-email: vrindisbacher77@gmail.com
 Requires-Python: >=3.10,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

