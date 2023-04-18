# Comparing `tmp/swh.scrubber-1.0.2.tar.gz` & `tmp/swh.scrubber-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.scrubber-1.0.2.tar", last modified: Tue Mar 28 13:16:03 2023, max compression
+gzip compressed data, was "dist/swh.scrubber-1.0.3.tar", last modified: Tue Apr 18 15:50:00 2023, max compression
```

## Comparing `swh.scrubber-1.0.2.tar` & `swh.scrubber-1.0.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/
--rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     2329 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1408 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/README.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1408 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/README.rst
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      156 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)      246 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      365 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      222 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       49 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh/scrubber/
--rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8189 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18626 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/db.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7601 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2764 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/journal_checker.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3052 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/origin_locator.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/py.typed
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh/scrubber/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/20-enums.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5048 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2911 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/60-indexes.sql
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)      942 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/2.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/3.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      989 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/4.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/5.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    15752 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/storage_checker.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh/scrubber/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/conftest.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12050 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/storage_checker_tests.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5345 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2693 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_db.py
--rw-r--r--   0 jenkins    (115) docker     (999)    11471 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_fixer.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1053 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3913 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_journal_kafka.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5408 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_origin_locator.py
--rw-r--r--   0 jenkins    (115) docker     (999)      830 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_storage_cassandra.py
--rw-r--r--   0 jenkins    (115) docker     (999)      780 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/tests/test_storage_postgresql.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/swh/scrubber/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     2329 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     1499 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       50 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      184 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-03-28 13:16:03.000000 swh.scrubber-1.0.2/swh.scrubber.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1514 2023-03-28 13:16:01.000000 swh.scrubber-1.0.2/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/
+-rw-r--r--   0 jenkins    (115) docker     (999)       83 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1039 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)      149 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     2329 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1408 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/README.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1408 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/README.rst
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      156 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      246 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      413 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      222 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       57 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      252 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2454 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/
+-rw-r--r--   0 jenkins    (115) docker     (999)      727 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8189 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18626 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7601 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2764 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/journal_checker.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3052 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/origin_locator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/py.typed
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)      201 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/20-enums.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5048 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2911 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/60-indexes.sql
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)      942 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/2.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2338 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/3.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      989 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/4.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1567 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/5.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    16545 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/storage_checker.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh/scrubber/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      901 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/conftest.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    14324 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/storage_checker_tests.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5345 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2693 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_db.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    11471 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_fixer.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1053 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3913 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_journal_kafka.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5408 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_origin_locator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1035 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_cassandra.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      780 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_postgresql.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1671 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/swh/scrubber/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2329 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     1499 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       50 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      192 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-04-18 15:50:00.000000 swh.scrubber-1.0.3/swh.scrubber.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1514 2023-04-18 15:49:58.000000 swh.scrubber-1.0.3/tox.ini
```

### Comparing `swh.scrubber-1.0.2/.pre-commit-config.yaml` & `swh.scrubber-1.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/CODE_OF_CONDUCT.md` & `swh.scrubber-1.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/LICENSE` & `swh.scrubber-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/PKG-INFO` & `swh.scrubber-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scrubber
-Version: 1.0.2
+Version: 1.0.3
 Summary: Software Heritage Datastore Scrubber
 Home-page: https://forge.softwareheritage.org/diffusion/swh-scrubber
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scrubber
```

### Comparing `swh.scrubber-1.0.2/README.rst` & `swh.scrubber-1.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/docs/README.rst` & `swh.scrubber-1.0.3/docs/README.rst`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/setup.py` & `swh.scrubber-1.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/__init__.py` & `swh.scrubber-1.0.3/swh/scrubber/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/cli.py` & `swh.scrubber-1.0.3/swh/scrubber/cli.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/db.py` & `swh.scrubber-1.0.3/swh/scrubber/db.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/fixer.py` & `swh.scrubber-1.0.3/swh/scrubber/fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/journal_checker.py` & `swh.scrubber-1.0.3/swh/scrubber/journal_checker.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/origin_locator.py` & `swh.scrubber-1.0.3/swh/scrubber/origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/sql/30-schema.sql` & `swh.scrubber-1.0.3/swh/scrubber/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/sql/60-indexes.sql` & `swh.scrubber-1.0.3/swh/scrubber/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/2.sql` & `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/2.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/3.sql` & `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/3.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/4.sql` & `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/4.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/sql/upgrades/5.sql` & `swh.scrubber-1.0.3/swh/scrubber/sql/upgrades/5.sql`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/storage_checker.py` & `swh.scrubber-1.0.3/swh/scrubber/storage_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
     Directory,
     ObjectType,
     Release,
     Revision,
     Snapshot,
     TargetType,
 )
-from swh.storage.algos.directory import directory_get_many
+from swh.storage.algos.directory import (
+    directory_get_many_with_possibly_duplicated_entries,
+)
 from swh.storage.algos.snapshot import snapshot_get_all_branches
 from swh.storage.cassandra.storage import CassandraStorage
 from swh.storage.interface import StorageInterface
 from swh.storage.postgresql.storage import Storage as PostgresqlStorage
 
 from .db import Datastore, ScrubberDb
 
@@ -209,15 +211,31 @@
                 page = method(partition_id, self.nb_partitions, page_token=page_token)
                 objects = page.results
             elif object_type == swhids.ObjectType.DIRECTORY:
                 page = self.storage.directory_get_id_partition(
                     partition_id, self.nb_partitions, page_token=page_token
                 )
                 directory_ids = page.results
