# Comparing `tmp/npstructures-0.2.8.tar.gz` & `tmp/npstructures-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npstructures-0.2.8.tar", last modified: Tue Dec  6 15:58:48 2022, max compression
+gzip compressed data, was "npstructures-0.2.9.tar", last modified: Tue Dec 20 15:26:49 2022, max compression
```

## Comparing `npstructures-0.2.8.tar` & `npstructures-0.2.9.tar`

### file list

```diff
@@ -1,72 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.078699 npstructures-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-06 15:58:16.000000 npstructures-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2022-12-06 15:58:16.000000 npstructures-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-06 15:58:16.000000 npstructures-0.2.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-06 15:58:16.000000 npstructures-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-06 15:58:16.000000 npstructures-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2022-12-06 15:58:48.078699 npstructures-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4204 2022-12-06 15:58:16.000000 npstructures-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.070699 npstructures-0.2.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/authors.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4984 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      319 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      774 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      233 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2022-12-06 15:58:16.000000 npstructures-0.2.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.074699 npstructures-0.2.8/npstructures/
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/arrayfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3486 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/bitarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.074699 npstructures-0.2.8/npstructures/cupy_compatible/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/cupy_compatible/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/cupy_compatible/bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/cupy_compatible/hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/cupy_compatible/raggedarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/cupy_compatible/raggedshape.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/cupy_compatible/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     9696 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/npdataclasses.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.074699 npstructures-0.2.8/npstructures/raggedarray/
--rw-r--r--   0 runner    (1001) docker     (123)    17096 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/raggedarray/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/raggedarray/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/raggedarray/indexablearray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/raggedarray/raggedslice.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/raggedshape.py
--rw-r--r--   0 runner    (1001) docker     (123)    18930 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/runlengtharray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2022-12-06 15:58:16.000000 npstructures-0.2.8/npstructures/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.074699 npstructures-0.2.8/npstructures.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2022-12-06 15:58:48.000000 npstructures-0.2.8/npstructures.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2022-12-06 15:58:48.000000 npstructures-0.2.8/npstructures.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 15:58:48.000000 npstructures-0.2.8/npstructures.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-06 15:58:47.000000 npstructures-0.2.8/npstructures.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-06 15:58:48.000000 npstructures-0.2.8/npstructures.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-06 15:58:48.000000 npstructures-0.2.8/npstructures.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-06 15:58:48.078699 npstructures-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2022-12-06 15:58:16.000000 npstructures-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.074699 npstructures-0.2.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/npbackend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:48.078699 npstructures-0.2.8/tests/property_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5823 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/strategies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/test_hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)    14065 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/test_ragged_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     6964 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/test_runlengtharray.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/property_tests/test_ufunc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_arrayfunctions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_bitarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_counter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_hashtable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_npdataclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12862 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_raggedarray.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_raggedshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2022-12-06 15:58:16.000000 npstructures-0.2.8/tests/test_runlengtharray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.819811 npstructures-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2022-12-20 15:26:16.000000 npstructures-0.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3579 2022-12-20 15:26:16.000000 npstructures-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2022-12-20 15:26:16.000000 npstructures-0.2.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-20 15:26:16.000000 npstructures-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2022-12-20 15:26:16.000000 npstructures-0.2.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2022-12-20 15:26:49.819811 npstructures-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4204 2022-12-20 15:26:16.000000 npstructures-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.807811 npstructures-0.2.9/npstructures/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/arrayfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3486 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/bitarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.811811 npstructures-0.2.9/npstructures/cupy_compatible/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/cupy_compatible/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/cupy_compatible/bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/cupy_compatible/hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/cupy_compatible/raggedarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/cupy_compatible/raggedshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/cupy_compatible/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9696 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/npdataclasses.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.811811 npstructures-0.2.9/npstructures/raggedarray/
+-rw-r--r--   0 runner    (1001) docker     (123)    19044 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/raggedarray/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/raggedarray/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5860 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/raggedarray/indexablearray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/raggedarray/raggedslice.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21563 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/raggedshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23824 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/runlengtharray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2022-12-20 15:26:16.000000 npstructures-0.2.9/npstructures/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.811811 npstructures-0.2.9/npstructures.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2022-12-20 15:26:49.000000 npstructures-0.2.9/npstructures.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2022-12-20 15:26:49.000000 npstructures-0.2.9/npstructures.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:26:49.000000 npstructures-0.2.9/npstructures.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 15:26:49.000000 npstructures-0.2.9/npstructures.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-20 15:26:49.000000 npstructures-0.2.9/npstructures.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-20 15:26:49.000000 npstructures-0.2.9/npstructures.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-20 15:26:49.819811 npstructures-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2022-12-20 15:26:16.000000 npstructures-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.815811 npstructures-0.2.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/npbackend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:49.819811 npstructures-0.2.9/tests/property_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5823 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/test_bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/test_hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14065 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/test_ragged_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/test_runlengtharray.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/property_tests/test_ufunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_arrayfunctions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_bitarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_counter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_hashtable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_npdataclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12894 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_raggedarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_raggedshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2022-12-20 15:26:16.000000 npstructures-0.2.9/tests/test_runlengtharray.py
```

### Comparing `npstructures-0.2.8/CONTRIBUTING.rst` & `npstructures-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/LICENSE` & `npstructures-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/PKG-INFO` & `npstructures-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npstructures
-Version: 0.2.8
+Version: 0.2.9
 Summary: Simple data structures that augments the numpy library
 Home-page: https://github.com/knutdrand/npstructures
 Author: Knut Rand
 Author-email: knutdrand@gmail.com
 License: MIT license
 Keywords: npstructures
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `npstructures-0.2.8/README.rst` & `npstructures-0.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/__init__.py` & `npstructures-0.2.9/npstructures/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,22 +3,23 @@
 arrays with different row sizes.
 
 
 """
 
 __author__ = """Knut Rand"""
 __email__ = "knutdrand@gmail.com"
-__version__ = '0.2.8'
+__version__ = '0.2.9'
 
 from . import raggedarray, raggedshape, hashtable
 
 from .raggedarray import RaggedArray
 from .raggedarray.raggedslice import ragged_slice
 from .raggedshape import RaggedShape, RaggedView
 from .hashtable import HashTable, Counter, HashSet
+from .bitarray import BitArray
 from .npdataclasses import npdataclass, VarLenArray
 from .runlengtharray import RunLength2dArray, RunLengthArray, RunLengthRaggedArray
 __all__ = [
     "HashTable",
     "Counter",
     "RaggedShape",
     "RaggedArray",
```

### Comparing `npstructures-0.2.8/npstructures/arrayfunctions.py` & `npstructures-0.2.9/npstructures/arrayfunctions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,15 @@
+import numpy.typing as npt
+from typing import Union, List, Tuple, Dict, NewType
 from numbers import Number
 import numpy as np
 from .raggedshape import RaggedView
 
+RaggedArray = NewType('RaggedArray', npt.ArrayLike)
+
 
 def get_ra_func(name):
     return lambda ragged_array, *args, **kwargs: getattr(ragged_array, name)(
         *args, **kwargs
     )
 
 
@@ -44,91 +48,163 @@
         HANDLED_FUNCTIONS[np_function] = func
         return func
 
     return decorator
 
 
 @implements(np.concatenate)
