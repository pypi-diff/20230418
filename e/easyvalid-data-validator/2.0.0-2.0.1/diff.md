# Comparing `tmp/easyvalid_data_validator-2.0.0.tar.gz` & `tmp/easyvalid_data_validator-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyvalid_data_validator-2.0.0.tar", max compression
+gzip compressed data, was "easyvalid_data_validator-2.0.1.tar", max compression
```

## Comparing `easyvalid_data_validator-2.0.0.tar` & `easyvalid_data_validator-2.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0        0 2023-03-09 22:18:32.634299 easyvalid_data_validator-2.0.0/easyvalid_data_validator/__init__.py
--rw-r--r--   0        0        0     2297 2023-03-09 22:40:13.595480 easyvalid_data_validator-2.0.0/easyvalid_data_validator/common.py
--rw-r--r--   0        0        0      781 2023-03-09 22:26:59.056769 easyvalid_data_validator-2.0.0/easyvalid_data_validator/constraints.py
--rw-r--r--   0        0        0        0 2023-03-09 22:35:17.446982 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/__init__.py
--rw-r--r--   0        0        0       49 2023-03-09 22:26:59.056769 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/array.py
--rw-r--r--   0        0        0      158 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/common.py
--rw-r--r--   0        0        0       41 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/integer.py
--rw-r--r--   0        0        0       95 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.0/easyvalid_data_validator/customexceptions/string.py
--rw-r--r--   0        0        0        0 2023-03-09 22:36:30.704664 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/__init__.py
--rw-r--r--   0        0        0     1253 2023-03-09 22:43:26.031175 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/array_checker.py
--rw-r--r--   0        0        0      328 2023-03-09 22:49:10.070446 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/boolean_checker.py
--rw-r--r--   0        0        0      445 2023-03-09 22:49:10.086069 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/dictionary_checker.py
--rw-r--r--   0        0        0     1566 2023-03-09 22:49:10.086069 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/float_checker.py
--rw-r--r--   0        0        0     1466 2023-03-09 22:49:10.039301 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/integer_checker.py
--rw-r--r--   0        0        0     1178 2023-03-09 22:49:10.039301 easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/string_checker.py
--rw-r--r--   0        0        0     7181 2023-04-17 22:53:49.767329 easyvalid_data_validator-2.0.0/easyvalid_data_validator/validator.py
--rw-r--r--   0        0        0      410 2023-04-17 22:59:55.802321 easyvalid_data_validator-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2843 2023-04-17 22:59:42.949214 easyvalid_data_validator-2.0.0/README.md
--rw-r--r--   0        0        0     3036 1970-01-01 00:00:00.000000 easyvalid_data_validator-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-09 22:18:32.634299 easyvalid_data_validator-2.0.1/easyvalid_data_validator/__init__.py
+-rw-r--r--   0        0        0     2297 2023-03-09 22:40:13.595480 easyvalid_data_validator-2.0.1/easyvalid_data_validator/common.py
+-rw-r--r--   0        0        0      781 2023-03-09 22:26:59.056769 easyvalid_data_validator-2.0.1/easyvalid_data_validator/constraints.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:35:17.446982 easyvalid_data_validator-2.0.1/easyvalid_data_validator/customexceptions/__init__.py
+-rw-r--r--   0        0        0       49 2023-03-09 22:26:59.056769 easyvalid_data_validator-2.0.1/easyvalid_data_validator/customexceptions/array.py
+-rw-r--r--   0        0        0      158 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.1/easyvalid_data_validator/customexceptions/common.py
+-rw-r--r--   0        0        0       41 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.1/easyvalid_data_validator/customexceptions/integer.py
+-rw-r--r--   0        0        0       95 2023-03-09 22:26:59.072392 easyvalid_data_validator-2.0.1/easyvalid_data_validator/customexceptions/string.py
+-rw-r--r--   0        0        0        0 2023-03-09 22:36:30.704664 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/__init__.py
+-rw-r--r--   0        0        0     1253 2023-03-09 22:43:26.031175 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/array_checker.py
+-rw-r--r--   0        0        0      328 2023-03-09 22:49:10.070446 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/boolean_checker.py
+-rw-r--r--   0        0        0      445 2023-03-09 22:49:10.086069 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/dictionary_checker.py
+-rw-r--r--   0        0        0     1566 2023-03-09 22:49:10.086069 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/float_checker.py
+-rw-r--r--   0        0        0     1466 2023-03-09 22:49:10.039301 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/integer_checker.py
+-rw-r--r--   0        0        0     1178 2023-03-09 22:49:10.039301 easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/string_checker.py
+-rw-r--r--   0        0        0     7181 2023-04-17 22:53:49.767329 easyvalid_data_validator-2.0.1/easyvalid_data_validator/validator.py
+-rw-r--r--   0        0        0      410 2023-04-18 10:04:33.953949 easyvalid_data_validator-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2821 2023-04-18 10:04:33.935176 easyvalid_data_validator-2.0.1/README.md
+-rw-r--r--   0        0        0     3014 1970-01-01 00:00:00.000000 easyvalid_data_validator-2.0.1/PKG-INFO
```

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/common.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/common.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/constraints.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/constraints.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/array_checker.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/array_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/float_checker.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/float_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/integer_checker.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/integer_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/datacheckers/string_checker.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/datacheckers/string_checker.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/easyvalid_data_validator/validator.py` & `easyvalid_data_validator-2.0.1/easyvalid_data_validator/validator.py`

 * *Files identical despite different names*

### Comparing `easyvalid_data_validator-2.0.0/README.md` & `easyvalid_data_validator-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -102,8 +102,8 @@
 
 ```
 ValidationError("age": ["Invalid integer expression - isn't grater or equal to compare value"])
 ```
 
 ## Documentation link
 
-[Click to read documentation](https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR/edit/master/README.md)
+[Click to read documentation](https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR)
```

### Comparing `easyvalid_data_validator-2.0.0/PKG-INFO` & `easyvalid_data_validator-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyvalid-data-validator
-Version: 2.0.0
+Version: 2.0.1
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
@@ -113,9 +113,9 @@
 
 ```
 ValidationError("age": ["Invalid integer expression - isn't grater or equal to compare value"])
 ```
 
 ## Documentation link
 
-[Click to read documentation](https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR/edit/master/README.md)
+[Click to read documentation](https://github.com/DSmolke/EASYVALID_DATA_VALIDATOR)
```

