# Comparing `tmp/especifico-3.0.8.tar.gz` & `tmp/especifico-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "especifico-3.0.8.tar", last modified: Mon Apr  4 18:09:21 2022, max compression
+gzip compressed data, was "especifico-3.0.9.tar", last modified: Mon Apr  4 18:14:08 2022, max compression
```

## Comparing `especifico-3.0.8.tar` & `especifico-3.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-04-04 18:09:19.000000 especifico-3.0.8/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      544 2022-04-04 18:09:19.000000 especifico-3.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-04-04 18:09:19.000000 especifico-3.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-04 18:09:19.000000 especifico-3.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    22893 2022-04-04 18:09:21.215833 especifico-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    21841 2022-04-04 18:09:19.000000 especifico-3.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/
--rwxr-xr-x   0 runner    (1001) docker     (121)     1863 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/apis/
--rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18943 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apis/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)    15823 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apis/aiohttp_api.py
--rw-r--r--   0 runner    (1001) docker     (121)    13314 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apis/flask_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apis/flask_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/apps/
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apps/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apps/aiohttp_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/apps/flask_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/decorators/
--rw-r--r--   0 runner    (1001) docker     (121)       99 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/coroutine_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/decorator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/metrics.py
--rw-r--r--   0 runner    (1001) docker     (121)     4385 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/parameter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/produces.py
--rw-r--r--   0 runner    (1001) docker     (121)     5099 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/response.py
--rw-r--r--   0 runner    (1001) docker     (121)    11810 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/uri_parsing.py
--rw-r--r--   0 runner    (1001) docker     (121)    15695 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/decorators/validation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/handlers.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/http_facts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/jsonifier.py
--rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/mock.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/operations/
--rw-r--r--   0 runner    (1001) docker     (121)      685 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15979 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/operations/abstract.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/operations/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    15799 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/operations/openapi.py
--rw-r--r--   0 runner    (1001) docker     (121)     8681 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/operations/secure.py
--rw-r--r--   0 runner    (1001) docker     (121)    12724 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/operations/swagger2.py
--rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/problem.py
--rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.211833 especifico-3.0.8/especifico/resources/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.211833 especifico-3.0.8/especifico/resources/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/resources/schemas/v2.0/
--rw-r--r--   0 runner    (1001) docker     (121)    40020 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/resources/schemas/v2.0/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/resources/schemas/v3.0/
--rw-r--r--   0 runner    (1001) docker     (121)    35456 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/resources/schemas/v3.0/schema.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico/security/
--rw-r--r--   0 runner    (1001) docker     (121)      776 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/security/aiohttp_security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/security/async_security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/security/flask_security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    15601 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/security/security_handler_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)     9157 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-04-04 18:09:19.000000 especifico-3.0.8/especifico/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:09:21.215833 especifico-3.0.8/especifico.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    22893 2022-04-04 18:09:21.000000 especifico-3.0.8/especifico.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-04-04 18:09:21.000000 especifico-3.0.8/especifico.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 18:09:21.000000 especifico-3.0.8/especifico.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-04 18:09:21.000000 especifico-3.0.8/especifico.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-04-04 18:09:21.000000 especifico-3.0.8/especifico.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-04 18:09:21.000000 especifico-3.0.8/especifico.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-04 18:09:19.000000 especifico-3.0.8/requirements-lint.txt
--rw-r--r--   0 runner    (1001) docker     (121)      114 2022-04-04 18:09:19.000000 especifico-3.0.8/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-04-04 18:09:19.000000 especifico-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      141 2022-04-04 18:09:21.219833 especifico-3.0.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     2634 2022-04-04 18:09:19.000000 especifico-3.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.363102 especifico-3.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-04-04 18:14:05.000000 especifico-3.0.9/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      544 2022-04-04 18:14:05.000000 especifico-3.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-04-04 18:14:05.000000 especifico-3.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-04-04 18:14:05.000000 especifico-3.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    22893 2022-04-04 18:14:08.363102 especifico-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    21841 2022-04-04 18:14:05.000000 especifico-3.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.355102 especifico-3.0.9/especifico/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1863 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      146 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.359102 especifico-3.0.9/especifico/apis/
+-rw-r--r--   0 runner    (1001) docker     (121)      742 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18943 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apis/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15823 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apis/aiohttp_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13314 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apis/flask_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apis/flask_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.359102 especifico-3.0.9/especifico/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)      253 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10892 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apps/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3206 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apps/aiohttp_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6705 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/apps/flask_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6864 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.359102 especifico-3.0.9/especifico/decorators/
+-rw-r--r--   0 runner    (1001) docker     (121)       99 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/coroutine_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2277 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1776 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4385 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1255 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/produces.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5099 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/response.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11810 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/uri_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15695 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/decorators/validation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4932 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2742 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/http_facts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5338 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2080 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/jsonifier.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1891 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1871 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/mock.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.359102 especifico-3.0.9/especifico/operations/
+-rw-r--r--   0 runner    (1001) docker     (121)      685 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15979 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/operations/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/operations/compat.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15799 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/operations/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8681 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/operations/secure.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12724 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/operations/swagger2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4681 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/options.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2380 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/problem.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8800 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.351102 especifico-3.0.9/especifico/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.351102 especifico-3.0.9/especifico/resources/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.359102 especifico-3.0.9/especifico/resources/schemas/v2.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    40020 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/resources/schemas/v2.0/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.359102 especifico-3.0.9/especifico/resources/schemas/v3.0/
+-rw-r--r--   0 runner    (1001) docker     (121)    35456 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/resources/schemas/v3.0/schema.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.363102 especifico-3.0.9/especifico/security/
+-rw-r--r--   0 runner    (1001) docker     (121)      776 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1425 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/security/aiohttp_security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4222 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/security/async_security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1397 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/security/flask_security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15601 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/security/security_handler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9157 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/spec.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6741 2022-04-04 18:14:05.000000 especifico-3.0.9/especifico/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-04 18:14:08.355102 especifico-3.0.9/especifico.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    22893 2022-04-04 18:14:08.000000 especifico-3.0.9/especifico.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-04-04 18:14:08.000000 especifico-3.0.9/especifico.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-04 18:14:08.000000 especifico-3.0.9/especifico.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       52 2022-04-04 18:14:08.000000 especifico-3.0.9/especifico.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-04-04 18:14:08.000000 especifico-3.0.9/especifico.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       11 2022-04-04 18:14:08.000000 especifico-3.0.9/especifico.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      471 2022-04-04 18:14:05.000000 especifico-3.0.9/requirements-lint.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      114 2022-04-04 18:14:05.000000 especifico-3.0.9/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-04-04 18:14:05.000000 especifico-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      141 2022-04-04 18:14:08.363102 especifico-3.0.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2634 2022-04-04 18:14:05.000000 especifico-3.0.9/setup.py
```

### Comparing `especifico-3.0.8/ARCHITECTURE.rst` & `especifico-3.0.9/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/CONTRIBUTING.rst` & `especifico-3.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/LICENSE` & `especifico-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/PKG-INFO` & `especifico-3.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: especifico
-Version: 3.0.8
+Version: 3.0.9
 Summary: Específico - API first applications with OpenAPI/Swagger and Flask
 Home-page: https://github.com/athenianco/especifico
 Author: Zalando SE & Athenian
 License: Apache License Version 2.0
 Keywords: openapi oai swagger rest api oauth flask microservice framework
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `especifico-3.0.8/README.md` & `especifico-3.0.9/README.md`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/__init__.py` & `especifico-3.0.9/especifico/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,8 +43,8 @@
     from .apps.aiohttp_app import AioHttpApp
 except ImportError as e:  # pragma: no cover
     _aiohttp_not_installed_error = not_installed_error(e)  # type: ignore
     AioHttpApi = _aiohttp_not_installed_error  # type: ignore
     AioHttpApp = _aiohttp_not_installed_error  # type: ignore
 
 # This version is replaced during release process.