-def concatenate(ragged_arrays, axis=0):
+def concatenate(ragged_arrays: List[RaggedArray], axis: int = 0) -> RaggedArray:
+    """Concatenate a set of raggedarrays along the given axis
+
+    Parameters
+    ----------
+    ragged_arrays : List[RaggedArray]
+    axis : int
+
+    Returns
+    -------
+    RaggedArray
+
+    """
     if axis == 0:
         data = np.concatenate([ra.ravel() for ra in ragged_arrays])
         row_sizes = np.concatenate([ra._shape.lengths for ra in ragged_arrays])
         return ragged_arrays[0].__class__(data, row_sizes)
     elif axis in [-1, 1]:
         return ragged_arrays[0].__class__([np.concatenate([row for row in rows])
                                            for rows in zip(*ragged_arrays)])
     else:
         return NotImplemented
 
 
 @implements(np.diff)
-def diff(ragged_array, n=1, axis=-1):
+def diff(ragged_array: RaggedArray, n: int = 1, axis: int = -1) -> RaggedArray:
+    """Return diffs for each row in a raggedarray
+
+    Parameters
+    ----------
+    ragged_array : RaggedArray
+    n : int
+    axis : int
+
+    """
     if axis not in [-1, 1]:
         return NotImplemented
-
-    # assert np.all(ragged_array._shape.lengths>=n)
     d = np.diff(ragged_array.ravel(), n=n)
     lengths = np.maximum(ragged_array._shape.lengths - n, 0)
     indices, shape = RaggedView(ragged_array._shape.starts, lengths).get_flat_indices()
     return ragged_array.__class__(d[indices], shape)
 
 
-# @implements(np.all):
-# def our_all(ragged_array, *args, **kwargs):
-#     return ragged_array.all(*args, **kwargs)
-#
-# @implements(np.sum):
-# def our_sum(ragged_array, *args, **kwargs):
-#     return ragged_array.sum(*args, **kwargs)
-#
-# @implements(np.nonzero)
-# def nonzero(ragged_array):
-#     return ragged_array.nonzero()
+@implements(np.zeros_like)
+def zeros_like(ragged_array: RaggedArray, dtype: npt.DTypeLike = None, shape: Tuple[int] = None) -> RaggedArray:
+    """Return a raggedarray with the same shape and dtype as raggedarray filled with zeros
 
+    Parameters
+    ----------
+    ragged_array : RaggedArray
+    dtype : npt.DTypeLike
+    shape : Tuple[int]
+
+    Returns
+    -------
+    RaggedArray
 
-@implements(np.zeros_like)
-def zeros_like(ragged_array, dtype=None, shape=None):
+    """
     shape = ragged_array._shape if shape is None else shape
     dtype = ragged_array.dtype if dtype is None else dtype
     data = np.zeros(shape.size, dtype=dtype)
     return ragged_array.__class__(data, shape=shape)
 
 
 @implements(np.ones_like)
-def ones_like(ragged_array, dtype=None, shape=None):
+def ones_like(ragged_array: RaggedArray, dtype: npt.DTypeLike=None, shape: Tuple[int]=None) -> RaggedArray:
+    """Return a raggedarray with the same shape and dtype as raggedarray filled with ones
+
+    Parameters
+    ----------
+    ragged_array : RaggedArray
+    dtype : npt.DTypeLike
+    shape : Tuple[int]
+
+    Returns
+    -------
+    RaggedArray
+
+    """
     shape = ragged_array._shape if shape is None else shape
     dtype = ragged_array.dtype if dtype is None else dtype
     data = np.ones(shape.size, dtype=dtype)
     return ragged_array.__class__(data, shape=shape)
 
 
 @implements(np.empty_like)
-def empty_like(ragged_array, dtype=None, shape=None):
+def empty_like(ragged_array: RaggedArray, dtype: npt.DTypeLike=None, shape: Tuple[int]=None) -> RaggedArray:
+    """Return an empty raggedarray with the same shape and dtype as raggedarray
+
+    Parameters
+    ----------
+    ragged_array : RaggedArray
+    dtype : npt.DTypeLike
+    shape : Tuple[int]
+
+    Returns
+    -------
+    RaggedArray
+
+    """
     shape = ragged_array._shape if shape is None else shape
     dtype = ragged_array.dtype if dtype is None else dtype
     data = np.empty(shape.size, dtype=dtype)
     return ragged_array.__class__(data, shape=shape)
 
 
 @implements(np.where)
-def where(ragged_mask, x=None, y=None):
+def where(ragged_mask: RaggedArray, x: RaggedArray=None, y: RaggedArray=None) -> RaggedArray:
+    """Perform an ifelse (tertiary operator) on a raggedarray
+
+    Inicies where ragged_mask is True gets the corresponding value
+    from x. Where False it gets from y
+
+    Parameters
+    ----------
+    ragged_mask : RaggedArray
+    x : RaggedArray
+    y : RaggedArray
+
+    Returns
+    -------
+    RaggedArray
+    """
     assert (x is not None) and (y is not None), "where is only supported for ifelse for ragged_array"
     cls = x.__class__
     if not isinstance(x, Number):
         if ragged_mask.size < x.size:
             ragged_mask = x._broadcast_rows(ragged_mask) #TODO: this is ugly, clean
         x = x.ravel()
     if not isinstance(y, Number):
         y = y.ravel()
     data = np.where(ragged_mask.ravel(), x, y)
     return cls(data, ragged_mask._shape)
 
 
 @implements(np.unique)
-def unique(ragged_array, axis=None, return_counts=False):
+def unique(ragged_array: RaggedArray, axis: int=None, return_counts: bool=False) -> Union[RaggedArray, Tuple[RaggedArray]]:                                                                                                             
+    """Get the unqiue values from ragged_array. If return_counts then also return the number of elemtents with each value
+
+    Parameters
+    ----------
+    ragged_array : RaggedArray
+    axis : int
+    return_counts : bool
+
+    Returns
+    -------
+    Union[RaggedArray, Tuple[RaggedArray]]
+    """
     if axis is None:
         return np.unique(ragged_array.ravel(), return_counts=return_counts)
 
     if axis not in (-1, 1):
         return NotImplemented
     if ragged_array.size == 0:
         if return_counts:
```

### Comparing `npstructures-0.2.8/npstructures/bitarray.py` & `npstructures-0.2.9/npstructures/bitarray.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/cupy_compatible/bitarray.py` & `npstructures-0.2.9/npstructures/cupy_compatible/bitarray.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/cupy_compatible/hashtable.py` & `npstructures-0.2.9/npstructures/cupy_compatible/hashtable.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/cupy_compatible/raggedarray.py` & `npstructures-0.2.9/npstructures/cupy_compatible/raggedarray.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/cupy_compatible/raggedshape.py` & `npstructures-0.2.9/npstructures/cupy_compatible/raggedshape.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/hashtable.py` & `npstructures-0.2.9/npstructures/hashtable.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/mixin.py` & `npstructures-0.2.9/npstructures/mixin.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/npdataclasses.py` & `npstructures-0.2.9/npstructures/npdataclasses.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/raggedarray/__init__.py` & `npstructures-0.2.9/npstructures/raggedarray/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,26 @@
+import types
+from typing import Tuple, Dict, List, Union
+import numpy.typing as npt
 import numpy as np
 from numbers import Number
 from .indexablearray import IndexableArray
 from ..raggedshape import RaggedShape, RaggedView, ViewBase, RaggedView2
 from ..util import unsafe_extend_left
 from ..arrayfunctions import HANDLED_FUNCTIONS, REDUCTIONS, ACCUMULATIONS
 
 
 class Shape(tuple):
     def __eq__(self, other):
         return (np.all(s == o) for s, o in zip(self, other))
 
 
