# Comparing `tmp/kfactory-0.6.0.tar.gz` & `tmp/kfactory-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.6.0.tar", last modified: Tue Apr 18 15:58:51 2023, max compression
+gzip compressed data, was "kfactory-0.6.1.tar", last modified: Tue Apr 18 16:39:37 2023, max compression
```

## Comparing `kfactory-0.6.0.tar` & `kfactory-0.6.1.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 15:58:28.000000 kfactory-0.6.0/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.200440 kfactory-0.6.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.200440 kfactory-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 15:58:28.000000 kfactory-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-18 15:58:28.000000 kfactory-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 15:58:28.000000 kfactory-0.6.0/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 15:58:28.000000 kfactory-0.6.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 15:58:28.000000 kfactory-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 15:58:28.000000 kfactory-0.6.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 15:58:51.208440 kfactory-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 15:58:28.000000 kfactory-0.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/klive.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/notebooks/02_DRC.py
--rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 15:58:28.000000 kfactory-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:58:51.208440 kfactory-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.200440 kfactory-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/generic_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)    80302 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/kcell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/pcells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/pcells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/utils/geo/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22912 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/fill.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.802903 kfactory-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 16:39:17.000000 kfactory-0.6.1/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.790902 kfactory-0.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 16:39:17.000000 kfactory-0.6.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.794902 kfactory-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 16:39:17.000000 kfactory-0.6.1/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 16:39:17.000000 kfactory-0.6.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-18 16:39:17.000000 kfactory-0.6.1/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 16:39:17.000000 kfactory-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-18 16:39:17.000000 kfactory-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 16:39:17.000000 kfactory-0.6.1/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 16:39:17.000000 kfactory-0.6.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 16:39:17.000000 kfactory-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 16:39:17.000000 kfactory-0.6.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 16:39:37.802903 kfactory-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 16:39:17.000000 kfactory-0.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.794902 kfactory-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.798903 kfactory-0.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/klive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.798903 kfactory-0.6.1/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 16:39:17.000000 kfactory-0.6.1/docs/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 16:39:17.000000 kfactory-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:39:37.802903 kfactory-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.790902 kfactory-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.798903 kfactory-0.6.1/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/generic_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80302 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/kcell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.798903 kfactory-0.6.1/src/kfactory/pcells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.798903 kfactory-0.6.1/src/kfactory/pcells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/pcells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.802903 kfactory-0.6.1/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.802903 kfactory-0.6.1/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.802903 kfactory-0.6.1/src/kfactory/utils/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/utils/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22912 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/utils/geo/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/utils/geo/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/utils/geo/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.802903 kfactory-0.6.1/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12502 2023-04-18 16:39:17.000000 kfactory-0.6.1/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.798903 kfactory-0.6.1/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 16:39:37.000000 kfactory-0.6.1/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 16:39:37.000000 kfactory-0.6.1/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:39:37.000000 kfactory-0.6.1/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 16:39:37.000000 kfactory-0.6.1/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 16:39:37.000000 kfactory-0.6.1/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:39:37.802903 kfactory-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-18 16:39:17.000000 kfactory-0.6.1/tests/test_spiral.py
```

### Comparing `kfactory-0.6.0/.github/workflows/pages.yml` & `kfactory-0.6.1/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/.github/workflows/release.yml` & `kfactory-0.6.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/.github/workflows/test_code.yml` & `kfactory-0.6.1/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/.pre-commit-config.yaml` & `kfactory-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/LICENSE` & `kfactory-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/Makefile` & `kfactory-0.6.1/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/PKG-INFO` & `kfactory-0.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.6.0
+Version: 0.6.1
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.6.0
+# KFactory 0.6.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.0/README.md` & `kfactory-0.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.6.0
+# KFactory 0.6.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.0/docs/Makefile` & `kfactory-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/README.md` & `kfactory-0.6.1/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.6.0
+# KFactory 0.6.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.0/docs/_static/complex.png` & `kfactory-0.6.1/docs/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/_static/klive.webm` & `kfactory-0.6.1/docs/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/_static/waveguide.png` & `kfactory-0.6.1/docs/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/complex_cell.py` & `kfactory-0.6.1/docs/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/conf.py` & `kfactory-0.6.1/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project = "kfactory"
-version = "0.6.0"
+version = "0.6.1"
 copyright = "2022"
 # author = "kfactory"
 
 # html_theme = "furo"
 # html_theme = "sphinx_rtd_theme"
 html_theme = "sphinx_book_theme"
```

### Comparing `kfactory-0.6.0/docs/index.rst` & `kfactory-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/intro.rst` & `kfactory-0.6.1/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/make.bat` & `kfactory-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/notebooks/00_geometry.py` & `kfactory-0.6.1/docs/notebooks/00_geometry.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/notebooks/01_references.py` & `kfactory-0.6.1/docs/notebooks/01_references.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/notebooks/02_DRC.py` & `kfactory-0.6.1/docs/notebooks/02_DRC.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/star.py` & `kfactory-0.6.1/docs/star.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/docs/waveguide.py` & `kfactory-0.6.1/docs/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/pyproject.toml` & `kfactory-0.6.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.6.0"
+version = "0.6.1"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
```

### Comparing `kfactory-0.6.0/src/kfactory/__init__.py` & `kfactory-0.6.1/src/kfactory/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     LayerEnum,
     show,
 )
 from . import pcells, placer, routing, utils, port
 from .config import logger
 
 