-__version__ = "3.0.8"
+__version__ = "3.0.9"
```

### Comparing `especifico-3.0.8/especifico/apis/__init__.py` & `especifico-3.0.9/especifico/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apis/abstract.py` & `especifico-3.0.9/especifico/apis/abstract.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apis/aiohttp_api.py` & `especifico-3.0.9/especifico/apis/aiohttp_api.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apis/flask_api.py` & `especifico-3.0.9/especifico/apis/flask_api.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apis/flask_utils.py` & `especifico-3.0.9/especifico/apis/flask_utils.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apps/abstract.py` & `especifico-3.0.9/especifico/apps/abstract.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apps/aiohttp_app.py` & `especifico-3.0.9/especifico/apps/aiohttp_app.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/apps/flask_app.py` & `especifico-3.0.9/especifico/apps/flask_app.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/cli.py` & `especifico-3.0.9/especifico/cli.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/decorator.py` & `especifico-3.0.9/especifico/decorators/decorator.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/metrics.py` & `especifico-3.0.9/especifico/decorators/metrics.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/parameter.py` & `especifico-3.0.9/especifico/decorators/parameter.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/produces.py` & `especifico-3.0.9/especifico/decorators/produces.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/response.py` & `especifico-3.0.9/especifico/decorators/response.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/uri_parsing.py` & `especifico-3.0.9/especifico/decorators/uri_parsing.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/decorators/validation.py` & `especifico-3.0.9/especifico/decorators/validation.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/exceptions.py` & `especifico-3.0.9/especifico/exceptions.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/handlers.py` & `especifico-3.0.9/especifico/handlers.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/json_schema.py` & `especifico-3.0.9/especifico/json_schema.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/jsonifier.py` & `especifico-3.0.9/especifico/jsonifier.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/lifecycle.py` & `especifico-3.0.9/especifico/lifecycle.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/mock.py` & `especifico-3.0.9/especifico/mock.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/operations/__init__.py` & `especifico-3.0.9/especifico/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/operations/abstract.py` & `especifico-3.0.9/especifico/operations/abstract.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/operations/openapi.py` & `especifico-3.0.9/especifico/operations/openapi.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/operations/secure.py` & `especifico-3.0.9/especifico/operations/secure.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/operations/swagger2.py` & `especifico-3.0.9/especifico/operations/swagger2.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/options.py` & `especifico-3.0.9/especifico/options.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/problem.py` & `especifico-3.0.9/especifico/problem.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/resolver.py` & `especifico-3.0.9/especifico/resolver.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/resources/schemas/v2.0/schema.json` & `especifico-3.0.9/especifico/resources/schemas/v2.0/schema.json`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/resources/schemas/v3.0/schema.json` & `especifico-3.0.9/especifico/resources/schemas/v3.0/schema.json`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/security/__init__.py` & `especifico-3.0.9/especifico/security/__init__.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/security/aiohttp_security_handler_factory.py` & `especifico-3.0.9/especifico/security/aiohttp_security_handler_factory.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/security/async_security_handler_factory.py` & `especifico-3.0.9/especifico/security/async_security_handler_factory.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/security/flask_security_handler_factory.py` & `especifico-3.0.9/especifico/security/flask_security_handler_factory.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/security/security_handler_factory.py` & `especifico-3.0.9/especifico/security/security_handler_factory.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/spec.py` & `especifico-3.0.9/especifico/spec.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico/utils.py` & `especifico-3.0.9/especifico/utils.py`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico.egg-info/PKG-INFO` & `especifico-3.0.9/especifico.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: especifico
-Version: 3.0.8
+Version: 3.0.9
 Summary: Específico - API first applications with OpenAPI/Swagger and Flask
 Home-page: https://github.com/athenianco/especifico
 Author: Zalando SE & Athenian
 License: Apache License Version 2.0
 Keywords: openapi oai swagger rest api oauth flask microservice framework
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `especifico-3.0.8/especifico.egg-info/SOURCES.txt` & `especifico-3.0.9/especifico.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/especifico.egg-info/requires.txt` & `especifico-3.0.9/especifico.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `especifico-3.0.8/setup.py` & `especifico-3.0.9/setup.py`

 * *Files identical despite different names*

