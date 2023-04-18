# Comparing `tmp/humanleague-2.1.9.tar.gz` & `tmp/humanleague-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "humanleague-2.1.9.tar", last modified: Sun Jul 18 12:47:59 2021, max compression
+gzip compressed data, was "humanleague-2.2.0.tar", last modified: Tue Apr 18 07:49:23 2023, max compression
```

## Comparing `humanleague-2.1.9.tar` & `humanleague-2.2.0.tar`

### file list

```diff
@@ -1,53 +1,57 @@
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2021-07-18 12:47:59.758573 humanleague-2.1.9/
--rw-rw-r--   0 az        (1000) az        (1000)     1151 2021-06-06 10:57:55.000000 humanleague-2.1.9/DESCRIPTION
--rw-r--r--   0 az        (1000) az        (1000)       43 2018-04-30 19:47:58.000000 humanleague-2.1.9/LICENCE
--rw-rw-r--   0 az        (1000) az        (1000)     1074 2021-06-06 11:21:40.000000 humanleague-2.1.9/LICENSE
--rw-r--r--   0 az        (1000) az        (1000)      103 2020-11-01 15:22:20.000000 humanleague-2.1.9/MANIFEST.in
--rw-rw-r--   0 az        (1000) az        (1000)     8234 2021-07-18 12:47:59.758573 humanleague-2.1.9/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)     6459 2021-06-06 16:33:11.000000 humanleague-2.1.9/README.md
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2021-07-18 12:47:59.750573 humanleague-2.1.9/humanleague.egg-info/
--rw-rw-r--   0 az        (1000) az        (1000)     8234 2021-07-18 12:47:59.000000 humanleague-2.1.9/humanleague.egg-info/PKG-INFO
--rw-rw-r--   0 az        (1000) az        (1000)      846 2021-07-18 12:47:59.000000 humanleague-2.1.9/humanleague.egg-info/SOURCES.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2021-07-18 12:47:59.000000 humanleague-2.1.9/humanleague.egg-info/dependency_links.txt
--rw-rw-r--   0 az        (1000) az        (1000)        1 2020-10-30 13:07:28.000000 humanleague-2.1.9/humanleague.egg-info/not-zip-safe
--rw-rw-r--   0 az        (1000) az        (1000)       14 2021-07-18 12:47:59.000000 humanleague-2.1.9/humanleague.egg-info/requires.txt
--rw-rw-r--   0 az        (1000) az        (1000)       12 2021-07-18 12:47:59.000000 humanleague-2.1.9/humanleague.egg-info/top_level.txt
--rw-rw-r--   0 az        (1000) az        (1000)      206 2021-06-06 08:42:00.000000 humanleague-2.1.9/pyproject.toml
--rw-rw-r--   0 az        (1000) az        (1000)       63 2021-07-18 12:47:59.758573 humanleague-2.1.9/setup.cfg
--rwxrwxr-x   0 az        (1000) az        (1000)     1803 2021-07-18 12:01:14.000000 humanleague-2.1.9/setup.py
-drwxrwxr-x   0 az        (1000) az        (1000)        0 2021-07-18 12:47:59.758573 humanleague-2.1.9/src/
--rw-r--r--   0 az        (1000) az        (1000)     7044 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/DDWR.h
--rw-r--r--   0 az        (1000) az        (1000)      301 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Global.h
--rw-r--r--   0 az        (1000) az        (1000)     3464 2021-01-22 10:29:11.000000 humanleague-2.1.9/src/IPF.h
--rw-r--r--   0 az        (1000) az        (1000)     4400 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Index.cpp
--rw-r--r--   0 az        (1000) az        (1000)     2692 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Index.h
--rw-r--r--   0 az        (1000) az        (1000)     2784 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Integerise.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1217 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Integerise.h
--rw-r--r--   0 az        (1000) az        (1000)     1290 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Log.h
--rw-rw-r--   0 az        (1000) az        (1000)     7966 2020-11-01 14:04:07.000000 humanleague-2.1.9/src/Microsynthesis.h
--rw-r--r--   0 az        (1000) az        (1000)     5274 2020-10-30 12:16:58.000000 humanleague-2.1.9/src/NDArray.h
--rw-r--r--   0 az        (1000) az        (1000)      480 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/NDArrayUtils.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     5724 2021-01-22 10:28:50.000000 humanleague-2.1.9/src/NDArrayUtils.h
--rw-r--r--   0 az        (1000) az        (1000)    11209 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/QIS.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1119 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/QIS.h
--rw-r--r--   0 az        (1000) az        (1000)     4652 2019-06-10 14:30:33.000000 humanleague-2.1.9/src/QISI.cpp
--rw-r--r--   0 az        (1000) az        (1000)      870 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/QISI.h
--rw-r--r--   0 az        (1000) az        (1000)     4104 2020-02-14 13:40:42.000000 humanleague-2.1.9/src/RcppExports.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1355 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Sobol.cpp
--rw-r--r--   0 az        (1000) az        (1000)      866 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/Sobol.h
--rw-r--r--   0 az        (1000) az        (1000)    57077 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/SobolData.h
--rw-r--r--   0 az        (1000) az        (1000)     6835 2021-07-18 12:13:18.000000 humanleague-2.1.9/src/SobolImpl.cpp
--rw-r--r--   0 az        (1000) az        (1000)      809 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/SobolImpl.h
--rw-r--r--   0 az        (1000) az        (1000)     8026 2021-07-18 12:12:45.000000 humanleague-2.1.9/src/StatFuncs.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1587 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/StatFuncs.h
--rw-r--r--   0 az        (1000) az        (1000)     5562 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/TestIndex.cpp
--rw-r--r--   0 az        (1000) az        (1000)     2319 2020-02-14 13:07:20.000000 humanleague-2.1.9/src/TestNDArray.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1231 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/TestReduce.cpp
--rw-r--r--   0 az        (1000) az        (1000)     6194 2018-12-05 09:27:47.000000 humanleague-2.1.9/src/TestSlice.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1146 2020-02-14 13:07:07.000000 humanleague-2.1.9/src/TestSobol.cpp
--rw-r--r--   0 az        (1000) az        (1000)     3331 2021-01-22 10:30:35.000000 humanleague-2.1.9/src/TestStatFuncs.cpp
--rw-r--r--   0 az        (1000) az        (1000)     1150 2021-01-22 12:00:10.000000 humanleague-2.1.9/src/UnitTester.cpp
--rw-rw-r--   0 az        (1000) az        (1000)     4431 2020-11-01 14:04:07.000000 humanleague-2.1.9/src/UnitTester.h
--rw-rw-r--   0 az        (1000) az        (1000)     5065 2021-06-06 11:25:46.000000 humanleague-2.1.9/src/docstr.inl
--rw-rw-r--   0 az        (1000) az        (1000)     9270 2021-06-06 11:25:31.000000 humanleague-2.1.9/src/module.cpp
--rw-rw-r--   0 az        (1000) az        (1000)    16770 2021-06-06 08:18:59.000000 humanleague-2.1.9/src/rcpp_api.cpp
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-18 07:49:23.701608 humanleague-2.2.0/
+-rw-rw-r--   0 az        (1000) az        (1000)     1151 2023-04-16 08:58:34.000000 humanleague-2.2.0/DESCRIPTION
+-rw-r--r--   0 az        (1000) az        (1000)       43 2018-04-30 19:47:58.000000 humanleague-2.2.0/LICENCE
+-rw-rw-r--   0 az        (1000) az        (1000)     1083 2023-01-07 10:08:14.000000 humanleague-2.2.0/LICENSE.md
+-rw-rw-r--   0 az        (1000) az        (1000)      106 2023-01-07 10:07:38.000000 humanleague-2.2.0/MANIFEST.in
+-rw-rw-r--   0 az        (1000) az        (1000)     7164 2023-04-18 07:49:23.705608 humanleague-2.2.0/PKG-INFO
+-rw-rw-r--   0 az        (1000) az        (1000)     6702 2023-04-17 07:57:09.000000 humanleague-2.2.0/README.md
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-18 07:49:23.697607 humanleague-2.2.0/humanleague/
+-rw-rw-r--   0 az        (1000) az        (1000)      118 2023-04-16 09:58:54.000000 humanleague-2.2.0/humanleague/__init__.py
+-rw-rw-r--   0 az        (1000) az        (1000)     7070 2023-04-16 20:01:12.000000 humanleague-2.2.0/humanleague/__init__.pyi
+-rw-rw-r--   0 az        (1000) az        (1000)        0 2022-03-19 15:16:50.000000 humanleague-2.2.0/humanleague/py.typed
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-18 07:49:23.697607 humanleague-2.2.0/humanleague.egg-info/
+-rw-rw-r--   0 az        (1000) az        (1000)     7164 2023-04-18 07:49:23.000000 humanleague-2.2.0/humanleague.egg-info/PKG-INFO
+-rw-rw-r--   0 az        (1000) az        (1000)      919 2023-04-18 07:49:23.000000 humanleague-2.2.0/humanleague.egg-info/SOURCES.txt
+-rw-rw-r--   0 az        (1000) az        (1000)        1 2023-04-18 07:49:23.000000 humanleague-2.2.0/humanleague.egg-info/dependency_links.txt
+-rw-rw-r--   0 az        (1000) az        (1000)        1 2020-10-30 13:07:28.000000 humanleague-2.2.0/humanleague.egg-info/not-zip-safe
+-rw-rw-r--   0 az        (1000) az        (1000)       14 2023-04-18 07:49:23.000000 humanleague-2.2.0/humanleague.egg-info/requires.txt
+-rw-rw-r--   0 az        (1000) az        (1000)       25 2023-04-18 07:49:23.000000 humanleague-2.2.0/humanleague.egg-info/top_level.txt
+-rw-rw-r--   0 az        (1000) az        (1000)      206 2021-06-06 08:42:00.000000 humanleague-2.2.0/pyproject.toml
+-rw-rw-r--   0 az        (1000) az        (1000)      256 2023-04-18 07:49:23.705608 humanleague-2.2.0/setup.cfg
+-rwxrwxr-x   0 az        (1000) az        (1000)     1891 2023-04-17 07:12:38.000000 humanleague-2.2.0/setup.py
+drwxrwxr-x   0 az        (1000) az        (1000)        0 2023-04-18 07:49:23.701608 humanleague-2.2.0/src/
+-rw-r--r--   0 az        (1000) az        (1000)     7044 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/DDWR.h
+-rw-r--r--   0 az        (1000) az        (1000)      301 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/Global.h
+-rw-r--r--   0 az        (1000) az        (1000)     3464 2021-01-22 10:29:11.000000 humanleague-2.2.0/src/IPF.h
+-rw-rw-r--   0 az        (1000) az        (1000)     4294 2023-01-07 10:07:38.000000 humanleague-2.2.0/src/Index.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     2726 2023-04-17 07:10:45.000000 humanleague-2.2.0/src/Index.h
+-rw-r--r--   0 az        (1000) az        (1000)     2784 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/Integerise.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1217 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/Integerise.h
+-rw-rw-r--   0 az        (1000) az        (1000)     1343 2023-01-07 10:08:47.000000 humanleague-2.2.0/src/Log.h
+-rw-rw-r--   0 az        (1000) az        (1000)     7966 2020-11-01 14:04:07.000000 humanleague-2.2.0/src/Microsynthesis.h
+-rw-r--r--   0 az        (1000) az        (1000)     5287 2023-04-17 07:10:48.000000 humanleague-2.2.0/src/NDArray.h
+-rw-r--r--   0 az        (1000) az        (1000)      480 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/NDArrayUtils.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)     5742 2023-01-07 10:28:35.000000 humanleague-2.2.0/src/NDArrayUtils.h
+-rw-r--r--   0 az        (1000) az        (1000)    11209 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/QIS.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1119 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/QIS.h
+-rw-r--r--   0 az        (1000) az        (1000)     4652 2019-06-10 14:30:33.000000 humanleague-2.2.0/src/QISI.cpp
+-rw-r--r--   0 az        (1000) az        (1000)      870 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/QISI.h
+-rw-r--r--   0 az        (1000) az        (1000)     4104 2020-02-14 13:40:42.000000 humanleague-2.2.0/src/RcppExports.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1274 2023-04-17 07:21:18.000000 humanleague-2.2.0/src/Sobol.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1047 2023-04-17 07:10:39.000000 humanleague-2.2.0/src/Sobol.h
+-rw-r--r--   0 az        (1000) az        (1000)    57077 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/SobolData.h
+-rw-r--r--   0 az        (1000) az        (1000)     6835 2021-07-18 12:13:18.000000 humanleague-2.2.0/src/SobolImpl.cpp
+-rw-r--r--   0 az        (1000) az        (1000)      809 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/SobolImpl.h
+-rw-r--r--   0 az        (1000) az        (1000)     8026 2021-07-18 12:12:45.000000 humanleague-2.2.0/src/StatFuncs.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1587 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/StatFuncs.h
+-rw-r--r--   0 az        (1000) az        (1000)     5562 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/TestIndex.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     2319 2020-02-14 13:07:20.000000 humanleague-2.2.0/src/TestNDArray.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1231 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/TestReduce.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     6194 2018-12-05 09:27:47.000000 humanleague-2.2.0/src/TestSlice.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1146 2020-02-14 13:07:07.000000 humanleague-2.2.0/src/TestSobol.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     3331 2021-01-22 10:30:35.000000 humanleague-2.2.0/src/TestStatFuncs.cpp
+-rw-r--r--   0 az        (1000) az        (1000)     1150 2021-01-22 12:00:10.000000 humanleague-2.2.0/src/UnitTester.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)     4431 2020-11-01 14:04:07.000000 humanleague-2.2.0/src/UnitTester.h
+-rw-rw-r--   0 az        (1000) az        (1000)     5562 2023-04-16 19:21:12.000000 humanleague-2.2.0/src/docstr.inl
+-rw-rw-r--   0 az        (1000) az        (1000)     9757 2023-04-16 19:13:37.000000 humanleague-2.2.0/src/module.cpp
+-rw-rw-r--   0 az        (1000) az        (1000)    16770 2021-06-06 08:18:59.000000 humanleague-2.2.0/src/rcpp_api.cpp
```

### Comparing `humanleague-2.1.9/DESCRIPTION` & `humanleague-2.2.0/DESCRIPTION`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Package: humanleague
 Type: Package
 Title: Synthetic Population Generator
-Version: 2.1.9
+Version: 2.2.0
 Description: Generates high-entropy integer synthetic populations from marginal and (optionally) seed data using quasirandom sampling,
   in arbitrary dimensionality (Smith, Lovelace and Birkin (2017) <doi:10.18564/jasss.3550>).
   The package also provides an implementation of the Iterative Proportional Fitting (IPF) algorithm (Zaloznik (2011) <doi:10.13140/2.1.2480.9923>).
 Authors@R: c(
   person("Andrew", "Smith", email="andrew@friarswood.net", role=c("aut", "cre")),
   person("Steven", "Johnson", role=c("ctb"), comment="Sobol sequence generator implementation"),
   person("Massachusetts Institute of Technology", role=c("cph"), comment="Sobol sequence generator implementation"),
```

