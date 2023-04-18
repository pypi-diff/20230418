# Comparing `tmp/pytest_netdut-0.4.0.tar.gz` & `tmp/pytest_netdut-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_netdut-0.4.0.tar", last modified: Tue Apr 11 03:59:03 2023, max compression
+gzip compressed data, was "pytest_netdut-0.5.0.tar", last modified: Tue Apr 18 05:24:10 2023, max compression
```

## Comparing `pytest_netdut-0.4.0.tar` & `pytest_netdut-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.596732 pytest_netdut-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.600732 pytest_netdut-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.github/workflows/build.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.604733 pytest_netdut-0.4.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.596732 pytest_netdut-0.4.0/docs/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.604733 pytest_netdut-0.4.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/images/failed_assertion.png
--rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/images/test_showver_results.png
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.604733 pytest_netdut-0.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_eapi_ssh_x.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_showver.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_skip_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/examples/test_using_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.596732 pytest_netdut-0.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.608733 pytest_netdut-0.4.0/src/pytest_netdut/
--rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/factories.py
--rw-r--r--   0 runner    (1001) docker     (123)    18701 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/px.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/src/pytest_netdut/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.608733 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-11 03:59:03.000000 pytest_netdut-0.4.0/src/pytest_netdut.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 03:59:03.612733 pytest_netdut-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_netdut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_wait_for.py
--rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tests/test_xapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-11 03:58:49.000000 pytest_netdut-0.4.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.436221 pytest_netdut-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.428221 pytest_netdut-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.432221 pytest_netdut-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/.github/workflows/build.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-18 05:24:10.436221 pytest_netdut-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8303 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.432221 pytest_netdut-0.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.428221 pytest_netdut-0.5.0/docs/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.432221 pytest_netdut-0.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   114704 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/docs/images/failed_assertion.png
+-rw-r--r--   0 runner    (1001) docker     (123)    90069 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/docs/images/test_showver_results.png
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.432221 pytest_netdut-0.5.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/examples/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/examples/test_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/examples/test_eapi_ssh_x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/examples/test_showver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/examples/test_skip_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/examples/test_using_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-18 05:24:10.436221 pytest_netdut-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.428221 pytest_netdut-0.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.432221 pytest_netdut-0.5.0/src/pytest_netdut/
+-rw-r--r--   0 runner    (1001) docker     (123)     6165 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/src/pytest_netdut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/src/pytest_netdut/factories.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18293 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/src/pytest_netdut/px.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/src/pytest_netdut/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9400 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/src/pytest_netdut/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.432221 pytest_netdut-0.5.0/src/pytest_netdut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10683 2023-04-18 05:24:10.000000 pytest_netdut-0.5.0/src/pytest_netdut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-18 05:24:10.000000 pytest_netdut-0.5.0/src/pytest_netdut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 05:24:10.000000 pytest_netdut-0.5.0/src/pytest_netdut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-18 05:24:10.000000 pytest_netdut-0.5.0/src/pytest_netdut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 05:24:10.000000 pytest_netdut-0.5.0/src/pytest_netdut.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:24:10.436221 pytest_netdut-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/tests/test_netdut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/tests/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/tests/test_wait_for.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2013 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/tests/test_xapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-18 05:23:50.000000 pytest_netdut-0.5.0/tox.ini
```

### Comparing `pytest_netdut-0.4.0/.github/workflows/build.yaml` & `pytest_netdut-0.5.0/.github/workflows/build.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -6,50 +6,50 @@
   pull_request:
 
 jobs:
   test:
     runs-on: ubuntu-latest
     strategy:
       matrix:
-        python-version: ["3.7", "3.8", "3.9", "3.10"]
+        python-version: ["3.7", "3.8", "3.9", "3.10", "3.11"]
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install pytest tox
-      
+
       - name: Test using tox
         run: |
