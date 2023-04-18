# Comparing `tmp/opencmiss2cmlibs-0.1.0.tar.gz` & `tmp/opencmiss2cmlibs-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencmiss2cmlibs-0.1.0.tar", last modified: Tue Apr 18 07:00:41 2023, max compression
+gzip compressed data, was "opencmiss2cmlibs-0.1.1.tar", last modified: Tue Apr 18 07:05:52 2023, max compression
```

## Comparing `opencmiss2cmlibs-0.1.0.tar` & `opencmiss2cmlibs-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.436468 opencmiss2cmlibs-0.1.0/
--rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2023-03-27 09:14:03.000000 opencmiss2cmlibs-0.1.0/LICENSE
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1014 2023-04-18 07:00:41.436601 opencmiss2cmlibs-0.1.0/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      544 2023-04-12 21:27:34.000000 opencmiss2cmlibs-0.1.0/README.rst
--rw-r--r--   0 hsor001  (1210695619) 1403514002       91 2023-03-28 00:57:24.000000 opencmiss2cmlibs-0.1.0/pyproject.toml
--rw-r--r--   0 hsor001  (1210695619) 1403514002      731 2023-04-18 07:00:41.437355 opencmiss2cmlibs-0.1.0/setup.cfg
--rw-r--r--   0 hsor001  (1210695619) 1403514002       69 2023-03-28 00:57:18.000000 opencmiss2cmlibs-0.1.0/setup.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.417084 opencmiss2cmlibs-0.1.0/src/
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.425859 opencmiss2cmlibs-0.1.0/src/libocm2cml/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:37:49.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6651 2023-03-28 08:02:24.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/btm_matcher.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     9983 2023-03-28 08:03:52.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/btm_utils.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     6644 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/fixer_base.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    14713 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/fixer_util.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.427189 opencmiss2cmlibs-0.1.0/src/libocm2cml/fixes/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:30:01.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/fixes/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5488 2023-03-30 20:28:26.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/fixes/fix_imports.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     7055 2023-03-28 07:49:09.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/patcomp.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.432782 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/
--rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:40:03.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/__init__.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5970 2023-03-28 07:45:09.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/driver.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     5565 2023-04-04 01:09:27.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/grammar.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1644 2023-03-28 07:49:35.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/literals.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     8159 2023-03-28 07:46:32.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/parse.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    13855 2023-04-04 01:13:18.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/pgen.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1320 2023-04-04 01:10:05.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/token.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    20916 2023-03-31 02:18:24.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/tokenize.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1254 2023-04-04 01:11:42.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pygram.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    28050 2023-03-28 07:43:56.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/pytree.py
--rw-r--r--   0 hsor001  (1210695619) 1403514002    27525 2023-03-28 07:59:16.000000 opencmiss2cmlibs-0.1.0/src/libocm2cml/refactor.py
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.435450 opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     1014 2023-04-18 07:00:41.000000 opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/PKG-INFO
--rw-r--r--   0 hsor001  (1210695619) 1403514002      862 2023-04-18 07:00:41.000000 opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/SOURCES.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-18 07:00:41.000000 opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/dependency_links.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002      125 2023-04-18 07:00:41.000000 opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/entry_points.txt
--rw-r--r--   0 hsor001  (1210695619) 1403514002       11 2023-04-18 07:00:41.000000 opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/top_level.txt
-drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:00:41.435833 opencmiss2cmlibs-0.1.0/tests/
--rw-r--r--   0 hsor001  (1210695619) 1403514002     3508 2023-03-30 20:42:48.000000 opencmiss2cmlibs-0.1.0/tests/test_import.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:52.012878 opencmiss2cmlibs-0.1.1/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      595 2023-03-27 09:14:03.000000 opencmiss2cmlibs-0.1.1/LICENSE
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1556 2023-04-18 07:05:52.013010 opencmiss2cmlibs-0.1.1/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      851 2023-04-18 07:04:17.000000 opencmiss2cmlibs-0.1.1/README.rst
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       91 2023-03-28 00:57:24.000000 opencmiss2cmlibs-0.1.1/pyproject.toml
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      731 2023-04-18 07:05:52.013542 opencmiss2cmlibs-0.1.1/setup.cfg
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       69 2023-03-28 00:57:18.000000 opencmiss2cmlibs-0.1.1/setup.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:51.996636 opencmiss2cmlibs-0.1.1/src/
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:52.004500 opencmiss2cmlibs-0.1.1/src/libocm2cml/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:37:49.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6651 2023-03-28 08:02:24.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/btm_matcher.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     9983 2023-03-28 08:03:52.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/btm_utils.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     6644 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/fixer_base.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    14713 2023-03-28 07:55:22.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/fixer_util.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:52.005584 opencmiss2cmlibs-0.1.1/src/libocm2cml/fixes/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:30:01.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/fixes/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5488 2023-03-30 20:28:26.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/fixes/fix_imports.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     7055 2023-03-28 07:49:09.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/patcomp.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:52.010172 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        0 2023-03-28 07:40:03.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/__init__.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5970 2023-03-28 07:45:09.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/driver.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     5565 2023-04-04 01:09:27.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/grammar.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1644 2023-03-28 07:49:35.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/literals.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     8159 2023-03-28 07:46:32.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/parse.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    13855 2023-04-04 01:13:18.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/pgen.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1320 2023-04-04 01:10:05.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/token.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    20916 2023-03-31 02:18:24.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/tokenize.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1254 2023-04-04 01:11:42.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pygram.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    28050 2023-03-28 07:43:56.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/pytree.py
+-rw-r--r--   0 hsor001  (1210695619) 1403514002    27525 2023-03-28 07:59:16.000000 opencmiss2cmlibs-0.1.1/src/libocm2cml/refactor.py
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:52.012125 opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     1556 2023-04-18 07:05:51.000000 opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/PKG-INFO
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      862 2023-04-18 07:05:51.000000 opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/SOURCES.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002        1 2023-04-18 07:05:51.000000 opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/dependency_links.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002      125 2023-04-18 07:05:51.000000 opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/entry_points.txt
+-rw-r--r--   0 hsor001  (1210695619) 1403514002       11 2023-04-18 07:05:51.000000 opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/top_level.txt
+drwxr-xr-x   0 hsor001  (1210695619) 1403514002        0 2023-04-18 07:05:52.012376 opencmiss2cmlibs-0.1.1/tests/
+-rw-r--r--   0 hsor001  (1210695619) 1403514002     3508 2023-03-30 20:42:48.000000 opencmiss2cmlibs-0.1.1/tests/test_import.py
```

### Comparing `opencmiss2cmlibs-0.1.0/LICENSE` & `opencmiss2cmlibs-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/setup.cfg` & `opencmiss2cmlibs-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/btm_matcher.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/btm_matcher.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/btm_utils.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/btm_utils.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/fixer_base.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/fixer_base.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/fixer_util.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/fixer_util.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/fixes/fix_imports.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/fixes/fix_imports.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/patcomp.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/patcomp.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/driver.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/driver.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/grammar.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/grammar.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/literals.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/literals.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/parse.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/parse.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/pgen.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/pgen.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/token.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/token.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pgen2/tokenize.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pgen2/tokenize.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pygram.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pygram.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/pytree.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/pytree.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/libocm2cml/refactor.py` & `opencmiss2cmlibs-0.1.1/src/libocm2cml/refactor.py`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/src/opencmiss2cmlibs.egg-info/SOURCES.txt` & `opencmiss2cmlibs-0.1.1/src/opencmiss2cmlibs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `opencmiss2cmlibs-0.1.0/tests/test_import.py` & `opencmiss2cmlibs-0.1.1/tests/test_import.py`

 * *Files identical despite different names*