### Comparing `humanleague-2.1.9/LICENSE` & `humanleague-2.2.0/LICENSE.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
+# MIT License
 
-Copyright (c) 2017-2021 Andrew Smith
+Copyright &copy; 2017-2023 Andrew Smith
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all
 copies or substantial portions of the Software.
 
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+**THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.**
```

### Comparing `humanleague-2.1.9/PKG-INFO` & `humanleague-2.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,178 +1,174 @@
 Metadata-Version: 2.1
 Name: humanleague
-Version: 2.1.9
+Version: 2.2.0
 Summary: Microsynthesis using quasirandom sampling and/or IPF
 Home-page: http://github.com/virgesmith/humanleague
 Author: Andrew P Smith
-Author-email: a.p.smith@leeds.ac.uk
-License: UNKNOWN
-Description: # humanleague
-        
-        [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
-        
-        [![python (pip) build](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)]()
-        [![python (conda) build](https://github.com/virgesmith/humanleague/actions/workflows/conda-package.yml/badge.svg)]()
-        [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/x9oypgryt21ndc3p?svg=true)](https://ci.appveyor.com/project/virgesmith/humanleague)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9cb56a2ff5f84817805d593823bee3e7)](https://app.codacy.com/app/virgesmith/humanleague?utm_source=github.com&utm_medium=referral&utm_content=virgesmith/humanleague&utm_campaign=Badge_Grade_Dashboard)
-        [![codecov](https://codecov.io/gh/virgesmith/humanleague/branch/master/graph/badge.svg)](https://codecov.io/gh/virgesmith/humanleague)
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1970941.svg)](https://doi.org/10.5281/zenodo.1970941)
-        [![status](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4/status.svg)](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4)
-        
-        [![PyPI version](https://badge.fury.io/py/humanleague.svg)](https://badge.fury.io/py/humanleague)
-        [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/humanleague/badges/version.svg)](https://anaconda.org/conda-forge/humanleague)
-        [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/humanleague/badges/downloads.svg)](https://anaconda.org/conda-forge/humanleague)
-        
-        [![CRAN\_Status\_Badge](https://www.r-pkg.org/badges/version/humanleague)](https://CRAN.R-project.org/package=humanleague)
-        [![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/humanleague?color=black)](https://cran.r-project.org/package=humanleague)
-        
-        ## Introduction
-        
-        *humanleague* is a python *and* an R package for microsynthesising populations from marginal and (optionally) seed data. The package is implemented in C++ for performance.
-        
-        The package contains algorithms that use a number of different microsynthesis techniques:
-        
-        - [Iterative Proportional Fitting (IPF)](https://en.wikipedia.org/wiki/Iterative_proportional_fitting)
-        - [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) (no seed population)
-        - Quasirandom Integer Sampling of IPF (QISI): A combination of the two techniques whereby the integral population is sampled (without replacement) from a distribution constructed from a dynamic IPF solution.
-        
-        The latter provides a bridge between deterministic reweighting and combinatorial optimisation, offering advantages of both techniques:
-        
-        - generates high-entropy integral populations
-        - can be used to generate multiple populations for sensitivity analysis
-        - goes some way to address the 'empty cells' issues that can occur in straight IPF
-        - relatively fast computation time
-        
-        The algorithms:
-        
-        - support arbitrary dimensionality* for both the marginals and the seed.
-        - produce statistical data to ascertain the likelihood/degeneracy of the population (where appropriate).
-        
-        The package also contains the following utility functions:
-        
-        - a Sobol sequence generator
-        - construct a closest integer population from a discrete univariate probability distribution.
-        - an algorithm for sampling an integer population from a discrete multivariate probability distribution, constrained to the marginal sums in every dimension (see [below](#multidimensional-integerisation)).
-        - 'flatten' a multidimensional population into a table: this converts a multidimensional array containing the population count for each state into a table listing individuals and their characteristics.
-        
-        Version 1.0.1 reflects the work described in the [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) paper.
-        
-        ## Installation
-        
-        ### Python
-        
-        Requires Python 3.5 or newer.
-        
-        #### PyPI
-        
-        ```bash
-        python3 -m pip install humanleague --user
-        ```
-        
-        #### Anaconda
-        
-        ```bash
-        conda install -c conda-forge humanleague
-        ```
-        
-        ### Build, install and test (from cloned repo)
-        
-        ```bash
-        python setup.py install --user
-        python setup.py test
-        ```
-        
-        ### R
-        
-        Official release:
-        
-        ```r
-        > install.packages("humanleague")
-        ```
-        
-        For a development version
-        
-        ```r
-        > devtools::install_github("virgesmith/humanleague")
-        ```
-        
-        Or, for the legacy version
-        
-        ```r
-        > devtools::install_github("virgesmith/humanleague@1.0.1")
-        ```
-        
-        ## Documentation and Examples
-        
-        ### R
-        
-        Consult the package documentation, e.g.
-        
-        ```r
-        > library(humanleague)
-        > ?humanleague
-        ```
-        
-        ### Python
-        
-        See [here](doc/api.md), or
-        
-        ```python
-        >>> import humanleague as hl
-        >>> help(hl)
-        ```
-        
-        ### Multidimensional integerisation
-        
-        Building on the `prob2IntFreq` function - which takes a discrete probability distribution and a count, and returns the closest integer population to the distribution that sums to the count - a multidimensional equivalent `integerise` is introduced.
-        In one dimension, for example:
-        
-        ```python
-        >>> import numpy as np
-        >>> import humanleague
-        >>> p=np.array([0.1, 0.2, 0.3, 0.4])
-        >>> humanleague.prob2IntFreq(p, 11)
-        {'freq': array([1, 2, 3, 5]), 'rmse': 0.3535533905932736}
-        
-        ```
-        
-        produces the optimal (i.e. closest possible) integer population to the discrete distribution.
-        
-        The `integerise` function generalises this problem and applies it to higher dimensions: given an n-dimensional array of real numbers where the 1-d marginal sums in every dimension are integral (and thus the total population is too), it attempts to find an integral array that also satisfies these constraints.
-        
-        The QISI algorithm is repurposed to this end. As it is a sampling algorithm it cannot guarantee that a solution is found, and if so, whether the solution is optimal. If it fails this does not prove that a solution does not exist for the given input.
-        
-        ```python
-        >>> a = np.array([[ 0.3,  1.2,  2. ,  1.5],
-                          [ 0.6,  2.4,  4. ,  3. ],
-                          [ 1.5,  6. , 10. ,  7.5],
-                          [ 0.6,  2.4,  4. ,  3. ]])
-        # marginal sums
-        >> sum(a)
-        array([ 3., 12., 20., 15.])
-        >>> sum(a.T)
-        array([ 5., 10., 25., 10.])
-        # perform integerisation
-        >>> r = humanleague.integerise(a)
-        >>> r["conv"]
-        True
-        >>> r["result"]
-        array([[ 0,  2,  2,  1],
-               [ 0,  3,  4,  3],
-               [ 2,  6, 10,  7],
-               [ 1,  1,  4,  4]])
-        >>> r["rmse"]
-        0.5766281297335398
-        # check marginals are preserved
-        >>> sum(r["result"]) == sum(a)
-        array([ True,  True,  True,  True])
-        >>> sum(r["result"].T) == sum(a.T)
-        array([ True,  True,  True,  True])
-        ```
-        
-        
-Platform: UNKNOWN
+Author-email: andrew@friarswood.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENCE
+License-File: LICENSE.md
+
+# humanleague
+
+[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
+
+[![PyPI version](https://badge.fury.io/py/humanleague.svg)](https://badge.fury.io/py/humanleague)
+[![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/humanleague/badges/version.svg)](https://anaconda.org/conda-forge/humanleague)
+[![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/humanleague/badges/downloads.svg)](https://anaconda.org/conda-forge/humanleague)
+[![CRAN\_Status\_Badge](https://www.r-pkg.org/badges/version/humanleague)](https://CRAN.R-project.org/package=humanleague)
+[![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/humanleague?color=black)](https://cran.r-project.org/package=humanleague)
+
+[![DOI](https://zenodo.org/badge/95961787.svg)](https://zenodo.org/badge/latestdoi/95961787)
+[![status](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4/status.svg)](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4)
+
+[![python (pip) build](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)
+[![python (conda) build](https://github.com/virgesmith/humanleague/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/conda.yml/badge.svg)
+[![r-cmd-check](https://github.com/virgesmith/humanleague/actions/workflows/r-cmd-check.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/r-cmd-check/badge.svg)
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/430da36db15f46978bfccd1ad3243ae9)](https://www.codacy.com/gh/virgesmith/humanleague/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=virgesmith/humanleague&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/virgesmith/humanleague/branch/main/graph/badge.svg)](https://codecov.io/gh/virgesmith/humanleague)
+
+## Introduction
+
+*humanleague* is a python *and* an R package for microsynthesising populations from marginal and (optionally) seed data. The package is implemented in C++ for performance.
+
+The package contains algorithms that use a number of different microsynthesis techniques:
+
+- [Iterative Proportional Fitting (IPF)](https://en.wikipedia.org/wiki/Iterative_proportional_fitting)
+- [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) (no seed population)
+- Quasirandom Integer Sampling of IPF (QISI): A combination of the two techniques whereby the integral population is sampled (without replacement) from a distribution constructed from a dynamic IPF solution.
+
+The latter provides a bridge between deterministic reweighting and combinatorial optimisation, offering advantages of both techniques:
+
+- generates high-entropy integral populations
+- can be used to generate multiple populations for sensitivity analysis
+- goes some way to address the 'empty cells' issues that can occur in straight IPF
+- relatively fast computation time
+
+The algorithms:
+
+- support arbitrary dimensionality* for both the marginals and the seed.
+- produce statistical data to ascertain the likelihood/degeneracy of the population (where appropriate).
+
+The package also contains the following utilities:
+
+- a Sobol sequence generator (implemented as a generator class in python)
+- a function to construct a closest integer population from a discrete univariate probability distribution.
+- an algorithm for sampling an integer population from a discrete multivariate probability distribution, constrained to the marginal sums in every dimension (see [below](#multidimensional-integerisation)).
+- 'flatten' a multidimensional population into a table: this converts a multidimensional array containing the population count for each state into a table listing individuals and their characteristics.
+
+Version 1.0.1 reflects the work described in the [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) paper.
+
+## Installation
+
+### Python
+
+Requires Python 3.9 or newer.
+
+#### PyPI
+
+```bash
+python -m pip install humanleague --user
+```
+
+#### Anaconda
+
+```bash
+conda install -c conda-forge humanleague
+```
+
+### Build, install and test (from cloned repo)
+
+```bash
+pip install -e .
+pytest
+```
+
+### R
+
+Official release:
+
+```r
+> install.packages("humanleague")
+```
+
+For a development version
+
+```r
+> devtools::install_github("virgesmith/humanleague")
+```
+
+Or, for the legacy version
+
+```r
+> devtools::install_github("virgesmith/humanleague@1.0.1")
+```
+
+## Documentation and Examples
+
+### R
+
+Consult the package documentation, e.g.
+
+```r
+> library(humanleague)
+> ?humanleague
+```
+
+### Python
+
+The package now contains type annotations and your IDE should automatically display this, e.g.:
+
+![help](./doc/help.png)
+
+### Multidimensional integerisation
+
+Building on the `prob2IntFreq` function - which takes a discrete probability distribution and a count, and returns the closest integer population to the distribution that sums to the count - a multidimensional equivalent `integerise` is introduced.
+In one dimension, for example:
+
+```python
+>>> import numpy as np
+>>> import humanleague
+>>> p=np.array([0.1, 0.2, 0.3, 0.4])
+>>> humanleague.prob2IntFreq(p, 11)
+{'freq': array([1, 2, 3, 5]), 'rmse': 0.3535533905932736}
+
+```
+
+produces the optimal (i.e. closest possible) integer population to the discrete distribution.
+
+The `integerise` function generalises this problem and applies it to higher dimensions: given an n-dimensional array of real numbers where the 1-d marginal sums in every dimension are integral (and thus the total population is too), it attempts to find an integral array that also satisfies these constraints.
+
+The QISI algorithm is repurposed to this end. As it is a sampling algorithm it cannot guarantee that a solution is found, and if so, whether the solution is optimal. If it fails this does not prove that a solution does not exist for the given input.
+
+```python
+>>> a = np.array([[ 0.3,  1.2,  2. ,  1.5],
+                  [ 0.6,  2.4,  4. ,  3. ],
+                  [ 1.5,  6. , 10. ,  7.5],
+                  [ 0.6,  2.4,  4. ,  3. ]])
+# marginal sums
+>> sum(a)
+array([ 3., 12., 20., 15.])
+>>> sum(a.T)
+array([ 5., 10., 25., 10.])
+# perform integerisation
+>>> r = humanleague.integerise(a)
+>>> r["conv"]
+True
+>>> r["result"]
+array([[ 0,  2,  2,  1],
+       [ 0,  3,  4,  3],
+       [ 2,  6, 10,  7],
+       [ 1,  1,  4,  4]])
+>>> r["rmse"]
+0.5766281297335398
+# check marginals are preserved
+>>> sum(r["result"]) == sum(a)
+array([ True,  True,  True,  True])
+>>> sum(r["result"].T) == sum(a.T)
+array([ True,  True,  True,  True])
+```
```

### Comparing `humanleague-2.1.9/README.md` & `humanleague-2.2.0/humanleague.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,41 @@
+Metadata-Version: 2.1
+Name: humanleague
+Version: 2.2.0
+Summary: Microsynthesis using quasirandom sampling and/or IPF
+Home-page: http://github.com/virgesmith/humanleague
+Author: Andrew P Smith
+Author-email: andrew@friarswood.net
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENCE
+License-File: LICENSE.md
+
 # humanleague
 
 [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
 
-[![python (pip) build](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)]()
-[![python (conda) build](https://github.com/virgesmith/humanleague/actions/workflows/conda-package.yml/badge.svg)]()
-[![Appveyor Build status](https://ci.appveyor.com/api/projects/status/x9oypgryt21ndc3p?svg=true)](https://ci.appveyor.com/project/virgesmith/humanleague)
-[![Codacy Badge](https://api.codacy.com/project/badge/Grade/9cb56a2ff5f84817805d593823bee3e7)](https://app.codacy.com/app/virgesmith/humanleague?utm_source=github.com&utm_medium=referral&utm_content=virgesmith/humanleague&utm_campaign=Badge_Grade_Dashboard)
-[![codecov](https://codecov.io/gh/virgesmith/humanleague/branch/master/graph/badge.svg)](https://codecov.io/gh/virgesmith/humanleague)
-
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1970941.svg)](https://doi.org/10.5281/zenodo.1970941)
-[![status](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4/status.svg)](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4)
-
 [![PyPI version](https://badge.fury.io/py/humanleague.svg)](https://badge.fury.io/py/humanleague)
 [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/humanleague/badges/version.svg)](https://anaconda.org/conda-forge/humanleague)
 [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/humanleague/badges/downloads.svg)](https://anaconda.org/conda-forge/humanleague)
-
 [![CRAN\_Status\_Badge](https://www.r-pkg.org/badges/version/humanleague)](https://CRAN.R-project.org/package=humanleague)
 [![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/humanleague?color=black)](https://cran.r-project.org/package=humanleague)
 
+[![DOI](https://zenodo.org/badge/95961787.svg)](https://zenodo.org/badge/latestdoi/95961787)
+[![status](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4/status.svg)](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4)
+
+[![python (pip) build](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)
+[![python (conda) build](https://github.com/virgesmith/humanleague/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/conda.yml/badge.svg)
+[![r-cmd-check](https://github.com/virgesmith/humanleague/actions/workflows/r-cmd-check.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/r-cmd-check/badge.svg)
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/430da36db15f46978bfccd1ad3243ae9)](https://www.codacy.com/gh/virgesmith/humanleague/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=virgesmith/humanleague&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/virgesmith/humanleague/branch/main/graph/badge.svg)](https://codecov.io/gh/virgesmith/humanleague)
+
 ## Introduction
 
 *humanleague* is a python *and* an R package for microsynthesising populations from marginal and (optionally) seed data. The package is implemented in C++ for performance.
 
 The package contains algorithms that use a number of different microsynthesis techniques:
 
 - [Iterative Proportional Fitting (IPF)](https://en.wikipedia.org/wiki/Iterative_proportional_fitting)
@@ -36,46 +50,46 @@
 - relatively fast computation time
 
 The algorithms:
 
 - support arbitrary dimensionality* for both the marginals and the seed.
 - produce statistical data to ascertain the likelihood/degeneracy of the population (where appropriate).
 
-The package also contains the following utility functions:
+The package also contains the following utilities:
 
-- a Sobol sequence generator
-- construct a closest integer population from a discrete univariate probability distribution.
+- a Sobol sequence generator (implemented as a generator class in python)
+- a function to construct a closest integer population from a discrete univariate probability distribution.
 - an algorithm for sampling an integer population from a discrete multivariate probability distribution, constrained to the marginal sums in every dimension (see [below](#multidimensional-integerisation)).
 - 'flatten' a multidimensional population into a table: this converts a multidimensional array containing the population count for each state into a table listing individuals and their characteristics.
 
 Version 1.0.1 reflects the work described in the [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) paper.
 
 ## Installation
 
 ### Python
 
-Requires Python 3.5 or newer.
+Requires Python 3.9 or newer.
 
 #### PyPI
 
 ```bash
-python3 -m pip install humanleague --user
+python -m pip install humanleague --user
 ```
 
 #### Anaconda
 
 ```bash
 conda install -c conda-forge humanleague
 ```
 
 ### Build, install and test (from cloned repo)
 
 ```bash
-python setup.py install --user
-python setup.py test
+pip install -e .
+pytest
 ```
 
 ### R
 
 Official release:
 
 ```r
@@ -103,20 +117,17 @@
 ```r
 > library(humanleague)
 > ?humanleague
 ```
 
 ### Python
 
-See [here](doc/api.md), or
+The package now contains type annotations and your IDE should automatically display this, e.g.:
 
-```python
->>> import humanleague as hl
->>> help(hl)
-```
+![help](./doc/help.png)
 
 ### Multidimensional integerisation
 
 Building on the `prob2IntFreq` function - which takes a discrete probability distribution and a count, and returns the closest integer population to the distribution that sums to the count - a multidimensional equivalent `integerise` is introduced.
 In one dimension, for example:
 
 ```python
@@ -157,8 +168,7 @@
 0.5766281297335398
 # check marginals are preserved
 >>> sum(r["result"]) == sum(a)
 array([ True,  True,  True,  True])
 >>> sum(r["result"].T) == sum(a.T)
 array([ True,  True,  True,  True])
 ```
-
```

### Comparing `humanleague-2.1.9/humanleague.egg-info/PKG-INFO` & `humanleague-2.2.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,178 +1,160 @@
-Metadata-Version: 2.1
-Name: humanleague
-Version: 2.1.9
-Summary: Microsynthesis using quasirandom sampling and/or IPF
-Home-page: http://github.com/virgesmith/humanleague
-Author: Andrew P Smith
-Author-email: a.p.smith@leeds.ac.uk
-License: UNKNOWN
-Description: # humanleague
-        
-        [![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
-        
-        [![python (pip) build](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)]()
-        [![python (conda) build](https://github.com/virgesmith/humanleague/actions/workflows/conda-package.yml/badge.svg)]()
-        [![Appveyor Build status](https://ci.appveyor.com/api/projects/status/x9oypgryt21ndc3p?svg=true)](https://ci.appveyor.com/project/virgesmith/humanleague)
-        [![Codacy Badge](https://api.codacy.com/project/badge/Grade/9cb56a2ff5f84817805d593823bee3e7)](https://app.codacy.com/app/virgesmith/humanleague?utm_source=github.com&utm_medium=referral&utm_content=virgesmith/humanleague&utm_campaign=Badge_Grade_Dashboard)
-        [![codecov](https://codecov.io/gh/virgesmith/humanleague/branch/master/graph/badge.svg)](https://codecov.io/gh/virgesmith/humanleague)
-        
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1970941.svg)](https://doi.org/10.5281/zenodo.1970941)
-        [![status](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4/status.svg)](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4)
-        
-        [![PyPI version](https://badge.fury.io/py/humanleague.svg)](https://badge.fury.io/py/humanleague)
-        [![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/humanleague/badges/version.svg)](https://anaconda.org/conda-forge/humanleague)
-        [![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/humanleague/badges/downloads.svg)](https://anaconda.org/conda-forge/humanleague)
-        
-        [![CRAN\_Status\_Badge](https://www.r-pkg.org/badges/version/humanleague)](https://CRAN.R-project.org/package=humanleague)
-        [![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/humanleague?color=black)](https://cran.r-project.org/package=humanleague)
-        
-        ## Introduction
-        
-        *humanleague* is a python *and* an R package for microsynthesising populations from marginal and (optionally) seed data. The package is implemented in C++ for performance.
-        
-        The package contains algorithms that use a number of different microsynthesis techniques:
-        
-        - [Iterative Proportional Fitting (IPF)](https://en.wikipedia.org/wiki/Iterative_proportional_fitting)
-        - [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) (no seed population)
-        - Quasirandom Integer Sampling of IPF (QISI): A combination of the two techniques whereby the integral population is sampled (without replacement) from a distribution constructed from a dynamic IPF solution.
-        
-        The latter provides a bridge between deterministic reweighting and combinatorial optimisation, offering advantages of both techniques:
-        
-        - generates high-entropy integral populations
-        - can be used to generate multiple populations for sensitivity analysis
-        - goes some way to address the 'empty cells' issues that can occur in straight IPF
-        - relatively fast computation time
-        
-        The algorithms:
-        
-        - support arbitrary dimensionality* for both the marginals and the seed.
-        - produce statistical data to ascertain the likelihood/degeneracy of the population (where appropriate).
-        
-        The package also contains the following utility functions:
-        
-        - a Sobol sequence generator
-        - construct a closest integer population from a discrete univariate probability distribution.
-        - an algorithm for sampling an integer population from a discrete multivariate probability distribution, constrained to the marginal sums in every dimension (see [below](#multidimensional-integerisation)).
-        - 'flatten' a multidimensional population into a table: this converts a multidimensional array containing the population count for each state into a table listing individuals and their characteristics.
-        
-        Version 1.0.1 reflects the work described in the [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) paper.
-        
-        ## Installation
-        
-        ### Python
-        
-        Requires Python 3.5 or newer.
-        
-        #### PyPI
-        
-        ```bash
-        python3 -m pip install humanleague --user
-        ```
-        
-        #### Anaconda
-        
-        ```bash
-        conda install -c conda-forge humanleague
-        ```
-        
-        ### Build, install and test (from cloned repo)
-        
-        ```bash
-        python setup.py install --user
-        python setup.py test
-        ```
-        
-        ### R
-        
-        Official release:
-        
-        ```r
-        > install.packages("humanleague")
-        ```
-        
-        For a development version
-        
-        ```r
-        > devtools::install_github("virgesmith/humanleague")
-        ```
-        
-        Or, for the legacy version
-        
-        ```r
-        > devtools::install_github("virgesmith/humanleague@1.0.1")
-        ```
-        
-        ## Documentation and Examples
-        
-        ### R
-        
-        Consult the package documentation, e.g.
-        
-        ```r
-        > library(humanleague)
-        > ?humanleague
-        ```
-        
-        ### Python
-        
-        See [here](doc/api.md), or
-        
-        ```python
-        >>> import humanleague as hl
-        >>> help(hl)
-        ```
-        
-        ### Multidimensional integerisation
-        
-        Building on the `prob2IntFreq` function - which takes a discrete probability distribution and a count, and returns the closest integer population to the distribution that sums to the count - a multidimensional equivalent `integerise` is introduced.
-        In one dimension, for example:
-        
-        ```python
-        >>> import numpy as np
-        >>> import humanleague
-        >>> p=np.array([0.1, 0.2, 0.3, 0.4])
-        >>> humanleague.prob2IntFreq(p, 11)
-        {'freq': array([1, 2, 3, 5]), 'rmse': 0.3535533905932736}
-        
-        ```
-        
-        produces the optimal (i.e. closest possible) integer population to the discrete distribution.
-        
-        The `integerise` function generalises this problem and applies it to higher dimensions: given an n-dimensional array of real numbers where the 1-d marginal sums in every dimension are integral (and thus the total population is too), it attempts to find an integral array that also satisfies these constraints.
-        
-        The QISI algorithm is repurposed to this end. As it is a sampling algorithm it cannot guarantee that a solution is found, and if so, whether the solution is optimal. If it fails this does not prove that a solution does not exist for the given input.
-        
-        ```python
-        >>> a = np.array([[ 0.3,  1.2,  2. ,  1.5],
-                          [ 0.6,  2.4,  4. ,  3. ],
-                          [ 1.5,  6. , 10. ,  7.5],
-                          [ 0.6,  2.4,  4. ,  3. ]])
-        # marginal sums
-        >> sum(a)
-        array([ 3., 12., 20., 15.])
-        >>> sum(a.T)
-        array([ 5., 10., 25., 10.])
-        # perform integerisation
-        >>> r = humanleague.integerise(a)
-        >>> r["conv"]
-        True
-        >>> r["result"]
-        array([[ 0,  2,  2,  1],
-               [ 0,  3,  4,  3],
-               [ 2,  6, 10,  7],
-               [ 1,  1,  4,  4]])
-        >>> r["rmse"]
-        0.5766281297335398
-        # check marginals are preserved
-        >>> sum(r["result"]) == sum(a)
-        array([ True,  True,  True,  True])
-        >>> sum(r["result"].T) == sum(a.T)
-        array([ True,  True,  True,  True])
-        ```
-        
-        
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
+# humanleague
+
+[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://opensource.org/licenses/MIT)
+
+[![PyPI version](https://badge.fury.io/py/humanleague.svg)](https://badge.fury.io/py/humanleague)
+[![Anaconda-Server Version Badge](https://anaconda.org/conda-forge/humanleague/badges/version.svg)](https://anaconda.org/conda-forge/humanleague)
+[![Anaconda-Server Downloads Badge](https://anaconda.org/conda-forge/humanleague/badges/downloads.svg)](https://anaconda.org/conda-forge/humanleague)
+[![CRAN\_Status\_Badge](https://www.r-pkg.org/badges/version/humanleague)](https://CRAN.R-project.org/package=humanleague)
+[![CRAN Downloads](https://cranlogs.r-pkg.org/badges/grand-total/humanleague?color=black)](https://cran.r-project.org/package=humanleague)
+
+[![DOI](https://zenodo.org/badge/95961787.svg)](https://zenodo.org/badge/latestdoi/95961787)
+[![status](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4/status.svg)](https://joss.theoj.org/papers/d5aaf6e1c2efed431c506762622473b4)
+
+[![python (pip) build](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/pip-package.yml/badge.svg)
+[![python (conda) build](https://github.com/virgesmith/humanleague/actions/workflows/conda.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/conda.yml/badge.svg)
+[![r-cmd-check](https://github.com/virgesmith/humanleague/actions/workflows/r-cmd-check.yml/badge.svg)](https://github.com/virgesmith/humanleague/actions/workflows/r-cmd-check/badge.svg)
+
+[![Codacy Badge](https://app.codacy.com/project/badge/Grade/430da36db15f46978bfccd1ad3243ae9)](https://www.codacy.com/gh/virgesmith/humanleague/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=virgesmith/humanleague&amp;utm_campaign=Badge_Grade)
+[![codecov](https://codecov.io/gh/virgesmith/humanleague/branch/main/graph/badge.svg)](https://codecov.io/gh/virgesmith/humanleague)
+
+## Introduction
+
+*humanleague* is a python *and* an R package for microsynthesising populations from marginal and (optionally) seed data. The package is implemented in C++ for performance.
+
+The package contains algorithms that use a number of different microsynthesis techniques:
+
+- [Iterative Proportional Fitting (IPF)](https://en.wikipedia.org/wiki/Iterative_proportional_fitting)
+- [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) (no seed population)
+- Quasirandom Integer Sampling of IPF (QISI): A combination of the two techniques whereby the integral population is sampled (without replacement) from a distribution constructed from a dynamic IPF solution.
+
+The latter provides a bridge between deterministic reweighting and combinatorial optimisation, offering advantages of both techniques:
+
+- generates high-entropy integral populations
+- can be used to generate multiple populations for sensitivity analysis
+- goes some way to address the 'empty cells' issues that can occur in straight IPF
+- relatively fast computation time
+
+The algorithms:
+
+- support arbitrary dimensionality* for both the marginals and the seed.
+- produce statistical data to ascertain the likelihood/degeneracy of the population (where appropriate).
+
+The package also contains the following utilities:
+
+- a Sobol sequence generator (implemented as a generator class in python)
+- a function to construct a closest integer population from a discrete univariate probability distribution.
+- an algorithm for sampling an integer population from a discrete multivariate probability distribution, constrained to the marginal sums in every dimension (see [below](#multidimensional-integerisation)).
+- 'flatten' a multidimensional population into a table: this converts a multidimensional array containing the population count for each state into a table listing individuals and their characteristics.
+
+Version 1.0.1 reflects the work described in the [Quasirandom Integer Sampling (QIS)](http://jasss.soc.surrey.ac.uk/20/4/14.html) paper.
+
+## Installation
+
+### Python
+
+Requires Python 3.9 or newer.
+
+#### PyPI
+
+```bash
+python -m pip install humanleague --user
+```
+
+#### Anaconda
+
+```bash
+conda install -c conda-forge humanleague
+```
+
+### Build, install and test (from cloned repo)
+
+```bash
+pip install -e .
+pytest
+```
+
+### R
+
+Official release:
+
+```r
+> install.packages("humanleague")
+```
+
+For a development version
+
+```r
+> devtools::install_github("virgesmith/humanleague")
+```
+
+Or, for the legacy version
+
+```r
+> devtools::install_github("virgesmith/humanleague@1.0.1")
+```
+
+## Documentation and Examples
+
+### R
+
+Consult the package documentation, e.g.
+
+```r
+> library(humanleague)
+> ?humanleague
+```
+
+### Python
+
+The package now contains type annotations and your IDE should automatically display this, e.g.:
+
+![help](./doc/help.png)
+
+### Multidimensional integerisation
+
+Building on the `prob2IntFreq` function - which takes a discrete probability distribution and a count, and returns the closest integer population to the distribution that sums to the count - a multidimensional equivalent `integerise` is introduced.
+In one dimension, for example:
+
+```python
+>>> import numpy as np
+>>> import humanleague
+>>> p=np.array([0.1, 0.2, 0.3, 0.4])
+>>> humanleague.prob2IntFreq(p, 11)
+{'freq': array([1, 2, 3, 5]), 'rmse': 0.3535533905932736}
+
+```
+
+produces the optimal (i.e. closest possible) integer population to the discrete distribution.
+
+The `integerise` function generalises this problem and applies it to higher dimensions: given an n-dimensional array of real numbers where the 1-d marginal sums in every dimension are integral (and thus the total population is too), it attempts to find an integral array that also satisfies these constraints.
+
+The QISI algorithm is repurposed to this end. As it is a sampling algorithm it cannot guarantee that a solution is found, and if so, whether the solution is optimal. If it fails this does not prove that a solution does not exist for the given input.
+
+```python
+>>> a = np.array([[ 0.3,  1.2,  2. ,  1.5],
+                  [ 0.6,  2.4,  4. ,  3. ],
+                  [ 1.5,  6. , 10. ,  7.5],
+                  [ 0.6,  2.4,  4. ,  3. ]])
+# marginal sums
+>> sum(a)
+array([ 3., 12., 20., 15.])
+>>> sum(a.T)
+array([ 5., 10., 25., 10.])
+# perform integerisation
+>>> r = humanleague.integerise(a)
+>>> r["conv"]
+True
+>>> r["result"]
+array([[ 0,  2,  2,  1],
+       [ 0,  3,  4,  3],
+       [ 2,  6, 10,  7],
+       [ 1,  1,  4,  4]])
+>>> r["rmse"]
+0.5766281297335398
+# check marginals are preserved
+>>> sum(r["result"]) == sum(a)
+array([ True,  True,  True,  True])
+>>> sum(r["result"].T) == sum(a.T)
+array([ True,  True,  True,  True])
+```
```

### Comparing `humanleague-2.1.9/humanleague.egg-info/SOURCES.txt` & `humanleague-2.2.0/humanleague.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 DESCRIPTION
 LICENCE
-LICENSE
+LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+humanleague/__init__.py
+humanleague/__init__.pyi
+humanleague/py.typed
 humanleague.egg-info/PKG-INFO
 humanleague.egg-info/SOURCES.txt
 humanleague.egg-info/dependency_links.txt
 humanleague.egg-info/not-zip-safe
 humanleague.egg-info/requires.txt
 humanleague.egg-info/top_level.txt
 src/DDWR.h
```

### Comparing `humanleague-2.1.9/setup.py` & `humanleague-2.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,71 +1,74 @@
 #!/usr/bin/env python3
 
 import glob
-from setuptools import setup
+from setuptools import setup  # type: ignore
 from pybind11.setup_helpers import Pybind11Extension, ParallelCompile
 
 
 def readme():
   with open('README.md') as f:
     return f.read()
 
+
 def version():
   """ The R file DESCRIPTION in the project root is now the single source of version info """
   with open("DESCRIPTION") as fd:
     lines = fd.readlines()
     for line in lines:
       if line.startswith("Version:"):
         return line.rstrip().split(":")[1].lstrip()
 
-def source_files():
 
+def source_files():
   sources = glob.glob("src/*.cpp")
   # can't use compile skips as some files are auto-generated
   skip = ["RcppExports.cpp", "rcpp_api.cpp"]
   for s in skip:
-    sources = [f for f in sources if not s in f]
+    sources = [f for f in sources if s not in f]
 
   return sources
 
-def header_files():
 
+def header_files():
   return glob.glob("src/*.h")
 
 
 def defines():
   return [
     ("HUMANLEAGUE_VERSION", version()),
     ("PYTHON_MODULE", None)
   ]
 
 
 ext_modules = [
   Pybind11Extension(
-    'humanleague',
+    '_humanleague',
     sources=source_files(),
     include_dirs=["src"],
     define_macros=defines(),
     depends=["setup.py", "DESCRIPTION", "src/docstr.inl"] + header_files(),
-    cxx_std=17
+    cxx_std=20,
   )
 ]
 
 
 ParallelCompile().install()
 
 setup(
-  name = 'humanleague',
-  version = version(),
-  description = 'Microsynthesis using quasirandom sampling and/or IPF',
-  author = 'Andrew P Smith',
-  author_email = 'a.p.smith@leeds.ac.uk',
-  url = 'http://github.com/virgesmith/humanleague',
-  long_description = readme(),
+  name='humanleague',
+  version=version(),
+  description='Microsynthesis using quasirandom sampling and/or IPF',
+  author='Andrew P Smith',
+  author_email='andrew@friarswood.net',
+  url='http://github.com/virgesmith/humanleague',
+  long_description=readme(),
   long_description_content_type="text/markdown",
+  packages=["humanleague"],
+  package_data={"humanleague": ["py.typed", "*.pyi"]},
   ext_modules=ext_modules,
   install_requires=['numpy>=1.19.1'],
   setup_requires=['pybind11>=2.5.0', 'pytest-runner'],
   tests_require=['pytest'],
   classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `humanleague-2.1.9/src/DDWR.h` & `humanleague-2.2.0/src/DDWR.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/IPF.h` & `humanleague-2.2.0/src/IPF.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/Index.cpp` & `humanleague-2.2.0/src/Index.cpp`

 * *Files 5% similar despite different names*

```diff
@@ -89,21 +89,19 @@
   return m_idx;
 }
 
 
 MappedIndex::MappedIndex(const Index& idx, const std::vector<int64_t>& mappedDimensions)
 : m_dim(mappedDimensions.size()), m_sizes(m_dim), m_mappedIndex(m_dim), m_atEnd(idx.end())
 {
-  int64_t n = idx.size();
-  (void)n; // avoid compiler warning about unused variable when assert exands to nothing
   // TODO check mappedDimensions are unique
   for (size_t d = 0; d < m_dim; ++d)
   {
     // check mappedDimensions are within dimension of index
-    assert(mappedDimensions[d] < n);
+    assert(mappedDimensions[d] < idx.size());
     m_sizes[d] = idx.sizes()[mappedDimensions[d]];
     m_mappedIndex[d] = &const_cast<Index&>(idx)[mappedDimensions[d]];
   }
 }
 
 const MappedIndex& MappedIndex::operator++()
 {
```

### Comparing `humanleague-2.1.9/src/Index.h` & `humanleague-2.2.0/src/Index.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 // Index.h
 
 #pragma once
 
 #include <vector>
 
+#if __cplusplus <= 201703l
 #include <cstddef>
+#endif
 #include <cstdint>
 
 // Indexer for elements in n-D array - iterates over entire array
 class Index
 {
 public:
```

### Comparing `humanleague-2.1.9/src/Integerise.cpp` & `humanleague-2.2.0/src/Integerise.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/Integerise.h` & `humanleague-2.2.0/src/Integerise.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/Log.h` & `humanleague-2.2.0/src/Log.h`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #pragma once
 
 #include <string>
 #include <iostream>
 
 
 // C++14 implements the ""s literal -> std::string but there are so many issues with it (namespace, gcc warnings)
-// just stick with the home-made version 
+// just stick with the home-made version
 
 inline std::string operator "" _s(const char* p, size_t s)
 {
   return std::string(p, p + s);
 }
 
 template<typename T>
@@ -19,16 +19,17 @@
   return std::to_string(v);
 }
 
 // print pointer
 template<typename T>
 std::string to_string_impl(T* p)
 {
-  char buf[20];
-  std::sprintf(buf, "0x%016zx", reinterpret_cast<size_t>(p));
+  constexpr size_t BUF_SIZE = 20;
+  static char buf[BUF_SIZE];
+  std::snprintf(buf, BUF_SIZE, "0x%016zx", reinterpret_cast<size_t>(p));
   return std::string(buf);
 }
 
 template<>
 inline std::string to_string_impl(const char* v)
 {
   return std::string(v);
@@ -40,29 +41,29 @@
 }
 
 template<typename T>
 std::string to_string_impl(const std::vector<T>& v)
 {
   if (v.empty())
     return "[]";
-  std::string result = "[" + to_string_impl(v[0]);  
+  std::string result = "[" + to_string_impl(v[0]);
 
   for (size_t i = 1; i < v.size(); ++i)
     result += ", " + to_string_impl(v[i]);
   result += "]";
 
   return result;
 }
 
 
 // need an rvalue ref as might/will be a temporary
-template<typename T> 
+template<typename T>
 std::string operator%(std::string&& str, T value)
 {
   size_t s = str.find("%%");
   if (s != std::string::npos)
   {
-    str.replace(s, 2, to_string_impl(value)); 
+    str.replace(s, 2, to_string_impl(value));
   }
   return std::move(str);
 }
```

### Comparing `humanleague-2.1.9/src/Microsynthesis.h` & `humanleague-2.2.0/src/Microsynthesis.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/NDArray.h` & `humanleague-2.2.0/src/NDArray.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 
 #pragma once
 
 #include <algorithm>
 #include <stdexcept>
 
 #include <vector>
+#if __cplusplus <= 201703l
 #include <cstddef>
+#endif
 #include <cassert>
 
 // The array storage
 template<typename T>
 class NDArray
 {
 public:
@@ -41,26 +43,26 @@
     assert(m_storageSize < MaxSize);
     for (size_t i = 1; i < m_dim; ++i)
     {
       assert(sizes[i] < MaxSize);
       m_storageSize *= sizes[i];
     }
     computeOffsets();
-    
+
     m_data = storage;
     m_owned = false;
   }
 
   // Disallow copy
   NDArray(const NDArray&) = delete;
   NDArray& operator=(const NDArray&) = delete;
 
   // Copying is strongly discouraged for efficiency reasons, however there will always be times when a copy is unavoidable...
   // By explictly providing a copy function we avoid sloppy/inefficient coding where implicit copies are (inadvertently) taken
-  static void copy(const NDArray<T>& src, NDArray<T>& dest) 
+  static void copy(const NDArray<T>& src, NDArray<T>& dest)
   {
     dest.resize(src.m_sizes);
     std::copy(src.m_data, src.m_data + src.m_storageSize, dest.m_data);
   }
 
   // But allow move
   NDArray(NDArray&& a)
@@ -143,45 +145,45 @@
 
   reference operator[](const std::vector<int64_t>& index)
   {
 // STL-like debugging
 #ifdef GLIBCXX_DEBUG
     if (offset[index] >= m_storageSize)
       throw std::runtime_error("NDArray bounds (index, non-const)");
-#endif    
+#endif
     return m_data[offset(index)];
   }
 
   const_reference operator[](const std::vector<int64_t>& index) const
   {
 // STL-like debugging
 #ifdef GLIBCXX_DEBUG
     if (offset[index] >= m_storageSize)
       throw std::runtime_error("NDArray bounds (index, const)");
-#endif    
+#endif
     return m_data[offset(index)];
   }
 
   reference operator[](const std::vector<int64_t*>& index)
   {
 // STL-like debugging
 #ifdef GLIBCXX_DEBUG
     if (offset[index] >= m_storageSize)
       throw std::runtime_error("NDArray bounds (mapped index, non-const)");
-#endif    
+#endif
     return m_data[offset(index)];
   }
 
   const_reference operator[](const std::vector<int64_t*>& index) const
   {
 // STL-like debugging
 #ifdef GLIBCXX_DEBUG
     if (offset[index] >= m_storageSize)
       throw std::runtime_error("NDArray bounds (mapped index, const)");
-#endif    
+#endif
     return m_data[offset(index)];
   }
 
   value_type* begin() const
   {
     return m_data;
   }
```

### Comparing `humanleague-2.1.9/src/NDArrayUtils.h` & `humanleague-2.2.0/src/NDArrayUtils.h`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #include "Index.h"
 
 #include <vector>
 #include <numeric>
 #include <limits>
 #include <cassert>
 #include <iostream>
+#include <string>
 #include <cmath>
 
 
 int32_t maxAbsElement(const std::vector<int32_t>& r);
 
 std::vector<int32_t> diff(const std::vector<uint32_t>& x, const std::vector<uint32_t>& y);
```

### Comparing `humanleague-2.1.9/src/QIS.cpp` & `humanleague-2.2.0/src/QIS.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/QIS.h` & `humanleague-2.2.0/src/QIS.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/QISI.cpp` & `humanleague-2.2.0/src/QISI.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/QISI.h` & `humanleague-2.2.0/src/QISI.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/RcppExports.cpp` & `humanleague-2.2.0/src/RcppExports.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/Sobol.cpp` & `humanleague-2.2.0/src/Sobol.cpp`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-//
-
 #include "Sobol.h"
 
 #include <limits>
 #include <stdexcept>
 #include <cstdint>
 
-#include <iostream>
 
-Sobol::Sobol(uint32_t dim, uint32_t nSkip) : m_dim(dim), m_buf(dim), m_pos(dim) // ensures m_buf gets populated on 1st access
+Sobol::Sobol(size_t dim, uint32_t nSkip) : m_dim(dim), m_buf(dim), m_pos(dim) // ensures m_buf gets populated on 1st access
 {
   m_s = nlopt_sobol_create(dim);
   if (nSkip > 0)
     skip(nSkip);
 }
 
 Sobol::~Sobol()
@@ -38,37 +35,42 @@
   }
   return m_buf[m_pos++];
 }
 
 // Skip largest 2^k-1 < n
 void Sobol::skip(uint32_t n)
 {
-  uint32_t k = 1;
-  while (k < n)
-    k *= 2;
-
-  //std::cout << "skips=" << k << std::endl;
-  //uint32_t skipped = 0;
-  while (--k > 0)
+  uint32_t b = 0;
+  while (n > 1)
+  {
+    ++b;
+    n >>= 1;
+  }
+
+  uint32_t k = 1 << b;
+  while (k--)
   {
-    //++skipped;
     buf();
   }
-  //std::cout << "skipped=" << skipped << std::endl;
 }
 
 
 void Sobol::reset(uint32_t nSkip)
 {
   nlopt_sobol_destroy(m_s);
   m_s = nlopt_sobol_create(m_dim);
   if (nSkip > 0)
     skip(nSkip);
 }
 
+uint32_t Sobol::dim() const
+{
+  return m_dim;
+}
+
 uint32_t Sobol::min() const
 {
   return 0;
 }
 
 uint32_t Sobol::max() const
 {
```

### Comparing `humanleague-2.1.9/src/Sobol.h` & `humanleague-2.2.0/src/Sobol.h`

 * *Files 27% similar despite different names*

```diff
@@ -4,44 +4,52 @@
 // TODO can this be moved into cpp?
 extern "C"
 {
 #include "SobolImpl.h"
 }
 
 #include <vector>
-
+#include <limits>
 #include <cstdint>
+#if __cplusplus <= 201703l
+#include <cstddef>
+#endif
 
 // This class is roughly compatible with C++11's distribution objects
 // NB check for 32 vs 64 bit issues (distribution may expect 64 bit variates, this class returns 32bit)
 class Sobol
 {
 public:
 
-  typedef uint32_t result_type;
+  static constexpr double SCALE = 1.0 / (1ull << std::numeric_limits<uint32_t>::digits);
+
+  explicit Sobol(size_t dim, uint32_t nSkip = 0u);
 
-  // TODO reset (somehow)
-  explicit Sobol(uint32_t dim, result_type nSkip = 0u);
+  Sobol(const Sobol&) = delete;
+  Sobol& operator=(const Sobol&) = delete;
 
   ~Sobol();
 
-  const std::vector<result_type>& buf();
+  const std::vector<uint32_t>& buf();
 
-  // NB use with care in std::distribtion objects, which may be expecting a 64-bit variate
-  result_type operator()();
+  // NB use with care in std::distribution objects, which may be expecting a 64-bit variate
+  uint32_t operator()();
 
   // Skip largest 2^k <= n
-  void skip(result_type n);
+  void skip(uint32_t n);
 
   void reset(uint32_t nSkip = 0u);
 
-  result_type min() const;
+  uint32_t dim() const;
 
-  result_type max() const;
+  uint32_t min() const;
+
+  uint32_t max() const;
 
 private:
 
   SobolData* m_s;
   uint32_t m_dim;
-  std::vector<result_type> m_buf;
+  std::vector<uint32_t> m_buf;
   uint32_t m_pos;
 };
+
```

### Comparing `humanleague-2.1.9/src/SobolData.h` & `humanleague-2.2.0/src/SobolData.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/SobolImpl.cpp` & `humanleague-2.2.0/src/SobolImpl.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/SobolImpl.h` & `humanleague-2.2.0/src/SobolImpl.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/StatFuncs.cpp` & `humanleague-2.2.0/src/StatFuncs.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/StatFuncs.h` & `humanleague-2.2.0/src/StatFuncs.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/TestIndex.cpp` & `humanleague-2.2.0/src/TestIndex.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/TestNDArray.cpp` & `humanleague-2.2.0/src/TestNDArray.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/TestReduce.cpp` & `humanleague-2.2.0/src/TestReduce.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/TestSlice.cpp` & `humanleague-2.2.0/src/TestSlice.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/TestSobol.cpp` & `humanleague-2.2.0/src/TestSobol.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/TestStatFuncs.cpp` & `humanleague-2.2.0/src/TestStatFuncs.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/UnitTester.cpp` & `humanleague-2.2.0/src/UnitTester.cpp`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/UnitTester.h` & `humanleague-2.2.0/src/UnitTester.h`

 * *Files identical despite different names*

### Comparing `humanleague-2.1.9/src/docstr.inl` & `humanleague-2.2.0/src/docstr.inl`

 * *Files 7% similar despite different names*

```diff
@@ -65,18 +65,33 @@
         length: The length of the returned sequence
 
     Returns:
 
         A 2d array containing Sobol sequence values in (0,1).
 )docstr";
 
+const char* SobolSequence_docstr = R"docstr(
+    Generator that returns the next value in a Sobol' sequence given of supplied dimension, optionally skipping values.
+
+        dim: The dimension of the sequence (between 1 and 1111).
+
+        length: The length of the returned sequence
+
+        skips: The number of values to skip. NB the actual number skipped will be the largest power of 2 smaller than the supplied value.
+
+    Returns:
+
+        A generator object that produces Sobol sequence values in (0,1).
+)docstr";
+
+
 const char* ipf_docstr = R"docstr(
     Uses iterative proportional fitting to construct an n-dimensional array from a seed population that matches the specified marginal sums.
 
-        seed: The seed population as an array.
+        seed: The seed population or distribution.
 
         indices: A list of the indices in the overall array that each marginal represents
 
         marginals: A list of arrays containing the marginal sums.
 
     Returns:
 
@@ -108,15 +123,15 @@
 
         A dictionary containing the result, a convergence flag, the total population, the iterations and the some statistical measures.
 )docstr";
 
 const char* qisi_docstr = R"docstr(
     Uses quasirandom integer sampling to construct an n-dimensional population array that matches the specified marginal sums.
 
-        seed: The dimension of the sequence (between 1 and 1111).
+        seed: The seed population or distribution.
 
         indices: A list of the indices in the overall array that each marginal represents
 
         marginals: A list of arrays containing the marginal sums.
 
         skips: The number of Sobol values to skip. NB the actual number skipped will be the largest power of 2 smaller than the supplied value.
 
@@ -124,15 +139,15 @@
 
         A dictionary containing the result, a convergence flag, the total population, the iterations and the some statistical measures.
 )docstr";
 
 const char* qisi2_docstr = R"docstr(
     Uses quasirandom integer sampling to construct an n-dimensional population array that matches the specified marginal sums.
 
-        seed: The dimension of the sequence (between 1 and 1111).
+        seed: The seed population or distribution.
 
         indices: A list of the indices in the overall array that each marginal represents
 
         marginals: A list of arrays containing the marginal sums.
 
     Returns:
```

### Comparing `humanleague-2.1.9/src/module.cpp` & `humanleague-2.2.0/src/module.cpp`

 * *Files 4% similar despite different names*

```diff
@@ -81,21 +81,14 @@
 template<typename T>
 py::array_t<T> fromNDArray(const NDArray<T>& a)
 {
   // TODO ensure this is safe. may need to explicitly copy data
   return py::array_t<T>(a.sizes(), a.rawData());
 
 }
-// explicit array_t(ShapeContainer shape, const T *ptr = nullptr, handle base = handle())
-//         : array_t(private_ctor{}, std::move(shape),
-//                 ExtraFlags & f_style
-//                 ? detail::f_strides(*shape, itemsize())
-//                 : detail::c_strides(*shape, itemsize()),
-//                 ptr, base) { }
-
 
 py::list flatten(const py::array_t<int64_t>& a)
 {
   const NDArray<int64_t> array = asNDArray<int64_t>(a);
 
   size_t pop = 0;
   for (Index i(array.sizes()); !i.end(); ++i)
@@ -146,24 +139,52 @@
     throw py::value_error("Dim %% is not in valid range [1,1111]"_s % dim);
   }
 
   std::vector<int64_t> sizes{ length, dim };
   py::array_t<double> sequence(sizes);
 
   Sobol sobol(dim, skips);
-  const double scale = 0.5 / (1u << 31);
 
-  for (double* p = begin(sequence); p != end(sequence); ++p)
-  {
-    *p = sobol() * scale;
-  }
+  std::generate(begin(sequence), end(sequence), [&]() { return sobol() * Sobol::SCALE; });
 
   return sequence;
 }
 
+
+class SobolGenerator
+{
+public:
+  SobolGenerator(uint32_t dim, uint32_t nSkip = 0) : m_sobol(dim, nSkip) { }
+
+  py::array_t<double> next()
+  {
+    py::array_t<double> sequence(m_sobol.dim());
+    try
+    {
+      const std::vector<uint32_t>& buf = m_sobol.buf();
+      std::transform(buf.cbegin(), buf.cend(), begin(sequence), [](uint32_t i) { return i * Sobol::SCALE; });
+      return sequence;
+    }
+    catch(const std::runtime_error&)
+    {
+      throw py::stop_iteration();
+    }
+  }
+
+  SobolGenerator& iter()
+  {
+    return *this;
+  }
+
+private:
+    Sobol m_sobol;
+};
+
+
+
 py::dict integerise(const py::array_t<double>& npseed)
 {
   const NDArray<double> seed = asNDArray<double>(npseed); // shallow copy
   Integeriser integeriser(seed);
 
   py::dict retval;
   retval["result"] = fromNDArray<int64_t>(integeriser.result());
@@ -290,15 +311,15 @@
 
 
 } // namespace hl
 
 using py::literals::operator ""_a;
 
 
-PYBIND11_MODULE(humanleague, m) {
+PYBIND11_MODULE(_humanleague, m) {
 
 #include "docstr.inl"
 
   m.doc() = module_docstr;
 
   m.attr("__version__") = STR(HUMANLEAGUE_VERSION);
 
@@ -342,14 +363,21 @@
         hl::qisi,
         qisi_docstr,
         "seed"_a, "indices"_a, "marginals"_a, "skips"_a)
    .def("qisi",
         [](const py::array_t<double>& seed, const py::list& indices, const py::list& marginals) { return hl::qisi(seed, indices, marginals, 0); },
         qisi2_docstr,
         "seed"_a, "indices"_a, "marginals"_a)
-   .def("unittest",
+   .def("_unittest",
         hl::unittest,
         unittest_docstr)
     ;
+
+  py::class_<hl::SobolGenerator>(m, "SobolSequence", SobolSequence_docstr)
+      .def(py::init<size_t, uint32_t>())
+      .def(py::init<size_t>())
+      .def("__iter__", &hl::SobolGenerator::iter, "__iter__ dunder")
+      .def("__next__", &hl::SobolGenerator::next, "__next__ dunder")
+      ;
 }
 
 #endif
```

### Comparing `humanleague-2.1.9/src/rcpp_api.cpp` & `humanleague-2.2.0/src/rcpp_api.cpp`

 * *Files identical despite different names*