+ShapeLike = Union[List[int], RaggedShape, RaggedView, Shape]
+
+
 def reduction(allowed_axis=(None, 0, -1, 1)):
     def reduction_func(func):
         def new_func(self, axis=None, keepdims=False):
             if axis is None:
                 return getattr(np, func.__name__)(self.ravel()).item()  # force return of scalar, not object
             else:
                 if axis not in allowed_axis:
@@ -31,20 +37,14 @@
 
 INVERSE_FUNCS = {
     np.add: (np.subtract, np.add),
     np.subtract: (np.subtract, np.add),
     np.bitwise_xor: (np.bitwise_xor, np.bitwise_xor),
 }
 
-# INVERSE_FUNCS = {
-#     np.add: lambda x: -x
-#     np.subtract:
-#     np.bitwise_xor: (np.bitwise_xor, np.bitwise_xor),
-# }
-
 
 class RaggedArray(IndexableArray, np.lib.mixins.NDArrayOperatorsMixin):
     """Class to represent 2d arrays with differing row lengths
 
     Provides objects that behaves similar to numpy ndarrays, but
     can represent arrays with differing row lengths. Numpy-like functionality is
     provided in three ways.
@@ -84,70 +84,88 @@
     array([3, 2])
     >>> ra[0:2]
     RaggedArray([[2, 4, 8], [3, 2]])
     >>> np.nonzero(ra>3)
     (array([0, 0, 2, 2]), array([1, 2, 0, 1]))
     """
 
-    def __init__(self, data, shape=None, dtype=None, safe_mode=True):
+    def __init__(self, data: npt.ArrayLike, shape: ShapeLike = None, dtype: npt.DTypeLike = None, safe_mode: bool = True):
         if shape is None:
             data, shape = self._from_array_list(data, dtype)
         elif isinstance(shape, (ViewBase, RaggedView2)):
             shape = shape
         else:
             shape = RaggedShape.asshape(shape)
         if not hasattr(data, "__array_ufunc__"):
             data = np.asanyarray(data, dtype=dtype)
         super().__init__(data, shape)
         self._safe_mode = safe_mode
 
     @property
-    def shape(self):
+    def shape(self) -> Shape:
         return Shape((self._shape.n_rows, self._shape.lengths))
 
     @property
-    def lengths(self):
+    def lengths(self) -> npt.ArrayLike:
         return self._shape.lengths
 
-    def astype(self, dtype):
+    def astype(self, dtype: npt.DTypeLike) -> 'RaggedArray':
+        """Return ragged array with underlying data changed to dtype
+
+        Parameters
+        ----------
+        dtype : npt.DTypeLike
+
+        Returns
+        -------
+        'RaggedArray'
+
+        """
         return RaggedArray(self.ravel().astype(dtype), self._shape)
 
-    def __len__(self):
+    def __len__(self) -> int:
         return self._shape.n_rows
 
-    def __iter__(self):
+    def __iter__(self) -> types.GeneratorType:
+        """Return an iterator over the rows in the ragged array
+
+        Returns
+        -------
+        types.GeneratorType
+
+        """
         flat = self.ravel()
         return (
             flat[start:start + l]
             for start, l in zip(self._shape.starts, self._shape.lengths)
         )
 
     def __repr__(self) -> str:
         if self.size > 100:
             rows = [str(row[:100]) for row in self[:100]]
         else:
             rows = [f"{row}" for row in self]
         text = "\n".join(rows)
         return f"ragged_array({text})"
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "\n".join(str(row) for row in self[:20])
 
     def save(self, filename):
         """Saves the ragged array to file using np.savez
 
         Parameters
         ----------
         filename : str
             name of the file
         """
         np.savez(filename, data=self.ravel(), **(self._shape.to_dict()))
 
     @classmethod
-    def load(cls, filename):
+    def load(cls, filename: str) -> 'RaggedArray':
         """Loads a ragged array from file
 
         Parameters
         ----------
         filename : str
             name of the file
 
@@ -161,27 +179,43 @@
         return cls(D["data"], shape)
 
     def equals(self, other):
         """Checks for euqality with `other`"""
         t = np.all(self.ravel() == other.ravel())
         return t and (self._shape == other._shape)
 
-    def tolist(self):
-        """Returns a list of list of rows"""
+    def tolist(self) -> List[List]:
+        """Return a list of list representing rows
+
+        Returns
+        -------
+        List[List]
+
+        """
         return [row.tolist() for row in self]
 
-    def to_numpy_array(self):
+    def to_numpy_array(self) -> np.ndarray:
+        """
+        Return a normal numpy array with the same shape and data
+
+        Requires that all the rows are of the same lengths
+
+        Returns
+        -------
+        np.ndarray
+        """
+
         if len(self) == 0:
             return np.empty(shape=(0, 0))
         L = self._shape.lengths[0]
         assert np.all(self._shape.lengths == L)
         return self.ravel().reshape(self._shape.n_rows, L)
 
     @classmethod
-    def from_numpy_array(cls, array):
+    def from_numpy_array(cls, array: npt.ArrayLike) -> 'RaggedArray':
         shape = RaggedShape.from_tuple_shape(array.shape)
         return cls(array.ravel(), shape)
 
     @classmethod
     def _from_array_list(cls, array_list, dtype=None):
         data = np.array(
             [element for array in array_list for element in array], dtype=dtype
@@ -237,15 +271,33 @@
     def _accumulate(self, ufunc, ra, axis=0, **kwargs):
         if ufunc in (np.add, np.subtract, np.bitwise_xor):
             return self._row_accumulate(ufunc)
         if ufunc not in ACCUMULATIONS:
             return NotImplemented
         return getattr(np, ACCUMULATIONS[ufunc])(ra, axis=axis, **kwargs)
 
-    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+    def __array_ufunc__(self, ufunc: callable, method: str, *inputs, **kwargs):
+        """Handles ufuncs called on raggedarray objects. 
+
+        Supports __call__ reduce and accumulate modes. Broadcasts any
+        column vectors to the shape of the raggedarray, and numbers to
+        the whole array
+
+        Parameters
+        ----------
+        ufunc : callable
+        method : str
+        *inputs :
+        **kwargs :
+
+        Raises
+        ------
+        TypeError
+
+        """
         if method not in ("__call__", "reduce", "accumulate"):
             return NotImplemented
         self.ravel()
         if method == "reduce":
             return self._reduce(ufunc, inputs[0], **kwargs)
         if method == "accumulate":
             return self._accumulate(ufunc, inputs[0], **kwargs)
@@ -263,27 +315,43 @@
                 datas.append(input.ravel())
                 if self._safe_mode and (input._shape != self._shape):
                     raise TypeError("inconsistent sizes")
             else:
                 return NotImplemented
         return RaggedArray(ufunc(*datas, **kwargs), self._shape)
 
-    def __array_function__(self, func, types, args, kwargs):
+    def __array_function__(self, func: callable, types: List, args: List, kwargs: Dict):
+        """Handles any numpy array functions called on a raggedarray
+
+        Parameters
+        ----------
+        func : callable
+        types : List
+        args : List
+        kwargs : Dict
+        """
         self.ravel()
         if func not in HANDLED_FUNCTIONS:
             return NotImplemented
         if func != np.where and not all(issubclass(t, self.__class__) for t in types):
             return NotImplemented
         return HANDLED_FUNCTIONS[func](*args, **kwargs)
 
-    def fill(self, value):
+    def fill(self, value: Number):
+        ''' Fill the whole array with value'''
         self.ravel().fill(value)
 
-    def nonzero(self):
-        """Return the row- and column indices of nonzero elements"""
+    def nonzero(self) -> Tuple[npt.ArrayLike]:
+        """Return the indices of all nonzero entries in the array
+
+        Returns
+        -------
+        Tuple[npt.ArrayLike]
+        """
+        
         flat_indices = np.flatnonzero(self.ravel())
         return self._shape.unravel_multi_index(flat_indices)
 
     @reduction(allowed_axis=(None, 0, 1, -1))
     def sum(self, axis=None):
         """Calculate sum or rowsums of the array
 
