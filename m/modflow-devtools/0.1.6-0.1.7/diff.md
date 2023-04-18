# Comparing `tmp/modflow-devtools-0.1.6.tar.gz` & `tmp/modflow-devtools-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-devtools-0.1.6.tar", last modified: Wed Feb 15 19:43:47 2023, max compression
+gzip compressed data, was "modflow-devtools-0.1.7.tar", last modified: Tue Apr 18 21:06:43 2023, max compression
```

## Comparing `modflow-devtools-0.1.6.tar` & `modflow-devtools-0.1.7.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 19:43:47.231438 modflow-devtools-0.1.6/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1627 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-02-15 19:43:47.227439 modflow-devtools-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 19:43:47.227439 modflow-devtools-0.1.6/modflow_devtools/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1923 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/executables.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 19:43:47.227439 modflow-devtools-0.1.6/modflow_devtools/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/test/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/modflow_devtools/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-15 19:43:47.227439 modflow-devtools-0.1.6/modflow_devtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-02-15 19:43:47.000000 modflow-devtools-0.1.6/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-02-15 19:43:47.000000 modflow-devtools-0.1.6/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 19:43:47.000000 modflow-devtools-0.1.6/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-15 19:43:34.000000 modflow-devtools-0.1.6/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-02-15 19:43:47.000000 modflow-devtools-0.1.6/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-15 19:43:47.000000 modflow-devtools-0.1.6/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-15 19:43:47.231438 modflow-devtools-0.1.6/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-15 19:43:23.000000 modflow-devtools-0.1.6/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1627 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.613777 modflow-devtools-0.1.7/modflow_devtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/executables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/modflow_devtools/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_executables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_markers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.613777 modflow-devtools-0.1.7/modflow_devtools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:06:31.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/version.txt
```

### Comparing `modflow-devtools-0.1.6/LICENSE.md` & `modflow-devtools-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/PKG-INFO` & `modflow-devtools-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
@@ -24,15 +24,14 @@
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # MODFLOW developer tools
 
-### Version 0.1.6 &mdash; release candidate
 [![GitHub tag](https://img.shields.io/github/tag/MODFLOW-USGS/modflow-devtools.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/tags/latest)
 [![PyPI Version](https://img.shields.io/pypi/v/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Versions](https://img.shields.io/pypi/pyversions/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Status](https://img.shields.io/pypi/status/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![CI](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/modflow-devtools/badge/?version=latest)](https://modflow-devtools.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `modflow-devtools-0.1.6/README.md` & `modflow-devtools-0.1.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # MODFLOW developer tools
 
-### Version 0.1.6 &mdash; release candidate
 [![GitHub tag](https://img.shields.io/github/tag/MODFLOW-USGS/modflow-devtools.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/tags/latest)
 [![PyPI Version](https://img.shields.io/pypi/v/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Versions](https://img.shields.io/pypi/pyversions/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Status](https://img.shields.io/pypi/status/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![CI](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/modflow-devtools/badge/?version=latest)](https://modflow-devtools.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `modflow-devtools-0.1.6/modflow_devtools/build.py` & `modflow-devtools-0.1.7/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/case.py` & `modflow-devtools-0.1.7/modflow_devtools/case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/context.py` & `modflow-devtools-0.1.7/modflow_devtools/context.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/download.py` & `modflow-devtools-0.1.7/modflow_devtools/download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/fixtures.py` & `modflow-devtools-0.1.7/modflow_devtools/fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/markers.py` & `modflow-devtools-0.1.7/modflow_devtools/markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/misc.py` & `modflow-devtools-0.1.7/modflow_devtools/misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_build.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_case.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_download.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_executables.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_fixtures.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_markers.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_misc.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/test/test_zip.py` & `modflow-devtools-0.1.7/modflow_devtools/test/test_zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools/zip.py` & `modflow-devtools-0.1.7/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/modflow_devtools.egg-info/PKG-INFO` & `modflow-devtools-0.1.7/modflow_devtools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
@@ -24,15 +24,14 @@
 Provides-Extra: lint
 Provides-Extra: test
 Provides-Extra: docs
 License-File: LICENSE.md
 
 # MODFLOW developer tools
 
-### Version 0.1.6 &mdash; release candidate
 [![GitHub tag](https://img.shields.io/github/tag/MODFLOW-USGS/modflow-devtools.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/tags/latest)
 [![PyPI Version](https://img.shields.io/pypi/v/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Versions](https://img.shields.io/pypi/pyversions/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![PyPI Status](https://img.shields.io/pypi/status/modflow-devtools.png)](https://pypi.python.org/pypi/modflow-devtools)
 [![CI](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml/badge.svg)](https://github.com/MODFLOW-USGS/modflow-devtools/actions/workflows/ci.yml)
 [![Documentation Status](https://readthedocs.org/projects/modflow-devtools/badge/?version=latest)](https://modflow-devtools.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `modflow-devtools-0.1.6/modflow_devtools.egg-info/SOURCES.txt` & `modflow-devtools-0.1.7/modflow_devtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.6/pyproject.toml` & `modflow-devtools-0.1.7/pyproject.toml`

 * *Files identical despite different names*

