# Comparing `tmp/sphinx-csv-filter-0.4.0.tar.gz` & `tmp/sphinx-csv-filter-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinx-csv-filter-0.4.0.tar", last modified: Mon Dec 12 13:41:45 2022, max compression
+gzip compressed data, was "sphinx-csv-filter-0.4.1.tar", last modified: Tue Apr 18 16:23:28 2023, max compression
```

## Comparing `sphinx-csv-filter-0.4.0.tar` & `sphinx-csv-filter-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,22 @@
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2022-12-12 13:41:45.959875 sphinx-csv-filter-0.4.0/
--rw-r--r--   0 amo        (501) staff       (20)    10775 2022-12-12 13:25:09.000000 sphinx-csv-filter-0.4.0/LICENSE
--rw-r--r--   0 amo        (501) staff       (20)       16 2021-12-07 11:53:21.000000 sphinx-csv-filter-0.4.0/MANIFEST.in
--rw-r--r--   0 amo        (501) staff       (20)     5499 2022-12-12 13:41:45.960005 sphinx-csv-filter-0.4.0/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)     3810 2022-12-12 13:26:23.000000 sphinx-csv-filter-0.4.0/README.rst
--rw-r--r--   0 amo        (501) staff       (20)      625 2022-12-12 13:41:45.960458 sphinx-csv-filter-0.4.0/setup.cfg
--rw-r--r--   0 amo        (501) staff       (20)     3438 2022-12-12 13:40:02.000000 sphinx-csv-filter-0.4.0/setup.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2022-12-12 13:41:45.954718 sphinx-csv-filter-0.4.0/src/
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2022-12-12 13:41:45.957047 sphinx-csv-filter-0.4.0/src/crate/
--rw-r--r--   0 amo        (501) staff       (20)     1217 2022-12-12 13:25:09.000000 sphinx-csv-filter-0.4.0/src/crate/__init__.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2022-12-12 13:41:45.957660 sphinx-csv-filter-0.4.0/src/crate/sphinx/
--rw-r--r--   0 amo        (501) staff       (20)        0 2021-10-19 14:24:45.000000 sphinx-csv-filter-0.4.0/src/crate/sphinx/__init__.py
--rw-r--r--   0 amo        (501) staff       (20)     4478 2022-12-12 13:25:09.000000 sphinx-csv-filter-0.4.0/src/crate/sphinx/csv.py
-drwxr-xr-x   0 amo        (501) staff       (20)        0 2022-12-12 13:41:45.959709 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/
--rw-r--r--   0 amo        (501) staff       (20)     5499 2022-12-12 13:41:45.000000 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/PKG-INFO
--rw-r--r--   0 amo        (501) staff       (20)      402 2022-12-12 13:41:45.000000 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/SOURCES.txt
--rw-r--r--   0 amo        (501) staff       (20)        1 2022-12-12 13:41:45.000000 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/dependency_links.txt
--rw-r--r--   0 amo        (501) staff       (20)        6 2022-12-12 13:41:45.000000 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/namespace_packages.txt
--rw-r--r--   0 amo        (501) staff       (20)      130 2022-12-12 13:41:45.000000 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/requires.txt
--rw-r--r--   0 amo        (501) staff       (20)        6 2022-12-12 13:41:45.000000 sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-18 16:23:28.711072 sphinx-csv-filter-0.4.1/
+-rw-r--r--   0 amo        (501) staff       (20)    10775 2022-12-12 14:00:44.000000 sphinx-csv-filter-0.4.1/LICENSE
+-rw-r--r--   0 amo        (501) staff       (20)       16 2021-12-07 11:53:21.000000 sphinx-csv-filter-0.4.1/MANIFEST.in
+-rw-r--r--   0 amo        (501) staff       (20)     5497 2023-04-18 16:23:28.711171 sphinx-csv-filter-0.4.1/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)     3808 2023-04-18 16:21:17.000000 sphinx-csv-filter-0.4.1/README.rst
+-rw-r--r--   0 amo        (501) staff       (20)      625 2023-04-18 16:23:28.711676 sphinx-csv-filter-0.4.1/setup.cfg
+-rw-r--r--   0 amo        (501) staff       (20)     3438 2023-04-18 16:22:53.000000 sphinx-csv-filter-0.4.1/setup.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-18 16:23:28.704921 sphinx-csv-filter-0.4.1/src/
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-18 16:23:28.707606 sphinx-csv-filter-0.4.1/src/crate/
+-rw-r--r--   0 amo        (501) staff       (20)     1217 2022-12-12 14:00:44.000000 sphinx-csv-filter-0.4.1/src/crate/__init__.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-18 16:23:28.708262 sphinx-csv-filter-0.4.1/src/crate/sphinx/
+-rw-r--r--   0 amo        (501) staff       (20)        0 2021-10-19 14:24:45.000000 sphinx-csv-filter-0.4.1/src/crate/sphinx/__init__.py
+-rw-r--r--   0 amo        (501) staff       (20)     4570 2023-04-18 16:22:53.000000 sphinx-csv-filter-0.4.1/src/crate/sphinx/csv.py
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-18 16:23:28.710251 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/
+-rw-r--r--   0 amo        (501) staff       (20)     5497 2023-04-18 16:23:28.000000 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/PKG-INFO
+-rw-r--r--   0 amo        (501) staff       (20)      420 2023-04-18 16:23:28.000000 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/SOURCES.txt
+-rw-r--r--   0 amo        (501) staff       (20)        1 2023-04-18 16:23:28.000000 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/dependency_links.txt
+-rw-r--r--   0 amo        (501) staff       (20)        6 2023-04-18 16:23:28.000000 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/namespace_packages.txt
+-rw-r--r--   0 amo        (501) staff       (20)      130 2023-04-18 16:23:28.000000 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/requires.txt
+-rw-r--r--   0 amo        (501) staff       (20)        6 2023-04-18 16:23:28.000000 sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/top_level.txt
+drwxr-xr-x   0 amo        (501) staff       (20)        0 2023-04-18 16:23:28.710536 sphinx-csv-filter-0.4.1/tests/
+-rw-r--r--   0 amo        (501) staff       (20)     4225 2022-12-10 01:02:59.000000 sphinx-csv-filter-0.4.1/tests/test_csv.py
```

### Comparing `sphinx-csv-filter-0.4.0/LICENSE` & `sphinx-csv-filter-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinx-csv-filter-0.4.0/PKG-INFO` & `sphinx-csv-filter-0.4.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-csv-filter
-Version: 0.4.0
+Version: 0.4.1
 Summary: A CSV filter directive for docutils and Sphinx, that extends the "csv-table" reStructuredText directive to add row filtering options.
 Home-page: https://github.com/crate/sphinx_csv_filter
 Author: Crate.IO GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Keywords: sphinx csv filter docutils directive plugin csv-table csv-filter restructuredtext
 Platform: any