-__version__ = "0.6.0"
+__version__ = "0.6.1"
 
 
 __all__ = [
     "KCell",
     "Instance",
     "Port",
     "Ports",
```

### Comparing `kfactory-0.6.0/src/kfactory/config.py` & `kfactory-0.6.1/src/kfactory/config.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/generic_tech.py` & `kfactory-0.6.1/src/kfactory/generic_tech.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/kcell.py` & `kfactory-0.6.1/src/kfactory/kcell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/bezier.py` & `kfactory-0.6.1/src/kfactory/pcells/bezier.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/circular.py` & `kfactory-0.6.1/src/kfactory/pcells/circular.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/dbu/taper.py` & `kfactory-0.6.1/src/kfactory/pcells/dbu/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/dbu/waveguide.py` & `kfactory-0.6.1/src/kfactory/pcells/dbu/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/euler.py` & `kfactory-0.6.1/src/kfactory/pcells/euler.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/taper.py` & `kfactory-0.6.1/src/kfactory/pcells/taper.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/pcells/waveguide.py` & `kfactory-0.6.1/src/kfactory/pcells/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/placer.py` & `kfactory-0.6.1/src/kfactory/placer.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/port.py` & `kfactory-0.6.1/src/kfactory/port.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/routing/electrical.py` & `kfactory-0.6.1/src/kfactory/routing/electrical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/routing/manhattan.py` & `kfactory-0.6.1/src/kfactory/routing/manhattan.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/routing/optical.py` & `kfactory-0.6.1/src/kfactory/routing/optical.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/utils/__init__.py` & `kfactory-0.6.1/src/kfactory/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/utils/geo/enclosure.py` & `kfactory-0.6.1/src/kfactory/utils/geo/enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/utils/geo/fill.py` & `kfactory-0.6.1/src/kfactory/utils/geo/fill.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/utils/geo/simplify.py` & `kfactory-0.6.1/src/kfactory/utils/geo/simplify.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/utils/violations.py` & `kfactory-0.6.1/src/kfactory/utils/violations.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory/widgets/interactive.py` & `kfactory-0.6.1/src/kfactory/widgets/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+"""Interactivate jupyter widget."""
+
 try:
     from pathlib import Path
     from typing import Any
 
-    import klayout.lay as lay
     from ipyevents import Event  # type: ignore[import]
     from IPython.display import display  # type: ignore[import]
     from ipytree import Node, Tree  # type: ignore[import]
     from ipywidgets import (  # type: ignore[import]
         Accordion,
         AppLayout,
         Box,
@@ -55,15 +56,15 @@
         self.layout_view.show_layout(cell.klib, False)
         self.layer_properties: Path | None = None
         if layer_properties is not None:
             self.layer_properties = Path(layer_properties)
             if self.layer_properties.exists() and self.layer_properties.is_file():
                 self.layer_properties = self.layer_properties
                 self.layout_view.load_layer_props(str(self.layer_properties))
-        self.show_cell(cell)
+        self.show_cell(cell._kdb_cell)
         png_data = self.layout_view.get_screenshot_pixels().to_png_data()
 
         self.image = Image(value=png_data, format="png")
         self.refresh()
         scroll_event = Event(source=self.image, watched_events=["wheel"], wait=10)
         scroll_event.on_dom_event(self.on_scroll)
 
@@ -345,24 +346,21 @@
         self.layout_view.timer()  # type: ignore[attr-defined]
         x = event["relativeX"]
         y = event["relativeY"]
         buttons = self._get_modifier_buttons(event)
 
         match event["event"]:
             case "mousedown":
-                # if event["event"] == "mousedown":
                 self.layout_view.send_mouse_press_event(
                     kdb.DPoint(float(x), float(y)), buttons
                 )
-            # elif event["event"] == "mouseup":
             case "mouseup":
                 self.layout_view.send_mouse_release_event(
                     kdb.DPoint(float(x), float(y)), buttons
                 )
-            # elif event["event"] == "mousemove":
             case "mousemove":
                 self.layout_view.send_mouse_move_event(
                     kdb.DPoint(float(x), float(y)), buttons
                 )
         self.refresh()
         self.layout_view.timer()  # type: ignore[attr-defined]
```

### Comparing `kfactory-0.6.0/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.6.1/src/kfactory.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.6.0
+Version: 0.6.1
 Summary: KLayout API implementation of gdsfactory
 Author-email: gdsfactory community <contact@gdsfactory.com>
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: ci
 Provides-Extra: ipy
 License-File: LICENSE
 
-# KFactory 0.6.0
+# KFactory 0.6.1
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.6.0/src/kfactory.egg-info/SOURCES.txt` & `kfactory-0.6.1/src/kfactory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/src/kfactory.egg-info/requires.txt` & `kfactory-0.6.1/src/kfactory.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/conftest.py` & `kfactory-0.6.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_cplxcells.py` & `kfactory-0.6.1/tests/test_cplxcells.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_enclosure.py` & `kfactory-0.6.1/tests/test_enclosure.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_extrude.py` & `kfactory-0.6.1/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_ports.py` & `kfactory-0.6.1/tests/test_ports.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_rename.py` & `kfactory-0.6.1/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_routing.py` & `kfactory-0.6.1/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.6.0/tests/test_spiral.py` & `kfactory-0.6.1/tests/test_spiral.py`

 * *Files identical despite different names*

