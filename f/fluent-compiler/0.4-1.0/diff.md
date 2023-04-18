# Comparing `tmp/fluent_compiler-0.4.tar.gz` & `tmp/fluent_compiler-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluent_compiler-0.4.tar", last modified: Thu Feb 16 18:36:40 2023, max compression
+gzip compressed data, was "fluent_compiler-1.0.tar", last modified: Tue Apr 18 15:18:47 2023, max compression
```

## Comparing `fluent_compiler-0.4.tar` & `fluent_compiler-1.0.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.265794 fluent_compiler-0.4/
--rw-r--r--   0 luke      (1000) luke      (1000)     1250 2022-12-31 09:10:45.000000 fluent_compiler-0.4/.pre-commit-config.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)       73 2022-12-31 09:10:45.000000 fluent_compiler-0.4/.readthedocs.yaml
--rw-r--r--   0 luke      (1000) luke      (1000)     4383 2022-12-31 09:10:45.000000 fluent_compiler-0.4/ARCHITECTURE.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1911 2023-02-16 18:30:41.000000 fluent_compiler-0.4/CHANGELOG.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1719 2022-12-31 09:10:45.000000 fluent_compiler-0.4/CONTRIBUTING.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      551 2022-12-31 09:10:45.000000 fluent_compiler-0.4/LICENSE
--rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-12-31 09:10:45.000000 fluent_compiler-0.4/MANIFEST.in
--rw-rw-rw-   0 luke      (1000) luke      (1000)     4440 2023-02-16 18:36:40.265794 fluent_compiler-0.4/PKG-INFO
--rw-r--r--   0 luke      (1000) luke      (1000)     3617 2022-12-31 09:10:45.000000 fluent_compiler-0.4/README.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      500 2023-02-16 18:31:40.000000 fluent_compiler-0.4/RELEASE.rst
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.257794 fluent_compiler-0.4/docs/
--rw-r--r--   0 luke      (1000) luke      (1000)      581 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/Makefile
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.257794 fluent_compiler-0.4/docs/api/
--rw-r--r--   0 luke      (1000) luke      (1000)     2421 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/api/bundle.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4325 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/api/compiler.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      119 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/api/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     1013 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/api/resource.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     5615 2023-02-16 18:32:08.000000 fluent_compiler-0.4/docs/conf.py
--rw-r--r--   0 luke      (1000) luke      (1000)       67 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/contributing.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     2271 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/errors.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     5678 2023-02-16 18:30:06.000000 fluent_compiler-0.4/docs/escaping.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4077 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/functions.rst
--rw-r--r--   0 luke      (1000) luke      (1000)       30 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/history.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     4962 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/implementations.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      380 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/index.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      253 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/installation.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      787 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/make.bat
--rw-r--r--   0 luke      (1000) luke      (1000)       14 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     3033 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/security.rst
--rw-r--r--   0 luke      (1000) luke      (1000)     8721 2022-12-31 09:10:45.000000 fluent_compiler-0.4/docs/usage.rst
--rw-r--r--   0 luke      (1000) luke      (1000)      295 2022-12-31 09:10:45.000000 fluent_compiler-0.4/pyproject.toml
--rwxr-xr--   0 luke      (1000) luke      (1000)      439 2022-12-31 09:10:45.000000 fluent_compiler-0.4/release.sh
--rw-r--r--   0 luke      (1000) luke      (1000)       43 2022-12-31 09:10:45.000000 fluent_compiler-0.4/requirements-linters.txt
--rw-r--r--   0 luke      (1000) luke      (1000)      105 2022-12-31 09:10:45.000000 fluent_compiler-0.4/requirements-test.txt
--rw-r--r--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-0.4/requirements.txt
--rw-r--r--   0 luke      (1000) luke      (1000)     1075 2023-02-16 18:36:40.269794 fluent_compiler-0.4/setup.cfg
--rwxr-xr--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-0.4/setup.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.249794 fluent_compiler-0.4/src/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.261794 fluent_compiler-0.4/src/fluent_compiler/
--rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-02-16 18:31:57.000000 fluent_compiler-0.4/src/fluent_compiler/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1172 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/ast_compat.py
--rw-r--r--   0 luke      (1000) luke      (1000)      158 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/builtins.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2139 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/bundle.py
--rw-r--r--   0 luke      (1000) luke      (1000)    29975 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/codegen.py
--rw-r--r--   0 luke      (1000) luke      (1000)    52647 2023-02-16 18:30:06.000000 fluent_compiler-0.4/src/fluent_compiler/compiler.py
--rw-r--r--   0 luke      (1000) luke      (1000)      660 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/errors.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5264 2023-02-16 18:30:06.000000 fluent_compiler-0.4/src/fluent_compiler/escapers.py
--rw-r--r--   0 luke      (1000) luke      (1000)      446 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/resource.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2614 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/runtime.py
--rw-r--r--   0 luke      (1000) luke      (1000)    14702 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/types.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6476 2022-12-31 09:10:45.000000 fluent_compiler-0.4/src/fluent_compiler/utils.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.261794 fluent_compiler-0.4/src/fluent_compiler.egg-info/
--rw-r-----   0 luke      (1000) luke      (1000)     4440 2023-02-16 18:36:40.000000 fluent_compiler-0.4/src/fluent_compiler.egg-info/PKG-INFO
--rw-r-----   0 luke      (1000) luke      (1000)     1781 2023-02-16 18:36:40.000000 fluent_compiler-0.4/src/fluent_compiler.egg-info/SOURCES.txt
--rw-r-----   0 luke      (1000) luke      (1000)        1 2023-02-16 18:36:40.000000 fluent_compiler-0.4/src/fluent_compiler.egg-info/dependency_links.txt
--rw-r-----   0 luke      (1000) luke      (1000)       52 2023-02-16 18:36:40.000000 fluent_compiler-0.4/src/fluent_compiler.egg-info/requires.txt
--rw-r-----   0 luke      (1000) luke      (1000)       16 2023-02-16 18:36:40.000000 fluent_compiler-0.4/src/fluent_compiler.egg-info/top_level.txt
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.265794 fluent_compiler-0.4/tests/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/__init__.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.265794 fluent_compiler-0.4/tests/format/
--rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/__init__.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2568 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_arguments.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6136 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_attributes.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6771 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_builtins.py
--rw-r--r--   0 luke      (1000) luke      (1000)    16852 2023-02-16 18:30:06.000000 fluent_compiler-0.4/tests/format/test_escapers.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9329 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_functions.py
--rw-r--r--   0 luke      (1000) luke      (1000)     2222 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_isolating.py
--rw-r--r--   0 luke      (1000) luke      (1000)     9908 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_parameterized_terms.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5828 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_placeables.py
--rw-r--r--   0 luke      (1000) luke      (1000)     5166 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_primitives.py
--rw-r--r--   0 luke      (1000) luke      (1000)    10567 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/format/test_select_expression.py
--rw-r--r--   0 luke      (1000) luke      (1000)     6053 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/test_bundle.py
--rw-r--r--   0 luke      (1000) luke      (1000)    20518 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/test_codegen.py
--rw-r--r--   0 luke      (1000) luke      (1000)    38696 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/test_compiler.py
--rw-r--r--   0 luke      (1000) luke      (1000)    13981 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/test_types.py
--rw-r--r--   0 luke      (1000) luke      (1000)     1560 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/test_utils.py
--rw-r--r--   0 luke      (1000) luke      (1000)       89 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tests/utils.py
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.249794 fluent_compiler-0.4/tools/
-drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-02-16 18:36:40.265794 fluent_compiler-0.4/tools/benchmarks/
--rw-r--r--   0 luke      (1000) luke      (1000)     1077 2023-02-01 21:53:58.000000 fluent_compiler-0.4/tools/benchmarks/README.md
--rwxr-xr--   0 luke      (1000) luke      (1000)     1409 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tools/benchmarks/compiler.py
--rw-r--r--   0 luke      (1000) luke      (1000)       64 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tools/benchmarks/requirements.txt
--rwxr-xr--   0 luke      (1000) luke      (1000)     8207 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tools/benchmarks/runtime.py
--rw-r--r--   0 luke      (1000) luke      (1000)      754 2022-12-31 09:10:45.000000 fluent_compiler-0.4/tox.ini
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.822632 fluent_compiler-1.0/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1250 2022-12-31 09:10:45.000000 fluent_compiler-1.0/.pre-commit-config.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)       73 2022-12-31 09:10:45.000000 fluent_compiler-1.0/.readthedocs.yaml
+-rw-r--r--   0 luke      (1000) luke      (1000)     4383 2022-12-31 09:10:45.000000 fluent_compiler-1.0/ARCHITECTURE.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2031 2023-04-18 15:06:15.000000 fluent_compiler-1.0/CHANGELOG.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1719 2022-12-31 09:10:45.000000 fluent_compiler-1.0/CONTRIBUTING.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      551 2022-12-31 09:10:45.000000 fluent_compiler-1.0/LICENSE
+-rw-r--r--   0 luke      (1000) luke      (1000)      422 2022-12-31 09:10:45.000000 fluent_compiler-1.0/MANIFEST.in
+-rw-rw-rw-   0 luke      (1000) luke      (1000)     4460 2023-04-18 15:18:47.822632 fluent_compiler-1.0/PKG-INFO
+-rw-r--r--   0 luke      (1000) luke      (1000)     3617 2022-12-31 09:10:45.000000 fluent_compiler-1.0/README.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      500 2023-02-16 18:31:40.000000 fluent_compiler-1.0/RELEASE.rst
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/docs/
+-rw-r--r--   0 luke      (1000) luke      (1000)      581 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/Makefile
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/docs/api/
+-rw-r--r--   0 luke      (1000) luke      (1000)     2421 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/bundle.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4325 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/compiler.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      119 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     1013 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/api/resource.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     5615 2023-04-18 15:14:26.000000 fluent_compiler-1.0/docs/conf.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       67 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/contributing.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     2271 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/errors.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     5678 2023-02-16 18:30:06.000000 fluent_compiler-1.0/docs/escaping.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4077 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/functions.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)       30 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/history.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     4962 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/implementations.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      380 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/index.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      253 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/installation.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      787 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/make.bat
+-rw-r--r--   0 luke      (1000) luke      (1000)       14 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     3033 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/security.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)     8721 2022-12-31 09:10:45.000000 fluent_compiler-1.0/docs/usage.rst
+-rw-r--r--   0 luke      (1000) luke      (1000)      295 2022-12-31 09:10:45.000000 fluent_compiler-1.0/pyproject.toml
+-rwxr-xr--   0 luke      (1000) luke      (1000)      439 2022-12-31 09:10:45.000000 fluent_compiler-1.0/release.sh
+-rw-r--r--   0 luke      (1000) luke      (1000)       43 2022-12-31 09:10:45.000000 fluent_compiler-1.0/requirements-linters.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)      105 2022-12-31 09:10:45.000000 fluent_compiler-1.0/requirements-test.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-1.0/requirements.txt
+-rw-r--r--   0 luke      (1000) luke      (1000)     1075 2023-04-18 15:18:47.822632 fluent_compiler-1.0/setup.cfg
+-rwxr-xr--   0 luke      (1000) luke      (1000)       60 2022-12-31 09:10:45.000000 fluent_compiler-1.0/setup.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.806632 fluent_compiler-1.0/src/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/src/fluent_compiler/
+-rw-r--r--   0 luke      (1000) luke      (1000)       20 2023-04-18 15:14:16.000000 fluent_compiler-1.0/src/fluent_compiler/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1791 2023-04-18 12:36:09.000000 fluent_compiler-1.0/src/fluent_compiler/ast_compat.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      158 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/builtins.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2139 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/bundle.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    29975 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/codegen.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    52647 2023-02-16 18:30:06.000000 fluent_compiler-1.0/src/fluent_compiler/compiler.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      660 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/errors.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5264 2023-02-16 18:30:06.000000 fluent_compiler-1.0/src/fluent_compiler/escapers.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      446 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/resource.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2614 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/runtime.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    14702 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/types.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6476 2022-12-31 09:10:45.000000 fluent_compiler-1.0/src/fluent_compiler/utils.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.814633 fluent_compiler-1.0/src/fluent_compiler.egg-info/
+-rw-r-----   0 luke      (1000) luke      (1000)     4460 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/PKG-INFO
+-rw-r-----   0 luke      (1000) luke      (1000)     1781 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/SOURCES.txt
+-rw-r-----   0 luke      (1000) luke      (1000)        1 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/dependency_links.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       52 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/requires.txt
+-rw-r-----   0 luke      (1000) luke      (1000)       16 2023-04-18 15:18:47.000000 fluent_compiler-1.0/src/fluent_compiler.egg-info/top_level.txt
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.818632 fluent_compiler-1.0/tests/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/__init__.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.818632 fluent_compiler-1.0/tests/format/
+-rw-r--r--   0 luke      (1000) luke      (1000)        0 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/__init__.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2568 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_arguments.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6136 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_attributes.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6771 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_builtins.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    16852 2023-02-16 18:30:06.000000 fluent_compiler-1.0/tests/format/test_escapers.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9329 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_functions.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     2222 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_isolating.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     9908 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_parameterized_terms.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5828 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_placeables.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     5166 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_primitives.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    10567 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/format/test_select_expression.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     6053 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_bundle.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    20518 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_codegen.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    38696 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_compiler.py
+-rw-r--r--   0 luke      (1000) luke      (1000)    13981 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_types.py
+-rw-r--r--   0 luke      (1000) luke      (1000)     1560 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/test_utils.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       89 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tests/utils.py
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.806632 fluent_compiler-1.0/tools/
+drwxrwxrwx   0 luke      (1000) luke      (1000)        0 2023-04-18 15:18:47.822632 fluent_compiler-1.0/tools/benchmarks/
+-rw-r--r--   0 luke      (1000) luke      (1000)     1077 2023-02-01 21:53:58.000000 fluent_compiler-1.0/tools/benchmarks/README.md
+-rwxr-xr--   0 luke      (1000) luke      (1000)     1409 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tools/benchmarks/compiler.py
+-rw-r--r--   0 luke      (1000) luke      (1000)       64 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tools/benchmarks/requirements.txt
+-rwxr-xr--   0 luke      (1000) luke      (1000)     8207 2022-12-31 09:10:45.000000 fluent_compiler-1.0/tools/benchmarks/runtime.py
+-rw-r--r--   0 luke      (1000) luke      (1000)      766 2023-04-18 15:13:49.000000 fluent_compiler-1.0/tox.ini
```

### Comparing `fluent_compiler-0.4/.pre-commit-config.yaml` & `fluent_compiler-1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/ARCHITECTURE.rst` & `fluent_compiler-1.0/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/CHANGELOG.rst` & `fluent_compiler-1.0/CHANGELOG.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 Changelog
 =========
 