@@ -415,15 +483,26 @@
         _, idxs = np.unique(rows, return_index=True)
         return cols[idxs]
 
     @reduction(allowed_axis=(-1, 1))
     def argmin(self, axis=None):
         return (-self).argmax(axis=-1)
 
-    def cumsum(self, axis=None, dtype=None):
+    def cumsum(self, axis: int = None, dtype: npt.DTypeLike = None) -> 'RaggedArray':
+        """Return an array with cumulative sums along the given axis
+
+        Parameters
+        ----------
+        axis : int
+        dtype : npt.DTypeLike
+
+        Returns
+        -------
+        RaggedArray
+        """
         if axis is None:
             return self.ravel().cumsum(dtype=dtype)
         assert axis in (1, -1)
         if self.size == 0:
             return np.empty_like(self)
         if np.issubdtype(self.dtype, np.integer):  # in (np.int8, np.int16, np.int32, np.int64):
             cm = np.cumsum(unsafe_extend_left(self.ravel()), dtype=dtype)
@@ -454,15 +533,15 @@
     def sort(self, axis=-1):
         if axis is None:
             return self.ravel().sort()
         if axis in (1, -1):
             args = np.lexsort((self.ravel(), self._shape.index_array()))
             return self.__class__(self.ravel()[args], self._shape)
 
-    def as_padded_matrix(self, fill_value=0, side='right'):
+    def _as_padded_matrix(self, fill_value=0, side='right'):
         assert side in ["left", "right"]
 
         ends = self._shape.ends
         starts = self._shape.starts
         max_chars = np.max(ends-starts)
         view_starts = starts if side == "right" else ends-max_chars
```

### Comparing `npstructures-0.2.8/npstructures/raggedarray/indexablearray.py` & `npstructures-0.2.9/npstructures/raggedarray/indexablearray.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 import types
+from typing import Dict, Tuple, List, Union
+import numpy.typing as npt
 import numpy as np
 from numbers import Number
 from ..raggedshape import RaggedView2, RaggedView
 from .base import RaggedBase
 import numpy as _np
 
 
 class IndexableArray(RaggedBase):
-
+    ''' 
+    Base class for ragged array that handles evertything to do with indexing
+    '''
     def __build_data_from_indices_generator(self, indices_generator, size):
         out_data = np.empty(int(size), dtype=self.dtype)
         offset = 0
         for indices in indices_generator:
             n_indices = indices.size
             out_data[offset:offset+n_indices] = self.ravel()[indices]
             offset += n_indices
         return out_data
 
-    def __getitem__(self, index):
-        # self.ravel()
+    def __getitem__(self, index: Union[Tuple, List[int], npt.ArrayLike, int, slice]):
         ret = self._get_row_subset(index, do_split=False)
         if ret == NotImplemented:
             raise NotImplementedError()
         if isinstance(ret, (RaggedView2, RaggedView)):
             return self._change_view(ret)
         index, shape = ret
         if shape is None:
@@ -73,15 +76,15 @@
             return self._get_multiple_rows(np.asanyarray(index), do_split)
         elif isinstance(index, IndexableArray):
             if np.issubdtype(index, bool):
                 return np.flatnonzero(index.ravel()), None
         else:
             return NotImplemented
 
-    def __setitem__(self, _index, value):
+    def __setitem__(self, _index: Union[Tuple, List[int], npt.ArrayLike, int, slice], value: npt.ArrayLike):
         self.ravel()
         ret = self._get_row_subset(_index)
         if ret == NotImplemented:
             raise TypeError(f"Invalid index for ragged array {type(_index)}: {_index}")
         if isinstance(ret, (RaggedView, RaggedView2)):
             ret = self._get_view(ret)
         index, shape = ret
```

### Comparing `npstructures-0.2.8/npstructures/raggedarray/raggedslice.py` & `npstructures-0.2.9/npstructures/raggedarray/raggedslice.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/raggedshape.py` & `npstructures-0.2.9/npstructures/raggedshape.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 from numbers import Number
 from dataclasses import dataclass
 import numpy as np
 
 
+def build_indices(view, to_shape, step):
+    step = 1 if step is None else step
+    index_builder = np.full(to_shape.size + 1, step, dtype=view._dtype)
+    if np.any(to_shape.lengths == 0):
+        np.add.at(index_builder, to_shape.starts[1:], view.starts[1:]-view.ends[:-1]-step+1)
+        np.add.at(index_builder, 0, view.starts[0]-step)
+    else:
+        index_builder[to_shape.starts[1:]] = view.starts[1:]-view.ends[:-1] + 1
+        index_builder[0] = view.starts[0]
+    np.cumsum(index_builder, out=index_builder)
+    return index_builder[:-1], to_shape
+
+
 class ViewBase:
     _dtype = np.int64
 
     @classmethod
     def set_dtype(cls, dtype):
         cls._dtype = dtype
 
@@ -371,52 +384,78 @@
             return 1
         return len(self.starts)
 
     def row_slice(self, row_slice):
         return self.__class__(self.starts[row_slice], self.ends[row_slice], self.col_step)
 
     def _calculate_lengths(self, col_slice):
-        start, stop, step = (col_slice.start, col_slice.stop, col_slice.step)        
+        """ Figure out how long each line will be after a col slice"""
+
+        start, stop, step = (col_slice.start, col_slice.stop, col_slice.step)
         if step is None:
             step = 1
         assert step != 0
         if start is None:
             start = 0 if step >= 0 else self.lengths-1
         elif start < 0:
             start = self.lengths+start
         if stop is None:
             stop = self.lengths if step >= 0 else -1
         elif stop < 0:
             stop = self.lengths+stop
 
