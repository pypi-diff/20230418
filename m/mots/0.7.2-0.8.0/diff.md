# Comparing `tmp/mots-0.7.2.tar.gz` & `tmp/mots-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mots-0.7.2.tar", last modified: Thu Feb  9 21:04:44 2023, max compression
+gzip compressed data, was "mots-0.8.0.tar", last modified: Tue Apr 18 15:00:12 2023, max compression
```

## Comparing `mots-0.7.2.tar` & `mots-0.8.0.tar`

### file list

```diff
@@ -1,64 +1,65 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.791437 mots-0.7.2/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.787438 mots-0.7.2/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-02-09 21:04:13.000000 mots-0.7.2/.circleci/config.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-02-09 21:04:13.000000 mots-0.7.2/.coveragerc
--rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-02-09 21:04:13.000000 mots-0.7.2/.flake8
--rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-02-09 21:04:13.000000 mots-0.7.2/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2023-02-09 21:04:13.000000 mots-0.7.2/.readthedocs.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-02-09 21:04:13.000000 mots-0.7.2/AUTHORS
--rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-02-09 21:04:13.000000 mots-0.7.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16727 2023-02-09 21:04:13.000000 mots-0.7.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-02-09 21:04:13.000000 mots-0.7.2/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-02-09 21:04:44.791437 mots-0.7.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      984 2023-02-09 21:04:13.000000 mots-0.7.2/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-02-09 21:04:13.000000 mots-0.7.2/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.787438 mots-0.7.2/documentation/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-02-09 21:04:13.000000 mots-0.7.2/documentation/Makefile
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-02-09 21:04:13.000000 mots-0.7.2/documentation/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13662 2023-02-09 21:04:13.000000 mots-0.7.2/documentation/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-02-09 21:04:13.000000 mots-0.7.2/mots.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-02-09 21:04:13.000000 mots-0.7.2/mots.yaml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-02-09 21:04:13.000000 mots-0.7.2/pyproject.toml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.787438 mots-0.7.2/requirements/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-02-09 21:04:13.000000 mots-0.7.2/requirements/base.in
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      159 2023-02-09 21:04:13.000000 mots-0.7.2/requirements/get_filename
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33052 2023-02-09 21:04:13.000000 mots-0.7.2/requirements/python3.10.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35675 2023-02-09 21:04:13.000000 mots-0.7.2/requirements/python3.7.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33297 2023-02-09 21:04:13.000000 mots-0.7.2/requirements/python3.8.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33276 2023-02-09 21:04:13.000000 mots-0.7.2/requirements/python3.9.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1053 2023-02-09 21:04:44.791437 mots-0.7.2/setup.cfg
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.783437 mots-0.7.2/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.791437 mots-0.7.2/src/mots/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2489 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/bmo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/ci.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15263 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14341 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7732 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/export.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/mach_interface.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/module.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/pmo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.791437 mots-0.7.2/src/mots/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/templates/directory.template.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2952 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-02-09 21:04:13.000000 mots-0.7.2/src/mots/yaml.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.791437 mots-0.7.2/src/mots.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-02-09 21:04:44.000000 mots-0.7.2/src/mots.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1099 2023-02-09 21:04:44.000000 mots-0.7.2/src/mots.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-09 21:04:44.000000 mots-0.7.2/src/mots.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-02-09 21:04:44.000000 mots-0.7.2/src/mots.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-02-09 21:04:44.000000 mots-0.7.2/src/mots.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-02-09 21:04:44.000000 mots-0.7.2/src/mots.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-09 21:04:44.791437 mots-0.7.2/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4618 2023-02-09 21:04:13.000000 mots-0.7.2/tests/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9829 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6862 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_directory.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_export.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5727 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_module.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_settings.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_style.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4489 2023-02-09 21:04:13.000000 mots-0.7.2/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.531195 mots-0.8.0/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-04-18 14:59:25.000000 mots-0.8.0/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       24 2023-04-18 14:59:25.000000 mots-0.8.0/.coveragerc
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      415 2023-04-18 14:59:25.000000 mots-0.8.0/.flake8
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       88 2023-04-18 14:59:25.000000 mots-0.8.0/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2023-04-18 14:59:25.000000 mots-0.8.0/.readthedocs.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       32 2023-04-18 14:59:25.000000 mots-0.8.0/AUTHORS
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      495 2023-04-18 14:59:25.000000 mots-0.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16727 2023-04-18 14:59:25.000000 mots-0.8.0/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3813 2023-04-18 14:59:25.000000 mots-0.8.0/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-18 15:00:12.535194 mots-0.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      984 2023-04-18 14:59:25.000000 mots-0.8.0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1447 2023-04-18 14:59:25.000000 mots-0.8.0/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.531195 mots-0.8.0/documentation/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      634 2023-04-18 14:59:25.000000 mots-0.8.0/documentation/Makefile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2153 2023-04-18 14:59:25.000000 mots-0.8.0/documentation/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13728 2023-04-18 14:59:25.000000 mots-0.8.0/documentation/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      454 2023-04-18 14:59:25.000000 mots-0.8.0/mots.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      795 2023-04-18 14:59:25.000000 mots-0.8.0/mots.yaml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      456 2023-04-18 14:59:25.000000 mots-0.8.0/pyproject.toml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.531195 mots-0.8.0/requirements/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/base.in
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      159 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/get_filename
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33052 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.10.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35675 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.7.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33297 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.8.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33276 2023-04-18 14:59:25.000000 mots-0.8.0/requirements/python3.9.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1053 2023-04-18 15:00:12.535194 mots-0.8.0/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.527194 mots-0.8.0/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/src/mots/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2489 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/bmo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      808 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/ci.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15263 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14341 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7732 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6454 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/export.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      713 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/mach_interface.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6937 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/pmo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2748 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/src/mots/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/templates/directory.template.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2381 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/templates/directory.template.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2952 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      536 2023-04-18 14:59:25.000000 mots-0.8.0/src/mots/yaml.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/src/mots.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      635 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1140 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       54 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        5 2023-04-18 15:00:12.000000 mots-0.8.0/src/mots.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-04-18 15:00:12.535194 mots-0.8.0/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4618 2023-04-18 14:59:25.000000 mots-0.8.0/tests/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9829 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6862 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_directory.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5225 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_export.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5727 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_module.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1749 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_settings.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_style.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4489 2023-04-18 14:59:25.000000 mots-0.8.0/tests/test_utils.py
```

### Comparing `mots-0.7.2/.circleci/config.yml` & `mots-0.8.0/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/LICENSE` & `mots-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/Makefile` & `mots-0.8.0/Makefile`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/PKG-INFO` & `mots-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mots
-Version: 0.7.2
+Version: 0.8.0
 Summary: Module Ownership in Tree System
 Home-page: https://github.com/mozilla-conduit/mots
 Author: Zeid Zabaneh
 Author-email: zeid@mozilla.com
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mots-0.7.2/README.md` & `mots-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/docker-compose.yml` & `mots-0.8.0/docker-compose.yml`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/documentation/Makefile` & `mots-0.8.0/documentation/Makefile`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/documentation/conf.py` & `mots-0.8.0/documentation/conf.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/documentation/index.rst` & `mots-0.8.0/documentation/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -268,15 +268,15 @@
 
 There is currently a known issue where the first pass of ``mots clean`` will fail if the other keys are missing from the new entry. If you run into a ``KeyError``, just run ``mots clean`` again. This issue is being tracked in `bug 1797083 <https://bugzilla.mozilla.org/show_bug.cgi?id=1797083>`_.
 
 
 Cleaning **mots.yaml**
 ----------------------
 
