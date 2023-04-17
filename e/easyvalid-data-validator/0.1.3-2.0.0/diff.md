# Comparing `tmp/easyvalid_data_validator-0.1.3.tar.gz` & `tmp/easyvalid_data_validator-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyvalid_data_validator-0.1.3.tar", max compression
+gzip compressed data, was "easyvalid_data_validator-2.0.0.tar", max compression
```

## Comparing `easyvalid_data_validator-0.1.3.tar` & `easyvalid_data_validator-2.0.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-03-09 22:18:32.634299 easyvalid_data_validator-0.1.3/easyvalid_data_validator/__init__.py
--rw-r--r--   0        0        0     2297 2023-03-09 22:40:13.595480 easyvalid_data_validator-0.1.3/easyvalid_data_validator/common.py
--rw-r--r--   0        0        0      781 2023-03-09 22:26:59.056769 easyvalid_data_validator-0.1.3/easyvalid_data_validator/constraints.py
--rw-r--r--   0        0        0        0 2023-03-09 22:35:17.446982 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/__init__.py
--rw-r--r--   0        0        0       49 2023-03-09 22:26:59.056769 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/array.py
--rw-r--r--   0        0        0      158 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/common.py
--rw-r--r--   0        0        0       41 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/integer.py
--rw-r--r--   0        0        0       95 2023-03-09 22:26:59.072392 easyvalid_data_validator-0.1.3/easyvalid_data_validator/customexceptions/string.py
--rw-r--r--   0        0        0        0 2023-03-09 22:36:30.704664 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/__init__.py
--rw-r--r--   0        0        0     1253 2023-03-09 22:43:26.031175 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/array.py
--rw-r--r--   0        0        0      328 2023-03-09 22:49:10.070446 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/boolean.py
--rw-r--r--   0        0        0      445 2023-03-09 22:49:10.086069 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/dictionary.py
--rw-r--r--   0        0        0     1566 2023-03-09 22:49:10.086069 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/float.py
--rw-r--r--   0        0        0     1466 2023-03-09 22:49:10.039301 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/integer.py
--rw-r--r--   0        0        0     1178 2023-03-09 22:49:10.039301 easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/string.py
--rw-r--r--   0        0        0     6775 2023-04-06 17:19:24.062391 easyvalid_data_validator-0.1.3/easyvalid_data_validator/validator.py
--rw-r--r--   0        0        0      410 2023-04-13 08:16:54.033553 easyvalid_data_validator-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-04-13 08:16:35.139598 easyvalid_data_validator-0.1.3/README.md
--rw-r--r--   0        0        0     2800 1970-01-01 00:00:00.000000 easyvalid_data_validator-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 22:18:32.634299 easyvalid_data_validator-2.0.0/easyvalid_data_validator/__init__.py
+-rw-r--r--   0        0        0     2297 2023-03-09 22:40:13.595480 easyvalid_data_validator-2.0.0/easyvalid_data_validator/common.py
+-rw-r--r--   0        0        0      781 2023-03-09 22:26:59.056769 easyvalid_data_validator-2.0.0/easyvalid_data_validator/constraints.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:35:17.446982 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/__init__.py
+-rw-r--r--   0        0        0       49 2023-03-09 22:26:59.056769 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/array.py
+-rw-r--r--   0        0        0      158 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/common.py
+-rw-r--r--   0        0        0       41 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/integer.py
+-rw-r--r--   0        0        0       95 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/string.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:36:30.704664 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/__init__.py
+-rw-r--r--   0        0        0     1253 2023-03-09 22:43:26.031175 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/array_checker.py
+-rw-r--r--   0        0        0      328 2023-03-09 22:49:10.070446 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/boolean_checker.py
+-rw-r--r--   0        0        0      445 2023-03-09 22:49:10.086069 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/dictionary_checker.py
+-rw-r--r--   0        0        0     1566 2023-03-09 22:49:10.086069 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/float_checker.py
+-rw-r--r--   0        0        0     1466 2023-03-09 22:49:10.039301 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/integer_checker.py
+-rw-r--r--   0        0        0     1178 2023-03-09 22:49:10.039301 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/string_checker.py
+-rw-r--r--   0        0        0     7181 2023-04-17 22:53:49.767329 easyvalid_data_validator-2.0.0/easyvalid_data_validator/validator.py
+-rw-r--r--   0        0        0      410 2023-04-17 22:59:55.802321 easyvalid_data_validator-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2843 2023-04-17 22:59:42.949214 easyvalid_data_validator-2.0.0/README.md
+-rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 easyvalid_data_validator-2.0.0/PKG-INFO
```

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/common.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/common.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/constraints.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/constraints.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/array.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/array_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/float.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/float_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/integer.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/integer_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/datacheckers/string.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/string_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-0.1.3/easyvalid_data_validator/validator.py` & `easyvalid_data_validator-2.0.0/easyvalid_data_validator/validator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from collections import defaultdict
 from itertools import chain
 from typing import Any
 
 from easyvalid_data_validator.common import is_type
 from easyvalid_data_validator.constraints import Constraint
 from easyvalid_data_validator.customexceptions.common import ValidationError
-from easyvalid_data_validator.datacheckers.boolean import is_true, is_false
-from easyvalid_data_validator.datacheckers.float import is_float_lower_than, is_float_le_than, is_float_equal, \
+from easyvalid_data_validator.datacheckers.boolean_checker import is_true, is_false
+from easyvalid_data_validator.datacheckers.float_checker import is_float_lower_than, is_float_le_than, is_float_equal, \
     is_float_not_equal, is_float_grater_than, is_float_ge_than
-from easyvalid_data_validator.datacheckers.string import matches_regex, is_decimal_string
-from easyvalid_data_validator.datacheckers.integer import is_in_range, is_lower_than, is_le_than, is_grater_than, \
+from easyvalid_data_validator.datacheckers.string_checker import matches_regex, is_decimal_string
+from easyvalid_data_validator.datacheckers.integer_checker import is_in_range, is_lower_than, is_le_than, is_grater_than, \
     is_ge_than, is_equal, is_not_equal
-from easyvalid_data_validator.datacheckers.array import is_array_length_of, are_members_of_type
-from easyvalid_data_validator.datacheckers.dictionary import are_keys_same_as
+from easyvalid_data_validator.datacheckers.array_checker import is_array_length_of, are_members_of_type
+from easyvalid_data_validator.datacheckers.dictionary_checker import are_keys_same_as
 
 
 def _validate_json_dict_member(key: str, constraint: dict[str, Any], validated_data: dict[str, Any]) -> list[tuple[str]]:
     """
         Validates if value represented by a key match provided constraints
     :param key: validated item key
     :param constraint: rules that value has to match
@@ -27,21 +27,23 @@
     validated_value = validated_data.get(key, False)
     if key not in validated_data.keys():
         raise KeyError('Invalid key')
 
     for constraint_name, constraint_value in constraint.items():
 
         match constraint_name:
+            # -------------- STRING --------------
             case Constraint.STRING_REGEX:
                 if not matches_regex(validated_value, constraint_value):
                     errors.append((key, "Invalid string expression - does not match regex"))
             case Constraint.STRING_IS_DECIMAL:
                 if not is_decimal_string(validated_value):
                     errors.append((key, "Invalid string expression - isn't decimal string "))
 
+            # -------------- INT --------------
             case Constraint.INT_BETWEEN:
                 if not is_in_range(validated_value, *constraint_value):
                     errors.append((key, "Invalid integer expression - isn't in range"))
             case Constraint.INT_LOWER:
                 if not is_lower_than(validated_value, constraint_value):
                     errors.append((key, "Invalid integer expression - isn't lower than compare value"))
             case Constraint.INT_LE:
@@ -56,25 +58,30 @@
             case Constraint.INT_EQUAL:
                 if not is_equal(validated_value, constraint_value):
                     errors.append((key, "Invalid integer expression - isn't equal to compare value"))
             case Constraint.INT_NOT_EQUAL:
                 if not is_not_equal(validated_value, constraint_value):
                     errors.append((key, "Invalid integer expression - validated value and compare value are equal"))
 
+
+            # -------------- LIST --------------
             case Constraint.ARRAY_IS_LENGTH_OF:
                 if not is_array_length_of(validated_value, constraint_value):
                     errors.append((key, "Invalid array - has different length than expected"))
             case Constraint.ARRAY_MEMBERS_TYPE:
                 if not are_members_of_type(validated_value, constraint_value):
                     errors.append((key, "Invalid array - some or all members have unexpected type"))
 
+            # -------------- DICT --------------
             case Constraint.DICT_HAS_SAME_KEYS:
                 if not are_keys_same_as(validated_value, constraint_value):
                     errors.append((key, "Invalid dictionary - keys are not the same"))
 
+
+            # -------------- FLOAT --------------
             case Constraint.FLOAT_LOWER:
                 if not is_float_lower_than(validated_value, constraint_value):
                     errors.append((key, "Invalid float - isn't lower than compare value"))
             case Constraint.FLOAT_LE:
                 if not is_float_le_than(validated_value, constraint_value):
                     errors.append((key, "Invalid float - isn't lower or equal than compare value"))
             case Constraint.FLOAT_EQUAL:
@@ -86,22 +93,25 @@
             case Constraint.FLOAT_GRATER:
                 if not is_float_grater_than(validated_value, constraint_value):
                     errors.append((key, "Invalid float - isn't grater than compare value"))
             case Constraint.FLOAT_GE:
                 if not is_float_ge_than(validated_value, constraint_value):
                     errors.append((key, "Invalid float - isn't grater or equal than compare value"))
 
+
+            # -------------- TYPE --------------
             case Constraint.IS_TYPE:
                 if not is_type(validated_value, constraint_value):
                     errors.append((key, "Invalid type - isn't same type like compare type"))
 
+
+            # -------------- BOOL --------------
             case Constraint.BOOL_TRUE:
                 if not is_true(validated_value):
                     errors.append((key, "Invalid boolean - isn't True"))
-
             case Constraint.BOOL_FALSE:
                 if not is_false(validated_value):
                     errors.append((key, "Invalid boolean - isn't False"))
 
             case _:
                 raise ValueError('Invalid constraint name')
```

