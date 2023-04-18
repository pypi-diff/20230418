# Comparing `tmp/python_property_based_testing-0.9.1.tar.gz` & `tmp/python_property_based_testing-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_property_based_testing-0.9.1.tar", max compression
+gzip compressed data, was "python_property_based_testing-0.9.2.tar", max compression
```

## Comparing `python_property_based_testing-0.9.1.tar` & `python_property_based_testing-0.9.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1076 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/LICENSE
--rw-r--r--   0        0        0     8292 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/README.md
--rw-r--r--   0        0        0        0 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/__init__.py
--rw-r--r--   0        0        0        0 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/core/__init__.py
--rw-r--r--   0        0        0     7516 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/core/core.py
--rw-r--r--   0        0        0     3195 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/core/util.py
--rw-r--r--   0        0        0        0 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/tests/__init__.py
--rw-r--r--   0        0        0      575 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/tests/simple_nonclass_test.py
--rw-r--r--   0        0        0      628 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pybt/tests/simple_unit_test.py
--rw-r--r--   0        0        0      432 2023-04-18 21:01:11.616785 python_property_based_testing-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 python_property_based_testing-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/LICENSE
+-rw-r--r--   0        0        0     8292 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/core/__init__.py
+-rw-r--r--   0        0        0     7516 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/core/core.py
+-rw-r--r--   0        0        0     3195 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/core/util.py
+-rw-r--r--   0        0        0        0 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/tests/__init__.py
+-rw-r--r--   0        0        0      575 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/tests/simple_nonclass_test.py
+-rw-r--r--   0        0        0      628 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pybt/tests/simple_unit_test.py
+-rw-r--r--   0        0        0      432 2023-04-18 21:04:57.544704 python_property_based_testing-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     8692 1970-01-01 00:00:00.000000 python_property_based_testing-0.9.2/PKG-INFO
```

### Comparing `python_property_based_testing-0.9.1/LICENSE` & `python_property_based_testing-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.9.1/README.md` & `python_property_based_testing-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.9.1/pybt/core/core.py` & `python_property_based_testing-0.9.2/pybt/core/core.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.9.1/pybt/core/util.py` & `python_property_based_testing-0.9.2/pybt/core/util.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.9.1/pybt/tests/simple_nonclass_test.py` & `python_property_based_testing-0.9.2/pybt/tests/simple_nonclass_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.9.1/pybt/tests/simple_unit_test.py` & `python_property_based_testing-0.9.2/pybt/tests/simple_unit_test.py`

 * *Files identical despite different names*

### Comparing `python_property_based_testing-0.9.1/PKG-INFO` & `python_property_based_testing-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: python-property-based-testing
-Version: 0.9.1
+Version: 0.9.2
 Summary: Property Based Testing in Python
 Author: vrindisbacher
 Author-email: vrindisbacher77@gmail.com
-Requires-Python: >=3.10,<=3.11
+Requires-Python: >=3.10,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 ## PyBT
```