-          tox -s -e "py37,py38,py39,py310"
+          tox -s -e "py37,py38,py39,py310,py311"
 
 #      - name: Test Summary
 #        uses: test-summary/action@v1
 #        with:
 #          paths: |
 #            test-reports/*.xml
 #        if: always()
-  
+
   lint:
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v3
 
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
-          python-version: "3.10"
+          python-version: "3.11"
 
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
           pip install tox build twine
 
       - name: Lint
```

### Comparing `pytest_netdut-0.4.0/.github/workflows/release.yaml` & `pytest_netdut-0.5.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/.gitignore` & `pytest_netdut-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/Dockerfile` & `pytest_netdut-0.5.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/LICENSE` & `pytest_netdut-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/Makefile` & `pytest_netdut-0.5.0/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/PKG-INFO` & `pytest_netdut-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_netdut
-Version: 0.4.0
+Version: 0.5.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
```

### Comparing `pytest_netdut-0.4.0/README.md` & `pytest_netdut-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/docs/images/failed_assertion.png` & `pytest_netdut-0.5.0/docs/images/failed_assertion.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/docs/images/test_showver_results.png` & `pytest_netdut-0.5.0/docs/images/test_showver_results.png`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/examples/test_daemon.py` & `pytest_netdut-0.5.0/examples/test_daemon.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/examples/test_eapi_ssh_x.py` & `pytest_netdut-0.5.0/examples/test_eapi_ssh_x.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/examples/test_skip_demo.py` & `pytest_netdut-0.5.0/examples/test_skip_demo.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/mkdocs.yml` & `pytest_netdut-0.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/setup.cfg` & `pytest_netdut-0.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut/__init__.py` & `pytest_netdut-0.5.0/src/pytest_netdut/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,35 +66,36 @@
 `pytest-netdut` adds a command line option:
 
 * `--device` -- specifies the hostname for the device. Netdut expects to be able to connect via ssh
     to this hostname.
 
 """
 from typing import Callable
+import logging
 import pytest
 from . import factories
 from .utils import wait_for
 from .wrappers import CLI, EAPI, eapi_enabled_fixture, xapi
 
 __all__ = ["CLI", "EAPI", "create", "eapi_enabled_fixture", "wait_for", "xapi"]
 
+logger = logging.getLogger(__name__)
+
 
 def pytest_configure(config):
     """pytest_configure hook that adds markers used by netdut.
 
     Args:
         config (pytest.Config): The pytest config object.
     """
 
     # register markers
     config.addinivalue_line("markers", "eos: mark a test as eos only.")
     config.addinivalue_line("markers", "mos: mark a test as mos only.")
-    config.addinivalue_line(
-        "markers", "skip_device_type: mark a test as excluding a particular SKU regex."
-    )
+    config.addinivalue_line("markers", "skip_device_type: mark a test as excluding a particular SKU regex.")
     config.addinivalue_line(
         "markers",
         "only_device_type: mark a test as only running on a particular SKU regex.",
     )
 
     # FIXME: not really part of netdut
     config.addinivalue_line("markers", "slow: slower than usual tests.")
@@ -144,15 +145,15 @@
         factories.create_sku_fixture(name),
         factories.create_softened_fixture(name),
         factories.create_ssh_fixture(name),
         factories.create_xapi_fixture(name),
     ]
 
     for fixture in fixtures:
-        globals()[fixture.__name__] = fixture
+        globals()[fixture._pytestfixturefunction.name] = fixture
 
     return fixtures[0]
 
 
 @pytest.fixture(scope="session")
 def dut_info(pytestconfig) -> dict:
     """A fixture providing the DUT configuration passed via config to pytest-netdut.
@@ -167,8 +168,9 @@
         "hostname": pytestconfig.getoption("dut_hostname"),
         "console_url": pytestconfig.getoption("dut_console_url"),
     }
     assert info["console_url"] or info["hostname"], "You must specify a device"
     return info
 
 
+logger.debug("Registering `dut`")
 create("dut")
```

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut/factories.py` & `pytest_netdut-0.5.0/src/pytest_netdut/factories.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,17 +15,19 @@
 # -
 # -------------------------------------------------------------------------------
 import logging
 import re
 import pytest
 from .wrappers import CLI, xapi
 