+fluent_compiler 1.0 (2023-04-18)
+--------------------------------
+
+* Tested against latest Python 3.11, and 3.12 alpha
+
 fluent_compiler 0.4 (2023-02-16)
 --------------------------------
 
 * Dropped support for Python 2.7 and Python < 3.6
 * Lots of code style cleanups using black etc.
 * Compiler actually respects documented ``use_isolating`` attribute of escapers
```

### Comparing `fluent_compiler-0.4/CONTRIBUTING.rst` & `fluent_compiler-1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/LICENSE` & `fluent_compiler-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/PKG-INFO` & `fluent_compiler-1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: fluent_compiler
-Version: 0.4
+Version: 1.0
 Summary: Blazing fast implementation of Fluent localization language.
 Home-page: https://github.com/django-ftl/fluent-compiler
 Author: Luke Plant
 Author-email: L.Plant.98@cantab.net
 License: APL 2
 Keywords: fluent,localization,l10n,compiler
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -96,7 +97,9 @@
 alternative implementation of ``FluentBundle``, but never got merged to the
 master branch. It has now been pulled out as a separate package. This is why
 the repo's history contains `fluent.syntax` and early versions of `fluent.runtime`,
 but the parts that are left in this repo all derive from the original version
 of `fluent.runtime` contributed by @spookylukey from `a540993a085e36a9679e12f1ee7317ddc1ece5ad <https://github.com/django-ftl/fluent-compiler/commit/a540993a085e36a9679e12f1ee7317ddc1ece5ad>`_ onwards and the new compiler implementation in `d1481d61e0bc1a28a228a4b6d5258350d436e765 <https://github.com/django-ftl/fluent-compiler/commit/d1481d61e0bc1a28a228a4b6d5258350d436e765>`_ (which is squashed version of work done over a much longer period). Thats why
 we also `corrected <https://github.com/django-ftl/fluent-compiler/commit/33c1b5b586858132d3ab7af749c2bde1bb5205b5>`_
 the copyright notice from Mozilla to Luke Plant.
