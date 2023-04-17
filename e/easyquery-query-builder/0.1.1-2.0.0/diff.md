# Comparing `tmp/easyquery_query_builder-0.1.1.tar.gz` & `tmp/easyquery_query_builder-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyquery_query_builder-0.1.1.tar", max compression
+gzip compressed data, was "easyquery_query_builder-2.0.0.tar", max compression
```

## Comparing `easyquery_query_builder-0.1.1.tar` & `easyquery_query_builder-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,10 @@
--rw-r--r--   0        0        0        0 2023-04-04 22:01:26.361168 easyquery_query_builder-0.1.1/easyquery_query_builder/__init__.py
--rw-r--r--   0        0        0     8486 2023-04-12 08:03:07.930811 easyquery_query_builder-0.1.1/easyquery_query_builder/queries.py
--rw-r--r--   0        0        0      505 2023-04-12 08:04:15.234451 easyquery_query_builder-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12961 2023-04-12 08:02:13.105404 easyquery_query_builder-0.1.1/README.md
--rw-r--r--   0        0        0    13319 1970-01-01 00:00:00.000000 easyquery_query_builder-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-04-04 22:01:26.361168 easyquery_query_builder-2.0.0/easyquery_query_builder/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:06:50.899067 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/__init__.py
+-rw-r--r--   0        0        0      122 2023-04-17 22:16:32.162595 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/query.py
+-rw-r--r--   0        0        0     2192 2023-04-17 22:16:32.139892 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query.py
+-rw-r--r--   0        0        0     3014 2023-04-17 22:16:32.122425 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_builder.py
+-rw-r--r--   0        0        0     2527 2023-04-17 22:16:32.114251 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_with_joins.py
+-rw-r--r--   0        0        0     1396 2023-04-17 22:16:32.155202 easyquery_query_builder-2.0.0/easyquery_query_builder/queries/read_query_with_joins_builder.py
+-rw-r--r--   0        0        0      505 2023-04-17 22:25:15.831231 easyquery_query_builder-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13170 2023-04-17 22:25:15.821965 easyquery_query_builder-2.0.0/README.md
+-rw-r--r--   0        0        0    13528 1970-01-01 00:00:00.000000 easyquery_query_builder-2.0.0/PKG-INFO
```

### Comparing `easyquery_query_builder-0.1.1/README.md` & `easyquery_query_builder-2.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -9,69 +9,78 @@
 ```bash
   pip install easyquery-query-builder
 ```
 Using poetry:
 ```bash
   poetry add easyquery-query-builder
 ```
+Using pipenv:
+```bash
+  pipenv install easyquery-query-builder
+```
 
 
     
 ## Tests and coverage
 
 All functionalities are fully tested.
 
 You are able to run tests on your own by using cloning repository and using it's virtual environment.
 
 ### 1. Clone repository and enter it's main directory
 ```bash
   git clone https://github.com/DSmolke/EASYQUERY_QUERY_BUILDER.git
   cd EASYQUERY_QUERY_BUILDER
 ```
-### 2. Set up and enter virtual environment using poetry
-
-* if you don't have poetry, first install it:
+### 2. Run tests using:
+#### pip:
 ```bash
-  pip install poetry
+  pip install pytest
+  pip install coverage
+  pip install easyvalid-data-validator
+  
+  pytest -vv
 ```
-* install environment and enter shell:
+
+#### poetry:
 ```bash
+  pip install poetry
   poetry update
   poetry shell
+  poetry run pytest -vv
 ```
 (poetry update is used due to some issue that I faced with newest Python version)
 
-### 3. Run tests using pytest
+#### pipenv:
 ```bash
-  poetry run pytest -vv
+   pip install pipenv
+   pipenv shell
+   pipenv run pytest -vv
 ```
 