@@ -40,15 +40,15 @@
 Sphinx CSV filter
 =================
 
 .. image:: https://github.com/crate/sphinx_csv_filter/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/crate/sphinx_csv_filter/actions/workflows/tests.yml
     :alt: CI outcome
 
-.. image:: https://codecov.io/gh/crate/sphinx_csv_filter/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/crate/sphinx_csv_filter/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/crate/sphinx_csv_filter
     :alt: Test suite code coverage
 
 .. image:: https://img.shields.io/pypi/v/sphinx-csv-filter.svg
     :target: https://pypi.org/project/sphinx-csv-filter/
     :alt: Supported Python versions
```

### Comparing `sphinx-csv-filter-0.4.0/README.rst` & `sphinx-csv-filter-0.4.1/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Sphinx CSV filter
 =================
 
 .. image:: https://github.com/crate/sphinx_csv_filter/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/crate/sphinx_csv_filter/actions/workflows/tests.yml
     :alt: CI outcome
 
-.. image:: https://codecov.io/gh/crate/sphinx_csv_filter/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/crate/sphinx_csv_filter/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/crate/sphinx_csv_filter
     :alt: Test suite code coverage
 
 .. image:: https://img.shields.io/pypi/v/sphinx-csv-filter.svg
     :target: https://pypi.org/project/sphinx-csv-filter/
     :alt: Supported Python versions
```

### Comparing `sphinx-csv-filter-0.4.0/setup.cfg` & `sphinx-csv-filter-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `sphinx-csv-filter-0.4.0/setup.py` & `sphinx-csv-filter-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 def read(path):
     with open(os.path.join(os.path.dirname(__file__), path)) as f:
         return f.read()
 
 
 setup(
     name='sphinx-csv-filter',
-    version='0.4.0',
+    version='0.4.1',
     url='https://github.com/crate/sphinx_csv_filter',
     author='Crate.IO GmbH',
     author_email='office@crate.io',
     package_dir={'': 'src'},
     description='A CSV filter directive for docutils and Sphinx, that extends the '
                 '"csv-table" reStructuredText directive to add row filtering options.',
     long_description=read('README.rst'),
```

### Comparing `sphinx-csv-filter-0.4.0/src/crate/__init__.py` & `sphinx-csv-filter-0.4.1/src/crate/__init__.py`

 * *Files identical despite different names*

### Comparing `sphinx-csv-filter-0.4.0/src/crate/sphinx/csv.py` & `sphinx-csv-filter-0.4.1/src/crate/sphinx/csv.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,7 +113,11 @@
                     'The CSV data does not contain that many columns.')
                 raise SystemMessagePropagation(error)
         return prepared_rows, len(included_cols_list)
 
 
 def setup(sphinx):
     sphinx.add_directive('csv-filter', CSVFilterDirective)
+    return {
+        'parallel_read_safe': True,
+        'parallel_write_safe': True,
+    }
```

### Comparing `sphinx-csv-filter-0.4.0/src/sphinx_csv_filter.egg-info/PKG-INFO` & `sphinx-csv-filter-0.4.1/src/sphinx_csv_filter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinx-csv-filter
-Version: 0.4.0
+Version: 0.4.1
 Summary: A CSV filter directive for docutils and Sphinx, that extends the "csv-table" reStructuredText directive to add row filtering options.
 Home-page: https://github.com/crate/sphinx_csv_filter
 Author: Crate.IO GmbH
 Author-email: office@crate.io
 License: Apache License 2.0
 Keywords: sphinx csv filter docutils directive plugin csv-table csv-filter restructuredtext
 Platform: any
@@ -40,15 +40,15 @@
 Sphinx CSV filter
 =================
 
 .. image:: https://github.com/crate/sphinx_csv_filter/actions/workflows/tests.yml/badge.svg
     :target: https://github.com/crate/sphinx_csv_filter/actions/workflows/tests.yml
     :alt: CI outcome
 
-.. image:: https://codecov.io/gh/crate/sphinx_csv_filter/branch/master/graph/badge.svg
+.. image:: https://codecov.io/gh/crate/sphinx_csv_filter/branch/main/graph/badge.svg
     :target: https://app.codecov.io/gh/crate/sphinx_csv_filter
     :alt: Test suite code coverage
 
 .. image:: https://img.shields.io/pypi/v/sphinx-csv-filter.svg
     :target: https://pypi.org/project/sphinx-csv-filter/
     :alt: Supported Python versions
```