-        mask = np.sign(stop-start) != np.sign(step)
-        mask |= (start<0) & (step<0)
-        mask |= (start >= self.lengths) & (step > 0)
-        mask |= (stop <= 0) & (step > 0)
-        mask |= (stop >= self.lengths) & (step < 0)
+        mask = np.sign(stop-start) != np.sign(step) # start is higher than stop and step is not negative
+        mask |= (start < 0) & (step < 0) # start is before 0 and step is negative
+        mask |= (start >= self.lengths) & (step > 0) # start is  after end and step is negative
+        mask |= (stop <= 0) & (step > 0) # stop is before 0 and step is positive
+        mask |= (stop >= self.lengths) & (step < 0) # stop is after end and step is negative
         start = np.maximum(np.minimum(start, self.lengths-1),
-                           0)
+                           0) #put start in range
         d = 0 if step >= 0 else -1
         stop = np.maximum(np.minimum(stop, self.lengths+d),
-                          0+d)
-        L = stop-start
+                          0+d) # put stop in range
+        L = stop-start #length 
         # mask = np.sign(L) != np.sign(step)
         return np.where(mask, 0,
                         (np.abs(L)-1)//np.abs(step)+1)
 
+    def _pos_col_slice(self, col_slice):
+        assert col_slice.step > 0
+        start = col_slice.start
+        if start is None:
+            start = 0
+        elif start >= 0:
+            start = np.minimum(start, self.lengths)
+            # new_start = self.starts + np.minimum(start, self.lengths)*self.col_step
+        else:
+            start = np.maximum(self.lengths+start, 0)
+            # new_start = self.starts + np.maximum(self.lengths+start, 0)*self.col_step
+        stop = col_slice.stop
+        if stop is None:
+            stop = self.lengths
+        elif stop < 0:
+            stop = np.maximum(self.lengths + stop, 0)
+        else:
+            stop = np.minimum(self.lengths, stop)
+        return self.__class__(self.starts+self.col_step*start,
+                              np.maximum(0, (stop-start+(col_slice.step-1))//col_slice.step),
+                              self.col_step*col_slice.step)
+
     def col_slice(self, col_slice):
         if isinstance(col_slice, Number):
             idx = col_slice
             if idx >= 0:
                 return self.__class__(self.starts + idx,
                                       np.ones_like(self.lengths))
             return self.__class__(self.ends + idx, np.ones_like(self.lengths))
 
         # starts, lengths, col_step = (self.starts, self.lengths, self.col_step)
         step = 1 if col_slice.step is None else col_slice.step
+        if step > 0:
+            return self._pos_col_slice(slice(col_slice.start, col_slice.stop, step))
         col_slice_start = col_slice.start
         if col_slice_start is None:
             col_slice_start = 0 if step >= 0 else self.lengths-1
         elif col_slice_start < 0:
             col_slice_start = self.lengths + col_slice_start
         col_slice_start = np.maximum(
             np.minimum(self.lengths-1, col_slice_start),
@@ -442,20 +481,21 @@
         Returns
         -------
         array
         """
         if not self.n_rows:
             return np.ones(0, dtype=self._dtype), self.get_shape()
         shape = self.get_shape()
-        step = 1 if self.col_step is None else self.col_step
-        index_builder = np.full(shape.size + 1, step, dtype=self._dtype)
-        np.add.at(index_builder, shape.starts[1:], self.starts[1:]-self.ends[:-1]-step+1)
-        np.add.at(index_builder, 0, self.starts[0]-step)
-        np.cumsum(index_builder, out=index_builder)
-        return index_builder[:-1], shape
+        return build_indices(self, shape, self.col_step)
+        # step = 1 if self.col_step is None else self.col_step
+        # index_builder = np.full(shape.size + 1, step, dtype=self._dtype)
+        # np.add.at(index_builder, shape.starts[1:], self.starts[1:]-self.ends[:-1]-step+1)
+        # np.add.at(index_builder, 0, self.starts[0]-step)
+        # np.cumsum(index_builder, out=index_builder)
+        # return index_builder[:-1], shape
 
     def get_flat_indices(self, do_split=False):
         return self._get_flat_indices(do_split)
         if self.col_step != 1 or np.any(self.starts[:-1] > self.starts[1:]):
             return self._get_flat_indices(do_split)
         if not self.n_rows:
             return np.ones(0, dtype=self._dtype), self.get_shape()
@@ -548,15 +588,15 @@
         if self.empty_rows_removed():
             return self._get_flat_indices_fast()
         shape = self.get_shape()
         chunk_size = 100000
         if do_split and self.starts.size > chunk_size:
             slices = (slice(i*chunk_size, (i+1)*chunk_size) for i in range((len(self.starts)-1)//chunk_size+1))
             return (self[s]._build_indices(shape[s])[0] for s in slices), shape
-
+        return build_indices(self, shape, self._step)
         return self._build_indices(shape)
 
     def _get_flat_indices_fast(self):
         shape = self.get_shape()
         index_builder = np.ones(shape.size, dtype=self._dtype)
         index_builder[shape.starts[1:]] = np.diff(self.starts) - self.lengths[:-1] + 1
         index_builder[0] = self.starts[0]
```

### Comparing `npstructures-0.2.8/npstructures/runlengtharray.py` & `npstructures-0.2.9/npstructures/runlengtharray.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,103 +1,183 @@
 import numpy as np
+from typing import Dict, List, Tuple, Union
+from numpy.typing import ArrayLike, DTypeLike
 from numbers import Number
 from .util import unsafe_extend_left, unsafe_extend_right, unsafe_extend_left_2d
 from .raggedarray import RaggedArray
 from .mixin import NPSArray, NPSIndexable
+from .raggedarray.raggedslice import ragged_slice
 import logging
 logger = logging.getLogger("RunLengthArray")
 
 
 class RunLengthArray(NPSIndexable, np.lib.mixins.NDArrayOperatorsMixin):
+    """Class for Run Length arrays
+
+    This is used to represent data where changes in values are
+    rare. Behaves much like a normal NumPy array.
+
+    Should be constructed using one of the classmethods, not initialized directly
+    """
     def __init__(self, events, values, do_clean=False):
         self._events, self._starts = (events, values)
-        self._events = events.view(NPSArray)
+        self._events = events# .view(NPSArray)
         self._starts = events[:-1]
         self._ends = events[1:]
-        self._values = values.view(NPSArray)
+        self._values = values# .view(NPSArray)
         assert events[0] == 0, events
         assert len(events) == len(values)+1, (events, values, len(events), len(values))
         assert np.all(events[1:] > events[:-1]), f"Empty run not allowed in RunLenghtArray (use remove_empty_intervals): {events}"
 
-    def __len__(self):
+    def __len__(self)->int:
         if len(self._ends) == 0:
             return 0
         return self._ends[-1]
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.size <= 1000:
             return str(self.to_array())
         return "[ {' ' .join(str(c) for cin self[:3].to_array())} ... .join(str(c) for cin self[-3:].to_array())}"
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         if self.size <= 1000:
             return repr(self.to_array())
 
     @property
-    def size(self):
+    def size(self) -> int:
+        """
+        Size of the array
+        """
         return self._ends[-1]
 
     @property
-    def shape(self):
+    def shape(self) -> Tuple[int]:
         return (self.size,)
 
     @property
-    def dtype(self):
+    def dtype(self) -> DTypeLike:
         return self._values.dtype
 
     @property
-    def starts(self):
+    def starts(self) -> ArrayLike:
+        """
+        All idxs where the value changes
+        """
         return self._events[:-1]
 
     @property
-    def ends(self):
+    def ends(self) -> ArrayLike:
+        """All indices that ends a run of equal values
+        """
         return self._events[1:]
 
     @property
-    def values(self):
+    def values(self) -> ArrayLike:
+        """All values that are not equal to previous value
+
+        Returns
+        -------
+        ArrayLike
+        """
         return self._values
 
     @classmethod
-    def from_array(cls, array):
+    def from_array(cls, array: ArrayLike) -> 'RunLengthArray':
+        """Construct a RunLengthArray from a normal numpy array
+
+        Parameters
+        ----------
+        array : ArrayLike
+            Normal numpy array
+
+        Returns
+        -------
+        'RunLengthArray'
+
+        """
         array = np.asanyarray(array)
         mask = unsafe_extend_left(array) != unsafe_extend_right(array)
         mask[0], mask[-1] = (True, True)
         indices = np.flatnonzero(mask)
         values = array[indices[:-1]]
         return cls(indices, values)
 
     @classmethod
-    def from_intervals(cls, starts, ends, size, values=True, default_value=0):
-        events = np.r_[0, np.vstack(starts, ends).T.ravel(), size]
+    def __from_intervals(cls, starts: ArrayLike, ends: ArrayLike, size: int , values: ArrayLike = True, default_value=0) -> 'RunLengthArray':
+        """Constuct a runlength array from a set of intervals and values
+
+        Parameters
+        ----------
+        starts : ArrayLike
+        ends : ArrayLike
+        size : int
+        values : ArrayLike
+        default_value :
+
+        Returns
+        -------
+        'RunLengthArray'
+        """
+        
+        assert np.all(ends > starts)
+        assert np.all(starts[1:] > ends[:-1])
+        prefix = [0] if (len(starts) == 0 or starts[0] != 0) else []
+        postfix = [size] if (len(ends) == 0 or ends[-1] != size) else []
+        events = np.concatenate([np.array(prefix, dtype=int), np.vstack((starts, ends)).T.ravel(), np.array(postfix, dtype=int)])
         if isinstance(values, Number):
-            values = np.tile([default_value, values], events.size//2)[:-1]
+            values = np.tile([default_value, values], events.size//2+1)
         else:
             values = np.vstack([np.broadcast(default_value, values.shape), values]).T.ravel()
-            values = np.append(values, default_value)
+            if ends[-1] != size:
+                values = np.append(values, default_value)
+        if (len(starts) > 0) and starts[0] == 0:
+            values = values[1:]
+        values = values[:(len(events)-1)]
         return cls(events, values, do_clean=True)
-        
-    def to_array(self):
+
+    def to_array(self) -> np.ndarray:
+        """Convert the runlength array to a normal numpy array
+
+        Returns
+        -------
+        np.ndarray
+        """
         if len(self) == 0:
             return np.empty_like(self._values, shape=(0,))
-        values = self._values
+        values = np.asarray(self._values)
         if values.dtype == np.float64:
             values = values.view(np.uint64)
         elif values.dtype == np.float32:
             values = values.view(np.uint32)
         elif values.dtype == np.float16:
             values = values.view(np.uint16)
 
         array = np.zeros_like(values, shape=len(self))
-        diffs = unsafe_extend_left(values)[:-1] ^ values
-        diffs[0] = values[0]
-        array[self._starts] = diffs
-        np.bitwise_xor.accumulate(array, out=array)
-        return array.view(self._values.dtype)
+        op = np.logical_xor if array.dtype == bool else np.bitwise_xor
+        diffs = op(values[:-1], values[1:])
+        assert np.all(self._starts[1:] > self._starts[:-1])
+        array[self._starts[1:]] = diffs
+        array[self._starts[0]] = values[0]
+        tmp = array.copy()
+        op.accumulate(array, out=tmp)
+        # array = op.accumulate(array, dtype=array.dtype)
+        return tmp.view(self._values.dtype)
 
-    def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+    def __array_ufunc__(self, ufunc: callable, method: str, *inputs, **kwargs):
+        """Handle numpy unfuncs called on the runlength array
+        
+        Currently only handles '__call__' modes and unary and binary functions
+
+        Parameters
+        ----------
+        ufunc : callable
+        method : str
+        *inputs :
+        **kwargs :
+        """
         if method not in ("__call__"):
             return NotImplemented
         if len(inputs) == 1:
             return self.__class__(self._events, ufunc(self._values))
         assert len(inputs) == 2, f"Only unary and binary operations supported for runlengtharray {len(inputs)}"
 
         if isinstance(inputs[1], Number):
@@ -113,32 +193,58 @@
         """TODO, this can be sped up by assuming no empty runs"""
         return np.any(self._values)
 
     def all(self, axis=-1, out=None):
         """TODO, this can be sped up by assuming no empty runs"""
         return np.all(self._values)
 
-    def astype(self, dtype):
+    def astype(self, dtype: DTypeLike) -> 'RunLengthArray':
         return self.__class__(self._events, self._values.astype(dtype))
 
     def mean(self, axis=-1, dtype=None, out=None):
         assert dtype is None and out is None
         if np.issubdtype(self.dtype, np.integer):
             return self.astype(float).mean(axis, dtype, out)
         return self.sum()/self.size
 
     @staticmethod
-    def remove_empty_intervals(events, values, delete_first=True):
+    def remove_empty_intervals(events: ArrayLike, values: ArrayLike, delete_first: bool = True) -> Tuple[ArrayLike, ArrayLike]:
+        """Remove any empty runs from a pair of indices and values.
+
+        Should be run before creating a runlength array from the
+        events and values
+
+        Parameters
+        ----------
+        events : ArrayLike
+        values : ArrayLike
+        delete_first : bool
+
+        Returns
+        -------
+        Tuple[ArrayLike, ArrayLike]
+        """
         mask = np.flatnonzero(events[:-1] == events[1:])
         if not delete_first:
             mask += 1
         return np.delete(events, mask), np.delete(values, mask)
 
     @staticmethod
-    def join_runs(events, values):
+    def join_runs(events: ArrayLike, values: ArrayLike) -> Tuple[ArrayLike, ArrayLike]:
+        """Join succesive runs with the same value
+
+        Parameters
+        ----------
+        events : ArrayLike
+        values : ArrayLike
+
+        Returns
+        -------
+        Tuple[ArrayLike, ArrayLike]
+        """
         mask = np.flatnonzero(values[1:] == values[:-1])+1
         return np.delete(events, mask), np.delete(values, mask)
 
     @classmethod
     def _apply_binary_func(cls, first, other, ufunc):
         logging.info(f"Applying ufunc {ufunc} to rla with {first._values.size} values")
         assert len(first) == len(other), (first, other)
@@ -246,22 +352,28 @@
         indices, values = self.remove_empty_intervals(indices, values)# , delete_first=False)
         indices, values = self.join_runs(indices, values)
         return self.__class__(indices, values)
 
     def _start_to_end(self, start, end):
         start_idx = np.searchsorted(self._events, start, side="right")-1
         end_idx = np.searchsorted(self._events, end, side="left")
-        values = self._values[start_idx:end_idx]
+        if isinstance(start_idx, np.ndarray):
+            values = ragged_slice(self._values, start_idx, end_idx)
+        else:
+            values = self._values[start_idx:end_idx]
         sub = start[:, np.newaxis] if isinstance(start, np.ndarray) else start
-        events = self._events[start_idx:end_idx+1]-sub
+        if isinstance(start_idx, np.ndarray):
+            events = ragged_slice(self._events, start_idx, end_idx+1)-sub
+        else:
+            events = self._events[start_idx:end_idx+1]-sub
         events[..., 0] = 0
         events[..., -1] = end-start
         return events, values
 
-    def __getitem__(self, idx):
+    def __getitem__(self, idx: Union[Tuple, List[int], Number, ArrayLike, slice]):
         try:
             return super().__getitem__(idx)
         except ValueError:
             pass
         if isinstance(idx, tuple):
             idx = tuple(i for i in idx if i is not Ellipsis)
             assert len(idx) <= 1, idx
@@ -284,42 +396,43 @@
         if idx is Ellipsis:
             return self
 
         # assert False, f"Invalid index for {self.__class__}: {idx}"
 
 
 class RunLength2dArray:
-    """Multiple run lenght arrays over the same space"""
+    ''' Multiple RunLengthArrays of the same size. Behaves like a 2d numpy array''' 
     def __init__(self, indices: RaggedArray, values: RaggedArray, row_len: int=None):
         self._values = values
         self._indices = indices
         self._row_len = row_len
 
-    def __str__(self):
+    def __str__(self) -> str:
         return "["+"\n ".join(str(row) for row in self) + "]"
 
     @property
-    def shape(self):
+    def shape(self) -> Tuple[int]:
         return (len(self._indices), self._row_len)
 
     @property
-    def size(self):
+    def size(self) -> int:
         return self.shape[0]*self.shape[1]
 
     @property
-    def dtype(self):
+    def dtype(self) -> DTypeLike:
         return self._values.dtype()
 
-    def to_array(self):
+    def to_array(self) -> ArrayLike:
+        ''' Convert to a normal 2d numpy array ''' 
         return np.array([row.to_array() for row in self])
 
-    def __len__(self, idx):
+    def __len__(self) -> int:
         return len(self._indices)
 
-    def __getitem__(self, raw_idx):
+    def __getitem__(self, raw_idx: Union[Tuple, int, List[int], ArrayLike]):
         if isinstance(raw_idx, tuple):
             idx = tuple(r for r in raw_idx if r is not Ellipsis)
             if len(idx) == 0:
                 return self
             if len(idx) == 1 and raw_idx[0] is Ellipsis:
                 idx = (slice(None),) + idx
             if len(idx) == 2:
@@ -340,35 +453,46 @@
         if isinstance(events, RaggedArray):
             return self.__class__(events, values, self._row_len)
         if self._row_len is not None:
             events = np.append(self._indices[idx], self._row_len)
         return RunLengthArray(events, values)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
+        """Handle numpy unfuncs called on the runlength array
+        
+        Currently only handles '__call__' modes and unary and binary functions
+
+        Parameters
+        ----------
+        ufunc : callable
+        method : str
+        *inputs :
+        **kwargs :
+        """
         if method not in ("__call__"):
             return NotImplemented
         if len(inputs) == 1:
             return self.__class__(self._indices, ufunc(self._values), self._row_len)
         assert len(inputs) == 2
 
         if isinstance(inputs[1], (Number, np.ndarray)):
             return self.__class__(self._indices, ufunc(self._values, inputs[1]), self._row_len)
         elif isinstance(inputs[0], (Number, np.ndarray)):
             return self.__class__(self._indices, ufunc(self._values, inputs[0]), self._row_len)
         return NotImplemented
 
-    def any(self, axis=None, out=None):
+    def any(self, axis: int = None, out=None) -> ArrayLike:
         if axis in (0, -2):
             return self._col_any()
         return self._values.any(axis=axis)
 
-    def all(self, axis=None, out=None):
+    def all(self, axis: int= None, out=None) -> ArrayLike:
         return self._values.all(axis=axis)
 
-    def sum(self, axis=None, out=None):
+    def sum(self, axis: int = None, out=None) -> ArrayLike:
         if axis in (0, -2):
             return self._col_sum()
         assert (axis == -1 or axis is None)
         internal_sum = np.sum(self._values[:, :-1] * (self._indices[:, 1:]-self._indices[:, :-1]), axis=-1)
         return internal_sum + self._values[:, -1]*(self._row_len-self._indices[:, -1])
 
     def _col_sum(self):
@@ -411,37 +535,66 @@
         if indices[-1] == self._row_len:
             values = values[:-1]
         else:
             indices = np.append(indices, self._row_len)
         return RunLengthArray(indices, values)
 
     @classmethod
-    def from_array(cls, array: np.ndarray):
+    def from_array(cls, array: ArrayLike) -> 'RunLength2dArray':
+        """Construct a Runlength2dArray from a normal 2d numpy array
+
+        Parameters
+        ----------
+        array : ArrayLike
+
+        Returns
+        -------
+        'RunLength2dArray'
+
+
+        """
         array = np.asanyarray(array)
         mask = unsafe_extend_left_2d(array)[:, :-1] != array
         mask[:, 0] = True
         mask[:, -1] = True
         indices = np.flatnonzero(mask)
         values = array.ravel()[indices]
         indices = RaggedArray(indices, mask.sum(axis=-1))
         values = RaggedArray(values, indices._shape)
         indices = indices-indices[:, 0][:, np.newaxis]
         return cls(indices, values, array.shape[-1])
 
     @staticmethod
-    def join_runs(indices, values):
+    def join_runs(indices: ArrayLike, values: ArrayLike) -> Tuple[ArrayLike, ArrayLike]:
         mask = unsafe_extend_left(values.ravel())[:-1] != values.ravel()
         mask[values._shape.starts] = True
         shape = RaggedArray(mask, values._shape).sum(axis=-1)
         indices = RaggedArray(indices.ravel()[mask], shape)
         values = RaggedArray(values.ravel()[mask], shape)
         return indices, values
 
     @classmethod
-    def from_intervals(cls, starts, ends, row_len, value=1):
+    def from_intervals(cls, starts: ArrayLike, ends: ArrayLike, row_len: int, value=1) -> 'RunLength2dArray':
+        """Construct a RunLength2dArray from a set of intervals
+
+        Each interval becomes a row in the 2d array
+
+        Parameters
+        ----------
+        cls :
+        starts : ArrayLike
+        ends : ArrayLike
+        row_len : int
+        value :
+
+        Returns
+        -------
+        'RunLength2dArray'
+
+        """
         starts_after_zero = starts > 0
         ends_before_end = ends < row_len
         value = np.asanyarray(value)
         shape = starts_after_zero + 1 + ends_before_end
         indices = RaggedArray(np.zeros(shape.sum(), int), shape)
         values = RaggedArray(np.zeros(shape.sum(), value.dtype), shape)
         indices[np.arange(len(starts)), starts_after_zero.astype(int)] = starts
@@ -456,19 +609,29 @@
     def __getitem__(self, idx):
         events = self._indices[idx]
         if self._row_len is not None:
             events = np.append(self._indices[idx], self._row_len[idx])
         return RunLengthArray(events, self._values[idx])
 
     def to_array(self):
-        # assert np.all(self._indices[:, -1] == self._indices[0, -1]), self._indices
         return RaggedArray([row.to_array() for row in self])
 
     @classmethod
-    def from_ragged_array(cls, ragged_array: RaggedArray):
+    def from_ragged_array(cls, ragged_array: RaggedArray) -> 'RunLengthRaggedArray':
+        """Construct runlengtharray from a RaggedArray
+
+        Parameters
+        ----------
+        ragged_array : RaggedArray
+
+        Returns
+        -------
+        RunLengthRaggedArray
+        """
+
         data = ragged_array.ravel()
         mask = unsafe_extend_left(data)[:-1] != data
         mask[ragged_array._shape.starts] = True
         indices = np.flatnonzero(mask)
         tmp = np.cumsum(unsafe_extend_left(mask))
         row_lens = tmp[ragged_array._shape.ends]-tmp[ragged_array._shape.starts]
         values = data[indices]
```

### Comparing `npstructures-0.2.8/npstructures/testing.py` & `npstructures-0.2.9/npstructures/testing.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures/util.py` & `npstructures-0.2.9/npstructures/util.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/npstructures.egg-info/PKG-INFO` & `npstructures-0.2.9/npstructures.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npstructures
-Version: 0.2.8
+Version: 0.2.9
 Summary: Simple data structures that augments the numpy library
 Home-page: https://github.com/knutdrand/npstructures
 Author: Knut Rand
 Author-email: knutdrand@gmail.com
 License: MIT license
 Keywords: npstructures
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `npstructures-0.2.8/npstructures.egg-info/SOURCES.txt` & `npstructures-0.2.9/npstructures.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -2,25 +2,14 @@
 CONTRIBUTING.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-docs/Makefile
-docs/authors.rst
-docs/conf.py
-docs/contributing.rst
-docs/history.rst
-docs/index.rst
-docs/installation.rst
-docs/make.bat
-docs/modules.rst
-docs/readme.rst
-docs/usage.rst
 npstructures/__init__.py
 npstructures/arrayfunctions.py
 npstructures/bitarray.py
 npstructures/hashtable.py
 npstructures/mixin.py
 npstructures/npdataclasses.py
 npstructures/raggedshape.py
```

### Comparing `npstructures-0.2.8/setup.py` & `npstructures-0.2.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 with open('README.rst') as readme_file:
     readme = readme_file.read()
 
 with open('HISTORY.rst') as history_file:
     history = history_file.read()
 
-requirements = ['numpy>=1.19']
+requirements = ['numpy>=1.19,<1.24']
 
 test_requirements = ['pytest>=4.6', 'hypothesis']
 
 setup(
     author="Knut Rand",
     author_email='knutdrand@gmail.com',
     python_requires='>=3.6',
@@ -35,13 +35,13 @@
     include_package_data=True,
     keywords='npstructures',
     name='npstructures',
     packages=find_packages(include=['npstructures', 'npstructures.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/knutdrand/npstructures',
-    version='0.2.8',
+    version='0.2.9',
     zip_safe=False,
 )
 
 # python -m build
 # twine upload dist/*
```

### Comparing `npstructures-0.2.8/tests/property_tests/strategies.py` & `npstructures-0.2.9/tests/property_tests/strategies.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/property_tests/test_bitarray.py` & `npstructures-0.2.9/tests/property_tests/test_bitarray.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/property_tests/test_hashtable.py` & `npstructures-0.2.9/tests/property_tests/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/property_tests/test_ragged_array.py` & `npstructures-0.2.9/tests/property_tests/test_ragged_array.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/property_tests/test_runlengtharray.py` & `npstructures-0.2.9/tests/property_tests/test_runlengtharray.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import hypothesis.extra.numpy as stnp
 ufuncs = [np.add, np.subtract, np.multiply, np.bitwise_and, np.bitwise_or, np.bitwise_xor]
 
 
 @given(arrays(array_shape=array_shapes(1, 1, 1)))
 def test_run_length_array(np_array):
     rlarray = RunLengthArray.from_array(np_array)
+    print(rlarray._values, rlarray._events)
     new_array = rlarray.to_array()
     assert_array_equal(np_array, new_array)
 
 
 # @pytest.mark.skip("unimplemented")
 @given(arrays(array_shape=array_shapes(1, 2, 2)))
 @example(array([[0]], dtype=int8))
@@ -158,7 +159,26 @@
     n_intervals = len(starts)
     row_len = len(vec)
     true = np.zeros((n_intervals, row_len), dtype=int)
     for i, (start, end) in enumerate(zip(starts, ends)):
         true[i, start:end] += 1
     result = RunLength2dArray.from_intervals(starts, ends, row_len).to_array()
     assert_array_equal(result, true)
+
+
+@given(vector_and_startends())
+def _test_from_intervals_1d(data):
+    vec, starts, ends = data
+    starts = np.asanyarray(starts)
+    ends = np.asanyarray(ends)
+
+    starts = np.minimum(starts, ends)
+    ends = np.maximum(starts, ends+1)
+    n_intervals = len(starts)
+    row_len = len(vec)
+    true = np.zeros((row_len), dtype=bool)
+    for (start, end) in enumerate(zip(starts, ends)):
+        true[int(start):int(end)] |= True
+    result = RunLength2dArray.from_intervals(starts, ends, row_len).to_array()
+    assert_array_equal(result, true)
+
+
```

### Comparing `npstructures-0.2.8/tests/test_arrayfunctions.py` & `npstructures-0.2.9/tests/test_arrayfunctions.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/test_bitarray.py` & `npstructures-0.2.9/tests/test_bitarray.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/test_hashtable.py` & `npstructures-0.2.9/tests/test_hashtable.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/test_npdataclass.py` & `npstructures-0.2.9/tests/test_npdataclass.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/test_raggedarray.py` & `npstructures-0.2.9/tests/test_raggedarray.py`

 * *Files 0% similar despite different names*

```diff
@@ -403,14 +403,15 @@
 
 def test_subset_with_boolean_ragged_array():
     ra = RaggedArray([[], [1, 2, 3], [1, 2], [1], [], []])
     subset_with = RaggedArray([[], [True, False, True], [True, False], [True], [], []])
     assert np.all(ra.subset(subset_with) == RaggedArray([[], [1, 3], [1], [1], [], []]))
 
 
+@pytest.mark.skip('depracated')
 def test_as_padded_matrix():
     ra = RaggedArray([[1, 2, 3], [1, 2], [1]])
     padded = ra.as_padded_matrix(side="right")
     assert np.all(padded == [[1, 2, 3], [1, 2, 0], [1, 0, 0]])
 
     padded = ra.as_padded_matrix(side="left")
     assert np.all(padded == [[1, 2, 3], [0, 1, 2], [0, 0, 1]])
```

### Comparing `npstructures-0.2.8/tests/test_raggedshape.py` & `npstructures-0.2.9/tests/test_raggedshape.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/test_random.py` & `npstructures-0.2.9/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `npstructures-0.2.8/tests/test_runlengtharray.py` & `npstructures-0.2.9/tests/test_runlengtharray.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,28 +7,32 @@
 
 arrays = [[0, 1, 1, 2, 3, 3, 3],
           [0, 20, 1, 1, 0, 3, 3],
           [2, 2, 2, 1],
           [1],
           [2.3, 19, 32.7, 32.7],
           [2.3, 19, 32.7, 32.7, 92.0, 0.32, 0.84, 0.91],
-          [0,1,1,2,2,2,3,3,3,3,2,2,2,1,1,0]]
+          [0,1,1,2,2,2,3,3,3,3,2,2,2,1,1,0],
+          [True,  True,  True,  True,  True, False, False, False, False,
+           False, False,  True,  True,  True,  True,  True,  True,  True,
+           True,  True]]
 
 arrays_2 = [[0, 1, 1, 2, 3, 3, 3],
             [10, 1, 1, 2, 3, 2, 2],
             [13, 13, 3, 0],
             [10],
             [32.3, 198, 932.2, 329.7],
             [32.3, 198, 932.2, 329.7, 29.0, 32.0, 34, 19.1]]
 
 
 @pytest.mark.parametrize("array", arrays)
 def test_run_length_array(array):
     array = np.asanyarray(array)
     rlarray = RunLengthArray.from_array(array)
+    print(rlarray._values, rlarray._events)
     new_array = rlarray.to_array()
     assert_array_equal(array, new_array)
 
 
 @pytest.mark.parametrize("array1,array2", tuple(zip(arrays, arrays_2)))
 def test_add_run_length_array(array1, array2):
     array1, array2 = (np.asanyarray(a) for a in (array1, array2))
@@ -79,7 +83,14 @@
 @pytest.mark.parametrize("array", arrays)
 def test_getitem_slice(array):
     rlarray = RunLengthArray.from_array(array)
     for start, _ in enumerate(array):
         for end in range(start+1, len(array)):
             assert_array_almost_equal(rlarray[start:end].to_array(), array[start:end])
 
+
+def _test_ragged_slice():
+    vector, starts, ends = (np.asanyarray(e) for e in data)
+    starts = np.minimum(starts, ends)
+    ends = np.maximum(starts, ends+1)
+    subset = vector.view(NPSArray)[starts:ends]
+    assert_raggedarray_equal(subset, RaggedArray([vector[start:end] for start, end in zip(starts, ends)]))
```