-### 4. Access coverage report
+### 3. Access coverage report
 
 If you haven't done step 1, start from here:
 ```bash
   git clone https://github.com/DSmolke/EASYQUERY_QUERY_BUILDER.git
   cd EASYQUERY_QUERY_BUILDER
 ```
 Then use this command to change branch
 ```bash
   git checkout with_coverage_files
 ```
 
 You should be able to see htmlcov directory. Enter it and open index.html file to see full coverage report.
 
 
-
-
-
-
 ## Basic usage
 Let's say we need to prepare query where we ask database for all records from drivers table, joined with licenses table on license id:
 ```
-from easyquery_query_builder.queries import ReadQueryWithJoinBuilder, ReadQueryWithJoins
+from easyquery_query_builder.queries.read_query_with_joins import ReadQueryWithJoins
+from easyquery_query_builder.queries.read_query_with_joins_builder import ReadQueryWithJoinsBuilder
 
 query: ReadQueryWithJoins = ReadQueryWithJoinBuilder() \
     .add_select_statement('*') \
     .add_from_statement('drivers') \
     .add_joins_statement([['licenses', 'l', 'l.id = drivers.license_id']])\
     .build()
 ```
```

### Comparing `easyquery_query_builder-0.1.1/PKG-INFO` & `easyquery_query_builder-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easyquery-query-builder
-Version: 0.1.1
+Version: 2.0.0
 Summary: 
 Author: Smolke
 Author-email: d.smolczynski1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: easyvalid-data-validator (>=0.1.1,<0.2.0)
@@ -21,69 +21,78 @@
 ```bash
   pip install easyquery-query-builder
 ```
 Using poetry:
 ```bash
   poetry add easyquery-query-builder
 ```
+Using pipenv:
+```bash
+  pipenv install easyquery-query-builder
+```
 
 
     
 ## Tests and coverage
 
 All functionalities are fully tested.
 
 You are able to run tests on your own by using cloning repository and using it's virtual environment.
 
 ### 1. Clone repository and enter it's main directory
 ```bash
   git clone https://github.com/DSmolke/EASYQUERY_QUERY_BUILDER.git
   cd EASYQUERY_QUERY_BUILDER
 ```
-### 2. Set up and enter virtual environment using poetry
-
-* if you don't have poetry, first install it:
+### 2. Run tests using:
+#### pip:
 ```bash
-  pip install poetry
+  pip install pytest
+  pip install coverage
+  pip install easyvalid-data-validator
+  
+  pytest -vv
 ```
-* install environment and enter shell:
+
+#### poetry:
 ```bash
+  pip install poetry
   poetry update
   poetry shell
+  poetry run pytest -vv
 ```
 (poetry update is used due to some issue that I faced with newest Python version)
 
-### 3. Run tests using pytest
+#### pipenv:
 ```bash
-  poetry run pytest -vv
+   pip install pipenv
+   pipenv shell
+   pipenv run pytest -vv
 ```
 
-### 4. Access coverage report
+### 3. Access coverage report
 
 If you haven't done step 1, start from here:
 ```bash
   git clone https://github.com/DSmolke/EASYQUERY_QUERY_BUILDER.git
   cd EASYQUERY_QUERY_BUILDER
 ```
 Then use this command to change branch
 ```bash
   git checkout with_coverage_files
 ```
 
 You should be able to see htmlcov directory. Enter it and open index.html file to see full coverage report.
 
 
-
-
-
-
 ## Basic usage
 Let's say we need to prepare query where we ask database for all records from drivers table, joined with licenses table on license id:
 ```
-from easyquery_query_builder.queries import ReadQueryWithJoinBuilder, ReadQueryWithJoins
+from easyquery_query_builder.queries.read_query_with_joins import ReadQueryWithJoins
+from easyquery_query_builder.queries.read_query_with_joins_builder import ReadQueryWithJoinsBuilder
 
 query: ReadQueryWithJoins = ReadQueryWithJoinBuilder() \
     .add_select_statement('*') \
     .add_from_statement('drivers') \
     .add_joins_statement([['licenses', 'l', 'l.id = drivers.license_id']])\
     .build()
 ```
```

