# Comparing `tmp/xtgeoviz-0.0.5.tar.gz` & `tmp/xtgeoviz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xtgeoviz-0.0.5.tar", last modified: Wed Mar 15 13:22:36 2023, max compression
+gzip compressed data, was "xtgeoviz-0.0.6.tar", last modified: Tue Apr 18 10:31:32 2023, max compression
```

## Comparing `xtgeoviz-0.0.5.tar` & `xtgeoviz-0.0.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.981991 xtgeoviz-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.973991 xtgeoviz-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/.github/workflows/ci-xtgeoviz.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/.github/workflows/xtgeoviz-publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-15 13:22:36.981991 xtgeoviz-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/docs/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/pytest.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/requirements/requirements_docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/requirements/requirements_setup.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/requirements/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/requirements/requirements_testx.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/scripts/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/scripts/setup_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-03-15 13:22:36.981991 xtgeoviz-0.0.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.973991 xtgeoviz-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/src/xtgeoviz/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/src/xtgeoviz/frontends/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/frontends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/frontends/_xsectplotting_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/frontends/_xsectplotting_load.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/frontends/_xsectplotting_plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/frontends/xsectplotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/src/xtgeoviz/mpl/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/_colortables.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/_libwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/baseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/grid3d_slice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/quickplot.py
--rw-r--r--   0 runner    (1001) docker     (123)    37790 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/xsection.py
--rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/src/xtgeoviz/mpl/xtmap.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-15 13:22:36.000000 xtgeoviz-0.0.5/src/xtgeoviz/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/src/xtgeoviz.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-15 13:22:36.000000 xtgeoviz-0.0.5/src/xtgeoviz.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-03-15 13:22:36.000000 xtgeoviz-0.0.5/src/xtgeoviz.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 13:22:36.000000 xtgeoviz-0.0.5/src/xtgeoviz.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-03-15 13:22:36.000000 xtgeoviz-0.0.5/src/xtgeoviz.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-15 13:22:36.000000 xtgeoviz-0.0.5/src/xtgeoviz.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.973991 xtgeoviz-0.0.5/tests/baseline_images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.977991 xtgeoviz-0.0.5/tests/baseline_images/test_baseplot/
--rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/tests/baseline_images/test_baseplot/canvas.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.981991 xtgeoviz-0.0.5/tests/baseline_images/test_regularsurface/
--rw-r--r--   0 runner    (1001) docker     (123)    45755 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/tests/baseline_images/test_regularsurface/quickplot1.png
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.981991 xtgeoviz-0.0.5/tests/test_mpl/
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/tests/test_mpl/test_baseplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/tests/test_mpl/test_regularsurface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 13:22:36.981991 xtgeoviz-0.0.5/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-03-15 13:22:19.000000 xtgeoviz-0.0.5/tests/test_scripts/test_xsectplot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.897888 xtgeoviz-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.github/workflows/ci-xtgeoviz.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.github/workflows/xtgeoviz-publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/docs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3144 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/pytest.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_setup.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/requirements/requirements_testx.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/scripts/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/scripts/setup_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2258 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.897888 xtgeoviz-0.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/src/xtgeoviz/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/src/xtgeoviz/frontends/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9232 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/frontends/xsectplotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/src/xtgeoviz/mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12019 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/_colortables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/_libwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8617 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/baseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6775 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/grid3d_slice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2524 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/quickplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37790 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/xsection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7691 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/src/xtgeoviz/mpl/xtmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.901888 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1354 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 10:31:32.000000 xtgeoviz-0.0.6/src/xtgeoviz.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.897888 xtgeoviz-0.0.6/tests/baseline_images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/baseline_images/test_baseplot/
+-rw-r--r--   0 runner    (1001) docker     (123)    19739 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/baseline_images/test_baseplot/canvas.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/baseline_images/test_regularsurface/
+-rw-r--r--   0 runner    (1001) docker     (123)    45755 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/baseline_images/test_regularsurface/quickplot1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/test_mpl/
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/test_mpl/test_baseplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/test_mpl/test_regularsurface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 10:31:32.905888 xtgeoviz-0.0.6/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     5194 2023-04-18 10:31:20.000000 xtgeoviz-0.0.6/tests/test_scripts/test_xsectplot.py
```

### Comparing `xtgeoviz-0.0.5/.github/workflows/ci-xtgeoviz.yml` & `xtgeoviz-0.0.6/.github/workflows/ci-xtgeoviz.yml`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/.github/workflows/xtgeoviz-publish-pypi.yml` & `xtgeoviz-0.0.6/.github/workflows/xtgeoviz-publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/.gitignore` & `xtgeoviz-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/.pylintrc` & `xtgeoviz-0.0.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/LICENSE` & `xtgeoviz-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/PKG-INFO` & `xtgeoviz-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtgeoviz
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plotting library for xtgeo objects
 Home-page: https://github.com/equinor/xtgeoviz
 Author: Equinor
 Author-email: ____@equinor.com
 License: LGPL-3.0
 Project-URL: Documentation, https://xtgeoviz.notyet_on_readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/equinor/xtgeoviz/issues
```