+logger = logging.getLogger(__name__)
+
 
 def create_dut_fixture(name):
-    @pytest.fixture(scope="session", name=f"{name}")
+    @pytest.fixture(name=f"{name}")
     def _dut(request):
         skipper = request.getfixturevalue(f"{name}_skipper")
         skipper(request.node)
 
         class Dut:
             def __getattr__(self, attr):
                 return request.getfixturevalue(f"{name}_{attr}")
@@ -73,17 +75,15 @@
                 if marker.name in {"mos", "eos"}:
                     allowed_os.add(marker.name)
 
                 elif marker.name == "only_device_type":
                     pattern = marker.args[0]
                     sku = request.getfixturevalue(f"{name}_sku")
                     if not re.search(pattern, sku):
-                        pytest.skip(
-                            f"Skipped on this SKU: {sku} (only runs on {pattern})"
-                        )
+                        pytest.skip(f"Skipped on this SKU: {sku} (only runs on {pattern})")
 
                 elif marker.name == "skip_device_type":
                     pattern = marker.args[0]
                     sku = request.getfixturevalue(f"{name}_sku")
                     if re.search(pattern, sku):
                         pytest.skip(f"Skipped on this SKU: {sku}")
```

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut/px.py` & `pytest_netdut-0.5.0/src/pytest_netdut/px.py`

 * *Files 7% similar despite different names*

