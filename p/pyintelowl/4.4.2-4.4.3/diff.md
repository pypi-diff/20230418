# Comparing `tmp/pyintelowl-4.4.2.tar.gz` & `tmp/pyintelowl-4.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyintelowl-4.4.2.tar", last modified: Mon Mar 27 15:22:42 2023, max compression
+gzip compressed data, was "pyintelowl-4.4.3.tar", last modified: Tue Apr 18 10:02:20 2023, max compression
```

## Comparing `pyintelowl-4.4.2.tar` & `pyintelowl-4.4.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:42.681478 pyintelowl-4.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-27 15:22:42.681478 pyintelowl-4.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:42.677478 pyintelowl-4.4.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:42.677478 pyintelowl-4.4.2/pyintelowl/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:42.681478 pyintelowl-4.4.2/pyintelowl/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/_jobs_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/analyse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    52097 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/domain_checkers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/cli/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    38029 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/pyintelowl.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyintelowl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:42.677478 pyintelowl-4.4.2/pyintelowl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5093 2023-03-27 15:22:42.000000 pyintelowl-4.4.2/pyintelowl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-27 15:22:42.000000 pyintelowl-4.4.2/pyintelowl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 15:22:42.000000 pyintelowl-4.4.2/pyintelowl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-03-27 15:22:42.000000 pyintelowl-4.4.2/pyintelowl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-03-27 15:22:42.000000 pyintelowl-4.4.2/pyintelowl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-27 15:22:42.000000 pyintelowl-4.4.2/pyintelowl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 15:22:42.681478 pyintelowl-4.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 15:22:42.681478 pyintelowl-4.4.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/tests/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/tests/test_general.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/tests/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-03-27 15:22:29.000000 pyintelowl-4.4.2/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.606759 pyintelowl-4.4.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.606759 pyintelowl-4.4.3/pyintelowl/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/pyintelowl/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/_jobs_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/analyse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8406 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52097 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/domain_checkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/cli/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/exceptions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1286 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38283 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/pyintelowl.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyintelowl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.606759 pyintelowl-4.4.3/pyintelowl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4906 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 10:02:20.000000 pyintelowl-4.4.3/pyintelowl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2570 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:02:20.610759 pyintelowl-4.4.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6399 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10651 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/test_general.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-04-18 10:02:10.000000 pyintelowl-4.4.3/tests/utils.py
```

### Comparing `pyintelowl-4.4.2/LICENSE` & `pyintelowl-4.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/PKG-INFO` & `pyintelowl-4.4.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: pyintelowl
-Version: 4.4.2
+Version: 4.4.3
 Summary: Robust Python SDK and CLI for IntelOwl's API
 Home-page: https://github.com/intelowlproject/pyintelowl
 Author: Matteo Lodi
 Project-URL: Documentation, https://github.com/intelowlproject/pyintelowl
 Project-URL: Funding, https://liberapay.com/IntelOwlProject/
 Project-URL: Source, https://github.com/intelowlproject/pyintelowl
 Project-URL: Tracker, https://github.com/intelowlproject/pyintelowl/issues
 Keywords: intelowl sdk python command line osint threat intel malware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # PyIntelOwl
 
 [![PyPI version](https://badge.fury.io/py/pyintelowl.svg)](https://badge.fury.io/py/pyintelowl)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/pyintelowl.svg)](https://pypi.python.org/pypi/pyintelowl/)
 
 [![Pull request automation](https://github.com/intelowlproject/pyintelowl/actions/workflows/pull_request_automation.yml/badge.svg)](https://github.com/intelowlproject/pyintelowl/actions/workflows/pull_request_automation.yml)
 [![codecov](https://codecov.io/gh/intelowlproject/pyintelowl/branch/master/graph/badge.svg?token=JF62UMZ0U6)](https://codecov.io/gh/intelowlproject/pyintelowl)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/intelowlproject/pyintelowl.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mlodic/pyintelowl/context:python)
 [![CodeFactor](https://www.codefactor.io/repository/github/intelowlproject/pyintelowl/badge)](https://www.codefactor.io/repository/github/intelowlproject/pyintelowl)
 
 Robust Python **SDK** and **Command Line Client** for interacting with [IntelOwl](https://github.com/intelowlproject/IntelOwl)'s API.
 
 ## Features
 
 - Easy one-time configuration with self documented help and hints along the way.
```

### Comparing `pyintelowl-4.4.2/README.md` & `pyintelowl-4.4.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # PyIntelOwl
 
 [![PyPI version](https://badge.fury.io/py/pyintelowl.svg)](https://badge.fury.io/py/pyintelowl)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/pyintelowl.svg)](https://pypi.python.org/pypi/pyintelowl/)
 
 [![Pull request automation](https://github.com/intelowlproject/pyintelowl/actions/workflows/pull_request_automation.yml/badge.svg)](https://github.com/intelowlproject/pyintelowl/actions/workflows/pull_request_automation.yml)
 [![codecov](https://codecov.io/gh/intelowlproject/pyintelowl/branch/master/graph/badge.svg?token=JF62UMZ0U6)](https://codecov.io/gh/intelowlproject/pyintelowl)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/intelowlproject/pyintelowl.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mlodic/pyintelowl/context:python)
 [![CodeFactor](https://www.codefactor.io/repository/github/intelowlproject/pyintelowl/badge)](https://www.codefactor.io/repository/github/intelowlproject/pyintelowl)
 
 Robust Python **SDK** and **Command Line Client** for interacting with [IntelOwl](https://github.com/intelowlproject/IntelOwl)'s API.
 
 ## Features
 
 - Easy one-time configuration with self documented help and hints along the way.
```

### Comparing `pyintelowl-4.4.2/docs/conf.py` & `pyintelowl-4.4.3/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import os
 import sys
 
-VERSION = "4.4.2"
+VERSION = "4.4.3"
 GITHUB_URL = "https://github.com/intelowlproject/pyintelowl"
 
 sys.path.append(os.path.abspath("../"))
 
 
 # -- Project information -----------------------------------------------------
```

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/_jobs_utils.py` & `pyintelowl-4.4.3/pyintelowl/cli/_jobs_utils.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/_utils.py` & `pyintelowl-4.4.3/pyintelowl/cli/_utils.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/analyse.py` & `pyintelowl-4.4.3/pyintelowl/cli/analyse.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/commands.py` & `pyintelowl-4.4.3/pyintelowl/cli/commands.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/config.py` & `pyintelowl-4.4.3/pyintelowl/cli/config.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/domain_checkers.py` & `pyintelowl-4.4.3/pyintelowl/cli/domain_checkers.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/jobs.py` & `pyintelowl-4.4.3/pyintelowl/cli/jobs.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/cli/tags.py` & `pyintelowl-4.4.3/pyintelowl/cli/tags.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/exceptions.py` & `pyintelowl-4.4.3/pyintelowl/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/main.py` & `pyintelowl-4.4.3/pyintelowl/main.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl/pyintelowl.py` & `pyintelowl-4.4.3/pyintelowl/pyintelowl.py`

 * *Files 1% similar despite different names*

```diff
@@ -500,26 +500,31 @@
             if playbook_mode:
                 # right now, we are only supporting single input result
                 answers = answer.get("results", [])
                 if answers:
                     answer = answers[0]
 
             warnings = answer.get("warnings", [])
+            errors = answer.get("errors", {})
             if self.cli:
                 info_log = f"""New Job running..
                     ID: {answer['job_id']} | Status: [u blue]{answer['status']}[/].
                     Got {len(warnings)} warnings:
                     [i yellow]{warnings if warnings else None}[/]
+                    Got {len(errors)} errors:
+                    [i red]{errors if errors else None}[/]
                 """
             else:
                 info_log = (
                     f"New Job running.. ID: {answer['job_id']} "
                     f"| Status: {answer['status']}."
                     f" Got {len(warnings)} warnings:"
                     f" {warnings if warnings else None}"
+                    f" Got {len(errors)} errors:"
+                    f" {errors if errors else None}"
                 )
             self.logger.info(info_log)
             response.raise_for_status()
         except Exception as e:
             raise IntelOwlClientException(e, response=response)
         return answer
```

### Comparing `pyintelowl-4.4.2/pyintelowl.egg-info/PKG-INFO` & `pyintelowl-4.4.3/pyintelowl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,39 @@
 Metadata-Version: 2.1
 Name: pyintelowl
-Version: 4.4.2
+Version: 4.4.3
 Summary: Robust Python SDK and CLI for IntelOwl's API
 Home-page: https://github.com/intelowlproject/pyintelowl
 Author: Matteo Lodi
 Project-URL: Documentation, https://github.com/intelowlproject/pyintelowl
 Project-URL: Funding, https://liberapay.com/IntelOwlProject/
 Project-URL: Source, https://github.com/intelowlproject/pyintelowl
 Project-URL: Tracker, https://github.com/intelowlproject/pyintelowl/issues
 Keywords: intelowl sdk python command line osint threat intel malware
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE
 
 # PyIntelOwl
 
 [![PyPI version](https://badge.fury.io/py/pyintelowl.svg)](https://badge.fury.io/py/pyintelowl)
 [![PyPI Supported Python Versions](https://img.shields.io/pypi/pyversions/pyintelowl.svg)](https://pypi.python.org/pypi/pyintelowl/)
 
 [![Pull request automation](https://github.com/intelowlproject/pyintelowl/actions/workflows/pull_request_automation.yml/badge.svg)](https://github.com/intelowlproject/pyintelowl/actions/workflows/pull_request_automation.yml)
 [![codecov](https://codecov.io/gh/intelowlproject/pyintelowl/branch/master/graph/badge.svg?token=JF62UMZ0U6)](https://codecov.io/gh/intelowlproject/pyintelowl)
-[![Language grade: Python](https://img.shields.io/lgtm/grade/python/g/intelowlproject/pyintelowl.svg?logo=lgtm&logoWidth=18)](https://lgtm.com/projects/g/mlodic/pyintelowl/context:python)
 [![CodeFactor](https://www.codefactor.io/repository/github/intelowlproject/pyintelowl/badge)](https://www.codefactor.io/repository/github/intelowlproject/pyintelowl)
 
 Robust Python **SDK** and **Command Line Client** for interacting with [IntelOwl](https://github.com/intelowlproject/IntelOwl)'s API.
 
 ## Features
 
 - Easy one-time configuration with self documented help and hints along the way.
```

### Comparing `pyintelowl-4.4.2/pyintelowl.egg-info/SOURCES.txt` & `pyintelowl-4.4.3/pyintelowl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/pyintelowl.egg-info/requires.txt` & `pyintelowl-4.4.3/pyintelowl.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 [dev]
 black==22.3.0
 flake8==4.0.1
 isort==5.10.1
 pre-commit==2.17.0
 tox==3.25.1
 tox-gh-actions==2.9.1
-codecov==2.1.12
+codecov==2.1.13
 requests>=2.28
 geocoder>=1.38
 click>=7.0
 rich>=12.5.1
 click-creds>=0.0.3
 typing_extensions>=4.3.0
 
 [test]
 black==22.3.0
 flake8==4.0.1
 isort==5.10.1
 pre-commit==2.17.0
 tox==3.25.1
 tox-gh-actions==2.9.1
-codecov==2.1.12
+codecov==2.1.13
 requests>=2.28
 geocoder>=1.38
 click>=7.0
 rich>=12.5.1
 click-creds>=0.0.3
 typing_extensions>=4.3.0
```

### Comparing `pyintelowl-4.4.2/setup.py` & `pyintelowl-4.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,21 +40,21 @@
         #   5 - Production/Stable
         "Development Status :: 5 - Production/Stable",
         # Indicate who your project is intended for
         "Intended Audience :: Developers",
         "Environment :: Web Environment",
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     packages=find_packages(),
-    python_requires=">=3.7",
+    python_requires=">=3.8",
     include_package_data=True,
     install_requires=requirements,
     project_urls={
         "Documentation": GITHUB_URL,
         "Funding": "https://liberapay.com/IntelOwlProject/",
         "Source": GITHUB_URL,
         "Tracker": "{}/issues".format(GITHUB_URL),
```

### Comparing `pyintelowl-4.4.2/tests/mocked_requests.py` & `pyintelowl-4.4.3/tests/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/tests/test_general.py` & `pyintelowl-4.4.3/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/tests/test_jobs.py` & `pyintelowl-4.4.3/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/tests/test_tags.py` & `pyintelowl-4.4.3/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `pyintelowl-4.4.2/tests/utils.py` & `pyintelowl-4.4.3/tests/utils.py`

 * *Files identical despite different names*

