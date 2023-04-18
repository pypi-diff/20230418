# Comparing `tmp/importlib_metadata-6.4.1.tar.gz` & `tmp/importlib_metadata-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "importlib_metadata-6.4.1.tar", last modified: Sat Apr 15 15:24:44 2023, max compression
+gzip compressed data, was "importlib_metadata-6.5.0.tar", last modified: Tue Apr 18 13:02:18 2023, max compression
```

## Comparing `importlib_metadata-6.4.1.tar` & `importlib_metadata-6.5.0.tar`

### file list

```diff
@@ -1,72 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.350520 importlib_metadata-6.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.github/FUNDING.yml
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.350520 importlib_metadata-6.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20794 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.350520 importlib_metadata-6.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/migration.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/docs/using.rst
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/exercises.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.354520 importlib_metadata-6.4.1/importlib_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)    28638 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_itertools.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/importlib_metadata/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/importlib_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-15 15:24:44.000000 importlib_metadata-6.4.1/importlib_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/mypy.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.342520 importlib_metadata-6.4.1/prepare/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example/example/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.358520 importlib_metadata-6.4.1/prepare/example2/example2/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example2/example2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/prepare/example2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/_path.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:44.362520 importlib_metadata-6.4.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/example-21.12-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/example-21.12-py3.6.egg
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/data/example2-1.0.0-py3-none-any.whl
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    13645 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_py39compat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tests/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-15 15:24:25.000000 importlib_metadata-6.4.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.239251 importlib_metadata-6.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.223251 importlib_metadata-6.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.github/FUNDING.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.227251 importlib_metadata-6.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20956 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-18 13:02:18.239251 importlib_metadata-6.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.227251 importlib_metadata-6.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/migration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13744 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/docs/using.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/exercises.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.231251 importlib_metadata-6.5.0/importlib_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)    29202 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_itertools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/importlib_metadata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.231251 importlib_metadata-6.5.0/importlib_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-04-18 13:02:18.000000 importlib_metadata-6.5.0/importlib_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-18 13:02:18.000000 importlib_metadata-6.5.0/importlib_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 13:02:18.000000 importlib_metadata-6.5.0/importlib_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 13:02:18.000000 importlib_metadata-6.5.0/importlib_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 13:02:18.000000 importlib_metadata-6.5.0/importlib_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/mypy.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.219251 importlib_metadata-6.5.0/prepare/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.231251 importlib_metadata-6.5.0/prepare/example/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.235251 importlib_metadata-6.5.0/prepare/example/example/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/prepare/example/example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/prepare/example/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.235251 importlib_metadata-6.5.0/prepare/example2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.235251 importlib_metadata-6.5.0/prepare/example2/example2/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/prepare/example2/example2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/prepare/example2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-04-18 13:02:18.239251 importlib_metadata-6.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.239251 importlib_metadata-6.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/_path.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 13:02:18.239251 importlib_metadata-6.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/data/example-21.12-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/data/example-21.12-py3.6.egg
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/data/example2-1.0.0-py3-none-any.whl
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11146 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2016 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14024 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/test_py39compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tests/test_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-18 13:01:59.000000 importlib_metadata-6.5.0/tox.ini
```

### Comparing `importlib_metadata-6.4.1/.github/workflows/main.yml` & `importlib_metadata-6.5.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/CHANGES.rst` & `importlib_metadata-6.5.0/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+v6.5.0
+======
+
+* #422: Removed ABC metaclass from ``Distribution`` and instead
+  deprecated construction of ``Distribution`` objects without
+  concrete methods.
+
 v6.4.1
 ======
 
 * Updated docs with tweaks from upstream CPython.
 
 v6.4.0
 ======
```

### Comparing `importlib_metadata-6.4.1/LICENSE` & `importlib_metadata-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/PKG-INFO` & `importlib_metadata-6.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib_metadata
-Version: 6.4.1
+Version: 6.5.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -66,15 +66,15 @@
    * - 1.4
      - 3.8
 
 
 Usage
 =====
 
-See the `online documentation <https://importlib_metadata.readthedocs.io/>`_
+See the `online documentation <https://importlib-metadata.readthedocs.io/>`_
 for usage details.
 
 `Finder authors
 <https://docs.python.org/3/reference/import.html#finders-and-loaders>`_ can
 also add support for custom package installers.  See the above documentation
 for details.
 
@@ -90,15 +90,15 @@
 
 Project details
 ===============
 
  * Project home: https://github.com/python/importlib_metadata
  * Report bugs at: https://github.com/python/importlib_metadata/issues
  * Code hosting: https://github.com/python/importlib_metadata
