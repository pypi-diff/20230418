# Comparing `tmp/barterdude-1.3.0.tar.gz` & `tmp/barterdude-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "barterdude-1.3.0.tar", last modified: Tue Apr 18 17:16:54 2023, max compression
+gzip compressed data, was "barterdude-1.3.1.tar", last modified: Tue Apr 18 21:08:55 2023, max compression
```

## Comparing `barterdude-1.3.0.tar` & `barterdude-1.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.767003 barterdude-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 17:16:33.000000 barterdude-1.3.0/.bandit
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 17:16:33.000000 barterdude-1.3.0/.coveralls.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-18 17:16:33.000000 barterdude-1.3.0/.github/workflows/blackbox-workflow.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-18 17:16:33.000000 barterdude-1.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 17:16:33.000000 barterdude-1.3.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-18 17:16:33.000000 barterdude-1.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 17:16:33.000000 barterdude-1.3.0/.tool-versions
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 17:16:33.000000 barterdude-1.3.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-18 17:16:33.000000 barterdude-1.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-18 17:16:33.000000 barterdude-1.3.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 17:16:33.000000 barterdude-1.3.0/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 17:16:33.000000 barterdude-1.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 17:16:33.000000 barterdude-1.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 17:16:33.000000 barterdude-1.3.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-18 17:16:54.767003 barterdude-1.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-18 17:16:33.000000 barterdude-1.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/
--rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/hooks/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/hooks/metrics/prometheus/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/mocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.767003 barterdude-1.3.0/barterdude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 17:16:54.000000 barterdude-1.3.0/barterdude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-18 17:16:33.000000 barterdude-1.3.0/barterdude.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 17:16:33.000000 barterdude-1.3.0/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:16:54.763003 barterdude-1.3.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-18 17:16:33.000000 barterdude-1.3.0/requirements/requirements_base.txt
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 17:16:33.000000 barterdude-1.3.0/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 17:16:54.767003 barterdude-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-18 17:16:33.000000 barterdude-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.208667 barterdude-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-18 21:08:32.000000 barterdude-1.3.1/.bandit
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 21:08:32.000000 barterdude-1.3.1/.coveralls.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.200667 barterdude-1.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.208667 barterdude-1.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-18 21:08:32.000000 barterdude-1.3.1/.github/workflows/blackbox-workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-04-18 21:08:32.000000 barterdude-1.3.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 21:08:32.000000 barterdude-1.3.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-18 21:08:32.000000 barterdude-1.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 21:08:32.000000 barterdude-1.3.1/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 21:08:32.000000 barterdude-1.3.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-18 21:08:32.000000 barterdude-1.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-04-18 21:08:32.000000 barterdude-1.3.1/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-18 21:08:32.000000 barterdude-1.3.1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 21:08:32.000000 barterdude-1.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 21:08:32.000000 barterdude-1.3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 21:08:32.000000 barterdude-1.3.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-18 21:08:55.208667 barterdude-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12371 2023-04-18 21:08:32.000000 barterdude-1.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.204667 barterdude-1.3.1/barterdude/
+-rw-r--r--   0 runner    (1001) docker     (123)     5360 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.204667 barterdude-1.3.1/barterdude/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.208667 barterdude-1.3.1/barterdude/hooks/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.208667 barterdude-1.3.1/barterdude/hooks/metrics/prometheus/
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/metrics/prometheus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/metrics/prometheus/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/hooks/metrics/prometheus/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2370 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.208667 barterdude-1.3.1/barterdude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13104 2023-04-18 21:08:55.000000 barterdude-1.3.1/barterdude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-04-18 21:08:55.000000 barterdude-1.3.1/barterdude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:08:55.000000 barterdude-1.3.1/barterdude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-18 21:08:55.000000 barterdude-1.3.1/barterdude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 21:08:55.000000 barterdude-1.3.1/barterdude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6906 2023-04-18 21:08:32.000000 barterdude-1.3.1/barterdude.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-18 21:08:32.000000 barterdude-1.3.1/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:08:55.208667 barterdude-1.3.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 21:08:32.000000 barterdude-1.3.1/requirements/requirements_base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-04-18 21:08:32.000000 barterdude-1.3.1/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-04-18 21:08:55.208667 barterdude-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-18 21:08:32.000000 barterdude-1.3.1/setup.py
```

### Comparing `barterdude-1.3.0/.github/workflows/blackbox-workflow.yml` & `barterdude-1.3.1/.github/workflows/blackbox-workflow.yml`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/.github/workflows/codeql-analysis.yml` & `barterdude-1.3.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/.github/workflows/main.yml` & `barterdude-1.3.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/.gitignore` & `barterdude-1.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/.travis.yml` & `barterdude-1.3.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/CODE_OF_CONDUCT.md` & `barterdude-1.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/CONTRIBUTING.md` & `barterdude-1.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/LICENSE` & `barterdude-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/Makefile` & `barterdude-1.3.1/Makefile`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/PKG-INFO` & `barterdude-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barterdude
-Version: 1.3.0
+Version: 1.3.1
 Summary: Message exchange engine to build pipelines using brokers like RabbitMQ
 Home-page: https://github.com/olxbr/BarterDude/
 Download-URL: https://github.com/olxbr/BarterDude/archive/master.zip
 Author: Olx
 License: Apache 2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `barterdude-1.3.0/README.md` & `barterdude-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/__init__.py` & `barterdude-1.3.1/barterdude/__init__.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/conf.py` & `barterdude-1.3.1/barterdude/conf.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/hooks/__init__.py` & `barterdude-1.3.1/barterdude/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/hooks/healthcheck.py` & `barterdude-1.3.1/barterdude/hooks/healthcheck.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/hooks/logging.py` & `barterdude-1.3.1/barterdude/hooks/logging.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/hooks/metrics/prometheus/__init__.py` & `barterdude-1.3.1/barterdude/hooks/metrics/prometheus/__init__.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/hooks/metrics/prometheus/definitions.py` & `barterdude-1.3.1/barterdude/hooks/metrics/prometheus/definitions.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/hooks/metrics/prometheus/metrics.py` & `barterdude-1.3.1/barterdude/hooks/metrics/prometheus/metrics.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/message.py` & `barterdude-1.3.1/barterdude/message.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/mocks.py` & `barterdude-1.3.1/barterdude/mocks.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude/monitor.py` & `barterdude-1.3.1/barterdude/monitor.py`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude.egg-info/PKG-INFO` & `barterdude-1.3.1/barterdude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: barterdude
-Version: 1.3.0
+Version: 1.3.1
 Summary: Message exchange engine to build pipelines using brokers like RabbitMQ
 Home-page: https://github.com/olxbr/BarterDude/
 Download-URL: https://github.com/olxbr/BarterDude/archive/master.zip
 Author: Olx
 License: Apache 2
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `barterdude-1.3.0/barterdude.egg-info/SOURCES.txt` & `barterdude-1.3.1/barterdude.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/barterdude.jpg` & `barterdude-1.3.1/barterdude.jpg`

 * *Files identical despite different names*

### Comparing `barterdude-1.3.0/setup.py` & `barterdude-1.3.1/setup.py`

 * *Files identical despite different names*