-Before changes to module information is merged into the repo, those changes should be cleaned and exported. Both the validated and cleaned **mots.yaml** as well as any exported documentation files need to be checked in and updated. A convenience command, ``mots export-and-clean`` is provided that will do both things.
+Before changes to module information is merged into the repo, those changes should be cleaned using the ``mots clean`` command.
 
 Use ``mots clean`` to automatically sort and synchronize data in the **mots.yaml** configuration file. This command requires a ``MOTS_BUGZILLA_API_KEY`` environment variable to be set, or the key to be defined in your settings. You can do this by running the following commands, replacing the redacted key with an actual Bugzilla API key:
 
 .. code-block:: shell
 
     $ mots settings write BUGZILLA_API_KEY
     $ Enter value for BUGZILLA_API_KEY: <hidden input>
@@ -311,15 +311,19 @@
 	$ mots query example.text example_submodule/test2
 	example.text:example
 	example_submodule/test2:example_submodule
 
 
 Exporting
 ---------
-Using the ``mots export`` command, the configuration can be exported in a different format. Currently only `reStructuredText` is supported. This command will output the result to standard output, or export it to the specified path in `mots.yaml`. The export paths and formats should be defined under `export.path` and `export.format`. E.g.,
+.. note::
+    Depending on your repo, the generated exported file may or may not be checked-in (tracked). For example, in mozilla-central, the exported file is automatically generated when running ``mach doc`` and is ignored by source control.
+
+
+Using the ``mots export`` command, the configuration can be exported in a different format. Currently `reStructuredText` and `Markdown` are supported. This command will output the result to standard output, or export it to the specified path in `mots.yaml`. The export paths and formats should be defined under `export.path` and `export.format`. E.g.,
 
 .. code-block:: yaml
 
    ...
    export:
      format: rst
      path: docs/mots.rst