```diff
@@ -54,29 +54,25 @@
         r")"
     )
     _prompt_regex = re.compile(_control_code_re + _hostname_re + _mode_and_path_re)
 
     def syncprompt(self):
         self.expect(self._prompt_regex)
         # Use captured serial number / hostname for finding the prompt
-        self._prompt = re.compile(
-            self._control_code_re + self.match.group(1) + self._mode_and_path_re
-        )
+        self._prompt = re.compile(self._control_code_re + self.match.group(1) + self._mode_and_path_re)
 
     def prompt(self, timeout=-1, reset=0):
         if reset:
             self.syncprompt()
         else:
             self.expect(self._prompt, timeout)
         return self.before.replace("\r\n", "\n")
 
     def sendcmd(self, cmd="", timeout=-1, reset=0, wait=True):
-        if not isinstance(self.after, six.string_types) or not self._prompt.match(
-            self.after
-        ):
+        if not isinstance(self.after, six.string_types) or not self._prompt.match(self.after):
             raise RuntimeError(
                 "Cannot find prompt. Refusing to send command.",
                 self.after,
                 self._prompt.pattern,
             )
 
         self.sendcmd_unchecked(cmd)
@@ -100,17 +96,15 @@
         self.sendline(cmd)
 
         try:
             self.expect(re.escape(cmd), timeout=10)
         except TIMEOUT:
             # This deals with long commands on the serial console
             if not cmd.startswith(
-                self.before[  # pylint: disable=unsubscriptable-object
-                    : self.before.index("\r")
-                ].strip()
+                self.before[: self.before.index("\r")].strip()  # pylint: disable=unsubscriptable-object
             ):
                 raise
 
         # This deals with disappearing newlines on tty
         try:
             self.expect("\r\n", timeout=10)
         except TIMEOUT:
@@ -250,17 +244,15 @@
         # Sendcmd via Shell directly to avoid messing with cli_timeouts
         # since we do not yet know for sure what OS the device is running.
         show_version = self.sendcmd_simple("show version", timeout=10)
         matcher = re.search("Serial number:[ \t]*(.*)", show_version)
         if matcher:
             self.serial = matcher.group(1)
 
-        matcher = re.search(
-            r"System management controller version: (\d+)", show_version
-        )
+        matcher = re.search(r"System management controller version: (\d+)", show_version)
         if matcher:
             self.micro_version = matcher.group(1)
 
         # More reliably determine the CLI flavor
         # MOS does not have a 'Hardware version' field in "show version'
         matcher = re.search("Hardware version:", show_version)
         if matcher:
@@ -273,17 +265,15 @@
             self.sendcmd_simple("enable")
         except TIMEOUT:
             self.expect("Password:", timeout=10)
             self.sendline("opensesame")  # This is used in some tests.
             output = self.prompt(timeout=timeout, reset=1)
             self.process_output(output)
 
-        self.sendcmd_simple(
-            "bash echo ===> px Determined the {} CLI flavor".format(self.cli_flavor)
-        )
+        self.sendcmd_simple("bash echo ===> px Determined the {} CLI flavor".format(self.cli_flavor))
 
         if self.cli_flavor == "mos":
             self.sendcmd_simple("set debug 1", timeout=10)
 
             # Set default cli timeout which
             # is the 2x the command timeout
             if self.enable_cli_timeout:
@@ -297,17 +287,15 @@
                 plm_ver = self.sendcmd("bash i2cget -f -y 1 0x77 0x8 w").strip()
                 self.device_generation = 1 if int(plm_ver, 16) < 0x200 else 2
 
             # If Gen2 device, determine PLM watchdog support by
             # querying register PLM_VER_PATCH(0x7e)
             try:
                 if self.device_generation == 2:
-                    plm_ver_patch = self.sendcmd(
-                        "bash i2cget -f -y 1 0x77 0x7e b"
-                    ).strip()
+                    plm_ver_patch = self.sendcmd("bash i2cget -f -y 1 0x77 0x7e b").strip()
                     self.plm_wd_supported = plm_ver_patch != "0xdb"
             except Exception:  # pylint: disable=broad-except
                 pass
 
         self.sendcmd("show clock", timeout=timeout)
 
     def login(self, timeout=30):  # noqa: MC0001
@@ -316,48 +304,40 @@
 
         print("\n -- Logged in. Sending password, etc. -- \n")
 
         if self.cli_flavor != "aboot":
             # This should also handle the case where a password prompt is presented
             # because a TACACS server has been configured even though there is no
             # password actually configured for the user.
-            index = self.expect(
-                [TIMEOUT, "Last login:.*\r\n", "Password:", "Aboot#"], timeout=10
-            )
+            index = self.expect([TIMEOUT, "Last login:.*\r\n", "Password:", "Aboot#"], timeout=10)
             if index == 2:
                 self.sendline(self.password)
 
         print("\n -- Waiting for prompt -- \n")
 
         try:
             self.prompt(reset=1)
         except TIMEOUT:
             # Check if the CLI is busted or if previous tests left a password set
             try:
-                index = self.expect(
-                    ["Traceback", "Login incorrect", "Password:"], timeout=10
-                )
+                index = self.expect(["Traceback", "Login incorrect", "Password:"], timeout=10)
                 if index == 0:
-                    raise RuntimeError(  # pylint: disable=raise-missing-from
-                        "CLI is busted, try logging in as root!"
-                    )
+                    raise RuntimeError("CLI is busted, try logging in as root!")  # pylint: disable=raise-missing-from
                 if index == 1:
                     self.expect("login:", timeout=2)
                     self.sendline(self.username)
                     self.expect(self.username + "(\r)?\r\n", timeout=10)
                     self.expect("Password:", timeout=10)
                     self.sendline("opensesame")  # This is used in some tests.
                     self.expect("Last login:.*\r\n", timeout=10)
                 elif index == 2:
                     self.sendline("opensesame")  # This is used in some tests.
                     self.expect("Last login:.*\r\n", timeout=10)
                 self.expect("Traceback", timeout=10)
-                raise RuntimeError(  # pylint: disable=raise-missing-from
-                    "CLI is busted, try logging in as root!"
-                )
+                raise RuntimeError("CLI is busted, try logging in as root!")  # pylint: disable=raise-missing-from
             except TIMEOUT:
                 self.prompt(reset=1)
 
         # Sometime there are weird control characters printed as "^[[0n"
         # on the first line that escape the control code filtering.
         # Resync just in case.
         self.sendline()
@@ -486,17 +466,15 @@
             error.output = output
             raise error
         return output
 
 
 class FlakyTimeoutError(Exception):
     def __init__(self, cmd, timeout, actual_time):
-        super(FlakyTimeoutError, self).__init__(  # pylint: disable=super-with-arguments
-            cmd, timeout, actual_time
-        )
+        super(FlakyTimeoutError, self).__init__(cmd, timeout, actual_time)  # pylint: disable=super-with-arguments
         self.cmd = cmd
         self.timeout = timeout
         self.actual_time = actual_time
 
     def __repr__(self):
         return "{}(cmd={!r}, timeout={!r}, actual_time={!r})".format(
             self.__class__.__name__, self.cmd, self.timeout, self.actual_time
@@ -504,32 +482,26 @@
 
     def __str__(self):
         return self.__repr__()
 
 
 class CommandTimeoutError(FlakyTimeoutError):
     def __repr__(self):
-        return (
-            "{}: "
-            "command {!r} took longer than expected "
-            "(actual time {!r}s, expected time {!r}s)"
-        ).format(self.__class__.__name__, self.cmd, self.actual_time, self.timeout)
+        return ("{}: " "command {!r} took longer than expected " "(actual time {!r}s, expected time {!r}s)").format(
+            self.__class__.__name__, self.cmd, self.actual_time, self.timeout
+        )
 
 
 class PromptTimeoutError(FlakyTimeoutError):
     def __repr__(self):
-        return (
-            "{}: command {!r} didn't finish after {!r}s (expected time {!r}s)".format(
-                self.__class__.__name__, self.cmd, self.actual_time, self.timeout
-            )
+        return "{}: command {!r} didn't finish after {!r}s (expected time {!r}s)".format(
+            self.__class__.__name__, self.cmd, self.actual_time, self.timeout
         )
 
 
-def run(  # pylint: disable=keyword-arg-before-vararg
-    command, quiet=False, *args, **kwargs
-):
+def run(command, quiet=False, *args, **kwargs):  # pylint: disable=keyword-arg-before-vararg
     output, status = pexpect.run(command, withexitstatus=1, *args, **kwargs)
     if status != 0:
         if not quiet:
             print(output)
         raise subprocess.CalledProcessError(status, command)
     return output
```

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut/utils.py` & `pytest_netdut-0.5.0/src/pytest_netdut/utils.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut/wrappers.py` & `pytest_netdut-0.5.0/src/pytest_netdut/wrappers.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut.egg-info/PKG-INFO` & `pytest_netdut-0.5.0/src/pytest_netdut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-netdut
-Version: 0.4.0
+Version: 0.5.0
 Summary: "Automated software testing for switches using pytest"
 Home-page: https://github.com/aristanetworks/pytest-netdut
 Author: "David Snowdon"
 Author-email: "daves@arista.com"
 Maintainer: "Alex Webster"
 Maintainer-email: "alexw@arista.com"
 License: "BSD 3-Clause License"
```

### Comparing `pytest_netdut-0.4.0/src/pytest_netdut.egg-info/SOURCES.txt` & `pytest_netdut-0.5.0/src/pytest_netdut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/tests/conftest.py` & `pytest_netdut-0.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/tests/test_netdut.py` & `pytest_netdut-0.5.0/tests/test_netdut.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/tests/test_translator.py` & `pytest_netdut-0.5.0/tests/test_translator.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/tests/test_wait_for.py` & `pytest_netdut-0.5.0/tests/test_wait_for.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/tests/test_xapi.py` & `pytest_netdut-0.5.0/tests/test_xapi.py`

 * *Files identical despite different names*

### Comparing `pytest_netdut-0.4.0/tox.ini` & `pytest_netdut-0.5.0/tox.ini`

 * *Files identical despite different names*