### Comparing `xtgeoviz-0.0.5/docs/conf.py` & `xtgeoviz-0.0.6/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/pyproject.toml` & `xtgeoviz-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/scripts/setup_functions.py` & `xtgeoviz-0.0.6/scripts/setup_functions.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/setup.py` & `xtgeoviz-0.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/frontends/_xsectplotting_config.py` & `xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_config.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/frontends/_xsectplotting_load.py` & `xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_load.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/frontends/_xsectplotting_plotting.py` & `xtgeoviz-0.0.6/src/xtgeoviz/frontends/_xsectplotting_plotting.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/frontends/xsectplotting.py` & `xtgeoviz-0.0.6/src/xtgeoviz/frontends/xsectplotting.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/_colortables.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/_colortables.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/_libwrapper.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/_libwrapper.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/baseplot.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/baseplot.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/grid3d_slice.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/grid3d_slice.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/quickplot.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/quickplot.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/xsection.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/xsection.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz/mpl/xtmap.py` & `xtgeoviz-0.0.6/src/xtgeoviz/mpl/xtmap.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz.egg-info/PKG-INFO` & `xtgeoviz-0.0.6/src/xtgeoviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtgeoviz
-Version: 0.0.5
+Version: 0.0.6
 Summary: Plotting library for xtgeo objects
 Home-page: https://github.com/equinor/xtgeoviz
 Author: Equinor
 Author-email: ____@equinor.com
 License: LGPL-3.0
 Project-URL: Documentation, https://xtgeoviz.notyet_on_readthedocs.io/
 Project-URL: Issue Tracker, https://github.com/equinor/xtgeoviz/issues
```

### Comparing `xtgeoviz-0.0.5/src/xtgeoviz.egg-info/SOURCES.txt` & `xtgeoviz-0.0.6/src/xtgeoviz.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/tests/baseline_images/test_baseplot/canvas.png` & `xtgeoviz-0.0.6/tests/baseline_images/test_baseplot/canvas.png`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/tests/baseline_images/test_regularsurface/quickplot1.png` & `xtgeoviz-0.0.6/tests/baseline_images/test_regularsurface/quickplot1.png`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/tests/test_mpl/test_baseplot.py` & `xtgeoviz-0.0.6/tests/test_mpl/test_baseplot.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/tests/test_mpl/test_regularsurface.py` & `xtgeoviz-0.0.6/tests/test_mpl/test_regularsurface.py`

 * *Files identical despite different names*

### Comparing `xtgeoviz-0.0.5/tests/test_scripts/test_xsectplot.py` & `xtgeoviz-0.0.6/tests/test_scripts/test_xsectplot.py`

 * *Files identical despite different names*