```

### Comparing `mots-0.7.2/mots.yaml` & `mots-0.8.0/mots.yaml`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/requirements/python3.10.txt` & `mots-0.8.0/requirements/python3.10.txt`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/requirements/python3.7.txt` & `mots-0.8.0/requirements/python3.7.txt`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/requirements/python3.8.txt` & `mots-0.8.0/requirements/python3.8.txt`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/requirements/python3.9.txt` & `mots-0.8.0/requirements/python3.9.txt`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/setup.cfg` & `mots-0.8.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/bmo.py` & `mots-0.8.0/src/mots/bmo.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/ci.py` & `mots-0.8.0/src/mots/ci.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/cli.py` & `mots-0.8.0/src/mots/cli.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/config.py` & `mots-0.8.0/src/mots/config.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/directory.py` & `mots-0.8.0/src/mots/directory.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/export.py` & `mots-0.8.0/src/mots/export.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,14 +30,23 @@
     # First we must escape backslashes, then everything else.
     characters = ("\\", "*", "`")
     for character in characters:
         value = value.replace(character, f"\\{character}")
     return value
 
 
+def escape_for_md(value: str) -> str:
+    """Escape rst special characters."""
+    # First we must escape backslashes, then everything else.
+    characters = "\\`*_{}[]<>()#+-.!|"
+    for character in characters:
+        value = value.replace(character, f"\\{character}")
+    return value
+
+
 def format_paths_for_rst(
     value: list[str], indent: int, directory: Directory = None
 ) -> str:
     """Escape and format a path string (e.g. for includes or excludes)."""
     config = directory.config_handle.config
     try:
         searchfox_enabled = config["export"]["searchfox_enabled"]
@@ -52,14 +61,36 @@
                 f"`{path} <{settings.SEARCHFOX_BASE_URL}"
                 f"/{config['repo']}/search?q=&path={path}>`__"
             )
         parsed_paths.append(path)
     return f"\n{' ' * indent}| " + f"\n{' ' * indent}| ".join(parsed_paths)
 
 