+
+
```

### Comparing `fluent_compiler-0.4/README.rst` & `fluent_compiler-1.0/README.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/Makefile` & `fluent_compiler-1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/api/bundle.rst` & `fluent_compiler-1.0/docs/api/bundle.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/api/compiler.rst` & `fluent_compiler-1.0/docs/api/compiler.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/api/resource.rst` & `fluent_compiler-1.0/docs/api/resource.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/conf.py` & `fluent_compiler-1.0/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 # -- Project information -----------------------------------------------------
 
 project = "fluent_compiler"
 copyright = "2019, Luke Plant"
 author = "Luke Plant"
 
 # The short X.Y version
-version = "0.4"
+version = "1.0"
 # The full version, including alpha/beta/rc tags
-release = "0.4"
+release = "1.0"
 
 
 # -- General configuration ---------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `fluent_compiler-0.4/docs/errors.rst` & `fluent_compiler-1.0/docs/errors.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/escaping.rst` & `fluent_compiler-1.0/docs/escaping.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/functions.rst` & `fluent_compiler-1.0/docs/functions.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/implementations.rst` & `fluent_compiler-1.0/docs/implementations.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/make.bat` & `fluent_compiler-1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/security.rst` & `fluent_compiler-1.0/docs/security.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/docs/usage.rst` & `fluent_compiler-1.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/setup.cfg` & `fluent_compiler-1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/bundle.py` & `fluent_compiler-1.0/src/fluent_compiler/bundle.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/codegen.py` & `fluent_compiler-1.0/src/fluent_compiler/codegen.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/compiler.py` & `fluent_compiler-1.0/src/fluent_compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/errors.py` & `fluent_compiler-1.0/src/fluent_compiler/errors.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/escapers.py` & `fluent_compiler-1.0/src/fluent_compiler/escapers.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/runtime.py` & `fluent_compiler-1.0/src/fluent_compiler/runtime.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/types.py` & `fluent_compiler-1.0/src/fluent_compiler/types.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler/utils.py` & `fluent_compiler-1.0/src/fluent_compiler/utils.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/src/fluent_compiler.egg-info/PKG-INFO` & `fluent_compiler-1.0/src/fluent_compiler.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: fluent-compiler