### Comparing `easyvalid_data_validator-0.1.3/README.md` & `easyvalid_data_validator-2.0.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -9,25 +9,45 @@
 
 All functions are fully tested
 
 You are able to run tests on your own cloning repo and using it's environment:
 ```
   git clone https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR.git
   cd EASYVALID_DATA_VALIDATOR
+```
+
+### poetry:
+```bash
   poetry update
   poetry shell
+  poetry run python -m unittest discover -v
+```
+or:
+```bash
+  poetry run pytest -vv
 ```
 
-And then:
+### pipenv:
 ```bash
-  poetry run python -m unittest discover -v
+  pipenv shell
+  pipenv run python -m unittest discover -v
+```
+or:
+```bash
+  pipenv run pytest -vv
+```
+
+### pip:
+```bash
+  python -m unittest discover -v
 ```
-or
+or:
 ```bash
-  poetry run pytest
+  pip install pytest
+  pytest -vv
 ```
 # easyvalid-data-validator
 
 It's a package developed mainly for validation of json dict that is created by using json.load().
 
 Here is an example of json dict, that has name, age, and balance.
 ```
```

### Comparing `easyvalid_data_validator-0.1.3/PKG-INFO` & `easyvalid_data_validator-2.0.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyvalid-data-validator
-Version: 0.1.3
+Version: 2.0.0
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -20,25 +20,45 @@
 
 All functions are fully tested
 
 You are able to run tests on your own cloning repo and using it's environment:
 ```
   git clone https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR.git
   cd EASYVALID_DATA_VALIDATOR
+```
+
+### poetry:
+```bash
   poetry update
   poetry shell
+  poetry run python -m unittest discover -v
+```
+or:
+```bash
+  poetry run pytest -vv
 ```
 
-And then:
+### pipenv:
 ```bash
-  poetry run python -m unittest discover -v
+  pipenv shell
+  pipenv run python -m unittest discover -v
+```
+or:
+```bash
+  pipenv run pytest -vv
+```
+
+### pip:
+```bash
+  python -m unittest discover -v
 ```
-or
+or:
 ```bash
-  poetry run pytest
+  pip install pytest
+  pytest -vv
 ```
 # easyvalid-data-validator
 
 It's a package developed mainly for validation of json dict that is created by using json.load().
 
 Here is an example of json dict, that has name, age, and balance.
 ```
```

