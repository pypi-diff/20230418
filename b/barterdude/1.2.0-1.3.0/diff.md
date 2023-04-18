# Comparing `tmp/barterdude-1.2.0.tar.gz` & `tmp/barterdude-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/BarterDude/BarterDude/dist/tmp52du30by/barterdude-1.2.0.tar", last modified: Thu Aug 18 17:32:09 2022, max compression
+gzip compressed data, was "barterdude-1.3.0.tar", last modified: Tue Apr 18 17:16:54 2023, max compression
```

## Comparing `barterdude-1.2.0.tar` & `barterdude-1.3.0.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-18 17:31:43.000000 barterdude-1.2.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-08-18 17:31:43.000000 barterdude-1.2.0/.coveralls.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1014 2022-08-18 17:31:43.000000 barterdude-1.2.0/.github/workflows/blackbox-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2063 2022-08-18 17:31:43.000000 barterdude-1.2.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1828 2022-08-18 17:31:43.000000 barterdude-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-08-18 17:31:43.000000 barterdude-1.2.0/.tool-versions
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-08-18 17:31:43.000000 barterdude-1.2.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-08-18 17:31:43.000000 barterdude-1.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     5119 2022-08-18 17:31:43.000000 barterdude-1.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-08-18 17:31:43.000000 barterdude-1.2.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-08-18 17:31:43.000000 barterdude-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-08-18 17:31:43.000000 barterdude-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      627 2022-08-18 17:31:43.000000 barterdude-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    13022 2022-08-18 17:32:09.000000 barterdude-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    12393 2022-08-18 17:31:43.000000 barterdude-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/barterdude/
--rw-r--r--   0 runner    (1001) docker     (121)     5356 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      768 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/barterdude/hooks/
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3449 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     2208 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/barterdude/hooks/metrics/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/barterdude/hooks/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2790 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/metrics/prometheus/definitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1265 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/hooks/metrics/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1928 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/message.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2012 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/barterdude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13022 2022-08-18 17:32:08.000000 barterdude-1.2.0/barterdude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1359 2022-08-18 17:32:09.000000 barterdude-1.2.0/barterdude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-18 17:32:08.000000 barterdude-1.2.0/barterdude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-08-18 17:32:08.000000 barterdude-1.2.0/barterdude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-08-18 17:32:08.000000 barterdude-1.2.0/barterdude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6906 2022-08-18 17:31:43.000000 barterdude-1.2.0/barterdude.jpg
--rw-r--r--   0 runner    (1001) docker     (121)      310 2022-08-18 17:31:43.000000 barterdude-1.2.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-18 17:32:09.000000 barterdude-1.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       80 2022-08-18 17:31:43.000000 barterdude-1.2.0/requirements/requirements_base.txt
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-08-18 17:31:43.000000 barterdude-1.2.0/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-18 17:32:09.000000 barterdude-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1300 2022-08-18 17:31:43.000000 barterdude-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.767003 barterdude-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 17:16:33.000000 barterdude-1.3.0/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 17:16:33.000000 barterdude-1.3.0/.coveralls.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-18 17:16:33.000000 barterdude-1.3.0/.github/workflows/blackbox-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-18 17:16:33.000000 barterdude-1.3.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 17:16:33.000000 barterdude-1.3.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-18 17:16:33.000000 barterdude-1.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:16:33.000000 barterdude-1.3.0/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 17:16:33.000000 barterdude-1.3.0/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-18 17:16:33.000000 barterdude-1.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-18 17:16:33.000000 barterdude-1.3.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 17:16:33.000000 barterdude-1.3.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 17:16:33.000000 barterdude-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 17:16:33.000000 barterdude-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 17:16:33.000000 barterdude-1.3.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-18 17:16:54.767003 barterdude-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-18 17:16:33.000000 barterdude-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/hooks/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.767003 barterdude-1.3.0/barterdude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 17:16:33.000000 barterdude-1.3.0/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 17:16:33.000000 barterdude-1.3.0/requirements/requirements_base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 17:16:33.000000 barterdude-1.3.0/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 17:16:54.767003 barterdude-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-18 17:16:33.000000 barterdude-1.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `barterdude-1.2.0/.github/workflows/blackbox-workflow.yml` & `barterdude-1.3.0/.github/workflows/blackbox-workflow.yml`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/.github/workflows/main.yml` & `barterdude-1.3.0/.github/workflows/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
         ports:
           - 5672:5672
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
 