- * Documentation: https://importlib_metadata.readthedocs.io/
+ * Documentation: https://importlib-metadata.readthedocs.io/
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
```

### Comparing `importlib_metadata-6.4.1/README.rst` & `importlib_metadata-6.5.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
    * - 1.4
      - 3.8
 
 
 Usage
 =====
 
-See the `online documentation <https://importlib_metadata.readthedocs.io/>`_
+See the `online documentation <https://importlib-metadata.readthedocs.io/>`_
 for usage details.
 
 `Finder authors
 <https://docs.python.org/3/reference/import.html#finders-and-loaders>`_ can
 also add support for custom package installers.  See the above documentation
 for details.
 
@@ -72,15 +72,15 @@
 
 Project details
 ===============
 
  * Project home: https://github.com/python/importlib_metadata
  * Report bugs at: https://github.com/python/importlib_metadata/issues
  * Code hosting: https://github.com/python/importlib_metadata
- * Documentation: https://importlib_metadata.readthedocs.io/
+ * Documentation: https://importlib-metadata.readthedocs.io/
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
```

### Comparing `importlib_metadata-6.4.1/conftest.py` & `importlib_metadata-6.5.0/conftest.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/docs/conf.py` & `importlib_metadata-6.5.0/docs/conf.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,8 +64,10 @@
 nitpick_ignore = [
     # Workaround for #316
     ('py:class', 'importlib_metadata.EntryPoints'),
     ('py:class', 'importlib_metadata.SelectableGroups'),
     ('py:class', 'importlib_metadata._meta._T'),
     # Workaround for #435
     ('py:class', '_T'),
+    # Other workarounds
+    ('py:class', 'importlib_metadata.DeprecatedNonAbstract'),
 ]
```

### Comparing `importlib_metadata-6.4.1/docs/index.rst` & `importlib_metadata-6.5.0/docs/index.rst`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 Project details
 ===============
 
  * Project home: https://github.com/python/importlib_metadata
  * Report bugs at: https://github.com/python/importlib_metadata/issues
  * Code hosting: https://github.com/python/importlib_metadata
- * Documentation: https://importlib_metadata.readthedocs.io/
+ * Documentation: https://importlib-metadata.readthedocs.io/
 
 
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
```

### Comparing `importlib_metadata-6.4.1/docs/migration.rst` & `importlib_metadata-6.5.0/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/docs/using.rst` & `importlib_metadata-6.5.0/docs/using.rst`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/exercises.py` & `importlib_metadata-6.5.0/exercises.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/__init__.py` & `importlib_metadata-6.5.0/importlib_metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,34 @@
     def __init__(self, spec):
         self.mode, _, self.value = spec.partition('=')
 
     def __repr__(self):
         return f'<FileHash mode: {self.mode} value: {self.value}>'
 
 