+def format_paths_for_md(
+    value: list[str], indent: int, directory: Directory = None
+) -> str:
+    """Escape and format a path string (e.g. for includes or excludes)."""
+    config = directory.config_handle.config
+    try:
+        searchfox_enabled = config["export"]["searchfox_enabled"]
+    except KeyError:
+        searchfox_enabled = False
+
+    parsed_paths = []
+    for path in value:
+        path = path.replace("*", "\\*")
+        if searchfox_enabled:
+            path = (
+                f"[{path}]({settings.SEARCHFOX_BASE_URL}"
+                f"/{config['repo']}/search?q=&path={path})"
+            )
+        parsed_paths.append(path)
+    return f"\n{' ' * indent}* " + f"\n{' ' * indent}* ".join(parsed_paths)
+
+
 def format_people_for_rst(value: list[dict], indent: int) -> str:
     """Escape and format a list of people."""
     people_base_url = settings.PMO_SEARCH_URL
     parsed_people = []
     for person in value:
         if "name" in person and person["name"]:
             parsed_person = (
@@ -69,14 +100,31 @@
         else:
             parsed_person = f"`{person['nick']} <{people_base_url}{person['nick']}>`__"
 
         parsed_people.append(parsed_person)
     return f"\n{' ' * indent}| " + f"\n{' ' * indent}| ".join(parsed_people)
 
 
+def format_people_for_md(value: list[dict], indent: int) -> str:
+    """Escape and format a list of people."""
+    people_base_url = settings.PMO_SEARCH_URL
+    parsed_people = []
+    for person in value:
+        if "name" in person and person["name"]:
+            parsed_person = (
+                f"[{person['name']} ({person['nick']})]"
+                f"({people_base_url}{person['nick']})"
+            )
+        else:
+            parsed_person = f"[{person['nick']}]({people_base_url}{person['nick']})"
+
+        parsed_people.append(parsed_person)
+    return f"\n{' ' * indent}* " + f"\n{' ' * indent}* ".join(parsed_people)
+
+
 def format_emeritus(value: list[dict | str]) -> str:
     """Return names of people if provided a mixed list."""
     parsed = []
     for person in value:
         if isinstance(person, str):
             parsed.append(person)
         elif isinstance(person, dict):
@@ -96,14 +144,17 @@
         loader = jinja2.FileSystemLoader(
             searchpath=importlib_resources.files("mots") / "templates"
         )
         env = jinja2.Environment(loader=loader, trim_blocks=True, lstrip_blocks=True)
         env.filters["escape_for_rst"] = escape_for_rst
         env.filters["format_paths_for_rst"] = format_paths_for_rst
         env.filters["format_people_for_rst"] = format_people_for_rst
+        env.filters["escape_for_md"] = escape_for_md
+        env.filters["format_paths_for_md"] = format_paths_for_md
+        env.filters["format_people_for_md"] = format_people_for_md
         env.filters["format_emeritus"] = format_emeritus
         return env
 
     def __init__(self, directory: Directory):
         self.directory = directory
         self.env = self._get_env()
 
@@ -114,16 +165,22 @@
 
     def _export_to_rst(self) -> str:
         """Render the template with this instance's directory context and return it."""
         template = self._get_template("rst")
         out = template.render(directory=self.directory)
         return f"{out.strip()}\n"
 
+    def _export_to_md(self) -> str:
+        """Render the template with this instance's directory context and return it."""
+        template = self._get_template("md")
+        out = template.render(directory=self.directory)
+        return f"{out.strip()}\n"
+
 
 def export_to_format(directory: Directory, frmt="rst"):
     """Export directory in a specified format."""
-    supported_formats = ["rst"]
+    supported_formats = ["rst", "md"]
     if frmt not in supported_formats:
         raise ValueError(f"{frmt} not one of {supported_formats}.")
 
     exporter = Exporter(directory)
     return getattr(exporter, f"_export_to_{frmt}")()
```

### Comparing `mots-0.7.2/src/mots/logging.py` & `mots-0.8.0/src/mots/logging.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/mach_interface.py` & `mots-0.8.0/src/mots/mach_interface.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/module.py` & `mots-0.8.0/src/mots/module.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/pmo.py` & `mots-0.8.0/src/mots/pmo.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/settings.py` & `mots-0.8.0/src/mots/settings.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/templates/directory.template.rst` & `mots-0.8.0/src/mots/templates/directory.template.rst`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/utils.py` & `mots-0.8.0/src/mots/utils.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots/yaml.py` & `mots-0.8.0/src/mots/yaml.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/src/mots.egg-info/PKG-INFO` & `mots-0.8.0/src/mots.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mots
-Version: 0.7.2
+Version: 0.8.0
 Summary: Module Ownership in Tree System
 Home-page: https://github.com/mozilla-conduit/mots
 Author: Zeid Zabaneh
 Author-email: zeid@mozilla.com
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `mots-0.7.2/src/mots.egg-info/SOURCES.txt` & `mots-0.8.0/src/mots.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,15 @@
 src/mots/yaml.py
 src/mots.egg-info/PKG-INFO
 src/mots.egg-info/SOURCES.txt
 src/mots.egg-info/dependency_links.txt
 src/mots.egg-info/entry_points.txt
 src/mots.egg-info/requires.txt
 src/mots.egg-info/top_level.txt
+src/mots/templates/directory.template.md
 src/mots/templates/directory.template.rst
 tests/conftest.py
 tests/test_cli.py
 tests/test_config.py
 tests/test_directory.py
 tests/test_export.py
 tests/test_module.py
```

### Comparing `mots-0.7.2/tests/conftest.py` & `mots-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/tests/test_config.py` & `mots-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/tests/test_directory.py` & `mots-0.8.0/tests/test_directory.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/tests/test_module.py` & `mots-0.8.0/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/tests/test_settings.py` & `mots-0.8.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/tests/test_style.py` & `mots-0.8.0/tests/test_style.py`

 * *Files identical despite different names*

### Comparing `mots-0.7.2/tests/test_utils.py` & `mots-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