-Version: 0.4
+Version: 1.0
 Summary: Blazing fast implementation of Fluent localization language.
 Home-page: https://github.com/django-ftl/fluent-compiler
 Author: Luke Plant
 Author-email: L.Plant.98@cantab.net
 License: APL 2
 Keywords: fluent,localization,l10n,compiler
+Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -96,7 +97,9 @@
 alternative implementation of ``FluentBundle``, but never got merged to the
 master branch. It has now been pulled out as a separate package. This is why
 the repo's history contains `fluent.syntax` and early versions of `fluent.runtime`,
 but the parts that are left in this repo all derive from the original version
 of `fluent.runtime` contributed by @spookylukey from `a540993a085e36a9679e12f1ee7317ddc1ece5ad <https://github.com/django-ftl/fluent-compiler/commit/a540993a085e36a9679e12f1ee7317ddc1ece5ad>`_ onwards and the new compiler implementation in `d1481d61e0bc1a28a228a4b6d5258350d436e765 <https://github.com/django-ftl/fluent-compiler/commit/d1481d61e0bc1a28a228a4b6d5258350d436e765>`_ (which is squashed version of work done over a much longer period). Thats why
 we also `corrected <https://github.com/django-ftl/fluent-compiler/commit/33c1b5b586858132d3ab7af749c2bde1bb5205b5>`_
 the copyright notice from Mozilla to Luke Plant.