-class Distribution(metaclass=abc.ABCMeta):
+class DeprecatedNonAbstract:
+    def __new__(cls, *args, **kwargs):
+        all_names = {
+            name for subclass in inspect.getmro(cls) for name in vars(subclass)
+        }
+        abstract = {
+            name
+            for name in all_names
+            if getattr(getattr(cls, name), '__isabstractmethod__', False)
+        }
+        if abstract:
+            warnings.warn(
+                f"Unimplemented abstract methods {abstract}",
+                DeprecationWarning,
+                stacklevel=2,
+            )
+        return super().__new__(cls)
+
+
+class Distribution(DeprecatedNonAbstract):
     """A Python distribution package."""
 
     @abc.abstractmethod
     def read_text(self, filename) -> Optional[str]:
         """Attempt to load metadata file given by the name.
 
         :param filename: The name of the file in the distribution info.
```

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_adapters.py` & `importlib_metadata-6.5.0/importlib_metadata/_adapters.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_collections.py` & `importlib_metadata-6.5.0/importlib_metadata/_collections.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_compat.py` & `importlib_metadata-6.5.0/importlib_metadata/_compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_functools.py` & `importlib_metadata-6.5.0/importlib_metadata/_functools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_itertools.py` & `importlib_metadata-6.5.0/importlib_metadata/_itertools.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_meta.py` & `importlib_metadata-6.5.0/importlib_metadata/_meta.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_py39compat.py` & `importlib_metadata-6.5.0/importlib_metadata/_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata/_text.py` & `importlib_metadata-6.5.0/importlib_metadata/_text.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/importlib_metadata.egg-info/PKG-INFO` & `importlib_metadata-6.5.0/importlib_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: importlib-metadata
-Version: 6.4.1
+Version: 6.5.0
 Summary: Read metadata from Python packages
 Home-page: https://github.com/python/importlib_metadata
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
@@ -66,15 +66,15 @@
    * - 1.4
      - 3.8
 
 
 Usage
 =====
 
-See the `online documentation <https://importlib_metadata.readthedocs.io/>`_
+See the `online documentation <https://importlib-metadata.readthedocs.io/>`_
 for usage details.
 
 `Finder authors
 <https://docs.python.org/3/reference/import.html#finders-and-loaders>`_ can
 also add support for custom package installers.  See the above documentation
 for details.
 
@@ -90,15 +90,15 @@
 
 Project details
 ===============
 
  * Project home: https://github.com/python/importlib_metadata
  * Report bugs at: https://github.com/python/importlib_metadata/issues
  * Code hosting: https://github.com/python/importlib_metadata
- * Documentation: https://importlib_metadata.readthedocs.io/
+ * Documentation: https://importlib-metadata.readthedocs.io/
 
 For Enterprise
 ==============
 
 Available as part of the Tidelift Subscription.
 
 This project and the maintainers of thousands of other packages are working with Tidelift to deliver one enterprise subscription that covers all of the open source you use.
```

### Comparing `importlib_metadata-6.4.1/importlib_metadata.egg-info/SOURCES.txt` & `importlib_metadata-6.5.0/importlib_metadata.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 importlib_metadata.egg-info/requires.txt
 importlib_metadata.egg-info/top_level.txt
 prepare/example/setup.py
 prepare/example/example/__init__.py
 prepare/example2/pyproject.toml
 prepare/example2/example2/__init__.py
 tests/__init__.py
+tests/_context.py
 tests/_path.py
 tests/fixtures.py
 tests/py39compat.py
 tests/test_api.py
 tests/test_integration.py
 tests/test_main.py
 tests/test_py39compat.py
```

### Comparing `importlib_metadata-6.4.1/pytest.ini` & `importlib_metadata-6.5.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/setup.cfg` & `importlib_metadata-6.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/_path.py` & `importlib_metadata-6.5.0/tests/_path.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/data/example-21.12-py3-none-any.whl` & `importlib_metadata-6.5.0/tests/data/example-21.12-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/data/example-21.12-py3.6.egg` & `importlib_metadata-6.5.0/tests/data/example-21.12-py3.6.egg`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/data/example2-1.0.0-py3-none-any.whl` & `importlib_metadata-6.5.0/tests/data/example2-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/fixtures.py` & `importlib_metadata-6.5.0/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/test_api.py` & `importlib_metadata-6.5.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/test_integration.py` & `importlib_metadata-6.5.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/test_main.py` & `importlib_metadata-6.5.0/tests/test_main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,39 @@
 import re
 import pickle
 import unittest
+import warnings
 import importlib
 import importlib_metadata
+import contextlib
 import itertools
 import pyfakefs.fake_filesystem_unittest as ffs
 
 from . import fixtures
+from ._context import suppress
 from importlib_metadata import (
     Distribution,
     EntryPoint,
     PackageNotFoundError,
     _unique,
     distributions,
     entry_points,
     metadata,
     packages_distributions,
     version,
 )
 
 
+@contextlib.contextmanager
+def suppress_known_deprecation():
+    with warnings.catch_warnings(record=True) as ctx:
+        warnings.simplefilter('default', category=DeprecationWarning)
+        yield ctx
+
+
 class BasicTests(fixtures.DistInfoPkg, unittest.TestCase):
     version_pattern = r'\d+\.\d+(\.\d)?'
 
     def test_retrieves_version_of_self(self):
         dist = Distribution.from_name('distinfo-pkg')
         assert isinstance(dist.version, str)
         assert re.match(self.version_pattern, dist.version)
@@ -40,14 +50,17 @@
         guide users toward the cause. See #124.
         """
         with self.assertRaises(PackageNotFoundError) as ctx:
             Distribution.from_name('does-not-exist')
 
         assert "metadata" in str(ctx.exception)
 
+    # expected to fail until ABC is enforced
+    @suppress(AssertionError)
+    @suppress_known_deprecation()
     def test_abc_enforced(self):
         with self.assertRaises(TypeError):
             type('DistributionSubclass', (Distribution,), {})()
 
     @fixtures.parameterize(
         dict(name=None),
         dict(name=''),
```

### Comparing `importlib_metadata-6.4.1/tests/test_py39compat.py` & `importlib_metadata-6.5.0/tests/test_py39compat.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tests/test_zip.py` & `importlib_metadata-6.5.0/tests/test_zip.py`

 * *Files identical despite different names*

### Comparing `importlib_metadata-6.4.1/tox.ini` & `importlib_metadata-6.5.0/tox.ini`

 * *Files identical despite different names*