-      - name: Setup python 3.7
+      - name: Setup python 3.11
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: 3.11
 
       - name: Install project dependencies
         run: make setup
 
       - name: Run security check
         run: make check-sec
 
@@ -38,18 +38,18 @@
     runs-on: ubuntu-latest
     environment: 'dev'
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
 
-      - name: Setup python 3.7
+      - name: Setup python 3.11
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: 3.11
 
       - name: Install project dependencies
         run: make install && python3 -m pip install build
 
       - name: Build package
         run: python3 -m build -s
 
@@ -66,18 +66,18 @@
     runs-on: ubuntu-latest
     environment: 'prod'
 
     steps:
       - name: Checkout repository
         uses: actions/checkout@v2
 
-      - name: Setup python 3.7
+      - name: Setup python 3.11
         uses: actions/setup-python@v2
         with:
-          python-version: 3.7
+          python-version: 3.11
 
       - name: Install project dependencies
         run: make install && python3 -m pip install build
 
       - name: Build package
         run: python3 -m build -s
```

### Comparing `barterdude-1.2.0/.gitignore` & `barterdude-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/.travis.yml` & `barterdude-1.3.0/.travis.yml`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/CODE_OF_CONDUCT.md` & `barterdude-1.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/CONTRIBUTING.md` & `barterdude-1.3.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/LICENSE` & `barterdude-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/Makefile` & `barterdude-1.3.0/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 lint:
 	@flake8 barterdude tests_unit tests_integration
 
 test:
 	@pytest --ignore="tests_integration" --cov=barterdude
 
 integration:
-	@pytest --ignore="tests_unit"
+	@pytest --ignore="tests_unit" -vv
 
 all-tests: | test integration lint check-sec
 
 all-tests-container:
 	@docker-compose run --rm barterdude make all-tests
 
 check-sec:
```

### Comparing `barterdude-1.2.0/PKG-INFO` & `barterdude-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: barterdude
-Version: 1.2.0
+Version: 1.3.0
 Summary: Message exchange engine to build pipelines using brokers like RabbitMQ
 Home-page: https://github.com/olxbr/BarterDude/
 Download-URL: https://github.com/olxbr/BarterDude/archive/master.zip
 Author: Olx
 License: Apache 2
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
@@ -361,15 +363,14 @@
 ### Side-effects
 
 If your callback has services with side-effects such as inserting a row in a database or updating an API, you can pass fake instances of these services that are going to be injected to prevent side-effects from happenning.
 
 ```python
 barterdude.add_callback_endpoint(
     routes=["/execute"],
-    methods=["POST"],
     hook=execute,
     mock_dependencies=[
         (
             fake_database_service,  # fake service instance to be used by the worker
             "database_service",     # name used in the data sharing/dependency injection
         ),
     ]
```

### Comparing `barterdude-1.2.0/README.md` & `barterdude-1.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -345,15 +345,14 @@
 ### Side-effects
 
 If your callback has services with side-effects such as inserting a row in a database or updating an API, you can pass fake instances of these services that are going to be injected to prevent side-effects from happenning.
 
 ```python
 barterdude.add_callback_endpoint(
     routes=["/execute"],
-    methods=["POST"],
     hook=execute,
     mock_dependencies=[
         (
             fake_database_service,  # fake service instance to be used by the worker
             "database_service",     # name used in the data sharing/dependency injection
         ),
     ]
```

### Comparing `barterdude-1.2.0/barterdude/__init__.py` & `barterdude-1.3.0/barterdude/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import traceback
 from aiohttp import web
 from asyncio import gather
 from asyncworker import App, RouteTypes
 from asyncworker.options import Options
 from asyncworker.connections import AMQPConnection
 from asyncworker.rabbitmq.message import RabbitMQMessage
-from collections import MutableMapping
+from collections.abc import MutableMapping
 from typing import Iterable, Optional, Callable, Any, Tuple
 from barterdude.monitor import Monitor
 from barterdude.message import MessageValidation, ValidationException
 from barterdude.mocks import RabbitMQMessageMock, BarterdudeMock
 
 
 class BarterDude(MutableMapping):