+
+
```

### Comparing `fluent_compiler-0.4/src/fluent_compiler.egg-info/SOURCES.txt` & `fluent_compiler-1.0/src/fluent_compiler.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_arguments.py` & `fluent_compiler-1.0/tests/format/test_arguments.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_attributes.py` & `fluent_compiler-1.0/tests/format/test_attributes.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_builtins.py` & `fluent_compiler-1.0/tests/format/test_builtins.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_escapers.py` & `fluent_compiler-1.0/tests/format/test_escapers.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_functions.py` & `fluent_compiler-1.0/tests/format/test_functions.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_isolating.py` & `fluent_compiler-1.0/tests/format/test_isolating.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_parameterized_terms.py` & `fluent_compiler-1.0/tests/format/test_parameterized_terms.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_placeables.py` & `fluent_compiler-1.0/tests/format/test_placeables.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_primitives.py` & `fluent_compiler-1.0/tests/format/test_primitives.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/format/test_select_expression.py` & `fluent_compiler-1.0/tests/format/test_select_expression.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/test_bundle.py` & `fluent_compiler-1.0/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/test_codegen.py` & `fluent_compiler-1.0/tests/test_codegen.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/test_compiler.py` & `fluent_compiler-1.0/tests/test_compiler.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/test_types.py` & `fluent_compiler-1.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tests/test_utils.py` & `fluent_compiler-1.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tools/benchmarks/README.md` & `fluent_compiler-1.0/tools/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tools/benchmarks/compiler.py` & `fluent_compiler-1.0/tools/benchmarks/compiler.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tools/benchmarks/runtime.py` & `fluent_compiler-1.0/tools/benchmarks/runtime.py`

 * *Files identical despite different names*

### Comparing `fluent_compiler-0.4/tox.ini` & `fluent_compiler-1.0/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # This config is for local testing. Where needed changes should be duplicated into
 # .github/workflows/pythonpackage.yml
 [tox]
-envlist = py36,py37,py38,py39,py310,pypy3.6,flake8,isort
+envlist = py36,py37,py38,py39,py310,py311,py312,pypy3.6,flake8,isort
 
 [testenv]
 deps =
      # Just '.[develop]' would be nice here.
      # Unfortunately it is super slow: https://github.com/pypa/pip/issues/2195
      # So we duplicate deps from setup.py for now.
      -r{toxinidir}/requirements.txt
```

