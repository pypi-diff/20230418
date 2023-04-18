# Comparing `tmp/shillelagh-1.2.1.tar.gz` & `tmp/shillelagh-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shillelagh-1.2.1.tar", last modified: Fri Apr 14 21:13:18 2023, max compression
+gzip compressed data, was "shillelagh-1.2.2.tar", last modified: Tue Apr 18 01:52:16 2023, max compression
```

## Comparing `shillelagh-1.2.1.tar` & `shillelagh-1.2.2.tar`

### file list

```diff
@@ -1,201 +1,201 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.824736 shillelagh-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.800736 shillelagh-1.2.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.800736 shillelagh-1.2.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.800736 shillelagh-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-integration.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-14 21:13:06.000000 shillelagh-1.2.1/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-04-14 21:13:06.000000 shillelagh-1.2.1/ARCHITECTURE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-14 21:13:06.000000 shillelagh-1.2.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8072 2023-04-14 21:13:06.000000 shillelagh-1.2.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-14 21:13:06.000000 shillelagh-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-14 21:13:06.000000 shillelagh-1.2.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-14 21:13:06.000000 shillelagh-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-14 21:13:06.000000 shillelagh-1.2.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-14 21:13:18.824736 shillelagh-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-14 21:13:06.000000 shillelagh-1.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.804736 shillelagh-1.2.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.804736 shillelagh-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    17733 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/adapters.rst
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/install.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-14 21:13:06.000000 shillelagh-1.2.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.808736 shillelagh-1.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/csvfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/github.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/test.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-14 21:13:06.000000 shillelagh-1.2.1/examples/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-14 21:13:06.000000 shillelagh-1.2.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-14 21:13:06.000000 shillelagh-1.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.808736 shillelagh-1.2.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-04-14 21:13:06.000000 shillelagh-1.2.1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-04-14 21:13:18.824736 shillelagh-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-14 21:13:06.000000 shillelagh-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.788735 shillelagh-1.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/datasette.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/generic_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/date.py
--rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/number.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/html_table.py
--rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/s3select.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/socrata.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/system.py
--rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/api/weatherapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/file/csvfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/memory/pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/adapters/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/gsheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/safe.py
--rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/backends/apsw/vt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/console.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-14 21:13:06.000000 shillelagh-1.2.1/src/shillelagh/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.812736 shillelagh-1.2.1/src/shillelagh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-14 21:13:18.000000 shillelagh-1.2.1/src/shillelagh.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/talks/
--rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-04-14 21:13:06.000000 shillelagh-1.2.1/talks/Python Brasil 2021.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.792735 shillelagh-1.2.1/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/templates/adapter/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/templates/adapter/hooks/
--rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/hooks/post_gen_project.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-14 21:13:06.000000 shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.816736 shillelagh-1.2.1/tests/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/datasette_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6375 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/generic_json_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/github_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/api/gsheets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/adapter_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/integration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/lib_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/date_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/number_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/html_table_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/s3select_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/socrata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/system_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/api/weatherapi_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/base_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/file/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/file/csvfile_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/adapters/memory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/memory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/memory/pandas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/adapters/registry_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/backends/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/backends/apsw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dbapi_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.820736 shillelagh-1.2.1/tests/backends/apsw/dialects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/gsheets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/dialects/safe_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/backends/apsw/vt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 21:13:18.824736 shillelagh-1.2.1/tests/fakes/
--rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/cdc_data_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/cdc_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_columns_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_data_response_1.json
--rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_data_response_2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_metadata_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/datasette_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/github_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/github_single_response.json
--rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/incidents.json
--rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fakes/weatherapi_response.json
--rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/fields_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/filters_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-14 21:13:06.000000 shillelagh-1.2.1/tests/types_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.540024 shillelagh-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.524024 shillelagh-1.2.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.524024 shillelagh-1.2.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.524024 shillelagh-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-integration.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-18 01:51:58.000000 shillelagh-1.2.2/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    13954 2023-04-18 01:51:58.000000 shillelagh-1.2.2/ARCHITECTURE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-18 01:51:58.000000 shillelagh-1.2.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8215 2023-04-18 01:51:58.000000 shillelagh-1.2.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-04-18 01:51:58.000000 shillelagh-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-18 01:51:58.000000 shillelagh-1.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-18 01:51:58.000000 shillelagh-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-04-18 01:51:58.000000 shillelagh-1.2.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-18 01:52:16.540024 shillelagh-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7573 2023-04-18 01:51:58.000000 shillelagh-1.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/adapters.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9479 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32853 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7428 2023-04-18 01:51:58.000000 shillelagh-1.2.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/csvfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/test.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-18 01:51:58.000000 shillelagh-1.2.2/examples/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 01:51:58.000000 shillelagh-1.2.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-04-18 01:51:58.000000 shillelagh-1.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-18 01:51:58.000000 shillelagh-1.2.2/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-04-18 01:52:16.540024 shillelagh-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 01:51:58.000000 shillelagh-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.512024 shillelagh-1.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/datasette.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/generic_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7494 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26713 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8982 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8159 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16029 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18376 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/number.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/html_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10603 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/s3select.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/socrata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7461 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/api/weatherapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8499 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/file/csvfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/memory/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/adapters/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/gsheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/safe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19351 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/backends/apsw/vt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6412 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21797 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11160 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17141 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2540 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-18 01:51:58.000000 shillelagh-1.2.2/src/shillelagh/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.528024 shillelagh-1.2.2/src/shillelagh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9934 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-18 01:52:16.000000 shillelagh-1.2.2/src/shillelagh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.532024 shillelagh-1.2.2/talks/
+-rw-r--r--   0 runner    (1001) docker     (123)  2331376 2023-04-18 01:51:58.000000 shillelagh-1.2.2/talks/Python Brasil 2021.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.516024 shillelagh-1.2.2/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/templates/adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/templates/adapter/hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      267 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/hooks/post_gen_project.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-18 01:51:58.000000 shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14353 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/datasette_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7637 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/generic_json_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18505 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/github_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/api/gsheets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73731 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/adapter_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5300 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/integration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9270 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/lib_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20013 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/date_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/number_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/html_table_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/s3select_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8515 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/socrata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/system_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/api/weatherapi_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8919 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/base_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/file/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/file/csvfile_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/adapters/memory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/memory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9285 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/memory/pandas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/adapters/registry_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/backends/apsw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14605 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dbapi_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.536024 shillelagh-1.2.2/tests/backends/apsw/dialects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15699 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/gsheets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/dialects/safe_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15362 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/backends/apsw/vt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5655 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 01:52:16.540024 shillelagh-1.2.2/tests/fakes/
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   400535 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/cdc_data_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   121689 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/cdc_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_columns_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   369983 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_data_response_1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    60078 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_data_response_2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_metadata_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   428142 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/datasette_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   220647 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/github_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18818 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/github_single_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)   165205 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/incidents.json
+-rw-r--r--   0 runner    (1001) docker     (123)    40785 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fakes/weatherapi_response.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13821 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/fields_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/filters_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13791 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-04-18 01:51:58.000000 shillelagh-1.2.2/tests/types_test.py
```

### Comparing `shillelagh-1.2.1/.coveragerc` & `shillelagh-1.2.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/ISSUE_TEMPLATE/bug_report.md` & `shillelagh-1.2.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/ISSUE_TEMPLATE/feature_request.md` & `shillelagh-1.2.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/pull_request_template.md` & `shillelagh-1.2.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/workflows/codeql-analysis.yml` & `shillelagh-1.2.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/workflows/python-integration.yml` & `shillelagh-1.2.2/.github/workflows/python-integration.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/workflows/python-package-daily.yml` & `shillelagh-1.2.2/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/workflows/python-package.yml` & `shillelagh-1.2.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.github/workflows/python-publish.yml` & `shillelagh-1.2.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.gitignore` & `shillelagh-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.pre-commit-config.yaml` & `shillelagh-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/.readthedocs.yml` & `shillelagh-1.2.2/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/ARCHITECTURE.rst` & `shillelagh-1.2.2/ARCHITECTURE.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/CHANGELOG.rst` & `shillelagh-1.2.2/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 1.2.2 - 2023-04-17
+==========================
+
+- Allow passing request headers to the generic JSON adapter via query arguments (#354)
+
 Version 1.2.1 - 2023-04-14
 ==========================
 
 - Allow specifying custom request headers when using the generic JSON adapter (#337)
 - Fix for escaping identifiers correctly (#340)
 - Support for S3-compatible storage (#343)
 - Adapters can now know which columns were requested (#345)
```

### Comparing `shillelagh-1.2.1/CODE_OF_CONDUCT.md` & `shillelagh-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/CONTRIBUTING.rst` & `shillelagh-1.2.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/LICENSE.txt` & `shillelagh-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/Makefile` & `shillelagh-1.2.2/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/PKG-INFO` & `shillelagh-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.1
+Version: 1.2.2
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.1/README.rst` & `shillelagh-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/docs/Makefile` & `shillelagh-1.2.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/docs/adapters.rst` & `shillelagh-1.2.2/docs/adapters.rst`

 * *Files 4% similar despite different names*

```diff
@@ -447,7 +447,15 @@
                     "request_headers": {
                         "X-Auth-Token": "SECRET",
                     },
                 },
             },
         },
     )
+
+Or via query parameters:
+
+.. code-block:: sql
+
+   SELECT * FROM "https://api.example.com/?_s_headers=(X-Auth-Token:SECRET)"
+
+Note that if passing the headers via query parameters the dictionary should be serialized using `RISON <https://pypi.org/project/prison/>`_.
```

### Comparing `shillelagh-1.2.1/docs/conf.py` & `shillelagh-1.2.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/docs/development.rst` & `shillelagh-1.2.2/docs/development.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/docs/install.rst` & `shillelagh-1.2.2/docs/install.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/docs/usage.rst` & `shillelagh-1.2.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/examples/csvfile.py` & `shillelagh-1.2.2/examples/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/examples/dataframe.py` & `shillelagh-1.2.2/examples/dataframe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/examples/datasette.py` & `shillelagh-1.2.2/examples/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/examples/generic_json.py` & `shillelagh-1.2.2/examples/generic_json.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/examples/weatherapi.py` & `shillelagh-1.2.2/examples/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/requirements/base.txt` & `shillelagh-1.2.2/requirements/base.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/requirements/test.txt` & `shillelagh-1.2.2/requirements/test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,16 @@
     # via
     #   pylint
     #   virtualenv
 pluggy==1.0.0
     # via pytest
 pre-commit==2.20.0
     # via shillelagh
+prison==0.2.1
+    # via shillelagh
 prompt-toolkit==3.0.30
     # via shillelagh
 psutil==5.9.1
     # via shillelagh
 pyasn1==0.4.8
     # via
     #   pyasn1-modules
@@ -163,14 +165,15 @@
     # via google-auth
 s3transfer==0.6.0
     # via boto3
 six==1.16.0
     # via
     #   google-auth
     #   html5lib
+    #   prison
     #   python-dateutil
     #   requests-mock
     #   url-normalize
     #   virtualenv
 soupsieve==2.3.2.post1
     # via beautifulsoup4
 sqlalchemy==1.4.39
```

### Comparing `shillelagh-1.2.1/setup.cfg` & `shillelagh-1.2.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -56,14 +56,15 @@
 	freezegun>=1.1.0
 	google-auth>=1.23.0
 	html5lib>=1.1
 	jsonpath-python>=1.0.5
 	pandas>=1.2.2
 	pip-tools>=6.4.0
 	pre-commit>=2.13.0
+	prison>=0.2.1
 	prompt_toolkit>=3
 	psutil>=5.8.0
 	pyfakefs>=4.3.3
 	pygments>=2.8
 	pylint>=2.16.2
 	pytest-cov>=2.11.1
 	pytest-integration==0.2.2
@@ -108,14 +109,15 @@
 	prompt_toolkit>=3
 	pygments>=2.8
 	tabulate==0.8.9
 datasetteapi = 
 	requests-cache==0.7.1
 genericjsonapi = 
 	jsonpath-python>=1.0.5
+	prison>=0.2.1
 	requests-cache==0.7.1
 githubapi = 
 	jsonpath-python>=1.0.5
 gsheetsapi = 
 	google-auth>=1.23.0
 	requests>=2.23.0
 htmltableapi =
```

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/datasette.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/datasette.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/generic_json.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/generic_json.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """
 An adapter for fetching JSON data.
 """
 
 # pylint: disable=invalid-name
 
 import logging
-import urllib.parse
-from typing import Any, Dict, Iterator, List, Optional, Set, Tuple
+from typing import Any, Dict, Iterator, List, Optional, Set, Tuple, Union
 
+import prison
 import requests_cache
 from jsonpath import JSONPath
+from yarl import URL
 
 from shillelagh.adapters.base import Adapter
 from shillelagh.exceptions import ProgrammingError
 from shillelagh.fields import Field
 from shillelagh.filters import Filter
 from shillelagh.lib import SimpleCostModel, analyze, flatten
 from shillelagh.typing import Maybe, RequestedOrder, Row
 
 _logger = logging.getLogger(__name__)
 
 SUPPORTED_PROTOCOLS = {"http", "https"}
 AVERAGE_NUMBER_OF_ROWS = 100
 CACHE_EXPIRATION = 180
+REQUEST_HEADERS_KEY = "_s_headers"
 
 
 def get_session(request_headers: Dict[str, str]) -> requests_cache.CachedSession:
     """
     Return a cached session.
     """
     session = requests_cache.CachedSession(
@@ -49,33 +51,47 @@
 
     supports_limit = False
     supports_offset = False
     supports_requested_columns = True
 
     @staticmethod
     def supports(uri: str, fast: bool = True, **kwargs: Any) -> Optional[bool]:
-        parsed = urllib.parse.urlparse(uri)
+        parsed = URL(uri)
         if parsed.scheme not in SUPPORTED_PROTOCOLS:
             return False
         if fast:
             return Maybe
 
-        request_headers = kwargs.get("request_headers", {})
+        if REQUEST_HEADERS_KEY in parsed.query:
+            request_headers = prison.loads(parsed.query[REQUEST_HEADERS_KEY])
+            parsed = parsed.with_query(
+                {k: v for k, v in parsed.query.items() if k != REQUEST_HEADERS_KEY},
+            )
+        else:
+            request_headers = kwargs.get("request_headers", {})
+
         session = get_session(request_headers)
-        response = session.head(uri)
+        response = session.head(str(parsed))
         return "application/json" in response.headers.get("content-type", "")
 
     @staticmethod
-    def parse_uri(uri: str) -> Tuple[str, str]:
-        parsed = urllib.parse.urlparse(uri)
+    def parse_uri(uri: str) -> Union[Tuple[str, str], Tuple[str, str, Dict[str, str]]]:
+        parsed = URL(uri)
+
+        path = parsed.fragment or "$[*]"
+        parsed = parsed.with_fragment("")
 
-        path = urllib.parse.unquote(parsed.fragment) or "$[*]"
-        uri = urllib.parse.urlunparse(parsed._replace(fragment=""))
+        if REQUEST_HEADERS_KEY in parsed.query:
+            request_headers = prison.loads(parsed.query[REQUEST_HEADERS_KEY])
+            parsed = parsed.with_query(
+                {k: v for k, v in parsed.query.items() if k != REQUEST_HEADERS_KEY},
+            )
+            return str(parsed), path, request_headers
 
-        return uri, path
+        return str(parsed), path
 
     def __init__(
         self,
         uri: str,
         path: str = "$[*]",
         request_headers: Optional[Dict[str, str]] = None,
     ):
```

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/github.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/github.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/adapter.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/adapter.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/fields.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/lib.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/base.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/date.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/date.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/parsing/number.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/parsing/number.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/types.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/gsheets/typing.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/gsheets/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/html_table.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/html_table.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/s3select.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/s3select.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/socrata.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/socrata.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/system.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/system.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/api/weatherapi.py` & `shillelagh-1.2.2/src/shillelagh/adapters/api/weatherapi.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/base.py` & `shillelagh-1.2.2/src/shillelagh/adapters/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/file/csvfile.py` & `shillelagh-1.2.2/src/shillelagh/adapters/file/csvfile.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/memory/pandas.py` & `shillelagh-1.2.2/src/shillelagh/adapters/memory/pandas.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/adapters/registry.py` & `shillelagh-1.2.2/src/shillelagh/adapters/registry.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/backends/apsw/db.py` & `shillelagh-1.2.2/src/shillelagh/backends/apsw/db.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/base.py` & `shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/base.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/gsheets.py` & `shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/gsheets.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/backends/apsw/dialects/safe.py` & `shillelagh-1.2.2/src/shillelagh/backends/apsw/dialects/safe.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/backends/apsw/vt.py` & `shillelagh-1.2.2/src/shillelagh/backends/apsw/vt.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/console.py` & `shillelagh-1.2.2/src/shillelagh/console.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/exceptions.py` & `shillelagh-1.2.2/src/shillelagh/exceptions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/fields.py` & `shillelagh-1.2.2/src/shillelagh/fields.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/filters.py` & `shillelagh-1.2.2/src/shillelagh/filters.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/functions.py` & `shillelagh-1.2.2/src/shillelagh/functions.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/lib.py` & `shillelagh-1.2.2/src/shillelagh/lib.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/types.py` & `shillelagh-1.2.2/src/shillelagh/types.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh/typing.py` & `shillelagh-1.2.2/src/shillelagh/typing.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh.egg-info/PKG-INFO` & `shillelagh-1.2.2/src/shillelagh.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shillelagh
-Version: 1.2.1
+Version: 1.2.2
 Summary: Making it easy to query APIs via SQL
 Home-page: https://github.com/betodealmeida/shillelagh/
 Author: Beto Dealmeida
 Author-email: roberto@dealmeida.net
 License: mit
 Project-URL: Documentation, https://shillelagh.readthedocs.io/
 Description: ==========
```

### Comparing `shillelagh-1.2.1/src/shillelagh.egg-info/SOURCES.txt` & `shillelagh-1.2.2/src/shillelagh.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh.egg-info/entry_points.txt` & `shillelagh-1.2.2/src/shillelagh.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/src/shillelagh.egg-info/requires.txt` & `shillelagh-1.2.2/src/shillelagh.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 requests-cache==0.7.1
 
 [docs]
 sphinx>=4.0.1
 
 [genericjsonapi]
 jsonpath-python>=1.0.5
+prison>=0.2.1
 requests-cache==0.7.1
 
 [githubapi]
 jsonpath-python>=1.0.5
 
 [gsheetsapi]
 google-auth>=1.23.0
@@ -87,14 +88,15 @@
 freezegun>=1.1.0
 google-auth>=1.23.0
 html5lib>=1.1
 jsonpath-python>=1.0.5
 pandas>=1.2.2
 pip-tools>=6.4.0
 pre-commit>=2.13.0
+prison>=0.2.1
 prompt_toolkit>=3
 psutil>=5.8.0
 pyfakefs>=4.3.3
 pygments>=2.8
 pylint>=2.16.2
 pytest-cov>=2.11.1
 pytest-integration==0.2.2
```

### Comparing `shillelagh-1.2.1/talks/Python Brasil 2021.pdf` & `shillelagh-1.2.2/talks/Python Brasil 2021.pdf`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py` & `shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/test_{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py` & `shillelagh-1.2.2/templates/adapter/{{cookiecutter.slug}}/{{cookiecutter.slug}}.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/datasette_test.py` & `shillelagh-1.2.2/tests/adapters/api/datasette_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/generic_json_test.py` & `shillelagh-1.2.2/tests/adapters/api/generic_json_test.py`

 * *Files 9% similar despite different names*

```diff
@@ -201,7 +201,48 @@
     )
     cursor = connection.cursor()
 
     sql = f'SELECT * FROM "{url}"'
     rows = list(cursor.execute(sql))
     assert rows == [("bar", '["one", "two"]')]
     assert data.last_request.headers["foo"] == "bar"
+
+
+def test_request_headers_in_url(mocker: MockerFixture, requests_mock: Mocker) -> None:
+    """
+    Test passing requests headers.
+    """
+    mocker.patch("shillelagh.adapters.api.generic_json.CACHE_EXPIRATION", 0)
+    supports = requests_mock.head(
+        "https://example.org/data.json",
+        headers={"content-type": "application/json"},
+    )
+
+    # for datassette and other probing adapters
+    requests_mock.head("https://exmaple.org/-/versions.json", status_code=404)
+
+    url = URL("https://example.org/")
+    data = requests_mock.head(str(url), headers={"content-type": "application/json"})
+    requests_mock.get(
+        str(url),
+        json=[
+            {
+                "foo": "bar",
+                "baz": ["one", "two"],
+            },
+        ],
+    )
+
+    # test the supports method
+    GenericJSONAPI.supports(
+        "https://example.org/data.json?_s_headers=(foo:bar)",
+        fast=False,
+    )
+    assert supports.last_request.headers["foo"] == "bar"
+
+    connection = connect(":memory:")
+    cursor = connection.cursor()
+
+    sql = 'SELECT * FROM "https://example.org/?_s_headers=(foo:bar)"'
+    rows = list(cursor.execute(sql))
+    assert rows == [("bar", '["one", "two"]')]
+    assert data.last_request.headers["foo"] == "bar"
```

### Comparing `shillelagh-1.2.1/tests/adapters/api/github_test.py` & `shillelagh-1.2.2/tests/adapters/api/github_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/adapter_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/adapter_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/fields_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/integration_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/integration_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/lib_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/base_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/date_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/date_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/gsheets/parsing/number_test.py` & `shillelagh-1.2.2/tests/adapters/api/gsheets/parsing/number_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/html_table_test.py` & `shillelagh-1.2.2/tests/adapters/api/html_table_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/s3select_test.py` & `shillelagh-1.2.2/tests/adapters/api/s3select_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/socrata_test.py` & `shillelagh-1.2.2/tests/adapters/api/socrata_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/system_test.py` & `shillelagh-1.2.2/tests/adapters/api/system_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/api/weatherapi_test.py` & `shillelagh-1.2.2/tests/adapters/api/weatherapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/base_test.py` & `shillelagh-1.2.2/tests/adapters/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/file/csvfile_test.py` & `shillelagh-1.2.2/tests/adapters/file/csvfile_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/memory/pandas_test.py` & `shillelagh-1.2.2/tests/adapters/memory/pandas_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/adapters/registry_test.py` & `shillelagh-1.2.2/tests/adapters/registry_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/backends/apsw/db_test.py` & `shillelagh-1.2.2/tests/backends/apsw/db_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/backends/apsw/dbapi_test.py` & `shillelagh-1.2.2/tests/backends/apsw/dbapi_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/backends/apsw/dialects/base_test.py` & `shillelagh-1.2.2/tests/backends/apsw/dialects/base_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/backends/apsw/dialects/gsheets_test.py` & `shillelagh-1.2.2/tests/backends/apsw/dialects/gsheets_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/backends/apsw/dialects/safe_test.py` & `shillelagh-1.2.2/tests/backends/apsw/dialects/safe_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/backends/apsw/vt_test.py` & `shillelagh-1.2.2/tests/backends/apsw/vt_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/conftest.py` & `shillelagh-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/console_test.py` & `shillelagh-1.2.2/tests/console_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/__init__.py` & `shillelagh-1.2.2/tests/fakes/__init__.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/cdc_data_response.json` & `shillelagh-1.2.2/tests/fakes/cdc_data_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/cdc_metadata_response.json` & `shillelagh-1.2.2/tests/fakes/cdc_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/datasette_columns_response.json` & `shillelagh-1.2.2/tests/fakes/datasette_columns_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/datasette_data_response_1.json` & `shillelagh-1.2.2/tests/fakes/datasette_data_response_1.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/datasette_data_response_2.json` & `shillelagh-1.2.2/tests/fakes/datasette_data_response_2.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/datasette_metadata_response.json` & `shillelagh-1.2.2/tests/fakes/datasette_metadata_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/datasette_results.json` & `shillelagh-1.2.2/tests/fakes/datasette_results.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/github_response.json` & `shillelagh-1.2.2/tests/fakes/github_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/github_single_response.json` & `shillelagh-1.2.2/tests/fakes/github_single_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/incidents.json` & `shillelagh-1.2.2/tests/fakes/incidents.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fakes/weatherapi_response.json` & `shillelagh-1.2.2/tests/fakes/weatherapi_response.json`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/fields_test.py` & `shillelagh-1.2.2/tests/fields_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/filters_test.py` & `shillelagh-1.2.2/tests/filters_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/functions_test.py` & `shillelagh-1.2.2/tests/functions_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/lib_test.py` & `shillelagh-1.2.2/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `shillelagh-1.2.1/tests/types_test.py` & `shillelagh-1.2.2/tests/types_test.py`

 * *Files identical despite different names*