-                objects = list(directory_get_many(self.storage, directory_ids))
+                objects = []
+                for (dir_id, item) in zip(
+                    directory_ids,
+                    directory_get_many_with_possibly_duplicated_entries(
+                        self.storage, directory_ids
+                    ),
+                ):
+                    assert item is not None, f"Directory {dir_id.hex()} disappeared"
+                    (has_duplicate_entries, object_) = item
+                    if has_duplicate_entries:
+                        self.statsd().increment("duplicate_directory_entries_total")
+                        self.db.corrupt_object_add(
+                            object_.swhid(),
+                            self.datastore_info(),
+                            value_to_kafka(object_.to_dict()),
+                        )
+                    objects.append(object_)
             elif object_type == swhids.ObjectType.SNAPSHOT:
                 page = self.storage.snapshot_get_id_partition(
                     partition_id, self.nb_partitions, page_token=page_token
                 )
                 snapshot_ids = page.results
                 objects = [
                     snapshot_get_all_branches(self.storage, snapshot_id)
```

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/conftest.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/storage_checker_tests.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/storage_checker_tests.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 import datetime
 
 import attr
+import msgpack
 import pytest
 
 from swh.journal.serializers import kafka_to_value
 from swh.model import model, swhids
 from swh.model.tests import swh_model_data
 from swh.scrubber.storage_checker import StorageChecker
 
@@ -219,14 +220,79 @@
     assert_checked_ranges(
         scrubber_db,
         datastore,
         {(swhids.ObjectType.SNAPSHOT, 0, 2), (swhids.ObjectType.SNAPSHOT, 1, 2)},
     )
 
 
+def test_directory_duplicate_entries(scrubber_db, datastore, swh_storage):
+    run_validators = attr.get_run_validators()
+    attr.set_run_validators(False)
+    try:
+        invalid_directory = model.Directory(
+            entries=(
+                model.DirectoryEntry(
+                    name=b"foo", type="dir", target=b"\x01" * 20, perms=1
+                ),
+                model.DirectoryEntry(
+                    name=b"foo", type="file", target=b"\x00" * 20, perms=0
+                ),
+            )
+        )
+    finally:
+        attr.set_run_validators(run_validators)
+    swh_storage.directory_add([invalid_directory])
+
+    deduplicated_directory = model.Directory(
+        id=invalid_directory.id,
+        entries=(
+            model.DirectoryEntry(name=b"foo", type="dir", target=b"\x01" * 20, perms=1),
+            model.DirectoryEntry(
+                name=b"foo_0000000000", type="file", target=b"\x00" * 20, perms=0
+            ),
+        ),
+        raw_manifest=(
+            # fmt: off
+            b"tree 52\x00"
+            + b"0 foo\x00" + b"\x00" * 20
+            + b"1 foo\x00" + b"\x01" * 20
+            # fmt: on
+        ),
+    )
+
+    before_date = datetime.datetime.now(tz=datetime.timezone.utc)
+    for object_type in ("snapshot", "release", "revision", "directory"):
+        StorageChecker(
+            db=scrubber_db,
+            storage=swh_storage,
+            object_type=object_type,
+            start_partition_id=0,
+            end_partition_id=1,
+            nb_partitions=1,
+        ).run()
+    after_date = datetime.datetime.now(tz=datetime.timezone.utc)
+
+    corrupt_objects = list(scrubber_db.corrupt_object_iter())
+    assert len(corrupt_objects) == 1
+    assert corrupt_objects[0].id == invalid_directory.swhid()
+    assert corrupt_objects[0].datastore == datastore
+    assert (
+        before_date - datetime.timedelta(seconds=5)
+        <= corrupt_objects[0].first_occurrence
+        <= after_date + datetime.timedelta(seconds=5)
+    )
+    assert kafka_to_value(corrupt_objects[0].object_) == msgpack.loads(
+        msgpack.dumps(deduplicated_directory.to_dict())  # turn entry list into tuple
+    )
+
+    assert_checked_ranges(
+        scrubber_db, datastore, EXPECTED_PARTITIONS, before_date, after_date
+    )
+
+
 def test_no_recheck(scrubber_db, datastore, swh_storage):
     """
     Tests that objects that were already checked are not checked again on
     the next run.
     """
     # Corrupt two snapshots
     snapshots = list(swh_model_data.SNAPSHOTS)
```

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_cli.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_db.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_db.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_fixer.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_fixer.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_init.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_journal_kafka.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_journal_kafka.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_origin_locator.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_origin_locator.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_storage_cassandra.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_cassandra.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,7 +26,15 @@
             {
                 "keyspace": swh_storage.keyspace,
                 "hosts": swh_storage.hosts,
                 "port": swh_storage.port,
             }
         ),
     )
+
+
+@pytest.mark.skip(  # type: ignore[no-redef]
+    "Duplicate directory entries are not representable in Cassandra, "
+    "so this feature is irrelevant"
+)
+def test_directory_duplicate_entries():
+    pass
```

### Comparing `swh.scrubber-1.0.2/swh/scrubber/tests/test_storage_postgresql.py` & `swh.scrubber-1.0.3/swh/scrubber/tests/test_storage_postgresql.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh/scrubber/utils.py` & `swh.scrubber-1.0.3/swh/scrubber/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/swh.scrubber.egg-info/PKG-INFO` & `swh.scrubber-1.0.3/swh.scrubber.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scrubber
-Version: 1.0.2
+Version: 1.0.3
 Summary: Software Heritage Datastore Scrubber
 Home-page: https://forge.softwareheritage.org/diffusion/swh-scrubber
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scrubber
```

### Comparing `swh.scrubber-1.0.2/swh.scrubber.egg-info/SOURCES.txt` & `swh.scrubber-1.0.3/swh.scrubber.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `swh.scrubber-1.0.2/tox.ini` & `swh.scrubber-1.0.3/tox.ini`

 * *Files identical despite different names*