```

### Comparing `barterdude-1.2.0/barterdude/conf.py` & `barterdude-1.3.0/barterdude/conf.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/hooks/__init__.py` & `barterdude-1.3.0/barterdude/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/hooks/healthcheck.py` & `barterdude-1.3.0/barterdude/hooks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/hooks/logging.py` & `barterdude-1.3.0/barterdude/hooks/logging.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/hooks/metrics/prometheus/__init__.py` & `barterdude-1.3.0/barterdude/hooks/metrics/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/hooks/metrics/prometheus/definitions.py` & `barterdude-1.3.0/barterdude/hooks/metrics/prometheus/definitions.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/hooks/metrics/prometheus/metrics.py` & `barterdude-1.3.0/barterdude/hooks/metrics/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/message.py` & `barterdude-1.3.0/barterdude/message.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude/mocks.py` & `barterdude-1.3.0/barterdude/mocks.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import asyncio
 from typing import Dict, Any, Iterable, Tuple
-from collections import MutableMapping
+from collections.abc import MutableMapping
 from aioamqp.properties import Properties
 
 
 class ObjectWithCallsTracking:
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
```

### Comparing `barterdude-1.2.0/barterdude/monitor.py` & `barterdude-1.3.0/barterdude/monitor.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/barterdude.egg-info/PKG-INFO` & `barterdude-1.3.0/barterdude.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Metadata-Version: 2.1
 Name: barterdude
-Version: 1.2.0
+Version: 1.3.0
 Summary: Message exchange engine to build pipelines using brokers like RabbitMQ
 Home-page: https://github.com/olxbr/BarterDude/
 Download-URL: https://github.com/olxbr/BarterDude/archive/master.zip
 Author: Olx
 License: Apache 2
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Description-Content-Type: text/markdown
 Provides-Extra: all
 License-File: LICENSE
 
@@ -361,15 +363,14 @@
 ### Side-effects
 
 If your callback has services with side-effects such as inserting a row in a database or updating an API, you can pass fake instances of these services that are going to be injected to prevent side-effects from happenning.
 
 ```python
 barterdude.add_callback_endpoint(
     routes=["/execute"],
-    methods=["POST"],
     hook=execute,
     mock_dependencies=[
         (
             fake_database_service,  # fake service instance to be used by the worker
             "database_service",     # name used in the data sharing/dependency injection
         ),
     ]
```

### Comparing `barterdude-1.2.0/barterdude.egg-info/SOURCES.txt` & `barterdude-1.3.0/barterdude.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 ./barterdude/hooks/metrics/__init__.py
 ./barterdude/hooks/metrics/prometheus/__init__.py
 ./barterdude/hooks/metrics/prometheus/definitions.py
 ./barterdude/hooks/metrics/prometheus/metrics.py
 ./requirements/requirements_base.txt
 ./requirements/requirements_test.txt
 .github/workflows/blackbox-workflow.yml
+.github/workflows/codeql-analysis.yml
 .github/workflows/main.yml
 barterdude/__init__.py
 barterdude/conf.py
 barterdude/message.py
 barterdude/mocks.py
 barterdude/monitor.py
 barterdude.egg-info/PKG-INFO
```

### Comparing `barterdude-1.2.0/barterdude.jpg` & `barterdude-1.3.0/barterdude.jpg`

 * *Files identical despite different names*

### Comparing `barterdude-1.2.0/setup.py` & `barterdude-1.3.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,23 @@
 
 extra = {
     "all": [],
 
 }
 
 with open("requirements/requirements_base.txt") as reqs:
-    requirements = reqs.read().split("\n")
+    raw_requirements = reqs.read().split("\n")
+
+requirements = []
+for r in raw_requirements:
+    if r.startswith("git+"):
+        name = r.split(".git@")[0].split("/")[-1]
+        requirements.append(f"{name} @ {r}")
+    else:
+        requirements.append(r)
 
 for lib in libs:
     with open(f"requirements/requirements_{lib}.txt") as reqs:
         extra[lib] = reqs.read().split("\n")
         extra["all"] = extra["all"] + extra[lib]
 
 with open("README.md", "r") as fh:
@@ -29,14 +37,16 @@
     url='https://github.com/olxbr/BarterDude/',
     download_url='https://github.com/olxbr/BarterDude/archive/master.zip',
     use_scm_version=True,
     setup_requires=['setuptools_scm'],
     install_requires=requirements,
     extras_require=extra,
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: Apache Software License",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Software Development :: Libraries :: Application Frameworks"
     ],
     packages=find_packages()
 )
```

