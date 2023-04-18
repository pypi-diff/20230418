# Comparing `tmp/kfactory-0.5.8.tar.gz` & `tmp/kfactory-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kfactory-0.5.8.tar", last modified: Sun Mar 26 15:36:12 2023, max compression
+gzip compressed data, was "kfactory-0.6.0.tar", last modified: Tue Apr 18 15:58:51 2023, max compression
```

## Comparing `kfactory-0.5.8.tar` & `kfactory-0.6.0.tar`

### file list

```diff
@@ -1,112 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.736010 kfactory-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-03-26 15:35:55.000000 kfactory-0.5.8/.bumpversion.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.724010 kfactory-0.5.8/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-26 15:35:55.000000 kfactory-0.5.8/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.724010 kfactory-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-03-26 15:35:55.000000 kfactory-0.5.8/.github/workflows/pages.yml
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-03-26 15:35:55.000000 kfactory-0.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-03-26 15:35:55.000000 kfactory-0.5.8/.github/workflows/test_code.yml
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-26 15:35:55.000000 kfactory-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-03-26 15:35:55.000000 kfactory-0.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-26 15:35:55.000000 kfactory-0.5.8/.sourcery.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-26 15:35:55.000000 kfactory-0.5.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-03-26 15:35:55.000000 kfactory-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-03-26 15:35:55.000000 kfactory-0.5.8/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-26 15:36:12.736010 kfactory-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-26 15:35:55.000000 kfactory-0.5.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.728010 kfactory-0.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.728010 kfactory-0.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/_static/complex.png
--rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/_static/klive.webm
--rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/_static/waveguide.png
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/complex_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     2214 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/klive.rst
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.config.rst
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.kcell.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.bezier.rst
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.circular.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.dbu.rst
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.dbu.taper.rst
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.dbu.waveguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.euler.rst
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.rst
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.taper.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.pcells.waveguide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.placer.rst
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.port.rst
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.routing.electrical.rst
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.routing.manhattan.rst
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.routing.optical.rst
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.routing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.tech.rst
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.utils.geo.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/modules/kfactory.utils.violations.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/docs/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)    11482 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/notebooks/00_geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    13525 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/notebooks/01_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/star.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-03-26 15:35:55.000000 kfactory-0.5.8/docs/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-26 15:35:55.000000 kfactory-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-26 15:36:12.736010 kfactory-0.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.724010 kfactory-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/generic_tech.py
--rw-r--r--   0 runner    (1001) docker     (123)    91630 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/kcell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory/pcells/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1845 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/bezier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/circular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory/pcells/dbu/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/dbu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/dbu/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/dbu/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     6647 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/euler.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/taper.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/pcells/waveguide.py
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/placer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/port.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory/routing/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/routing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/routing/electrical.py
--rw-r--r--   0 runner    (1001) docker     (123)    11093 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/routing/manhattan.py
--rw-r--r--   0 runner    (1001) docker     (123)    17882 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/routing/optical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23781 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/utils/geo.py
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/utils/violations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-03-26 15:35:55.000000 kfactory-0.5.8/src/kfactory/widgets/interactive.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.732010 kfactory-0.5.8/src/kfactory.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-03-26 15:36:12.000000 kfactory-0.5.8/src/kfactory.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-03-26 15:36:12.000000 kfactory-0.5.8/src/kfactory.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-26 15:36:12.000000 kfactory-0.5.8/src/kfactory.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-03-26 15:36:12.000000 kfactory-0.5.8/src/kfactory.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-26 15:36:12.000000 kfactory-0.5.8/src/kfactory.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-26 15:36:12.736010 kfactory-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_cell.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_cplxcells.py
--rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_enclosure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_extrude.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_ports.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_rename.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_routing.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_shapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-03-26 15:35:55.000000 kfactory-0.5.8/tests/test_spiral.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-04-18 15:58:28.000000 kfactory-0.6.0/.bumpversion.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.200440 kfactory-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.200440 kfactory-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/workflows/pages.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-04-18 15:58:28.000000 kfactory-0.6.0/.github/workflows/test_code.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-18 15:58:28.000000 kfactory-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     4676 2023-04-18 15:58:28.000000 kfactory-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-18 15:58:28.000000 kfactory-0.6.0/.sourcery.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 15:58:28.000000 kfactory-0.6.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-18 15:58:28.000000 kfactory-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 15:58:28.000000 kfactory-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 15:58:51.208440 kfactory-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 15:58:28.000000 kfactory-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)   138035 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/_static/complex.png
+-rw-r--r--   0 runner    (1001) docker     (123)   985194 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/_static/klive.webm
+-rw-r--r--   0 runner    (1001) docker     (123)   129785 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/_static/waveguide.png
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/complex_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2633 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/klive.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/docs/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    11525 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/notebooks/00_geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13535 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/notebooks/01_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/notebooks/02_DRC.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/star.py
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-04-18 15:58:28.000000 kfactory-0.6.0/docs/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-04-18 15:58:28.000000 kfactory-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:58:51.208440 kfactory-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.200440 kfactory-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/src/kfactory/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3471 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/generic_tech.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80302 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/kcell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/pcells/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/bezier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/circular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/pcells/dbu/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/dbu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/dbu/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/dbu/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/euler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/taper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/pcells/waveguide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/placer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5294 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/port.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/electrical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12486 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/manhattan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/routing/optical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/utils/geo/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22912 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/fill.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/geo/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/utils/violations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/src/kfactory/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12635 2023-04-18 15:58:28.000000 kfactory-0.6.0/src/kfactory/widgets/interactive.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.204440 kfactory-0.6.0/src/kfactory.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2040 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 15:58:51.000000 kfactory-0.6.0/src/kfactory.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:58:51.208440 kfactory-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_cell.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_cplxcells.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1598 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_enclosure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_extrude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_routing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-04-18 15:58:28.000000 kfactory-0.6.0/tests/test_spiral.py
```

### Comparing `kfactory-0.5.8/.github/workflows/pages.yml` & `kfactory-0.6.0/.github/workflows/pages.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/.github/workflows/release.yml` & `kfactory-0.6.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/.github/workflows/test_code.yml` & `kfactory-0.6.0/.github/workflows/test_code.yml`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/.pre-commit-config.yaml` & `kfactory-0.6.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     rev: 5.12.0
     hooks:
       - id: isort
         files: src/kfactory/.*
         args: [--profile, black, --filter-files]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   # - repo: https://github.com/omnilib/ufmt
   #   rev: v2.0.0b1
   #   hooks:
   #     - id: ufmt
@@ -62,31 +62,32 @@
   - repo: https://github.com/asottile/pyupgrade
     rev: v3.3.1
     hooks:
       - id: pyupgrade
         args: [--py37-plus, --keep-runtime-typing]
 
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.2
+    rev: v2.2.4
     hooks:
       - id: codespell
-        args: ["-L TE,TE/TM,te,ba,FPR,fpr_spacing,ro,nd,donot,schem"]
+        additional_dependencies:
+          - tomli
 
   # - repo: https://github.com/shellcheck-py/shellcheck-py
   #   rev: 98854f809ca9d0e235c0bd5c0ad5e986e02120a4
   #   hooks:
   #     - id: shellcheck
 
   # - repo: https://github.com/pre-commit/pygrep-hooks
   #   rev: 77c4a0f2d3edd699ff7c2c5e430d46cd85358768 # Use the ref you want to point at
   #   hooks:
   #     - id: python-use-type-annotations
 
   - repo: https://github.com/PyCQA/bandit
-    rev: 1.7.4
+    rev: 1.7.5
     hooks:
       - id: bandit
         args: [--exit-zero]
         # ignore all tests, not just tests data
         exclude: ^tests/
   # - repo: https://github.com/PyCQA/pylint
   #   rev: v2.14.1
```

### Comparing `kfactory-0.5.8/LICENSE` & `kfactory-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/Makefile` & `kfactory-0.6.0/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/PKG-INFO` & `kfactory-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.5.8
+Version: 0.6.0
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
 
-# KFactory 0.5.8
+# KFactory 0.6.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.5.8/README.md` & `kfactory-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.5.8
+# KFactory 0.6.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.5.8/docs/Makefile` & `kfactory-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/README.md` & `kfactory-0.6.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# KFactory 0.5.8
+# KFactory 0.6.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.5.8/docs/_static/complex.png` & `kfactory-0.6.0/docs/_static/complex.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/_static/klive.webm` & `kfactory-0.6.0/docs/_static/klive.webm`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/_static/waveguide.png` & `kfactory-0.6.0/docs/_static/waveguide.png`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/complex_cell.py` & `kfactory-0.6.0/docs/complex_cell.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/conf.py` & `kfactory-0.6.0/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 project = "kfactory"
-version = "0.5.8"
+version = "0.6.0"
 copyright = "2022"
 # author = "kfactory"
 
 # html_theme = "furo"
 # html_theme = "sphinx_rtd_theme"
 html_theme = "sphinx_book_theme"
 
@@ -74,15 +74,15 @@
 
 autodoc_pydantic_model_signature_prefix = "class"
 autodoc_pydantic_field_signature_prefix = "attribute"
 autodoc_pydantic_model_show_config_member = False
 autodoc_pydantic_model_show_config_summary = False
 autodoc_pydantic_model_show_validator_summary = False
 autodoc_pydantic_model_show_validator_members = False
-
+autodoc_typehints = "description"
 
 autodoc_default_options = {
     "member-order": "bysource",
     "special-members": "__init__",
     "undoc-members": True,
     "exclude-members": "__weakref__",
     "inherited-members": True,
```

### Comparing `kfactory-0.5.8/docs/index.rst` & `kfactory-0.6.0/docs/index.rst`

 * *Files 20% similar despite different names*

```diff
@@ -11,13 +11,19 @@
    README
    intro
    klive
    tutorial
    api
    CHANGELOG
 
+.. autosummary::
+   :toctree: modules
+   :recursive:
+
+   kfactory
+
 Indices and tables
 ==================
 
 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
```

### Comparing `kfactory-0.5.8/docs/intro.rst` & `kfactory-0.6.0/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/make.bat` & `kfactory-0.6.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/docs/notebooks/00_geometry.py` & `kfactory-0.6.0/docs/notebooks/00_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,17 @@
 ### complex transformation example:ce
 #     magnification(float): magnification, DO NOT USE on cells or references, only shapes, most foundries will not allow magnifications on actual cell references or cells
 #     rotation(float): rotation in degrees
 #     mirror(bool): boolean to mirror at x axis and then rotate if true
 #     x(float): x coordinate
 #     y(float): y coordinate
 #
-text2 = t.transformed(kf.kdb.CplxTrans(2.0, 45.0, False, 5.0, 30.0))
+text2 = t.transformed(
+    kf.kdb.DCplxTrans(2.0, 45.0, False, 5.0, 30.0).to_itrans(c.klib.dbu)
+)
 # text1.movey(25)
 # text2.move([5, 30])
 # text2.rotate(45)
 r.move(
     -5, 0
 )  # boxes can be moved like this, other shapes and cellss/refs need to be moved with .transform
 r.move(-5, 0)
@@ -126,19 +128,18 @@
 def straight(length=10, width=1, layer=(1, 0)):
     wg = kf.KCell()
     box = kf.kdb.DBox(length, width)
     int_box = box.to_itype(wg.klib.dbu)
     _layer = kf.klib.layer(*layer)
     wg.shapes(_layer).insert(box)
     wg.add_port(
-        kf.DPort(
+        kf.Port(
             name="o1",
-            position=(box.left, box.center().y),
-            width=width,
-            angle=2,
+            dwidth=width,
+            dcplx_trans=kf.kdb.DCplxTrans(1, 180, False, box.left, box.center().y),
             layer=_layer,
         )
     )
     wg.create_port(
         name="o2",
         trans=kf.kdb.Trans(int_box.right, int_box.center().y),
         layer=_layer,
```

### Comparing `kfactory-0.5.8/docs/notebooks/01_references.py` & `kfactory-0.6.0/docs/notebooks/01_references.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,15 +129,15 @@
 
 # As you've seen you have two ways to add a reference to our component:
 #
 # 1. create the reference and add it to the component
 
 c = kf.KCell(name="reference_sample")
 w = kf.pcells.waveguide.waveguide(length=10, width=0.6, layer=c.klib.layer(1, 0))
-wr = kf.kdb.CellInstArray(w, kf.kdb.Trans.R0)
+wr = kf.kdb.CellInstArray(w._kdb_cell, kf.kdb.Trans.R0)
 c.insert(wr)
 c
 
 # 2. or do it in a single line
 
 c = kf.KCell(name="reference_sample_shorter_syntax")
 wr = c << kf.pcells.waveguide.waveguide(length=10, width=0.6, layer=c.klib.layer(1, 0))
```

### Comparing `kfactory-0.5.8/docs/star.py` & `kfactory-0.6.0/docs/star.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import random
 
 
 @kf.autocell
 def star(
     size: float, proportion: float, n_diamonds: int = 3, layer: kf.LayerEnum = LAYER.SI
 ) -> kf.KCell:
-
     """Create a diamond star cell
 
     Args:
         size: size in um
         proportion: width of the center vs size (0 < proportion <= 1)
         n_diamonds: number of diamonds in the star (>=1)
```

### Comparing `kfactory-0.5.8/docs/waveguide.py` & `kfactory-0.6.0/docs/waveguide.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/pyproject.toml` & `kfactory-0.6.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,35 +9,39 @@
 classifiers = [
 	"Programming Language :: Python :: 3.10",
 	"Operating System :: OS Independent",
 ]
 requires-python = ">=3.10"
 
 
-version = "0.5.8"
+version = "0.6.0"
 authors = [
     {name = "gdsfactory community", email = "contact@gdsfactory.com"},
 ]
 dependencies = [
 	"klayout >= 0.28.3",
 	"scipy",
 	"ruamel.yaml",
 	"cachetools >= 5.2.0",
   "pydantic",
 	"loguru",
+	"tomli",
 ]
 
 [project.optional-dependencies]
 dev = [
-	"black>=21",
+	"black>=23",
 	"mypy",
 	"pre-commit",
 	"gitpython",
 	"pylsp-mypy",
-	"types-cachetools"
+	"python-lsp-server[all]",
+	"python-lsp-ruff",
+	"types-cachetools",
+	"python-lsp-black",
 ]
 docs = [
 	"sphinx",
 	"docutils==0.17.1",
 	"sphinx_rtd_theme",
 	"sphinxcontrib-video",
 	"sphinx-autodoc-typehints",
@@ -162,7 +166,24 @@
 allow_multiline_lambdas = true
 
 [tool.coverage.run]
 omit = "**/test_*.py"
 
 [tool.coverage.html]
 directory = "_build/coverage_html_report"
+
+[tool.codespell]
+ignore-words-list = "euclidian,TE,TE/TM,te,ba,FPR,fpr_spacing,ro,nd,donot,schem"
+skip = "pyproject.toml"
+
+[tool.ruff]
+line-length = 88
+src = ["src"]
+select = [
+  "E",   # pycodestyle
+  "F",   # pyflakes
+  "UP",  # pyupgrade
+  "D",   # pydocstyle
+]
+
+[tool.ruff.pydocstyle]
+convention = "google"
```

### Comparing `kfactory-0.5.8/src/kfactory/config.py` & `kfactory-0.6.0/src/kfactory/config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,55 +1,80 @@
+"""Kfactory configuration."""
+
 from __future__ import annotations
 
 import re
 import sys
 import traceback
 from itertools import takewhile
-from typing import Any, Optional
 
 import loguru
 from loguru import logger as logger
 
 
 def add_traceback(record: loguru.Record) -> None:
+    """Add a traceback to the logger."""
     extra = record["extra"]
     if extra.get("with_traceback", False):
         extra["traceback"] = "\n" + "".join(traceback.format_stack())
     else:
         extra["traceback"] = ""
 
 
 def tracing_formatter(record: loguru.Record) -> str:
-    # Filter out frames coming from Loguru internals
+    """Traceback filtering.
+
+    Filter out frames coming from Loguru internals.
+    """
     frames = takewhile(
         lambda f: "/loguru/" not in f.filename, traceback.extract_stack()
     )
     stack = " > ".join(f"{f.filename}:{f.name}:{f.lineno}" for f in frames)
     record["extra"]["stack"] = stack
 
     if record["extra"].get("with_backtrace", False):
-        return "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | <cyan>{extra[stack]}</cyan> - <level>{message}</level>\n{exception}"
+        return (
+            "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level>"
+            " | <cyan>{extra[stack]}</cyan> - <level>{message}</level>\n{exception}"
+        )
+
     else:
-        return "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>\n{exception}"
+        return (
+            "<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}"
+            "</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan>"
+            " - <level>{message}</level>\n{exception}"
+        )
 
 
 class LogFilter:
-    def __init__(self, level: str, regex: Optional[str] = None) -> None:
+    """Filter certain messages by log level or regex.
+
+    Filtered messages are not evaluated and discarded.
+    """
+
+    def __init__(self, level: str, regex: str | None = None) -> None:
+        """Create new filter.
+
+        Args:
+            level: Minimum log level to print to log. Options:
+                ["DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"]
+            regex: Discard messages matching the regex string. Set to `None` to disable.
+        """
         self.level = level
         self.regex = regex
 
     def __call__(self, record: loguru.Record) -> bool:
+        """Loguru needs the filter to be callable."""
         levelno = logger.level(self.level).no
         if self.regex is None:
             return record["level"].no >= levelno
         else:
             return record["level"].no >= levelno and not bool(
                 re.search(self.regex, record["message"])
             )
 
 
 filter = LogFilter("DEBUG")
 logger.remove()
 logger.add(sys.stdout, format=tracing_formatter, filter=filter)
-# format="<green>{time:YYYY-MM-DD HH:mm:ss.SSS}</green> | <level>{level: <8}</level> | <cyan>{name}</cyan>:<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}{extra[traceback]}</level>",
 
 __all__ = ["logger", "filter"]
```

### Comparing `kfactory-0.5.8/src/kfactory/generic_tech.py` & `kfactory-0.6.0/src/kfactory/generic_tech.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """Technology settings."""
 from __future__ import annotations
 
-from enum import Enum
-from typing import Any, Dict, Iterator, List, Optional, Tuple
+from typing import Any
 
 from pydantic import BaseModel
 
-from .kcell import KCell, KLib, LayerEnum, klib
+from .kcell import LayerEnum
 
 # from kfactory import KCell, KLib, library
 
 
 class LAYER(LayerEnum):
     #     """Generic layermap based on book.
 
@@ -115,15 +114,15 @@
             into: etch into another layer.
                 https://gdsfactory.github.io/klayout_pyxs/DocGrow.html
             doping_concentration: for implants.
             resistivity: for metals.
             bias: in um for the etch.
     """
 
-    layer: Optional[Tuple[int, int]]
+    layer: tuple[int, int] | None
     thickness: float
-    thickness_tolerance: Optional[float] = None
+    thickness_tolerance: float | None = None
     zmin: float
-    material: Optional[str] = None
+    material: str | None = None
     sidewall_angle: float = 0
-    z_to_bias: Optional[Tuple[List[float], List[float]]] = None
-    info: Dict[str, Any] = {}
+    z_to_bias: tuple[list[float], list[float]] | None = None
+    info: dict[str, Any] = {}
```

### Comparing `kfactory-0.5.8/src/kfactory/kcell.py` & `kfactory-0.6.0/src/kfactory/kcell.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,260 +1,286 @@
-import abc
+"""Core module of kfactory.
+
+Defines the :py:class:`KCell` providing klayout Cells with Ports
+and other convenience functions.
+
+:py:class:`Instance` are the kfactory instances used to also acquire
+ports etc from instances.
+
+"""
+
 import functools
 import importlib
 import json
 import socket
-import struct
-from abc import ABC, abstractmethod
-from dataclasses import InitVar, dataclass
+from collections.abc import Callable, Hashable, Iterable, Iterator
 
 # from enum import IntEnum
-from enum import Enum
+from enum import Enum, IntEnum
 from hashlib import sha3_512
 from inspect import signature
 from pathlib import Path
 from tempfile import gettempdir
-from typing import (  # ParamSpec, # >= python 3.10
-    Any,
-    Callable,
-    Concatenate,
-    Generic,
-    Hashable,
-    Iterable,
-    Iterator,
-    Optional,
-    Protocol,
-    Sequence,
-    Type,
-    TypeAlias,
-    TypeGuard,
-    TypeVar,
-    Union,
-    cast,
-    overload,
-)
+from typing import Any, Literal, cast, overload  # ParamSpec, # >= python 3.10
 
 # from cachetools import Cache, cached
 import cachetools.func
 import numpy as np
 import ruamel.yaml
 from typing_extensions import ParamSpec
 
-from . import kdb, lay
+from . import kdb
 from .config import logger
 from .port import rename_clockwise
 
+# import struct
+# from abc import abstractmethod
+
+
 try:
     from __main__ import __file__ as mf
 except ImportError:
     mf = "shell"
 
 
 KCellParams = ParamSpec("KCellParams")
-OP = ParamSpec("OP")
 
 
-def is_simple_port(port: "Port | DPort | ICplxPort | DCplxPort") -> "TypeGuard[Port]":
-    return port.int_based() and not port.complex()
+class PROPID(IntEnum):
+    """Mapping for GDS properties."""
+
+    NAME = 0
 
 
 class PortWidthMismatch(ValueError):
+    """Error thrown when two ports don't have a matching `width`."""
+
     @logger.catch
     def __init__(
         self,
         inst: "Instance",
-        other_inst: "Instance | Port | DPort | ICplxPort | DCplxPort",
-        p1: "Port | DPort | ICplxPort | DCplxPort",
-        p2: "Port | DPort | ICplxPort | DCplxPort",
+        other_inst: "Instance | Port",
+        p1: "Port",
+        p2: "Port",
         *args: Any,
     ):
+        """Throw error for the two ports `p1`/`p1`."""
         if isinstance(other_inst, Instance):
             super().__init__(
-                f'Width mismatch between the ports {inst.cell.name}["{p1.name}"] and {other_inst.cell.name}["{p2.name}"] ({p1.width}/{p2.width})',
+                f'Width mismatch between the ports {inst.cell.name}["{p1.name}"]'
+                f'and {other_inst.cell.name}["{p2.name}"] ({p1.width}/{p2.width})',
                 *args,
             )
         else:
             super().__init__(
-                f'Width mismatch between the ports {inst.cell.name}["{p1.name}"] and Port "{p2.name}" ({p1.width}/{p2.width})',
+                f'Width mismatch between the ports {inst.cell.name}["{p1.name}"]'
+                f' and Port "{p2.name}" ({p1.width}/{p2.width})',
                 *args,
             )
 
 
 class PortLayerMismatch(ValueError):
+    """Error thrown when two ports don't have a matching `layer`."""
+
     @logger.catch
     def __init__(
         self,
         lib: "KLib",
         inst: "Instance",
-        other_inst: "Instance | Port | DPort | ICplxPort | DCplxPort",
-        p1: "Port | DPort | ICplxPort | DCplxPort",
-        p2: "Port | DPort | ICplxPort | DCplxPort",
+        other_inst: "Instance | Port",
+        p1: "Port",
+        p2: "Port",
         *args: Any,
     ):
+        """Throw error for the two ports `p1`/`p1`."""
         l1 = (
             f"{p1.layer.name}({p1.layer.__int__()})"
             if isinstance(p1.layer, LayerEnum)
             else str(lib.get_info(p1.layer))
         )
         l2 = (
             f"{p2.layer.name}({p2.layer.__int__()})"
             if isinstance(p2.layer, LayerEnum)
             else str(lib.get_info(p2.layer))
         )
         if isinstance(other_inst, Instance):
             super().__init__(
-                f'Layer mismatch between the ports {inst.cell.name}["{p1.name}"] and {other_inst.cell.name}["{p2.name}"] ({l1}/{l2})',
+                f'Layer mismatch between the ports {inst.cell.name}["{p1.name}"]'
+                f' and {other_inst.cell.name}["{p2.name}"] ({l1}/{l2})',
                 *args,
             )
         else:
             super().__init__(
-                f'Layer mismatch between the ports {inst.cell.name}["{p1.name}"] and Port "{p2.name}" ({l1}/{l2})',
+                f'Layer mismatch between the ports {inst.cell.name}["{p1.name}"]'
+                f' and Port "{p2.name}" ({l1}/{l2})',
                 *args,
             )
 
 
 class PortTypeMismatch(ValueError):
+    """Error thrown when two ports don't have a matching `port_type`."""
+
     @logger.catch
     def __init__(
         self,
         inst: "Instance",
-        other_inst: "Instance | Port | DPort | ICplxPort | DCplxPort",
-        p1: "Port | DPort | ICplxPort | DCplxPort",
-        p2: "Port | DPort | ICplxPort | DCplxPort",
+        other_inst: "Instance | Port",
+        p1: "Port",
+        p2: "Port",
         *args: Any,
     ):
+        """Throw error for the two ports `p1`/`p1`."""
         if isinstance(other_inst, Instance):
             super().__init__(
-                f'Type mismatch between the ports {inst.cell.name}["{p1.name}"] and {other_inst.cell.name}["{p2.name}"] ({p1.port_type}/{p2.port_type})',
+                f'Type mismatch between the ports {inst.cell.name}["{p1.name}"]'
+                f' and {other_inst.cell.name}["{p2.name}"]'
+                f" ({p1.port_type}/{p2.port_type})",
                 *args,
             )
         else:
             super().__init__(
-                f'Type mismatch between the ports {inst.cell.name}["{p1.name}"] and Port "{p2.name}" ({p1.port_type}/{p2.port_type})',
+                f'Type mismatch between the ports {inst.cell.name}["{p1.name}"]'
+                f' and Port "{p2.name}" ({p1.port_type}/{p2.port_type})',
                 *args,
             )
 
 
 class FrozenError(AttributeError):
-    """Raised if a KCell has been frozen and shouldn't be modified anymore"""
+    """Raised if a KCell has been frozen and shouldn't be modified anymore."""
 
     pass
 
 
 def default_save() -> kdb.SaveLayoutOptions:
+    """Default options for saving GDS/OAS."""
     save = kdb.SaveLayoutOptions()
     save.gds2_write_cell_properties = True
     save.gds2_write_file_properties = True
     save.gds2_write_timestamps = False
 
     return save
 
 
 class KLib(kdb.Layout):
-    """This is a small extension to the ``klayout.db.Layout``. It adds tracking for the :py:class:`~kfactory.kcell.KCell` objects
-    instead of only the :py:class:`klayout.db.Cell` objects. Additionally it allows creation and registration through :py:func:`~create_cell`
+    """Small extension to the ``klayout.db.Layout``.
+
+    It adds tracking for the :py:class:`~kfactory.kcell.KCell` objects
+    instead of only the :py:class:`klayout.db.Cell` objects.
+    Additionally it allows creation and registration through :py:func:`~create_cell`
 
     All attributes of ``klayout.db.Layout`` are transparently accessible
 
     Attributes:
         editable: Whether the layout should be opened in editable mode (default: True)
         rename_function: function that takes an Iterable[Port] and renames them
     """
 
     def __init__(self, editable: bool = True) -> None:
-        self.kcells: dict[int, "KCell | CplxKCell"] = {}  # dict[str, "KCell"] = {}
+        """Crete a library of cells.
+
+        Args:
+            editable: Open the KLayout Layout in editable mode if `True`.
+        """
+        self.kcells: dict[int, "KCell"] = {}
         kdb.Layout.__init__(self, editable)
         self.rename_function: Callable[..., None] = rename_clockwise
 
     def dup(self, init_cells: bool = True) -> "KLib":
-        """Create a duplication of the `~KLib` object
+        """Create a duplication of the `~KLib` object.
 
         Args:
             init_cells: initialize the all cells in the new KLib object
 
         Returns:
             Copy of itself
         """
         klib = KLib()
         klib.assign(super().dup())
         if init_cells:
             for i, kc in self.kcells.items():
-                if isinstance(kc, KCell):
-                    klib.kcells[i] = KCell(
-                        name=kc.name,
-                        klib=klib,
-                        kdb_cell=klib.cell(kc.name),
-                        ports=kc.ports,
-                    )
-                else:
-                    klib.kcells[i] = CplxKCell(
-                        name=kc.name,
-                        klib=klib,
-                        kdb_cell=klib.cell(kc.name),
-                        ports=kc.ports,
-                    )
+                klib.kcells[i] = KCell(
+                    name=kc.name,
+                    klib=klib,
+                    kdb_cell=klib.cell(kc.name),
+                    ports=kc.ports,
+                )
         klib.rename_function = self.rename_function
         return klib
 
     def create_cell(  # type: ignore[override]
         self,
         name: str,
-        *args: Union[
-            list[str], list[Union[str, dict[str, Any]]], list[Union[str, str]]
-        ],
+        *args: str,
         allow_duplicate: bool = False,
     ) -> kdb.Cell:
-        """Create a new cell in the library. This shouldn't be called manually. The constructor of KCell will call this method.
+        """Create a new cell in the library.
+
+        This shouldn't be called manually.
+        The constructor of KCell will call this method.
 
         Args:
             kcell: The KCell to be registered in the Layout.
-            name: The (initial) name of the cell. Can be changed through :py:func:`~update_cell_name`
-            allow_duplicate: Allow the creation of a cell with the same name which already is registered in the Layout.\
-            This will create a cell with the name :py:attr:`name` + `$1` or `2..n` increasing by the number of existing duplicates
-            args: additional arguments passed to :py:func:`~klayout.db.Layout.create_cell`
-            kwargs: additional keyword arguments passed to :py:func:`klayout.db.Layout.create_cell`
+            name: The (initial) name of the cell. Can be changed through
+                :py:func:`~update_cell_name`
+            allow_duplicate: Allow the creation of a cell with the same name which
+                already is registered in the Layout.
+                This will create a cell with the name :py:attr:`name` + `$1` or `2..n`
+                increasing by the number of existing duplicates
+            args: additional arguments passed to
+                :py:func:`~klayout.db.Layout.create_cell`
 
         Returns:
             klayout.db.Cell: klayout.db.Cell object created in the Layout
 
         """
-
         if allow_duplicate or (self.cell(name) is None):
             # self.kcells[name] = kcell
             return kdb.Layout.create_cell(self, name, *args)
         else:
             raise ValueError(
-                f"Cellname {name} already exists. Please make sure the cellname is unique or pass `allow_duplicate` when creating the library"
+                f"Cellname {name} already exists. Please make sure the cellname is"
+                " unique or pass `allow_duplicate` when creating the library"
             )
 
-    def delete_cell(self, cell: "KCell | CplxKCell | int") -> None:
+    def delete_cell(self, cell: "KCell | int") -> None:
+        """Delete a cell in the klib object."""
         if isinstance(cell, int):
-            cell = self[self.cell(cell).name]
-        super().delete_cell(cell.cell_index())
+            super().delete_cell(cell)
+            del self.kcells[cell]
+        else:
+            ci = cell.cell_index()
+            super().delete_cell(ci)
+            del self.kcells[ci]
 
-    def register_cell(
-        self, kcell: "KCell | CplxKCell", allow_reregister: bool = False
-    ) -> None:
-        """Register an existing cell in the KLib object
+    def register_cell(self, kcell: "KCell", allow_reregister: bool = False) -> None:
+        """Register an existing cell in the KLib object.
 
         Args:
             kcell: KCell to be registered in the KLib
+            allow_reregister: Overwrite the existing KCell registration with this one.
+                Doesn't allow name duplication.
         """
 
-        def check_name(other: "KCell | CplxKCell") -> bool:
-            return other.name == kcell.name
+        def check_name(other: "KCell") -> bool:
+            return other._kdb_cell.name == kcell._kdb_cell.name
 
         if (kcell.cell_index() not in self.kcells) or allow_reregister:
             self.kcells[kcell.cell_index()] = kcell
         else:
             raise ValueError(
-                "Cannot register a new cell with a name that already exists in the library"
+                "Cannot register a new cell with a name that already"
+                " exists in the library"
             )
 
-    def __getitem__(self, obj: str | int) -> "KCell | CplxKCell":
+    def __getitem__(self, obj: str | int) -> "KCell":
+        """Retrieve a cell by name(str) or index(int).
+
+        Attrs:
+            obj: name of cell or cell_index
+        """
         if isinstance(obj, int):
             try:
                 return self.kcells[obj]
             except KeyError:
                 if self.cell(obj) is None:
                     raise
 
@@ -266,23 +292,34 @@
                     return self.kcells[self.cell(obj).cell_index()]
                 except KeyError:
                     c = self.cell(obj)
                     return KCell(name=c.name, klib=self, kdb_cell=self.cell(obj))
             from pprint import pformat
 
             raise ValueError(
-                f"Library doesn't have a KCell named {obj}, available KCells are {pformat(sorted([cell.name for cell in self.kcells.values()]))}"
+                f"Library doesn't have a KCell named {obj},"
+                " available KCells are"
+                f"{pformat(sorted([cell.name for cell in self.kcells.values()]))}"
             )
 
     def read(
         self,
         filename: str | Path,
-        options: Optional[kdb.LoadLayoutOptions] = None,
+        options: kdb.LoadLayoutOptions | None = None,
         register_cells: bool = False,
     ) -> kdb.LayerMap:
+        """Read a GDS file into the existing Layout.
+
+        Args:
+            filename: Path of the GDS file.
+            options: KLayout options to load from the GDS. Can determine how merge
+                conflicts are handled for example. See
+                https://www.klayout.de/doc-qt5/code/class_LoadLayoutOptions.html
+            register_cells: If `True` create KCells for all cells in the GDS.
+        """
         if register_cells:
             cells = set(self.cells("*"))
         fn = str(Path(filename).resolve())
         if options is None:
             lm = kdb.Layout.read(self, fn)
         else:
             lm = kdb.Layout.read(self, fn, options)
@@ -296,1268 +333,729 @@
 
     def write(  # type: ignore[override]
         self,
         filename: str | Path,
         gzip: bool = False,
         options: kdb.SaveLayoutOptions = default_save(),
     ) -> None:
+        """Write a GDS file into the existing Layout.
+
+        Args:
+            filename: Path of the GDS file.
+            gzip: directly make the GDS a .gds.gz file.
+            options: KLayout options to load from the GDS. Can determine how merge
+                conflicts are handled for example. See
+                https://www.klayout.de/doc-qt5/code/class_LoadLayoutOptions.html
+        """
         return kdb.Layout.write(self, str(filename), options)
 
 
-klib = (
-    KLib()
-)  #: Default library object. :py:class:`~kfactory.kcell.KCell` uses this object unless another one is specified in the constructor
+klib = KLib()
+"""Default library object.
+
+:py:class:`~kfactory.kcell.KCell` uses this object unless another one is
+specified in the constructor."""
 
 
 class LayerEnum(int, Enum):
-    """Class for having the layers stored and a mapping int <-> layer,datatype
+    """Class for having the layers stored and a mapping int <-> layer,datatype.
 
-    This Enum can also be treated as a tuple, i.e. it implements __getitem__ and __len__.
+    This Enum can also be treated as a tuple, i.e. it implements __getitem__ and __len__
 
     Attributes:
         layer: layer number
         datatype: layer datatype
-        lib: library
     """
 
     layer: int
     datatype: int
 
     def __new__(  # type: ignore[misc]
         cls: "LayerEnum",
         layer: int,
         datatype: int,
         lib: KLib = klib,
     ) -> "LayerEnum":
+        """Create a new Enum.
+
+        Because it needs to act like an integer an enum is created and expanded.
+
+        Args:
+            layer: Layer number of the layer.
+            datatype: Datatype of the layer.
+            lib: :py:class:~`KLib` to register the layer to.
+        """
         value = lib.layer(layer, datatype)
         obj: int = int.__new__(cls, value)  # type: ignore[call-overload]
         obj._value_ = value  # type: ignore[attr-defined]
         obj.layer = layer  # type: ignore[attr-defined]
         obj.datatype = datatype  # type: ignore[attr-defined]
         return obj  # type: ignore[return-value]
 
     def __getitem__(self, key: int) -> int:
+        """Retrieve layer number[0] / datatype[1] of a layer."""
         if key == 0:
             return self.layer
         elif key == 1:
             return self.datatype
 
         else:
             raise ValueError(
                 "LayerMap only has two values accessible like"
                 " a list, layer == [0] and datatype == [1]"
             )
 
     def __len__(self) -> int:
+        """A layer has length 2, layer number and datatype."""
         return 2
 
     def __iter__(self) -> Iterator[int]:
+        """Allow for loops to iterate over the LayerEnum."""
         yield from [self.layer, self.datatype]
 
     def __str__(self) -> str:
+        """Return the name of the LayerEnum."""
         return self.name
 
 
-TT = TypeVar("TT", bound=kdb.Trans | kdb.DTrans | kdb.ICplxTrans | kdb.DCplxTrans)
-TD = TypeVar("TD", bound=kdb.DTrans | kdb.DCplxTrans)
-TI = TypeVar("TI", bound=kdb.Trans | kdb.ICplxTrans)
-TS = TypeVar("TS", bound=kdb.Trans | kdb.DTrans)
-TC = TypeVar("TC", bound=kdb.ICplxTrans | kdb.DCplxTrans)
-FI = TypeVar("FI", bound=int | float)
-
-PT = TypeVar("PT", bound="Port | DCplxPort")
-CellType = TypeVar("CellType", bound="KCell | CplxKCell")
-
-
-class PortLike(ABC, Generic[TT, FI]):
-    yaml_tag: str
-    name: str
-    width: FI
-    layer: int
-    trans: TT
-    port_type: str
-
-    def move(
-        self,
-        origin: tuple[FI, FI],
-        destination: tuple[FI, FI] = (cast(FI, 0), cast(FI, 0)),
-    ) -> None:
-        ...
-
-    @property
-    @abstractmethod
-    def center(self) -> tuple[FI, FI]:
-        ...
-
-    @center.setter
-    @abstractmethod
-    def center(self, value: tuple[FI, FI]) -> None:
-        ...
-
-    @property
-    @abstractmethod
-    def x(self) -> FI:
-        ...
-
-    @property
-    @abstractmethod
-    def y(self) -> FI:
-        ...
-
-    @abstractmethod
-    def hash(self) -> bytes:
-        ...
+class Port:
+    """A port is the photonics equivalent to a pin in electronics.
 
-    @staticmethod
-    @abstractmethod
-    def complex() -> bool:
-        ...
+    In addition to the location and layer
+    that defines a pin, a port also contains an orientation and a width.
+    This can be fully represented with a transformation, integer and layer_index.
 
-    @staticmethod
-    @abstractmethod
-    def int_based() -> bool:
-        ...
-
-    @abstractmethod
-    def dcplx_trans(self, dbu: float) -> kdb.DCplxTrans:
-        ...
-
-    def copy_cplx(self, trans: kdb.DCplxTrans, dbu: float) -> "DCplxPort":
-        if self.int_based():
-            return DCplxPort(
-                width=self.width * dbu,
-                layer=self.layer,
-                name=self.name,
-                port_type=self.port_type,
-                trans=trans * self.dcplx_trans(dbu),
-            )
-        else:
-            return DCplxPort(
-                width=self.width,
-                layer=self.layer,
-                name=self.name,
-                port_type=self.port_type,
-                trans=trans * self.dcplx_trans(dbu),
-            )
-
-    @abstractmethod
-    def copy(self) -> "PortLike[TT, FI]":
-        ...
 
+    Attributes:
+        name: String to name the port.
+        width: The width of the port in dbu.
+        trans: Transformation in dbu. If the port can be represented in 90° intervals
+            this is the safe way to do so.
+        dcplx_trans: Transformation in micrometer. The port will autoconvert between
+            trans and dcplx_trans on demand.
+        port_type: A string defining the type of the port
+        layer: Index of the layer or a LayerEnum that acts like an integer, but can
+            contain layer number and datatype
+        info: A dictionary with additional info. Not reflected in GDS. Copy will make a
+            (shallow) copy of it.
+    """
 
-class IPortLike(PortLike[TI, int]):
-    """Protocol for integer based ports"""
+    yaml_tag = "!Port"
+    name: str | None
+    width: int
+    layer: int
+    _trans: kdb.Trans | None
+    _dcplx_trans: kdb.DCplxTrans | None
+    port_type: str
 
     @overload
     def __init__(
         self,
         *,
-        name: str,
-        trans: TI,
+        name: str | None = None,
         width: int,
-        layer: int,
+        layer: LayerEnum | int,
+        trans: kdb.Trans,
+        klib: KLib = klib,
         port_type: str = "optical",
-    ) -> None:
+        info: dict[str, Any] = {},
+    ):
         ...
 
     @overload
     def __init__(
         self,
         *,
-        name: Optional[str] = None,
-        port: "IPortLike[TI]",
-    ) -> None:
+        name: str | None = None,
+        dwidth: float,
+        layer: LayerEnum | int,
+        dcplx_trans: kdb.DCplxTrans,
+        klib: KLib = klib,
+        port_type: str = "optical",
+        info: dict[str, Any] = {},
+    ):
         ...
 
     @overload
     def __init__(
         self,
         *,
-        name: str,
+        name: str | None = None,
         width: int,
-        position: tuple[int, int],
-        angle: int,
-        layer: int,
-        port_type: str = "optical",
-        mirror_x: bool = False,
-    ) -> None:
-        ...
-
-    def __init__(
-        self,
-        *,
-        width: Optional[int] = None,
-        layer: Optional[int] = None,
-        name: Optional[str] = None,
+        layer: LayerEnum | int,
         port_type: str = "optical",
-        trans: Optional[TI | str] = None,
-        angle: Optional[int] = None,
-        position: Optional[tuple[int, int]] = None,
+        angle: int,
+        position: tuple[int, int],
         mirror_x: bool = False,
-        port: "Optional[IPortLike[TI]]" = None,
+        klib: KLib = klib,
+        info: dict[str, Any] = {},
     ):
         ...
 
-    def __repr__(self) -> str:
-        return f"Port(name: {self.name}, trans: {self.trans}, width: {self.width}, layer: {f'{self.layer} ({int(self.layer)})' if isinstance(self.layer, LayerEnum) else str(self.layer)}, port_type: {self.port_type})"
-
-    @property
-    def position(self) -> tuple[int, int]:
-        """Gives the x and y coordinates of the Port. This is info stored in the transformation of the port.
-
-        Returns:
-            position: `(self.trans.disp.x, self.trans.disp.y)`
-        """
-        return (self.trans.disp.x, self.trans.disp.y)
-
-    @property
-    def mirror(self) -> bool:
-        """Flag to mirror the transformation. Mirroring is in increments of 45° planes.
-        E.g. a rotation of 90° and mirror flag result in a mirroring on the 45° plane.
-        """
-        return self.trans.is_mirror()
-
-    @property
-    def x(self) -> int:
-        """Convenience for :py:attr:`Port.trans.disp.x`"""
-        return self.trans.disp.x
-
-    @property
-    def y(self) -> int:
-        """Convenience for :py:attr:`Port.trans.disp.y`"""
-        return self.trans.disp.y
-
-    def hash(self) -> bytes:
-        """Provides a hash function to provide a (hopefully) unique id of a port
-
-        Returns:
-            hash-digest: A byte representation from sha3_512()
-        """
-        h = sha3_512()
-        h.update(self.name.encode("UTF-8"))
-        h.update(self.trans.hash().to_bytes(8, "big"))
-        h.update(self.width.to_bytes(8, "big"))
-        h.update(self.port_type.encode("UTF-8"))
-        h.update(self.layer.to_bytes(8, "big"))
-        return h.digest()
-
-    @classmethod
-    def to_yaml(cls, representer, node):  # type: ignore
-        """Internal function used by ruamel.yaml to convert Port to yaml"""
-        return representer.represent_mapping(
-            cls.yaml_tag,
-            {
-                "name": node.name,
-                "width": node.width,
-                "layer": node.layer,
-                "port_type": node.port_type,
-                "trans": node.trans.to_s(),
-            },
-        )
-
-    @property
-    def center(self) -> tuple[int, int]:
-        """Returns port position for gdsfactory compatibility."""
-        return self.position
-
-    @center.setter
-    def center(self, value: tuple[int, int]) -> None:
-        self.trans.disp = kdb.Vector(*value)
-
-    @staticmethod
-    def int_based() -> bool:
-        return True
-
-
-class DPortLike(PortLike[TD, float]):
-    """Protocol for floating number based ports"""
-
     @overload
     def __init__(
         self,
         *,
-        name: str,
-        trans: TD,
-        width: float,
-        layer: int,
-        port_type: str = "optical",
-    ) -> None:
-        ...
-
-    @overload
-    def __init__(
-        self,
-        *,
-        name: Optional[str] = None,
-        port: "DPortLike[TD]",
-    ) -> None:
-        ...
-
-    def __init__(
-        self,
-        *,
-        width: Optional[float] = None,
-        layer: Optional[int] = None,
-        name: Optional[str] = None,
+        name: str | None = None,
+        dwidth: float,
+        layer: LayerEnum | int,
         port_type: str = "optical",
-        trans: Optional[TD | str] = None,
-        angle: Optional[int] = None,
-        position: Optional[tuple[float, float]] = None,
+        dangle: float,
+        dposition: tuple[float, float],
         mirror_x: bool = False,
-        port: "Optional[DPortLike[TD]]" = None,
+        klib: KLib = klib,
+        info: dict[str, Any] = {},
     ):
         ...
 
-    def __repr__(self) -> str:
-        return f"Port(name: {self.name}, trans: {self.trans}, width: {self.width}, layer: {f'{self.layer} ({int(self.layer)})' if isinstance(self.layer, LayerEnum) else str(self.layer)}, port_type: {self.port_type})"
-
-    @property
-    def position(self) -> tuple[float, float]:
-        """Gives the x and y coordinates of the Port. This is info stored in the transformation of the port.
-
-        Returns:
-            position: `(self.trans.disp.x, self.trans.disp.y)`
-        """
-        return (self.trans.disp.x, self.trans.disp.y)
-
-    @property
-    def mirror(self) -> bool:
-        """Flag to mirror the transformation. Mirroring is in increments of 45° planes.
-        E.g. a rotation of 90° and mirror flag result in a mirroring on the 45° plane.
-        """
-        return self.trans.is_mirror()
-
-    @property
-    def x(self) -> float:
-        """Convenience for :py:attr:`Port.trans.disp.x`"""
-        return self.trans.disp.x
-
-    @property
-    def y(self) -> float:
-        """Convenience for :py:attr:`Port.trans.disp.y`"""
-        return self.trans.disp.y
-
-    def hash(self) -> bytes:
-        """Provides a hash function to provide a (hopefully) unique id of a port
-
-        Returns:
-            hash-digest: A byte representation from sha3_512()
-        """
-        h = sha3_512()
-        h.update(self.name.encode("UTF-8"))
-        h.update(self.trans.hash().to_bytes(8, "big"))
-        h.update(self.width.hex().encode("UTF-8"))
-        h.update(self.port_type.encode("UTF-8"))
-        h.update(self.layer.to_bytes(8, "big"))
-        return h.digest()
-
-    @classmethod
-    def to_yaml(cls, representer, node):  # type: ignore
-        """Internal function used by ruamel.yaml to convert Port to yaml"""
-        return representer.represent_mapping(
-            cls.yaml_tag,
-            {
-                "name": node.name,
-                "width": node.width,
-                "layer": node.layer,
-                "port_type": node.port_type,
-                "trans": node.trans.to_s(),
-            },
-        )
-
-    @property
-    def center(self) -> tuple[float, float]:
-        """Returns port position for gdsfactory compatibility."""
-        return self.position
-
-    @center.setter
-    def center(self, value: tuple[float, float]) -> None:
-        self.trans.disp = kdb.DVector(*value)
-
-    @staticmethod
-    def int_based() -> bool:
-        return False
-
-
-class SPortLike(PortLike[TS, Any]):
-    """Protocol for simple transformation based ports"""
-
-    @property
-    def angle(self) -> int:
-        """Angle of the transformation. In the range of [0,1,2,3] which are increments in 90°. Not to be confused with `rot`
-        of the transformation which keeps additional info about the mirror flag."""
-        return self.trans.angle
-
-    @property
-    def orientation(self) -> float:
-        """Returns orientation in degrees for gdsfactory compatibility."""
-        return self.trans.angle * 90
-
-    @orientation.setter
-    def orientation(self, value: int) -> None:
-        self.trans.angle = int(value // 90)
-
-    @staticmethod
-    def complex() -> bool:
-        return False
-
-
-class CPortLike(PortLike[TC, Any]):
-    """Protocol for complex transformation based ports"""
-
-    trans: TC
-
-    @property
-    def angle(self) -> float:
-        """Angle of the transformation. In the range of [0,1,2,3] which are increments in 90°. Not to be confused with `rot`
-        of the transformation which keeps additional info about the mirror flag."""
-        return self.trans.angle
-
-    @property
-    def orientation(self) -> float:
-        """Returns orientation in degrees for gdsfactory compatibility."""
-        return self.trans.angle
-
-    @orientation.setter
-    def orientation(self, value: float) -> None:
-        self.trans.angle = value
-
-    @staticmethod
-    def complex() -> bool:
-        return True
-
-
-class Port(IPortLike[kdb.Trans], SPortLike[kdb.Trans]):
-    """A port is similar to a pin in electronics. In addition to the location and layer
-    that defines a pin, a port also contains an orientation and a width. This can be fully represented with a transformation, integer and layer_index.
-    """
-
-    yaml_tag = "!Port"
-    name: str
-    width: int
-    layer: int
-    trans: kdb.Trans
-    port_type: str
-
     def __init__(
         self,
         *,
-        width: Optional[int] = None,
-        layer: Optional[int] = None,
-        name: Optional[str] = None,
+        name: str | None = None,
+        width: int | None = None,
+        dwidth: float | None = None,
+        layer: int | None = None,
         port_type: str = "optical",
-        trans: Optional[kdb.Trans | str] = None,
-        angle: Optional[int] = None,
-        position: Optional[tuple[int, int]] = None,
+        trans: kdb.Trans | str | None = None,
+        dcplx_trans: kdb.DCplxTrans | str | None = None,
+        angle: int | None = None,
+        dangle: float | None = None,
+        position: tuple[int, int] | None = None,
+        dposition: tuple[float, float] | None = None,
         mirror_x: bool = False,
-        port: Optional["Port"] = None,
+        port: "Port | None" = None,
+        klib: KLib = klib,
+        info: dict[str, Any] = {},
     ):
+        """Create a port from dbu or um based units."""
+        self.klib = klib
+        self.d = DPart(self)
+        self.info = info.copy()
         if port is not None:
             self.name = port.name if name is None else name
-            self.trans = port.trans.dup()
-            self.port_type = port.port_type
-            self.layer = port.layer
-            self.width = port.width
-        elif name is None or width is None or layer is None:
-            raise ValueError("name, width, layer must be given if the 'port is None'")
-        else:
-            self.name = name
-            self.width = width
-            self.layer = layer
-            self.port_type = port_type
-            if trans is not None:
-                self.trans = (
-                    kdb.Trans.from_s(trans) if isinstance(trans, str) else trans.dup()
-                )
-            elif angle is None or position is None:
-                raise ValueError(
-                    "angle and position must be given if creating a gdsfactory like port"
-                )
-            else:
-                self.trans = kdb.Trans(angle, mirror_x, kdb.Vector(*position))
-
-    def move(
-        self, origin: tuple[int, int], destination: Optional[tuple[int, int]] = None
-    ) -> None:
-        """Convenience from the equivalent of gdsfactory. Moves the"""
-        dest = kdb.Vector(*(origin if destination is None else destination))
-        org = kdb.Vector(0, 0) if destination is None else kdb.Vector(*origin)
-
-        self.trans = self.trans * kdb.Trans(dest - org)
-
-    @classmethod
-    def from_yaml(cls: "Type[Port]", constructor, node) -> "Port":  # type: ignore
-        """Internal function used by the placer to convert yaml to a Port"""
-        d = dict(constructor.construct_pairs(node))
-        return cls(**d)
-
-    def rotate(self, angle: int) -> None:
-        """Rotate the Port
-
-        Args:
-            angle: The angle to rotate in increments of 90°
-        """
-        self.trans = self.trans * kdb.Trans(angle, False, 0, 0)
-
-    def copy(self, trans: kdb.Trans = kdb.Trans.R0) -> "Port":
-        """Get a copy of a port
-
-        Args:
-            trans: an optional transformation applied to the port to be copied
-
-        Returns:
-            port (:py:class:`Port`): a copy of the port
-        """
-        _trans = trans * self.trans
-        return Port(
-            name=self.name,
-            trans=_trans,
-            layer=self.layer,
-            port_type=self.port_type,
-            width=self.width,
-        )
-
-    def dcplx_trans(self, dbu: float) -> kdb.DCplxTrans:
-        return kdb.DCplxTrans(self.trans.to_dtype(dbu))
 
-
-class DPort(DPortLike[kdb.DTrans], SPortLike[kdb.DTrans]):
-    """A port is similar to a pin in electronics. In addition to the location and layer
-    that defines a pin, a port also contains an orientation and a width. This can be fully represented with a transformation, integer and layer_index.
-    """
-
-    yaml_tag = "!DPort"
-    name: str
-    width: float
-    layer: int
-    trans: kdb.DTrans
-    port_type: str
-
-    def __init__(
-        self,
-        *,
-        width: Optional[float] = None,
-        layer: Optional[int] = None,
-        name: Optional[str] = None,
-        port_type: str = "optical",
-        trans: Optional[kdb.DTrans | str] = None,
-        angle: Optional[int] = None,
-        position: Optional[tuple[float, float]] = None,
-        mirror_x: bool = False,
-        port: Optional["DPort"] = None,
-    ):
-        if port is not None:
-            self.name: str = port.name if name is None else name
-            self.trans: kdb.DTrans = port.trans.dup()
-            self.port_type: str = port.port_type
-            self.layer: int = port.layer
-            self.width: float = port.width
-        elif name is None or width is None or layer is None:
-            raise ValueError("name, width, layer must be given if the 'port is None'")
-        else:
-            self.name = name
-            self.width = width
-            self.layer = layer
-            self.port_type = port_type
-            if trans is not None:
-                self.trans = (
-                    kdb.DTrans.from_s(trans) if isinstance(trans, str) else trans.dup()
-                )
-            elif angle is None or position is None:
-                raise ValueError(
-                    "angle and position must be given if creating a gdsfactory like port"
-                )
+            if port.dcplx_trans.is_complex():
+                self.dcplx_trans = port.dcplx_trans
             else:
-                self.trans = kdb.DTrans(angle, mirror_x, *position)
-
-    def move(
-        self,
-        origin: tuple[float, float],
-        destination: Optional[tuple[float, float]] = None,
-    ) -> None:
-        """Convenience from the equivalent of gdsfactory. Moves the"""
-        dest = kdb.DVector(*(origin if destination is None else destination))
-        org = kdb.DVector(0, 0) if destination is None else kdb.DVector(*origin)
-
-        self.trans = self.trans * kdb.DTrans(dest - org)
-
-    @classmethod
-    def from_yaml(cls: "Type[DPort]", constructor: Any, node: Any) -> "DPort":
-        """Internal function used by the placer to convert yaml to a Port"""
-        d = dict(constructor.construct_pairs(node))
-        return cls(**d)
+                self.trans = port.trans
 
-    def rotate(self, angle: int) -> None:
-        """Rotate the Port
-
-        Args:
-            angle: The angle to rotate in increments of 90°
-        """
-        self.trans = self.trans * kdb.DTrans(angle, False, 0, 0)
-
-    def copy(self, trans: kdb.DTrans = kdb.DTrans.R0) -> "DPort":
-        """Get a copy of a port
-
-        Args:
-            trans: an optional transformation applied to the port to be copied
-
-        Returns:
-            port (:py:class:`Port`): a copy of the port
-        """
-        _trans = trans * self.trans
-        return DPort(
-            name=self.name,
-            trans=_trans,
-            layer=self.layer,
-            port_type=self.port_type,
-            width=self.width,
-        )
-
-    def dcplx_trans(self, dbu: float) -> kdb.DCplxTrans:
-        return kdb.DCplxTrans(self.trans)
-
-
-class ICplxPort(IPortLike[kdb.ICplxTrans], CPortLike[kdb.ICplxTrans]):
-    """A port is similar to a pin in electronics. In addition to the location and layer
-    that defines a pin, a port also contains an orientation and a width. This can be fully represented with a transformation, integer and layer_index.
-    """
-
-    yaml_tag = "!ICplxPort"
-    name: str
-    width: int
-    layer: int
-    trans: kdb.ICplxTrans
-    port_type: str
-
-    def __init__(
-        self,
-        *,
-        width: Optional[int] = None,
-        layer: Optional[int] = None,
-        name: Optional[str] = None,
-        port_type: str = "optical",
-        trans: Optional[kdb.ICplxTrans | str] = None,
-        angle: Optional[int] = None,
-        position: Optional[tuple[int, int]] = None,
-        mirror_x: bool = False,
-        port: Optional["ICplxPort"] = None,
-    ):
-        if port is not None:
-            self.name = port.name if name is None else name
-            self.trans = port.trans.dup()
             self.port_type = port.port_type
             self.layer = port.layer
             self.width = port.width
-        elif name is None or width is None or layer is None:
-            raise ValueError("name, width, layer must be given if the 'port is None'")
+        elif (width is None and dwidth is None) or layer is None:
+            raise ValueError("width, layer must be given if the 'port is None'")
         else:
-            self.name = name
-            self.width = width
-            self.layer = layer
-            self.port_type = port_type
             if trans is not None:
-                self.trans = (
-                    kdb.ICplxTrans.from_s(trans)
-                    if isinstance(trans, str)
-                    else trans.dup()
-                )
-            elif angle is None or position is None:
-                raise ValueError(
-                    "angle and position must be given if creating a gdsfactory like port"
-                )
-            else:
-                self.trans = kdb.ICplxTrans(1, angle, mirror_x, *position)
-
-    def move(
-        self,
-        origin: tuple[int, int],
-        destination: Optional[tuple[int, int]] = None,
-    ) -> None:
-        """Convenience from the equivalent of gdsfactory. Moves the"""
-        dest = kdb.Vector(*(origin if destination is None else destination))
-        org = kdb.Vector(0, 0) if destination is None else kdb.Vector(*origin)
-
-        self.trans = self.trans * kdb.ICplxTrans(dest - org)
-
-    @classmethod
-    def from_yaml(cls: "Type[ICplxPort]", constructor: Any, node: Any) -> "ICplxPort":
-        """Internal function used by the placer to convert yaml to a Port"""
-        d = dict(constructor.construct_pairs(node))
-        return cls(**d)
-
-    def rotate(self, angle: int) -> None:
-        """Rotate the Port
-
-        Args:
-            angle: The angle to rotate in increments of 90°
-        """
-        self.trans = self.trans * kdb.ICplxTrans(1, angle, False, 0, 0)
-
-    def copy(self, trans: kdb.ICplxTrans = kdb.ICplxTrans.R0) -> "ICplxPort":
-        """Get a copy of a port
-
-        Args:
-            trans: an optional transformation applied to the port to be copied
-
-        Returns:
-            port (:py:class:`Port`): a copy of the port
-        """
-        _trans = trans * self.trans
-        return ICplxPort(
-            name=self.name,
-            trans=_trans,
-            layer=self.layer,
-            port_type=self.port_type,
-            width=self.width,
-        )
-
-    def dcplx_trans(self, dbu: float) -> kdb.DCplxTrans:
-        return self.trans.to_itrans(dbu)
-
-
-class DCplxPort(DPortLike[kdb.DCplxTrans], CPortLike[kdb.DCplxTrans]):
-    """A port is similar to a pin in electronics. In addition to the location and layer
-    that defines a pin, a port also contains an orientation and a width. This can be fully represented with a transformation, integer and layer_index.
-    """
-
-    yaml_tag = "!DCplxPort"
-    name: str
-    width: float
-    layer: int
-    trans: kdb.DCplxTrans
-    port_type: str
+                # self.width = cast(int, width)
+                if isinstance(trans, str):
+                    self.trans = kdb.Trans.from_s(trans)
+                else:
+                    self.trans = trans.dup()
+                assert width is not None
+                self.width = width
+                self.port_type = port_type
+            elif dcplx_trans is not None:
+                if isinstance(dcplx_trans, str):
+                    self.dcplx_trans = kdb.DCplxTrans.from_s(dcplx_trans)
+                else:
+                    self.dcplx_trans = dcplx_trans.dup()
+                assert dwidth is not None
+                self.d.width = dwidth
+                assert self.width * self.klib.dbu == float(
+                    dwidth
+                ), "When converting to dbu the width does not match the desired width!"
+            elif width is not None:
+                assert angle is not None
+                assert position is not None
+                self.trans = kdb.Trans(angle, mirror_x, *position)
+                self.width = width
+                self.port_type = port_type
+            elif dwidth is not None:
+                assert dangle is not None
+                assert dposition is not None
+                self.dcplx_trans = kdb.DCplxTrans(1, dangle, mirror_x, *dposition)
 
-    def __init__(
-        self,
-        *,
-        width: Optional[float] = None,
-        layer: Optional[int] = None,
-        name: Optional[str] = None,
-        port_type: str = "optical",
-        trans: Optional[kdb.DCplxTrans | str] = None,
-        angle: Optional[float] = None,
-        position: Optional[tuple[float, float]] = None,
-        mirror_x: bool = False,
-        port: Optional["DCplxPort"] = None,
-    ):
-        if port is not None:
-            self.name: str = port.name if name is None else name
-            self.trans: kdb.DCplxTrans = port.trans.dup()
-            self.port_type: str = port.port_type
-            self.layer: int = port.layer
-            self.width: float = port.width
-        elif name is None or width is None or layer is None:
-            raise ValueError("name, width, layer must be given if the 'port is None'")
-        else:
+            assert layer is not None
             self.name = name
-            self.width = width
             self.layer = layer
             self.port_type = port_type
-            if trans is not None:
-                self.trans = (
-                    kdb.DCplxTrans.from_s(trans)
-                    if isinstance(trans, str)
-                    else trans.dup()
-                )
-            elif angle is None or position is None:
-                raise ValueError(
-                    "angle and position must be given if creating a gdsfactory like port"
-                )
-            else:
-                self.trans = kdb.DCplxTrans(1, angle, mirror_x, *position)
-
-    def move(
-        self,
-        origin: tuple[float, float],
-        destination: Optional[tuple[float, float]] = None,
-    ) -> None:
-        """Convenience from the equivalent of gdsfactory. Moves the"""
-        dest = kdb.DVector(*(origin if destination is None else destination))
-        org = kdb.DVector(0, 0) if destination is None else kdb.DVector(*origin)
-
-        self.trans = self.trans * kdb.DCplxTrans(dest - org)
 
     @classmethod
-    def from_yaml(
-        cls: "Callable[..., DCplxPort]", constructor: Any, node: Any
-    ) -> "DCplxPort":
-        """Internal function used by the placer to convert yaml to a Port"""
+    def from_yaml(cls: "type[Port]", constructor, node) -> "Port":  # type: ignore
+        """Internal function used by the placer to convert yaml to a Port."""
         d = dict(constructor.construct_pairs(node))
         return cls(**d)
 
-    def rotate(self, angle: int) -> None:
-        """Rotate the Port
-
-        Args:
-            angle: The angle to rotate in increments of 90°
-        """
-        self.trans = self.trans * kdb.DCplxTrans(1, angle, False, 0, 0)
-
-    def copy(self, trans: kdb.DCplxTrans = kdb.DCplxTrans.R0) -> "DCplxPort":
-        """Get a copy of a port
+    def copy(self, trans: kdb.Trans | kdb.DCplxTrans = kdb.Trans.R0) -> "Port":
+        """Get a copy of a port.
 
         Args:
             trans: an optional transformation applied to the port to be copied
 
         Returns:
             port (:py:class:`Port`): a copy of the port
         """
-        _trans = trans * self.trans
-        return DCplxPort(
+        if self._trans:
+            if isinstance(trans, kdb.Trans):
+                _trans = trans * self.trans
+                return Port(
+                    name=self.name,
+                    trans=_trans,
+                    layer=self.layer,
+                    port_type=self.port_type,
+                    width=self.width,
+                    klib=self.klib,
+                )
+            elif not trans.is_complex():
+                _trans = trans.s_trans().to_itype(self.klib.dbu) * self.trans
+                return Port(
+                    name=self.name,
+                    trans=_trans,
+                    layer=self.layer,
+                    port_type=self.port_type,
+                    width=self.width,
+                    klib=self.klib,
+                )
+        if isinstance(trans, kdb.Trans):
+            dtrans = kdb.DCplxTrans(trans.to_dtype(self.klib.dbu))
+            _dtrans = dtrans * self.dcplx_trans
+        else:
+            _dtrans = trans * self.dcplx_trans
+        return Port(
             name=self.name,
-            trans=_trans,
+            dcplx_trans=_dtrans,
+            dwidth=self.d.width,
             layer=self.layer,
+            klib=self.klib,
             port_type=self.port_type,
-            width=self.width,
+            info=self.info,
         )
 
-    def dcplx_trans(self, dbu: float) -> kdb.DCplxTrans:
-        return self.trans.dup()
-
+    @property
+    def x(self) -> int:
+        """X coordinate of the port in dbu."""
+        return self.trans.disp.x
 
-class ABCKCell(kdb.Cell, ABC, Generic[PT]):
+    @x.setter
+    def x(self, value: int) -> None:
+        if self._trans:
+            vec = self._trans.disp
+            vec.x = value
+            self._trans.disp = vec
+        elif self._dcplx_trans:
+            vec = self.trans.disp
+            vec.x = value
+            self._dcplx_trans.disp = vec.to_dtype(self.klib.dbu)
 
-    """Derived from :py:class:`klayout.db.Cell`. Additionally to a standard cell, this one will keep track of :py:class:`Port` and allow to store metadata in a dictionary
+    @property
+    def y(self) -> int:
+        """Y coordinate of the port in dbu."""
+        return self.trans.disp.x
 
-    Attributes:
-        ports (:py:class:`Ports`):  Contains all the ports of the cell and makes them accessible
-        insts (:py:class:`list`[:py:class:`Instance`]): All instances intantiated in this KCell
-        settings (:py:class:`dict`): Dictionary containing additional metadata of the KCell. Can be autopopulated by :py:func:`autocell`
-        _kdb_cell (:py:class:`klayout.db.Cell`): Internal reference to the :py:class:`klayout.db.Cell` object. Not intended for direct access
-    """
+    @y.setter
+    def y(self, value: int) -> None:
+        if self._trans:
+            vec = self._trans.disp
+            vec.y = value
+            self._trans.disp = vec
+        elif self._dcplx_trans:
+            vec = self.trans.disp
+            vec.y = value
+            self._dcplx_trans.disp = vec.to_dtype(self.klib.dbu)
 
-    yaml_tag: str = "!NotImplemented"
-    _ports: "Ports | CplxPorts"
-    complex: bool
-
-    def __new__(
-        cls,
-        name: Optional[str] = None,
-        klib: KLib = klib,
-        kdb_cell: Optional[kdb.Cell] = None,
-        ports: "Optional[CplxPorts | Ports]" = None,
-    ) -> "KCell":
-        """Create a KLayout cell and change its class to KCell
+    @property
+    def trans(self) -> kdb.Trans:
+        """Simple Transformation of the Port.
 
-        Args:
-            name: name of the cell, if `None`, it will set the name to "Unnamed_"
-            library: KLib object that stores the layout and metadata about the KCells
-            kdb_cell
+        If this is set with the setter, it will overwrite any transformation or
+        dcplx transformation
         """
+        return self._trans or self.dcplx_trans.s_trans().to_itype(self.klib.dbu)
 
-        if kdb_cell is None:
-            _name = "Unnamed_" if name is None else name
-            cell = klib.create_cell(
-                name=_name,
-            )
-        else:
-            cell = kdb_cell
-        cell.__class__ = cls
-        return cell  # type: ignore[return-value]
-
-    def __init__(
-        self,
-        name: Optional[str] = None,
-        klib: KLib = klib,
-        kdb_cell: Optional[kdb.Cell] = None,
-        ports: "Optional[CplxPorts | Ports]" = None,
-    ) -> None:
-        self.klib = klib
-        self.insts: list[Instance] = []
-        self.settings: dict[str, Any] = {}
-        self._locked = False
-        self.info: dict[str, Any] = {}
-        if name is None and kdb_cell is None:
-            self.name = f"Unnamed_{self.cell_index()}"
+    @trans.setter
+    def trans(self, value: kdb.Trans) -> None:
+        self._trans = value.dup()
+        self._dcplx_trans = None
 
     @property
-    def ports(self) -> "Ports | CplxPorts":
-        return self._ports
+    def dcplx_trans(self) -> kdb.DCplxTrans:
+        """Complex transformation (µm based).
 
-    @ports.setter
-    def ports(self, new_ports: "InstancePorts | Ports | CplxPorts") -> None:
-        self._ports = new_ports.copy()
+        If the internal transformation is simple, return a complex copy.
 
-    @overload
-    def create_port(
-        self,
-        *,
-        name: str,
-        trans: kdb.Trans,
-        width: int,
-        layer: int | LayerEnum,
-        port_type: str = "optical",
-    ) -> None:
-        ...
-
-    @overload
-    def create_port(
-        self,
-        *,
-        name: Optional[str] = None,
-        port: Port,
-    ) -> None:
-        ...
-
-    @overload
-    def create_port(
-        self,
-        *,
-        name: str,
-        width: int,
-        position: tuple[int, int],
-        angle: int,
-        layer: int | LayerEnum,
-        port_type: str = "optical",
-        mirror_x: bool = False,
-    ) -> None:
-        ...
-
-    def create_port(self, **kwargs: Any) -> None:
-        """Create a new port. Equivalent to :py:attr:`~add_port(Port(...))`"""
-        self.ports.create_port(**kwargs)
-
-    @abstractmethod
-    def add_port(self, port: PortLike[TT, FI], name: Optional[str] = None) -> None:
-        """Add an existing port. E.g. from an instance to propagate the port
-
-        Args:
-            port: The port to add. Port should either be a :py:class:`~Port`, or will be converted to an integer based port with 90° increment
-            name: Overwrite the name of the port
+        The setter will set a complex transformation and overwrite the internal
+        transformation (set simple to `None` and the complex to the provided value.
         """
-        ...
-
-    @overload
-    def create_inst(
-        self,
-        cell: "KCell",
-        trans: kdb.Trans | kdb.Vector = kdb.Trans.R0,
-        a: Optional[kdb.Vector] = None,
-        b: kdb.Vector = kdb.Vector(),
-        na: int = 1,
-        nb: int = 1,
-    ) -> "Instance":
-        ...
-
-    @overload
-    def create_inst(
-        self,
-        cell: "CplxKCell",
-        trans: kdb.DCplxTrans | kdb.DVector = kdb.DCplxTrans.R0,
-        a: Optional[kdb.DVector] = None,
-        b: kdb.DVector = kdb.DVector(),
-        na: int = 1,
-        nb: int = 1,
-    ) -> "Instance":
-        ...
+        return self._dcplx_trans or kdb.DCplxTrans(self.trans.to_dtype(self.klib.dbu))
 
-    def create_inst(
-        self,
-        cell: CellType,
-        trans: kdb.Trans | kdb.DCplxTrans | kdb.Vector | kdb.DVector = kdb.Trans(),
-        a: Optional[kdb.Vector | kdb.DVector] = None,
-        b: kdb.Vector | kdb.DVector = kdb.Vector(),
-        na: int = 1,
-        nb: int = 1,
-    ) -> "Instance":
-        """Add an instance of another KCell
+    @dcplx_trans.setter
+    def dcplx_trans(self, value: kdb.DCplxTrans) -> None:
+        self._dcplx_trans = value.dup()
+        self._trans = None
 
-        Args:
-            cell: The cell to be added
-            trans: The transformation applied to the reference
+    @property
+    def angle(self) -> int:
+        """Angle of the transformation.
 
-        Returns:
-            :py:class:`~Instance`: The created instance
+        In the range of [0,1,2,3] which are increments in 90°. Not to be confused
+        with `rot` of the transformation which keeps additional info about the
+        mirror flag.
         """
-        if isinstance(cell, KCell):
-            ca = (
-                self.insert(kdb.CellInstArray(cell, trans))  # type: ignore[arg-type]
-                if a is None
-                else self.insert(kdb.CellInstArray(cell, trans, a, b, na, nb))  # type: ignore[arg-type]
-            )
-        elif a is None:
-            ca = self.insert(kdb.DCellInstArray(cell, trans))  # type: ignore[arg-type]
-        else:
-            ca = self.insert(kdb.DCellInstArray(cell, trans, a, b, na, nb))  # type: ignore[arg-type]
-
-        inst = Instance(cell, ca)  # type: ignore[misc]
-        self.insts.append(inst)
-        return inst
+        return self.trans.angle
 
-    def _kdb_copy(self) -> kdb.Cell:
-        return kdb.Cell.dup(self)
+    @angle.setter
+    def angle(self, value: int) -> None:
+        self._trans = self.trans.dup()
+        self._dcplx_trans = None
+        self._trans.angle = value
 
-    def layer(self, *args: Any, **kwargs: Any) -> int:
-        """Get the layer info, convenience for klayout.db.Layout.layer"""
-        return self.klib.layer(*args, **kwargs)
+    @property
+    def orientation(self) -> float:
+        """Returns orientation in degrees for gdsfactory compatibility."""
+        return self.dcplx_trans.angle
 
-    def __lshift__(self, cell: CellType) -> "Instance":
-        """Convenience function for :py:attr:"~create_inst(cell)`
+    @orientation.setter
+    def orientation(self, value: float) -> None:
+        if not self.dcplx_trans.is_complex() and value in [0, 90, 180, 270]:
+            self.trans.angle = int(value / 90)
+        else:
+            self._dcplx_trans = self.dcplx_trans
+            self.dcplx_trans.angle = value
 
-        Args:
-            cell: The cell to be added as an instance
-        """
-        return self.create_inst(cell)  # type: ignore[arg-type]
+    @property
+    def mirror(self) -> bool:
+        """Returns `True`/`False` depending on the mirror flag on the transformation."""
+        return self.trans.is_mirror()
 
     def hash(self) -> bytes:
-        """Provide a unique hash of the cell"""
+        """Hash of Port."""
         h = sha3_512()
-        h.update(self.name.encode("ascii", "ignore"))
-
-        for l in self.layout().layer_indexes():
-            h.update(l.to_bytes(8, "big"))
-            for shape in self.shapes(l).each(kdb.Shapes.SRegions):
-                h.update(shape.polygon.hash().to_bytes(8, "big"))
-            for shape in self.shapes(l).each(kdb.Shapes.STexts):
-                h.update(shape.text.hash().to_bytes(8, "big"))
-        port_hashs = list(sorted(p.hash() for p in self.ports._ports))
-        for _hash in port_hashs:
-            h.update(_hash)
-        insts_hashs = list(sorted(inst.hash() for inst in self.insts))
-        for _hash in insts_hashs:
-            h.update(_hash)
+        name = self.name if self.name else ""
+        h.update(name.encode("UTF-8"))
+        h.update(self.trans.hash().to_bytes(8, "big"))
+        h.update(self.width.to_bytes(8, "big"))
+        h.update(self.port_type.encode("UTF-8"))
+        h.update(self.layer.to_bytes(8, "big"))
         return h.digest()
 
-    def autorename_ports(
-        self, rename_func: Optional[Callable[..., None]] = None
-    ) -> None:
-        """Rename the ports with the schema angle -> "NSWE" and sort by x and y
+    def __repr__(self) -> str:
+        """String representation of port."""
+        ln = self.layer.name if isinstance(self.layer, LayerEnum) else self.layer
+        if self._trans:
+            return (
+                f"Port({'name: ' + self.name if self.name else ''}"
+                f", width: {self.width}, trans: {self.trans.to_s()}, layer: "
+                f"{ln}, port_type: {self.port_type})"
+            )
+        else:
+            return (
+                f"Port({'name: ' + self.name if self.name else ''}"
+                f", dwidth: {self.d.width}, trans: {self.dcplx_trans.to_s()}, layer: "
+                f"{ln}, port_type: {self.port_type})"
+            )
+
+
+class DPart:
+    """Make the port able to dynamically give um based info."""
+
+    def __init__(self, parent: Port):
+        """Constructor, just needs a pointer to the port.
 
         Args:
-            rename_func: Function that takes Iterable[Port] and renames them. This can of course contain a filter and only rename some of the ports
+            parent: port that this should be attached to
         """
+        self.parent = parent
 
-        if rename_func is None:
-            self.klib.rename_function(self.ports._ports)
-        else:
-            rename_func(self.ports._ports)
+    @property
+    def x(self) -> float:
+        """X coordinate of the port in um."""
+        return self.parent.dcplx_trans.disp.x
 
-    def flatten(self, prune: bool = True, merge: bool = True) -> None:  # type: ignore[override]
-        """Flatten the cell. Pruning will delete the klayout.db.Cell if unused, but might cause artifacts at the moment
+    @x.setter
+    def x(self, value: float) -> None:
+        vec = self.parent.dcplx_trans.disp
+        vec.x = value
+        if self.parent._trans:
+            self.parent._trans.disp = vec.to_itype(self.parent.klib.dbu)
+        elif self.parent._dcplx_trans:
+            self.parent._dcplx_trans.disp = vec
 
-        Args:
-            prune: Delete unused child cells if they aren't used in any other KCell
-            merge: Merge the shapes on all layers"""
-        super().flatten(False)  # prune)
-        self.insts = []
+    @property
+    def y(self) -> float:
+        """Y coordinate of the port in um."""
+        return self.parent.dcplx_trans.disp.y
 
-        if merge:
-            for layer in self.layout().layer_indexes():
-                reg = kdb.Region(self.begin_shapes_rec(layer))
-                reg.merge()
-                self.clear(layer)
-                self.shapes(layer).insert(reg)
+    @y.setter
+    def y(self, value: float) -> None:
+        vec = self.parent.dcplx_trans.disp
+        vec.y = value
+        if self.parent._trans:
+            self.parent._trans.disp = vec.to_itype(self.parent.klib.dbu)
+        elif self.parent._dcplx_trans:
+            self.parent._dcplx_trans.disp = vec
 
-    def draw_ports(self) -> None:
-        """Draw all the ports on their respective :py:attr:`Port.layer`:"""
+    @property
+    def position(self) -> tuple[float, float]:
+        """Coordinate of the port in um."""
+        vec = self.parent.dcplx_trans.disp
+        return (vec.x, vec.y)
+
+    @position.setter
+    def position(self, pos: tuple[float, float]) -> None:
+        if self.parent._trans:
+            self.parent._trans.disp = kdb.DVector(*pos).to_itype(self.parent.klib.dbu)
+        elif self.parent._dcplx_trans:
+            self.parent._dcplx_trans.disp = kdb.DVector(*pos)
 
-        for port in self.ports._ports:
-            if isinstance(port, IPortLike):
-                w = port.width
-                poly = kdb.Polygon(
-                    [kdb.Point(0, -w // 2), kdb.Point(0, w // 2), kdb.Point(w // 2, 0)]
-                )
-                self.shapes(port.layer).insert(poly.transformed(port.trans))
-                self.shapes(port.layer).insert(
-                    kdb.Text(port.name, kdb.Trans.R0).transformed(port.trans)
-                )
-            elif isinstance(port, DPortLike):
-                wd = port.width
-                dpoly = kdb.DPolygon(
-                    [
-                        kdb.DPoint(0, -wd / 2),
-                        kdb.DPoint(0, wd / 2),
-                        kdb.DPoint(wd / 2, 0),
-                    ]
-                )
-                self.shapes(port.layer).insert(dpoly.transformed(port.trans))
-                self.shapes(port.layer).insert(
-                    kdb.DText(port.name, kdb.DTrans.R0).transformed(port.trans)
-                )
+    @property
+    def angle(self) -> float:
+        """Angle of the port in degrees."""
+        return self.parent.dcplx_trans.angle
 
-    def write(
-        self, filename: str | Path, save_options: kdb.SaveLayoutOptions = default_save()
-    ) -> None:
-        return super().write(str(filename), save_options)
+    @angle.setter
+    def angle(self, value: float) -> None:
+        if value in [0, 90, 180, 270]:
+            if self.parent._trans:
+                self.parent._trans.angle = int(value / 90)
+                return
+
+        trans = self.parent.dcplx_trans
+        trans.angle = value
+        self.parent.dcplx_trans = trans
 
-    @classmethod
-    def to_yaml(cls, representer, node):  # type: ignore
-        """Internal function to convert the cell to yaml"""
-        d = {
-            "name": node.name,
-            "ports": node.ports,  # Ports.to_yaml(representer, node.ports),
-        }
+    @property
+    def width(self) -> float:
+        """Width of the port in um."""
+        return self.parent.width * self.parent.klib.dbu
+
+    @width.setter
+    def width(self, value: float) -> None:
+        self.parent.width = int(value / self.parent.klib.dbu)
+        assert self.parent.width * self.parent.klib.dbu == float(value), (
+            "When converting to dbu the width does not match the desired width"
+            f"({self.width} / {value})!"
+        )
 
-        insts = [
-            {"cellname": inst.cell.name, "trans": inst.instance.trans.to_s()}
-            for inst in node.insts
-        ]
-        shapes = {
-            node.layout()
-            .get_info(layer)
-            .to_s(): [shape.to_s() for shape in node.shapes(layer).each()]
-            for layer in node.layout().layer_indexes()
-            if not node.shapes(layer).is_empty()
-        }
 
-        if insts:
-            d["insts"] = insts
-        if shapes:
-            d["shapes"] = shapes
-        if len(node.settings) > 0:
-            d["settings"] = node.settings
-        return representer.represent_mapping(cls.yaml_tag, d)
+class KCell:
+    """KLayout cell and change its class to KCell.
 
-    @classmethod
-    @abstractmethod
-    def from_yaml(
-        cls: "Callable[..., ABCKCell[PT]]",
-        constructor: Any,
-        node: Any,
-        verbose: bool = False,
-    ) -> "ABCKCell[PT]":
-        ...
+    A KCell is a dynamic proxy for :py:class:~`kdb.Cell`. It has all the
+    attributes of the official KLayout class. Some attributes have been adjusted
+    to return KCell specific sub classes. If the function is listed here in the
+    docs, they have been adjusted for KFactory specifically. This object will
+    transparently proxy to :py:class:`kdb.Cell`. Meaning any attribute not directly
+    defined in this class that are available from the KLayout counter part can
+    still be accessed. The pure KLayout object can be accessed with
+    :py:attr:`KCell._kdb_cell`.
 
+    Attributes:
+        klib: Library object that is the manager of the KLayout
+            :py:class:`kdb.Layout`
+        settings: A dictionary containing settings populated by:py:func:`autocell`
+        info: Dictionary for storing additional info if necessary. This is not
+            passed to the GDS and therefore not reversible.
+        _kdb_cell: Pure KLayout cell object.
+        _locked: If set the cell shouldn't be modified anymore.
+        ports: Manages the ports of the cell.
+    """
 
-class KCell(ABCKCell[Port]):
     yaml_tag = "!KCell"
+    _ports: "Ports"
 
     def __init__(
         self,
-        name: Optional[str] = None,
+        name: str | None = None,
         klib: KLib = klib,
-        kdb_cell: Optional[kdb.Cell] = None,
-        ports: "Optional[Ports]" = None,
+        kdb_cell: kdb.Cell | None = None,
+        ports: "Ports | None" = None,
     ):
-        super().__init__(name=name, klib=klib, kdb_cell=kdb_cell)
+        """Constructor of KCell.
+
+        Args:
+            name: Name of the cell, if None will autogenerate name to
+                "Unnamed_<cell_index>".
+            klib: KLib the cell should be attached to.
+            kdb_cell: If not `None`, a KCell will be created from and existing
+                KLayout Cell
+            ports: Attach an existing :py:class:`~Ports` object to the KCell,
+                if `None` create an empty one.
+        """
+        self.klib = klib
+        self.insts: Instances = Instances()
+        self.settings: dict[str, Any] = {}
+        self.info: dict[str, Any] = {}
+        self._locked = False
+        if name is None:
+            _name = "Unnamed_!"
+        else:
+            _name = name
+        self._kdb_cell = kdb_cell or klib.create_cell(_name)
+        if _name == "Unnamed_!":
+            self._kdb_cell.name = f"Unnamed_{self.cell_index()}"
         self.klib.register_cell(self, allow_reregister=True)
-        self.ports: Ports = ports or Ports()
+        self.ports: Ports = ports or Ports(self.klib)
         self.complex = False
 
         if kdb_cell is not None:
             for inst in kdb_cell.each_inst():
-                self.insts.append(Instance(self.klib[inst.cell.name], inst))  # type: ignore[misc]
+                self.insts.append(Instance(self.klib, inst))
+
+    @property
+    def name(self) -> str:
+        """Name of the KCell."""
+        return self._kdb_cell.name
+
+    @name.setter
+    def name(self, value: str) -> None:
+        self._kdb_cell.name = value
+
+    @property
+    def prop_id(self) -> int:
+        """Gets the properties ID associated with the cell."""
+        return self._kdb_cell.prop_id
+
+    @prop_id.setter
+    def prop_id(self, value: int) -> None:
+        self._kdb_cell.prop_id = value
+
+    @property
+    def ghost_cell(self) -> bool:
+        """Returns a value indicating whether the cell is a "ghost cell"."""
+        return self._kdb_cell.ghost_cell
+
+    @ghost_cell.setter
+    def ghost_cell(self, value: bool) -> None:
+        self._kdb_cell.ghost_cell = value
+
+    def __getattr__(self, name):  # type: ignore[no-untyped-def]
+        """If KCell doesn't have an attribute, look in the KLayout Cell."""
+        return getattr(self._kdb_cell, name)
 
     def dup(self) -> "KCell":
-        """Copy the full cell
+        """Copy the full cell.
+
+        Sets :py:attr:_locked to `False`
 
         Returns:
-            cell: exact copy of the current cell
+            cell: Exact copy of the current cell.
+                The name will have `$1` as duplicate names are not allowed
         """
         kdb_copy = self._kdb_copy()
 
         c = KCell(klib=self.klib, kdb_cell=kdb_copy)
         c.ports = self.ports.copy()
         for inst in kdb_copy.each_inst():
-            c.insts.append(Instance(cell=self.klib[inst.cell.name], reference=inst))  # type: ignore[misc]
+            c.insts.append(Instance(self.klib, instance=inst))
         c._locked = False
         return c
 
     def __copy__(self) -> "KCell":
+        """Enables use of :py:func:`copy.copy` and :py:func:`copy.deep_copy`."""
         return self.dup()
 
-    def add_port(self, port: PortLike[TT, FI], name: Optional[str] = None) -> None:
-        """Add an existing port. E.g. from an instance to propagate the port
+    def add_port(self, port: Port, name: str | None = None) -> None:
+        """Add an existing port. E.g. from an instance to propagate the port.
 
         Args:
-            port: The port to add. Port should either be a :py:class:`~Port`, or will be converted to an integer based port with 90° increment
+            port: The port to add. Port should either be a :py:class:`~Port`,
+                or will be converted to an integer based port with 90° increment
             name: Overwrite the name of the port
         """
+        self.ports.add_port(port=port, name=name)
 
-        if isinstance(port, Port):
-            self.ports.add_port(port=port, name=name)
-        else:
-            logger.warning(
-                f"Port {str(port)} is not an integer based port, converting to integer based",
-            )
+    def add_ports(self, ports: Iterable[Port], prefix: str = "") -> None:
+        """Add a sequence of ports to the cells.
 
-            strans = port.trans.s_trans() if port.complex() else port.trans.dup()  # type: ignore[union-attr]
-            trans = strans if port.int_based() else strans.to_itype(self.klib.dbu)  # type: ignore[union-attr]
-            _port = Port(
-                name=port.name,
-                width=port.width  # type: ignore[arg-type]
-                if port.int_based()
-                else int(port.width / self.klib.dbu),
-                trans=trans,  # type: ignore[arg-type]
-                port_type=port.port_type,
-                layer=port.layer,
-            )
-            self.ports.add_port(port=_port, name=name)
+        Can be useful to add all ports of a instance for example.
 
-    def add_ports(self, ports: Sequence[PortLike[TT, FI]], prefix: str = "") -> None:
-        for port in ports:
-            self.add_port(port, name=prefix + port.name)
+        Args:
+            ports: list/tuple (anything iterable) of ports.
+            prefix: string to add in front of all the port names
+        """
+        self.ports.add_ports(ports=ports, prefix=prefix)
 
     @classmethod
     def from_yaml(
         cls: "Callable[..., KCell]",
         constructor: Any,
         node: Any,
         verbose: bool = False,
     ) -> "KCell":
-        """Internal function used by the placer to convert yaml to a KCell"""
+        """Internal function used by the placer to convert yaml to a KCell."""
         d = ruamel.yaml.constructor.SafeConstructor.construct_mapping(
             constructor,
             node,
             deep=True,
         )
         cell = cls(d["name"])
         if verbose:
             print(f"Building {d['name']}")
-        cell.ports = d.get("ports", Ports([]))
+        cell.ports = d.get("ports", Ports(ports=[], klib=cell.klib))
         cell.settings = d.get("settings", {})
         for inst in d.get("insts", []):
             if "cellname" in inst:
                 _cell = cell.klib[inst["cellname"]]
             elif "cellfunction" in inst:
                 module_name, fname = inst["cellfunction"].rsplit(".", 1)
                 module = importlib.import_module(module_name)
                 cellf = getattr(module, fname)
                 _cell = cellf(**inst["settings"])
                 del module
             else:
                 raise NotImplementedError(
-                    'To define an instance, either a "cellfunction" or a "cellname" needs to be defined'
+                    'To define an instance, either a "cellfunction" or'
+                    ' a "cellname" needs to be defined'
                 )
             t = inst.get("trans", {})
             if isinstance(t, str):
                 cell.create_inst(
-                    _cell,  # type: ignore[arg-type]
+                    _cell,
                     kdb.Trans.from_s(inst["trans"]),
                 )
             else:
                 angle = t.get("angle", 0)
                 mirror = t.get("mirror", False)
 
                 kinst = cell.create_inst(
-                    _cell,  # type: ignore[arg-type]
+                    _cell,
                     kdb.Trans(angle, mirror, 0, 0),
                 )
 
                 x0_yml = t.get("x0", DEFAULT_TRANS["x0"])
                 y0_yml = t.get("y0", DEFAULT_TRANS["y0"])
                 x_yml = t.get("x", DEFAULT_TRANS["x"])
                 y_yml = t.get("y", DEFAULT_TRANS["y"])
                 margin = t.get("margin", DEFAULT_TRANS["margin"])
-                margin_x = margin.get("x", DEFAULT_TRANS["margin"]["x"])  # type: ignore[index]
-                margin_y = margin.get("y", DEFAULT_TRANS["margin"]["y"])  # type: ignore[index]
-                margin_x0 = margin.get("x0", DEFAULT_TRANS["margin"]["x0"])  # type: ignore[index]
-                margin_y0 = margin.get("y0", DEFAULT_TRANS["margin"]["y0"])  # type: ignore[index]
+                margin_x = margin.get(
+                    "x", DEFAULT_TRANS["margin"]["x"]  # type: ignore[index]
+                )
+                margin_y = margin.get(
+                    "y", DEFAULT_TRANS["margin"]["y"]  # type: ignore[index]
+                )
+                margin_x0 = margin.get(
+                    "x0", DEFAULT_TRANS["margin"]["x0"]  # type: ignore[index]
+                )
+                margin_y0 = margin.get(
+                    "y0", DEFAULT_TRANS["margin"]["y0"]  # type: ignore[index]
+                )
                 ref_yml = t.get("ref", DEFAULT_TRANS["ref"])
                 if isinstance(ref_yml, str):
                     for i in reversed(cell.insts):
                         if i.cell.name == ref_yml:
                             ref = i
                             break
                     else:
                         IndexError(f"No instance with cell name: <{ref_yml}> found")
                 elif isinstance(ref_yml, int) and len(cell.insts) > 1:
                     ref = cell.insts[ref_yml]
 
-                # margins for x0/y0 need to be in with opposite sign of x/y due to them being subtracted later
+                # margins for x0/y0 need to be in with opposite sign of
+                # x/y due to them being subtracted later
+
                 # x0
                 match x0_yml:
                     case "W":
                         x0 = kinst.bbox().left - margin_x0
                     case "E":
                         x0 = kinst.bbox().right + margin_x0
                     case _:
@@ -1650,791 +1148,1016 @@
                 cell.shapes(cell.layout().layer(linfo)).insert(
                     type_to_class[shapetype](shapestring)
                 )
 
         return cell
 
     def show(self) -> None:
+        """Stream the gds to klive.
+
+        Will create a temporary file of the gds and load it in KLayout via klive
+        """
         show(self)
 
     def _ipython_display_(self) -> None:
-        """Display a cell in a Jupyter Cell when it is passed as a last argument alone"""
+        """Display a cell in a Jupyter Cell.
+
+        Usage: Pass the kcell variable as an argument in the cell at the end
+        """
         from .widgets.interactive import display_kcell
 
         display_kcell(self)
 
+    @property
+    def ports(self) -> "Ports":
+        """Ports associated with the cell."""
+        return self._ports
 
-class CplxKCell(ABCKCell[DCplxPort]):
-    """Derived from :py:class:`klayout.db.Cell`. Additionally to a standard cell, this one will keep track of :py:class:`Port` and allow to store metadata in a dictionary
+    @ports.setter
+    def ports(self, new_ports: "InstancePorts | Ports") -> None:
+        self._ports = new_ports.copy()
 
-    Attributes:
-        ports (:py:class:`Ports`):  Contains all the ports of the cell and makes them accessible
-        insts (:py:class:`list`[:py:class:`Instance`]): All instances intantiated in this KCell
-        settings (:py:class:`dict`): Dictionary containing additional metadata of the KCell. Can be autopopulated by :py:func:`autocell`
-        _kdb_cell (:py:class:`klayout.db.Cell`): Internal reference to the :py:class:`klayout.db.Cell` object. Not intended for direct access
-    """
+    @overload
+    def create_port(
+        self,
+        *,
+        name: str,
+        trans: kdb.Trans,
+        width: int,
+        layer: LayerEnum | int,
+        port_type: str = "optical",
+    ) -> None:
+        ...
 
-    yaml_tag = "!CplxKCell"
+    @overload
+    def create_port(
+        self,
+        *,
+        name: str,
+        dcplx_trans: kdb.DCplxTrans,
+        dwidth: float,
+        layer: LayerEnum | int,
+        port_type: str = "optical",
+    ) -> None:
+        ...
 
-    def __init__(
+    @overload
+    def create_port(
         self,
-        name: Optional[str] = None,
-        klib: KLib = klib,
-        kdb_cell: Optional[kdb.Cell] = None,
-        ports: "Optional[CplxPorts]" = None,
-    ):
-        super().__init__(name=name, klib=klib, kdb_cell=kdb_cell)
-        self.klib.register_cell(self, allow_reregister=True)
-        self.ports: CplxPorts = ports or CplxPorts()
-        self.complex = True
+        *,
+        name: str | None = None,
+        port: Port,
+    ) -> None:
+        ...
 
-        if kdb_cell is not None:
-            for inst in kdb_cell.each_inst():
-                self.insts.append(Instance(self.klib[kdb_cell.name], inst))  # type: ignore[misc]
+    @overload
+    def create_port(
+        self,
+        *,
+        name: str,
+        width: int,
+        position: tuple[int, int],
+        angle: int,
+        layer: LayerEnum | int,
+        port_type: str = "optical",
+        mirror_x: bool = False,
+    ) -> None:
+        ...
 
-    def add_port(self, port: PortLike[TT, FI], name: Optional[str] = None) -> None:
-        """Add an existing port. E.g. from an instance to propagate the port
+    def create_port(self, **kwargs: Any) -> None:
+        """Create a new port. Equivalent to :py:attr:`~add_port(Port(...))`."""
+        self.ports.create_port(**kwargs)
+
+    @overload
+    def create_inst(
+        self,
+        cell: "KCell | int",
+        trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector = kdb.Trans(),
+    ) -> "Instance":
+        ...
+
+    @overload
+    def create_inst(
+        self,
+        cell: "KCell | int",
+        *,
+        dtrans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector,
+    ) -> "Instance":
+        ...
+
+    @overload
+    def create_inst(
+        self,
+        cell: "KCell | int",
+        trans: kdb.Trans | kdb.ICplxTrans | kdb.Vector,
+        *,
+        a: kdb.Vector,
+        b: kdb.Vector,
+        na: int = 1,
+        nb: int = 1,
+    ) -> "Instance":
+        ...
+
+    @overload
+    def create_inst(
+        self,
+        cell: "KCell | int",
+        *,
+        dtrans: kdb.DTrans | kdb.DCplxTrans,
+        a: kdb.DVector,
+        b: kdb.DVector,
+        na: int = 1,
+        nb: int = 1,
+    ) -> "Instance":
+        ...
+
+    def create_inst(
+        self,
+        cell: "KCell | int",
+        trans: kdb.Trans | kdb.Vector | kdb.ICplxTrans = kdb.Trans(),
+        dtrans: kdb.DTrans | kdb.DCplxTrans | kdb.DVector | None = None,
+        a: kdb.Vector | kdb.DVector | None = None,
+        b: kdb.Vector | kdb.DVector | None = None,
+        na: int = 1,
+        nb: int = 1,
+    ) -> "Instance":
+        """Add an instance of another KCell.
 
         Args:
-            port: The port to add. Port should either be a :py:class:`~Port`, or will be converted to an integer based port with 90° increment
-            name: Overwrite the name of the port
+            cell: The cell to be added
+            trans: The integer transformation applied to the reference
+            dtrans: um transformation of the reference. If not `None`,
+                will overwrite :py:attr:`trans`
+            a: Vector (DVector if trans is um based) for the array.
+                Needs to be in positive X-direction
+            b: Vector (DVector if trans is um based) for the array.
+                Needs to be in positive Y-direction
+            na: Number of elements in direction of :py:attr:`a`
+            nb: Number of elements in direction of :py:attr:`b`
+
+        Returns:
+            :py:class:`~Instance`: The created instance
         """
+        if isinstance(cell, int):
+            ci = cell
+        else:
+            ci = cell.cell_index()
 
-        if isinstance(port, DCplxPort):
-            self.ports.add_port(port=port, name=name)
+        if dtrans is None:
+            if a is None:
+                ca = self._kdb_cell.insert(kdb.CellInstArray(ci, trans))
+            else:
+                if b is None:
+                    b = kdb.Vector()
+                cast(kdb.DVector, a)
+                cast(kdb.DVector, b)
+                ca = self._kdb_cell.insert(
+                    kdb.CellInstArray(ci, trans, a, b, na, nb)  # type: ignore[arg-type]
+                )
         else:
-            self.ports.add_port(
-                port=port.copy_cplx(kdb.DCplxTrans.R0, self.klib.dbu), name=name
-            )
+            if a is None:
+                ca = self._kdb_cell.insert(kdb.DCellInstArray(ci, dtrans))
+            else:
+                if b is None:
+                    b = kdb.DVector()
+                cast(kdb.DVector, a)
+                cast(kdb.DVector, b)
+                ca = self._kdb_cell.insert(
+                    kdb.DCellInstArray(
+                        ci, dtrans, a, b, na, nb  # type: ignore[arg-type]
+                    )
+                )
+        inst = Instance(self.klib, ca)
+        self.insts.append(inst)
+        return inst
 
-    def dup(self) -> "CplxKCell":
-        """Copy the full cell
+    def _kdb_copy(self) -> kdb.Cell:
+        return self._kdb_cell.dup()
 
-        Returns:
-            cell: exact copy of the current cell
+    def layer(self, *args: Any, **kwargs: Any) -> int:
+        """Get the layer info, convenience for klayout.db.Layout.layer."""
+        return self.klib.layer(*args, **kwargs)
+
+    def __lshift__(self, cell: "KCell") -> "Instance":
+        """Convenience function for :py:attr:"~create_inst(cell)`.
+
+        Args:
+            cell: The cell to be added as an instance
         """
-        kdb_copy = self._kdb_copy()
+        return self.create_inst(cell)
 
-        c = CplxKCell(klib=self.klib, kdb_cell=kdb_copy)
-        c.ports = self.ports.copy()
-        for inst in kdb_copy.each_inst():
-            c.insts.append(Instance(cell=self.klib[inst.cell.name], reference=inst))  # type: ignore[misc]
-        c._locked = False
-        return c
+    def hash(self) -> bytes:
+        """Provide a unique hash of the cell."""
+        h = sha3_512()
+        h.update(self.name.encode("ascii", "ignore"))
 
-    def __copy__(self) -> "CplxKCell":
-        return self.dup()
+        for layer_index in self.layout().layer_indexes():
+            h.update(layer_index.to_bytes(8, "big"))
+            for shape in self.shapes(layer_index).each(kdb.Shapes.SRegions):
+                h.update(shape.polygon.hash().to_bytes(8, "big"))
+            for shape in self.shapes(layer_index).each(kdb.Shapes.STexts):
+                h.update(shape.text.hash().to_bytes(8, "big"))
+        port_hashs = list(sorted(p.hash() for p in self.ports._ports))
+        for _hash in port_hashs:
+            h.update(_hash)
+        insts_hashs = list(sorted(inst.hash for inst in self.insts))
+        for _hash in insts_hashs:
+            h.update(_hash)
+        return h.digest()
 
-    def show(self) -> None:
-        show(self)
+    def autorename_ports(self, rename_func: Callable[..., None] | None = None) -> None:
+        """Rename the ports with the schema angle -> "NSWE" and sort by x and y.
 
-    @classmethod
-    def from_yaml(
-        cls: "Callable[..., CplxKCell]",
-        constructor: Any,
-        node: Any,
-        verbose: bool = False,
-    ) -> "CplxKCell":
-        """Internal function used by the placer to convert yaml to a KCell"""
-        d = ruamel.yaml.constructor.SafeConstructor.construct_mapping(
-            constructor,
-            node,
-            deep=True,
-        )
+        Args:
+            rename_func: Function that takes Iterable[Port] and renames them.
+            This can of course contain a filter and only rename some of the ports
+        """
+        if rename_func is None:
+            self.klib.rename_function(self.ports._ports)
+        else:
+            rename_func(self.ports._ports)
 
-        logger.warning(
-            "Conversion of YAML to Complex KCells is currently experimental and likely to cause errors or faulty cells"
-        )
-        cell = cls(d["name"])
-        if verbose:
-            print(f"Building {d['name']}")
-        cell.ports = d.get("ports", Ports([]))
-        cell.settings = d.get("settings", {})
-        for inst in d.get("insts", []):
-            if "cellname" in inst:
-                _cell = cell.klib[inst["cellname"]]
-            elif "cellfunction" in inst:
-                module_name, fname = inst["cellfunction"].rsplit(".", 1)
-                module = importlib.import_module(module_name)
-                cellf = getattr(module, fname)
-                _cell = cellf(**inst["settings"])
-                del module
+    def flatten(self, prune: bool = True, merge: bool = True) -> None:
+        """Flatten the cell.
+
+        Pruning will delete the klayout.db.Cell if unused,
+        but might cause artifacts at the moment.
+
+        Args:
+            prune: Delete unused child cells if they aren't used in any other KCell
+            merge: Merge the shapes on all layers
+        """
+        self._kdb_cell.flatten(False)  # prune)
+        self.insts = Instances()
+
+        if merge:
+            for layer in self.layout().layer_indexes():
+                reg = kdb.Region(self.begin_shapes_rec(layer))
+                reg.merge()
+                self.clear(layer)
+                self.shapes(layer).insert(reg)
+
+    def draw_ports(self) -> None:
+        """Draw all the ports on their respective :py:attr:`Port.layer`:."""
+        polys: dict[int, kdb.Region] = {}
+
+        for port in self.ports:
+            w = port.width
+
+            if w in polys:
+                poly = polys[w]
             else:
-                raise NotImplementedError(
-                    'To define an instance, either a "cellfunction" or a "cellname" needs to be defined'
+                poly = kdb.Region()
+                poly.insert(
+                    kdb.Polygon(
+                        [
+                            kdb.Point(0, -w // 2),
+                            kdb.Point(0, w // 2),
+                            kdb.Point(w // 2, 0),
+                        ]
+                    )
                 )
-            t = inst.get("trans", {})
-            if isinstance(t, str):
-                cell.create_inst(
-                    _cell,  # type: ignore[arg-type]
-                    kdb.Trans.from_s(inst["trans"]),
+                if w > 20:
+                    poly -= kdb.Region(
+                        kdb.Polygon(
+                            [
+                                kdb.Point(w // 20, 0),
+                                kdb.Point(w // 20, -w // 2 + int(w * 2.5 // 20)),
+                                kdb.Point(w // 2 - int(w * 1.41 / 20), 0),
+                            ]
+                        )
+                    )
+            polys[w] = poly
+            if port._trans:
+                self.shapes(port.layer).insert(poly.transformed(port.trans))
+                self.shapes(port.layer).insert(
+                    kdb.Text(port.name if port.name else "", port.trans)
                 )
             else:
-                angle = t.get("angle", 0)
-                mirror = t.get("mirror", False)
-
-                kinst = cell.create_inst(
-                    _cell,  # type: ignore[arg-type]
-                    kdb.Trans(angle, mirror, 0, 0),
+                self.shapes(port.layer).insert(poly, port.dcplx_trans)
+                self.shapes(port.layer).insert(
+                    kdb.Text(port.name if port.name else "", port.trans)
                 )
 
-                x0_yml = t.get("x0", DEFAULT_TRANS["x0"])
-                y0_yml = t.get("y0", DEFAULT_TRANS["y0"])
-                x_yml = t.get("x", DEFAULT_TRANS["x"])
-                y_yml = t.get("y", DEFAULT_TRANS["y"])
-                margin = t.get("margin", DEFAULT_TRANS["margin"])
-                margin_x = margin.get("x", DEFAULT_TRANS["margin"]["x"])  # type: ignore[index]
-                margin_y = margin.get("y", DEFAULT_TRANS["margin"]["y"])  # type: ignore[index]
-                margin_x0 = margin.get("x0", DEFAULT_TRANS["margin"]["x0"])  # type: ignore[index]
-                margin_y0 = margin.get("y0", DEFAULT_TRANS["margin"]["y0"])  # type: ignore[index]
-                ref_yml = t.get("ref", DEFAULT_TRANS["ref"])
-                if isinstance(ref_yml, str):
-                    for i in reversed(cell.insts):
-                        if i.cell.name == ref_yml:
-                            ref = i
-                            break
-                    else:
-                        IndexError(f"No instance with cell name: <{ref_yml}> found")
-                elif isinstance(ref_yml, int) and len(cell.insts) > 1:
-                    ref = cell.insts[ref_yml]
+    def write(
+        self, filename: str | Path, save_options: kdb.SaveLayoutOptions = default_save()
+    ) -> None:
+        """Write a KCell to a GDS. See :py:func:`KLib.write` for more info."""
+        return self._kdb_cell.write(str(filename), save_options)
 
-                # margins for x0/y0 need to be in with opposite sign of x/y due to them being subtracted later
-                # x0
-                match x0_yml:
-                    case "W":
-                        x0 = kinst.bbox().left - margin_x0
-                    case "E":
-                        x0 = kinst.bbox().right + margin_x0
-                    case _:
-                        if isinstance(x0_yml, int):
-                            x0 = x0_yml
-                        else:
-                            NotImplementedError("unknown format for x0")
-                # y0
-                match y0_yml:
-                    case "S":
-                        y0 = kinst.bbox().bottom - margin_y0
-                    case "N":
-                        y0 = kinst.bbox().top + margin_y0
-                    case _:
-                        if isinstance(y0_yml, int):
-                            y0 = y0_yml
-                        else:
-                            NotImplementedError("unknown format for y0")
-                # x
-                match x_yml:
-                    case "W":
-                        if len(cell.insts) > 1:
-                            x = ref.bbox().left
-                            if x_yml != x0_yml:
-                                x -= margin_x
-                        else:
-                            x = margin_x
-                    case "E":
-                        if len(cell.insts) > 1:
-                            x = ref.bbox().right
-                            if x_yml != x0_yml:
-                                x += margin_x
-                        else:
-                            x = margin_x
-                    case _:
-                        if isinstance(x_yml, int):
-                            x = x_yml
-                        else:
-                            NotImplementedError("unknown format for x")
-                # y
-                match y_yml:
-                    case "S":
-                        if len(cell.insts) > 1:
-                            y = ref.bbox().bottom
-                            if y_yml != y0_yml:
-                                y -= margin_y
-                        else:
-                            y = margin_y
-                    case "N":
-                        if len(cell.insts) > 1:
-                            y = ref.bbox().top
-                            if y_yml != y0_yml:
-                                y += margin_y
-                        else:
-                            y = margin_y
-                    case _:
-                        if isinstance(y_yml, int):
-                            y = y_yml
-                        else:
-                            NotImplementedError("unknown format for y")
-                kinst.transform(kdb.Trans(0, False, x - x0, y - y0))
-        type_to_class: dict[
-            str,
-            Callable[
-                [str],
-                kdb.Box
-                | kdb.DBox
-                | kdb.Polygon
-                | kdb.DPolygon
-                | kdb.Edge
-                | kdb.DEdge
-                | kdb.Text
-                | kdb.DText,
-            ],
-        ] = {
-            "box": kdb.Box.from_s,
-            "polygon": kdb.Polygon.from_s,
-            "edge": kdb.Edge.from_s,
-            "text": kdb.Text.from_s,
-            "dbox": kdb.DBox.from_s,
-            "dpolygon": kdb.DPolygon.from_s,
-            "dedge": kdb.DEdge.from_s,
-            "dtext": kdb.DText.from_s,
+    @classmethod
+    def to_yaml(cls, representer, node):  # type: ignore
+        """Internal function to convert the cell to yaml."""
+        d = {
+            "name": node.name,
+            "ports": node.ports,  # Ports.to_yaml(representer, node.ports),
         }
 
-        for layer, shapes in dict(d.get("shapes", {})).items():
-            linfo = kdb.LayerInfo.from_string(layer)
-            for shape in shapes:
-                shapetype, shapestring = shape.split(" ", 1)
-                cell.shapes(cell.layout().layer(linfo)).insert(
-                    type_to_class[shapetype](shapestring)
-                )
+        insts = [
+            {"cellname": inst.cell.name, "trans": inst.instance.trans.to_s()}
+            for inst in node.insts
+        ]
+        shapes = {
+            node.layout()
+            .get_info(layer)
+            .to_s(): [shape.to_s() for shape in node.shapes(layer).each()]
+            for layer in node.layout().layer_indexes()
+            if not node.shapes(layer).is_empty()
+        }
 
-        return cell
+        if insts:
+            d["insts"] = insts
+        if shapes:
+            d["shapes"] = shapes
+        if len(node.settings) > 0:
+            d["settings"] = node.settings
+        return representer.represent_mapping(cls.yaml_tag, d)
+
+    def each_inst(self) -> Iterator["Instance"]:
+        """Iterates over all child instances (which may actually be instance arrays)."""
+        yield from (Instance(self.klib, inst) for inst in self._kdb_cell.each_inst())
+
+    def each_overlapping_inst(self, b: kdb.Box | kdb.DBox) -> Iterator["Instance"]:
+        """Gets the instances overlapping the given rectangle."""
+        yield from (
+            Instance(self.klib, inst)
+            for inst in self._kdb_cell.each_overlapping_inst(b)
+        )
+
+    def each_touching_inst(self, b: kdb.Box | kdb.DBox) -> Iterator["Instance"]:
+        """Gets the instances overlapping the given rectangle."""
+        yield from (
+            Instance(self.klib, inst) for inst in self._kdb_cell.each_touching_inst(b)
+        )
+
+    @overload
+    def insert(
+        self, inst: "Instance | kdb.CellInstArray | kdb.DCellInstArray"
+    ) -> "Instance":
+        ...
+
+    @overload
+    def insert(
+        self, inst: "kdb.CellInstArray | kdb.DCellInstArray", property_id: int
+    ) -> "Instance":
+        ...
+
+    def insert(
+        self,
+        inst: "Instance | kdb.CellInstArray | kdb.DCellInstArray",
+        property_id: int | None = None,
+    ) -> "Instance":
+        """Inserts a cell instance given by another reference."""
+        if isinstance(inst, Instance):
+            return Instance(self.klib, self._kdb_cell.insert(inst._instance))
+        else:
+            if not property_id:
+                return Instance(self.klib, self._kdb_cell.insert(inst))
+            else:
+                assert isinstance(inst, kdb.CellInstArray | kdb.DCellInstArray)
+                return Instance(self.klib, self._kdb_cell.insert(inst, property_id))
 
 
 class Instance:
-    """An Instance of a KCell. An Instance is a reference to a KCell with a transformation
+    """An Instance of a KCell.
+
+    An Instance is a reference to a KCell with a transformation.
 
     Attributes:
-        cell: The KCell that is referenced
-        instance: The internal klayout.db.Instance reference
-        ports: Transformed ports of the KCell"""
+        _instance: The internal :py:class:~`kdb.Instance` reference
+        ports: Transformed ports of the KCell
+    """
 
     yaml_tag = "!Instance"
 
-    def __init__(self, cell: ABCKCell[PT], reference: kdb.Instance) -> None:
-        self.cell = cell
-        self.instance = reference
+    def __init__(self, klib: KLib, instance: kdb.Instance) -> None:
+        """Create an instance from a KLayout Instance."""
+        self._instance = instance
+        self.klib = klib
         self.ports = InstancePorts(self)
 
+    def __getattr__(self, name):  # type: ignore[no-untyped-def]
+        """If we don't have an attribute, get it from the instance."""
+        return getattr(self._instance, name)
+
+    @property
+    def name(self) -> str | None:
+        """Name of instance in GDS."""
+        prop = self.property(PROPID.NAME)
+        return str(prop) if prop is not None else None
+
+    @name.setter
+    def name(self, value: str) -> None:
+        self.set_property(PROPID.NAME, value)
+
+    @property
+    def cell_index(self) -> int:
+        """Get the index of the cell this instance refers to."""
+        return self._instance.cell_index
+
+    @cell_index.setter
+    def cell_index(self, value: int) -> None:
+        self._instance_.cell_index = value
+
+    @property
+    def cell(self) -> KCell:
+        """Parent KCell  of the Instance."""
+        return self.klib[self.cell_index]
+
+    @cell.setter
+    def cell(self, value: KCell) -> None:
+        self.cell_index = value.cell_index()
+
+    @property
+    def a(self) -> kdb.Vector:
+        """Returns the displacement vector for the 'a' axis."""
+        return self._instance.a
+
+    @a.setter
+    def a(self, vec: kdb.Vector | kdb.DVector) -> None:
+        self._instance.a = vec  # type: ignore[assignment]
+
+    @property
+    def b(self) -> kdb.Vector:
+        """Returns the displacement vector for the 'b' axis."""
+        return self._instance.b
+
+    @b.setter
+    def b(self, vec: kdb.Vector | kdb.DVector) -> None:
+        self._instance.b = vec  # type: ignore[assignment]
+
+    @property
+    def cell_inst(self) -> kdb.CellInstArray:
+        """Gets the basic CellInstArray object associated with this instance."""
+        return self._instance.cell_inst
+
+    @cell_inst.setter
+    def cell_inst(self, cell_inst: kdb.CellInstArray | kdb.DCellInstArray) -> None:
+        self._instance.cell_inst = cell_inst  # type: ignore[assignment]
+
+    @property
+    def cplx_trans(self) -> kdb.ICplxTrans:
+        """Gets the complex transformation of the instance.
+
+        Or the first instance in the array.
+        """
+        return self._instance.cplx_trans
+
+    @cplx_trans.setter
+    def cplx_trans(self, trans: kdb.ICplxTrans | kdb.DCplxTrans) -> None:
+        self._instance.cplx_trans = trans  # type: ignore[assignment]
+
+    @property
+    def dcplx_trans(self) -> kdb.DCplxTrans:
+        """Gets the complex transformation of the instance.
+
+        Or the first instance in the array.
+        """
+        return self._instance.dcplx_trans
+
+    @dcplx_trans.setter
+    def dcplx_trans(self, trans: kdb.DCplxTrans) -> None:
+        self._instance.dcplx_trans = trans
+
+    @property
+    def dtrans(self) -> kdb.DTrans:
+        """Gets the complex transformation of the instance.
+
+        Or the first instance in the array.
+        """
+        return self._instance.dtrans
+
+    @dtrans.setter
+    def dtrans(self, trans: kdb.DTrans) -> None:
+        self._instance.dtrans = trans
+
+    @property
+    def trans(self) -> kdb.Trans:
+        """Gets the complex transformation of the instance.
+
+        Or the first instance in the array.
+        """
+        return self._instance.trans
+
+    @trans.setter
+    def trans(self, trans: kdb.Trans | kdb.DTrans) -> None:
+        self._instance.trans = trans  # type: ignore[assignment]
+
+    @property
+    def na(self) -> int:
+        """Returns the displacement vector for the 'a' axis."""
+        return self._instance.na
+
+    @na.setter
+    def na(self, value: int) -> None:
+        self._instance.na = value
+
+    @property
+    def nb(self) -> int:
+        """Returns the number of instances in the 'b' axis."""
+        return self._instance.nb
+
+    @nb.setter
+    def nb(self, value: int) -> None:
+        self._instance.nb = value
+
+    @property
+    def parent_cell(self) -> KCell:
+        """Gets the cell this instance is contained in."""
+        return self.klib[self._instance.parent_cell.cell_index()]
+
+    @parent_cell.setter
+    def parent_cell(self, cell: KCell | kdb.Cell) -> None:
+        if isinstance(cell, KCell):
+            self._instance.parent_cell = cell._kdb_cell
+        else:
+            self._instance.parent_cell = cell
+
+    @property
+    def prop_id(self) -> int:
+        """Gets the properties ID associated with the instance."""
+        return self._instance.prop_id
+
+    @prop_id.setter
+    def prop_id(self, value: int) -> None:
+        self._instance.prop_id = value
+
+    @property
     def hash(self) -> bytes:
+        """Hash the instance."""
         h = sha3_512()
         h.update(self.cell.hash())
-        h.update(self.instance.trans.hash().to_bytes(8, "big"))
+        if not self.is_complex():
+            h.update(self.trans.hash().to_bytes(8, "big"))
+        else:
+            h.update(self.dcplx_trans.hash().to_bytes(8, "big"))
         return h.digest()
 
     @overload
     def connect(
-        self, portname: str, other: Port | DCplxPort, *, mirror: bool = False
+        self, port: str | Port | None, other: Port, *, mirror: bool = False
     ) -> None:
         ...
 
     @overload
     def connect(
         self,
-        portname: str,
+        port: str | Port | None,
         other: "Instance",
-        other_port_name: str,
+        other_port_name: str | None,
         *,
         mirror: bool = False,
     ) -> None:
         ...
 
     def connect(
         self,
-        portname: str,
-        other: "Instance | Port | DCplxPort",
-        other_port_name: Optional[str] = None,
+        port: str | Port | None,
+        other: "Instance | Port",
+        other_port_name: str | None = None,
         *,
         mirror: bool = False,
         allow_width_mismatch: bool = False,
         allow_layer_mismatch: bool = False,
         allow_type_mismatch: bool = False,
     ) -> None:
-        """Function to allow to transform this instance so that a port of this instance is connected (same position with 180° turn) to another instance.
+        """Align port with name ``portname`` to a port.
+
+        .. deprecated:: 0.6.0
+            Use :py:func:`align` instead.
+            :py:func:`connect` will be removed in 0.7.0
+
+        Function to allow to transform this instance so that a port of this instance is
+        aligned (same position with 180° turn) to another instance.
+
+        Args:
+            port: The name of the port of this instance to be connected, or directly an
+                instance port. Can be `None` because port names can be `None`.
+            other: The other instance or a port. Skip `other_port_name` if it's a port.
+            other_port_name: The name of the other port. Ignored if
+                :py:attr:`~other_instance` is a port.
+            mirror: Instead of applying klayout.db.Trans.R180 as a connection
+                transformation, use klayout.db.Trans.M90, which effectively means this
+                instance will be mirrored and connected.
+            allow_width_mismatch: Skip width check between the ports if set.
+            allow_layer_mismatch: Skip layer check between the ports if set.
+            allow_type_mismatch: Skip port_type check between the ports if set.
+        """
+        logger.warning(
+            "Instance.connect will be removed in 0.7.0, please use Instance.align"
+        )
+        self.align(  # type: ignore[call-overload]
+            port=port,
+            other=other,
+            other_port_name=other_port_name,
+            mirror=mirror,
+            allow_width_mismatch=allow_layer_mismatch,
+            allow_layer_mismatch=allow_layer_mismatch,
+            allow_type_mismatch=allow_type_mismatch,
+        )
+
+    @overload
+    def align(
+        self, port: str | Port | None, other: Port, *, mirror: bool = False
+    ) -> None:
+        ...
+
+    @overload
+    def align(
+        self,
+        port: str | Port | None,
+        other: "Instance",
+        other_port_name: str | None,
+        *,
+        mirror: bool = False,
+    ) -> None:
+        ...
+
+    def align(
+        self,
+        port: str | Port | None,
+        other: "Instance | Port",
+        other_port_name: str | None = None,
+        *,
+        mirror: bool = False,
+        allow_width_mismatch: bool = False,
+        allow_layer_mismatch: bool = False,
+        allow_type_mismatch: bool = False,
+    ) -> None:
+        """Align port with name ``portname`` to a port.
+
+        Function to allow to transform this instance so that a port of this instance is
+        aligned (same position with 180° turn) to another instance.
 
         Args:
-            portname: The name of the port of this instance to be connected
-            other_instance: The other instance or a port
-            other_port_name: The name of the other port. Ignored if :py:attr:`~other_instance` is a port.
-            mirror: Instead of applying klayout.db.Trans.R180 as a connection transformation, use klayout.db.Trans.M90, which effectively means this instance will be mirrored and connected.
+            port: The name of the port of this instance to be connected, or directly an
+                instance port. Can be `None` because port names can be `None`.
+            other: The other instance or a port. Skip `other_port_name` if it's a port.
+            other_port_name: The name of the other port. Ignored if
+                :py:attr:`~other_instance` is a port.
+            mirror: Instead of applying klayout.db.Trans.R180 as a connection
+                transformation, use klayout.db.Trans.M90, which effectively means this
+                instance will be mirrored and connected.
+            allow_width_mismatch: Skip width check between the ports if set.
+            allow_layer_mismatch: Skip layer check between the ports if set.
+            allow_type_mismatch: Skip port_type check between the ports if set.
         """
         if isinstance(other, Instance):
             if other_port_name is None:
                 raise ValueError(
-                    "portname cannot be None if an Instance Object is given. For complex connections (non-90 degree and floating point ports) use connect_cplx instead"
+                    "portname cannot be None if an Instance Object is given. For"
+                    "complex connections (non-90 degree and floating point ports) use"
+                    "connect_cplx instead"
                 )
             op = other.ports[other_port_name]
         elif isinstance(other, Port):
             op = other
         else:
             raise ValueError("other_instance must be of type Instance or Port")
-        p = self.cell.ports[portname]
+        if isinstance(port, Port):
+            p = port
+        else:
+            p = self.cell.ports[port]
         if p.width != op.width and not allow_width_mismatch:
             raise PortWidthMismatch(
                 self,
                 other,
                 p,
                 op,
             )
         elif int(p.layer) != int(op.layer) and not allow_layer_mismatch:
             raise PortLayerMismatch(self.cell.klib, self, other, p, op)
         elif p.port_type != op.port_type and not allow_type_mismatch:
             raise PortTypeMismatch(self, other, p, op)
         else:
-            if not self.cell.complex:
-                if is_simple_port(op):
-                    conn_trans = kdb.Trans.M90 if mirror else kdb.Trans.R180
-                    self.instance.trans = op.trans * conn_trans * p.trans.inverted()  # type: ignore[operator]
-                else:
-                    if isinstance(op.trans, DPort):
-                        d_conn_trans = kdb.DTrans.M90 if mirror else kdb.DTrans.R180
-                        d_p_trans = p.trans.to_dtype(self.cell.klib.dbu).inverted()
-                        self.instance.dtrans = op.trans, *d_conn_trans * d_p_trans
-                    elif isinstance(op.trans, ICplxPort):
-                        icplx_conn_trans = (
-                            kdb.ICplxTrans.M90 if mirror else kdb.ICplxTrans.R180
-                        )
-                        i_p_trans = kdb.ICplxTrans(p.trans).inverted()
-                        self.instance.cplx_trans = (
-                            op.trans * icplx_conn_trans * i_p_trans
-                        )
-                    elif isinstance(op.trans, DCplxPort):
-                        d_cplx_conn_trans = (
-                            kdb.DCplxTrans.M90 if mirror else kdb.DCplxTrans.R180
-                        )
-                        d_p_trans = kdb.DCplxTrans(
-                            p.trans.to_dtype(self.cell.klib.dbu)
-                        ).inverted()
-                        self.instance.dcplx_trans = (
-                            op.trans * d_cplx_conn_trans * d_p_trans
-                        )
-            else:
-                cplx_conn_trans = kdb.DCplxTrans.M90 if mirror else kdb.DCplxTrans.R180
-
-                self.instance.dcplx_trans = (
-                    op.copy_cplx(kdb.DCplxTrans.R0, self.cell.klib.dbu).trans
-                    * cplx_conn_trans
-                    * p.copy_cplx(
-                        kdb.DCplxTrans.R0, self.cell.klib.dbu
-                    ).trans.inverted()
-                )
-
-    def connect_cplx(
-        self,
-        portname: str,
-        other: "Instance | PortLike[TT, FI]",
-        other_port_name: Optional[str] = None,
-        *,
-        mirror: bool = False,
-        allow_width_mismatch: bool = False,
-        allow_layer_mismatch: bool = False,
-        allow_type_mismatch: bool = False,
-    ) -> None:
-        if isinstance(other, Instance):
-            if other_port_name is None:
-                raise ValueError(
-                    "portname cannot be None if an Instance Object is given"
-                )
-            op = other.ports[other_port_name]
-        elif isinstance(other, (Port, DPort, ICplxPort, DCplxPort)):
-            op = other
-        else:
-            raise ValueError("other_instance must be of type Instance or Port")
-        p = self.cell.ports[portname]
-        if p.width != op.width and not allow_width_mismatch:
-            if p.int_based() == op.int_based():
-                raise PortWidthMismatch(
-                    self,
-                    other,
-                    p,
-                    op,
+            if p._dcplx_trans or op._dcplx_trans:
+                dconn_trans = kdb.DCplxTrans.M90 if mirror else kdb.DCplxTrans.R180
+                self.dcplx_trans = (
+                    op.dcplx_trans * dconn_trans * p.dcplx_trans.inverted()
                 )
-            w1 = p.width * self.cell.klib.dbu if p.int_based() else p.width
-            w2 = op.width * self.cell.klib.dbu if op.int_based() else op.width
-            if w1 != w2:
-                raise PortWidthMismatch(
-                    self,
-                    other,
-                    p,
-                    op,
-                )
-        if int(p.layer) != int(op.layer) and not allow_layer_mismatch:
-            raise PortLayerMismatch(self.cell.klib, self, other, p, op)
-        if p.port_type != op.port_type and not allow_type_mismatch:
-            raise PortTypeMismatch(self, other, p, op)
-        # reset the transformation
-        self.trans = kdb.Trans.R0
-        # apply the transformations piece by piece
-        self.transform(op.trans)
-        self.transform(kdb.Trans.M90 if mirror else kdb.Trans.R180)
-        self.transform(p.trans.inverted())
-
-    def __getattribute__(self, attr_name: str) -> Any:
-        return super().__getattribute__(attr_name)
-
-    def _get_attr(self, attr_name: str) -> Any:
-        return super().__getattribute__(attr_name)
-
-    def __getattr__(self, attr_name: str) -> Any:
-        return kdb.Instance.__getattribute__(self.instance, attr_name)
-
-    def __setattr__(self, attr_name: str, attr_value: Any) -> None:
-        if attr_name == "instance":
-            super().__setattr__(attr_name, attr_value)
-        try:
-            kdb.Instance.__setattr__(self._get_attr("instance"), attr_name, attr_value)
-        except AttributeError as a:
-            super().__setattr__(attr_name, attr_value)
+            else:
+                conn_trans = kdb.Trans.M90 if mirror else kdb.Trans.R180
+                self.trans = op.trans * conn_trans * p.trans.inverted()
 
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore[no-untyped-def]
-        d = {"cellname": node.cell.name, "trans": node.instance.trans}
+        """Convert the instance to a yaml representation."""
+        d = {
+            "cellname": node.cell.name,
+            "trans": node._trans,
+            "dcplx_trans": node._dcplx_trans,
+        }
         return representer.represent_mapping(cls.yaml_tag, d)
 
 
+class Instances:
+    """Holder for instances.
+
+    Allows retrieval by name or index
+    """
+
+    def __init__(self) -> None:
+        """Constructor."""
+        self._insts: list[Instance] = []
+
+    def append(self, inst: Instance) -> None:
+        """Append a new instance."""
+        self._insts.append(inst)
+
+    def __getitem__(self, key: str | int) -> Instance:
+        """Retrieve instance by index or by name."""
+        if isinstance(key, int):
+            return self._insts[key]
+
+        else:
+            return next(filter(lambda inst: inst.name == key, self._insts))
+
+    def __len__(self) -> int:
+        """Length of the instances."""
+        return self._insts.__len__()
+
+    def __iter__(self) -> Iterator[Instance]:
+        """Get instance iterator."""
+        return self._insts.__iter__()
+
+    def get_inst_names(self) -> dict[str | None, int]:
+        """Get count of names of named instances.
+
+        Not named instances will be added to the `None` key.
+        """
+        names: dict[str | None, int] = {}
+        for inst in self._insts:
+            if inst.name in names:
+                names[inst.name] += 1
+            else:
+                names[inst.name] = 1
+        return names
+
+
 class Ports:
-    """A list of ports. It is not a traditional dictionary. Elements can be retrieved as in a tradional dictionary. But to keep tabs on names etc, the ports are stored as a list
+    """A collection of ports.
+
+    It is not a traditional dictionary. Elements can be retrieved as in a tradional
+    dictionary. But to keep tabs on names etc, the ports are stored as a list
 
     Attributes:
-        _ports: Internal storage of the ports. Normally ports should be retrieved with :py:func:`__getitem__` or with :py:func:`~get_all`
+        _ports: Internal storage of the ports. Normally ports should be retrieved with
+            :py:func:`__getitem__` or with :py:func:`~get_all`
     """
 
     yaml_tag = "!Ports"
 
-    def __init__(self, ports: Iterable[Port] = []) -> None:
-        """Constructor"""
+    def __init__(self, klib: KLib, ports: Iterable[Port] = []) -> None:
+        """Constructor."""
         self._ports: list[Port] = list(ports)
-        self.complex = False
+        self.klib = klib
 
     def copy(self) -> "Ports":
-        """Get a copy of each port"""
-        return Ports(ports=[p.copy() for p in self._ports])
+        """Get a copy of each port."""
+        return Ports(ports=[p.copy() for p in self._ports], klib=self.klib)
 
     def contains(self, port: Port) -> bool:
-        """Check whether a port is already in the list"""
+        """Check whether a port is already in the list."""
         return port.hash() in [v.hash() for v in self._ports]
 
     def __iter__(self) -> Iterator[Port]:
+        """Iterator, that allows for loops etc to directly access the object."""
         yield from self._ports
 
-    def each(self) -> Iterator[Port]:
-        return self.__iter__()
-
-    def add_port(self, port: Port, name: Optional[str] = None) -> None:
-        """Add a port object
+    def add_port(self, port: Port, name: str | None = None) -> None:
+        """Add a port object.
 
         Args:
             port: The port to add
             name: Overwrite the name of the port
         """
         _port = port.copy()
         if name is not None:
             _port.name = name
-        if self.get_all().get(_port.name, None) is not None:
-            raise ValueError("Port hase already been added to this cell")
         self._ports.append(_port)
 
+    def add_ports(self, ports: Iterable[Port], prefix: str = "") -> None:
+        """Append a list of ports."""
+        for p in ports:
+            name = p.name or ""
+            self.add_port(port=p, name=prefix + name)
+
     @overload
     def create_port(
         self,
         *,
-        name: str,
         trans: kdb.Trans,
         width: int,
         layer: int,
+        name: str | None = None,
+        port_type: str = "optical",
+    ) -> Port:
+        ...
+
+    @overload
+    def create_port(
+        self,
+        *,
+        dcplx_trans: kdb.DCplxTrans,
+        dwidth: int,
+        layer: LayerEnum | int,
+        name: str | None = None,
         port_type: str = "optical",
     ) -> Port:
         ...
 
     @overload
     def create_port(
         self,
         *,
-        name: str,
         width: int,
-        layer: int,
+        layer: LayerEnum | int,
         position: tuple[int, int],
-        angle: int,
+        angle: Literal[0, 1, 2, 3],
+        name: str | None = None,
         port_type: str = "optical",
     ) -> Port:
         ...
 
     def create_port(
         self,
         *,
-        name: str,
-        width: int,
-        layer: int,
+        name: str | None = None,
+        width: int | None = None,
+        dwidth: float | None = None,
+        layer: LayerEnum | int,
         port_type: str = "optical",
-        trans: Optional[kdb.Trans] = None,
-        position: Optional[tuple[int, int]] = None,
-        angle: Optional[int] = None,
+        trans: kdb.Trans | None = None,
+        dcplx_trans: kdb.DCplxTrans | None = None,
+        position: tuple[int, int] | None = None,
+        angle: Literal[0, 1, 2, 3] | None = None,
         mirror_x: bool = False,
     ) -> Port:
-        """Create a new port in the list"""
+        """Create a new port in the list.
 
+        Args:
+            name: Optional name of port.
+            width: Width of the port in dbu. If `trans` is set (or the manual creation
+                with `position` and `angle`), this needs to be as well.
+            dwidth: Width of the port in um. If `dcplx_trans` is set, this needs to be
+                as well.
+            layer: Layer index of the port.
+            port_type: Type of the port (electrical, optical, etc.)
+            trans: Transformation object of the port. [dbu]
+            dcplx_trans: Complex transformation for the port.
+                Use if a non-90° port is necessary.
+            position: Tuple of the position. [dbu]
+            angle: Angle in 90° increments. Used for simple/dbu transformations.
+            mirror_x: Mirror the transformation of the port.
+        """
         if trans is not None:
+            assert width is not None
             port = Port(
-                name=name, trans=trans, width=width, layer=layer, port_type=port_type
+                name=name,
+                trans=trans,
+                width=width,
+                layer=layer,
+                port_type=port_type,
+                klib=self.klib,
+            )
+        elif dcplx_trans is not None:
+            assert dwidth is not None
+            port = Port(
+                name=name,
+                dwidth=dwidth,
+                dcplx_trans=dcplx_trans,
+                layer=layer,
+                port_type=port_type,
+                klib=self.klib,
             )
         elif angle is not None and position is not None:
+            assert width is not None
             port = Port(
                 name=name,
                 width=width,
                 layer=layer,
                 port_type=port_type,
                 angle=angle,
                 position=position,
                 mirror_x=mirror_x,
+                klib=self.klib,
             )
         else:
             raise ValueError(
-                f"You need to define trans {trans} or angle {angle} and position {position}"
+                f"You need to define width {width} and trans {trans} or angle {angle}"
+                f" and position {position} or dcplx_trans {dcplx_trans}"
+                f" and dwidth {dwidth}"
             )
 
         self._ports.append(port)
         return port
 
-    def get_all(self) -> dict[str, Port]:
-        """Get all ports in a dictionary with names as keys"""
-        return {v.name: v for v in self._ports}
+    def get_all_named(self) -> dict[str, Port]:
+        """Get all ports in a dictionary with names as keys."""
+        return {v.name: v for v in self._ports if v.name is not None}
 
-    def __getitem__(self, key: str) -> Port:
-        """Get a specific port by name"""
+    def __getitem__(self, key: str | None) -> Port:
+        """Get a specific port by name."""
         try:
             return next(filter(lambda port: port.name == key, self._ports))
         except StopIteration:
             raise ValueError(
                 f"{key} is not a port. Available ports: {[v.name for v in self._ports]}"
             )
 
     def hash(self) -> bytes:
-        """Get a hash of the port to compare"""
+        """Get a hash of the port to compare."""
         h = sha3_512()
-        for port in sorted(
-            sorted(self._ports, key=lambda port: port.name), key=lambda port: hash(port)
-        ):
-            h.update(port.name.encode("UTF-8"))
-            h.update(port.trans.hash().to_bytes(8, "big"))
-            if port.int_based():
-                h.update(port.width.to_bytes(8, "big"))
+        for port in sorted(self._ports, key=lambda port: hash(port)):
+            h.update(port.name.encode("UTF-8") if port.name else b"")
+            if port._trans:
+                h.update(port.trans.hash().to_bytes(8, "big"))
             else:
-                h.update(struct.pack("f", port.width))
+                h.update(port.dcplx_trans.hash().to_bytes(8, "big"))
+            h.update(port.width.to_bytes(8, "big"))
             h.update(port.port_type.encode("UTF-8"))
 
         return h.digest()
 
     def __repr__(self) -> str:
-        return repr({v.name: v for v in self._ports})
+        """Representation of the Ports as strings."""
+        return repr([repr(p) for p in self._ports])
 
     @classmethod
     def to_yaml(cls, representer, node):  # type: ignore[no-untyped-def]
+        """Convert the ports to a yaml representations."""
         return representer.represent_sequence(
             cls.yaml_tag,
             node._ports,
         )
 
     @classmethod
-    def from_yaml(cls: "Type[Ports]", constructor: Any, node: Any) -> "Ports":
+    def from_yaml(cls: "type[Ports]", constructor: Any, node: Any) -> "Ports":
+        """Load Ports from a yaml representation."""
         return cls(constructor.construct_sequence(node))
 
 
-class CplxPorts:
-    """A list of ports. It is not a traditional dictionary. Elements can be retrieved as in a tradional dictionary. But to keep tabs on names etc, the ports are stored as a list
-
-    Attributes:
-        _ports: Internal storage of the ports. Normally ports should be retrieved with :py:func:`__getitem__` or with :py:func:`~get_all`
-    """
-
-    yaml_tag = "!CplxPorts"
+class InstancePorts:
+    """Ports of an instance.
 
-    def __init__(self, ports: Iterable[DCplxPort] = []) -> None:
-        """Constructor"""
-        self._ports = list(ports)
-        self.complex = True
-
-    def copy(self) -> "CplxPorts":
-        """Get a copy of each port"""
-        return CplxPorts([p.copy() for p in self._ports])
+    These act as virtual ports as the positions needs to change if the
+    instance changes etc.
 
-    def contains(self, port: Port) -> bool:
-        """Check whether a port is already in the list"""
-        return port.hash() in [v.hash() for v in self._ports]
-
-    def __iter__(self) -> Iterator[DCplxPort]:
-        yield from self._ports
 
-    def each(self) -> Iterator[DCplxPort]:
-        return self.__iter__()
+    Attributes:
+        cell_ports: A pointer to the :py:class:~`Ports` of the cell
+        instance: A pointer to the :py:class:~`Instance` related to this.
+            This provides a way to dynamically calculate the ports.
+    """
 
-    def add_port(self, port: DCplxPort, name: Optional[str] = None) -> None:
-        """Add a port object
+    def __init__(self, instance: Instance) -> None:
+        """Creates the virtual ports object.
 
         Args:
-            port: The port to add
-            name: Overwrite the name of the port
+            instance: The related instance
         """
-        _port = port.copy()
-        if name is not None:
-            _port.name = name
-        if self.get_all().get(_port.name, None) is not None:
-            raise ValueError("Port hase already been added to this cell")
-        self._ports.append(_port)
-
-    @overload
-    def create_port(
-        self,
-        *,
-        name: str,
-        trans: kdb.DCplxTrans,
-        width: float,
-        layer: int,
-        port_type: str = "optical",
-    ) -> DCplxPort:
-        ...
-
-    @overload
-    def create_port(
-        self,
-        *,
-        name: str,
-        width: float,
-        layer: int,
-        position: tuple[float, float],
-        angle: float,
-        port_type: str = "optical",
-    ) -> DCplxPort:
-        ...
-
-    def create_port(
-        self,
-        *,
-        name: str,
-        width: float,
-        layer: int,
-        port_type: str = "optical",
-        trans: Optional[kdb.DCplxTrans] = None,
-        position: Optional[tuple[float, float]] = None,
-        angle: Optional[float] = None,
-        mirror_x: bool = False,
-    ) -> DCplxPort:
-        """Create a new port in the list"""
-
-        if trans is not None:
-            port = DCplxPort(
-                name=name, trans=trans, width=width, layer=layer, port_type=port_type
-            )
-        elif angle is not None and position is not None:
-            port = DCplxPort(
-                name=name,
-                width=width,
-                layer=layer,
-                port_type=port_type,
-                angle=angle,
-                position=position,
-                mirror_x=mirror_x,
-            )
-        else:
-            raise ValueError(
-                f"You need to define trans {trans} or angle {angle} and position {position}"
-            )
-
-        self._ports.append(port)
-        return port
-
-    def get_all(self) -> dict[str, DCplxPort]:
-        """Get all ports in a dictionary with names as keys"""
-        return {v.name: v for v in self._ports}
-
-    def __getitem__(self, key: str) -> DCplxPort:
-        """Get a specific port by name"""
-        try:
-            return next(filter(lambda port: port.name == key, self._ports))
-        except StopIteration:
-            raise ValueError(
-                f"{key} is not a port. Available ports: {[v.name for v in self._ports]}"
-            )
-
-    def hash(self) -> bytes:
-        """Get a hash of the port to compare"""
-        h = sha3_512()
-        for port in sorted(
-            sorted(self._ports, key=lambda port: port.name), key=lambda port: hash(port)
-        ):
-            h.update(port.name.encode("UTF-8"))
-            h.update(port.trans.hash().to_bytes(8, "big"))
-            h.update(struct.pack("f", port.width))
-            h.update(port.port_type.encode("UTF-8"))
-            h.update(port.port_type.encode("UTF-8"))
-
-        return h.digest()
-
-    def __repr__(self) -> str:
-        return repr({v.name: v for v in self._ports})
-
-    @classmethod
-    def to_yaml(cls, representer, node):  # type: ignore[no-untyped-def]
-        return representer.represent_sequence(
-            cls.yaml_tag,
-            node._ports,
-        )
-
-    @classmethod
-    def from_yaml(cls: "Type[CplxPorts]", constructor: Any, node: Any) -> "CplxPorts":
-        return cls(constructor.construct_sequence(node))
-
-
-class InstancePorts:
-    def __init__(self, instance: Instance) -> None:
         self.cell_ports = instance.cell.ports
         self.instance = instance
 
-    def __getitem__(self, key: str) -> Port | DCplxPort:
+    def __getitem__(self, key: str | None) -> Port:
+        """Get a port by name."""
         p = self.cell_ports[key]
-        return (
-            p.copy_cplx(
-                trans=self.instance.instance.dcplx_trans,
-                dbu=self.instance.cell.klib.dbu,
-            )
-            if (
-                self.instance.instance.is_complex()
-                or p.complex()
-                or not p.int_based()
-                or self.instance.cell.complex
-            )
-            else p.copy(trans=self.instance.trans)  # type: ignore[arg-type]
-        )
+        if self.instance.is_complex():
+            return p.copy(self.instance.dcplx_trans)
+        else:
+            return p.copy(self.instance.trans)
 
-    def __iter__(self) -> Iterator[Port | DCplxPort]:
-        return (self[port.name] for port in self.cell_ports)
+    def __iter__(self) -> Iterator[Port]:
+        """Create a copy of the ports to iterate through."""
+        if not self.instance.is_complex():
+            yield from (p.copy(self.instance.trans) for p in self.cell_ports)
+        else:
+            yield from (p.copy(self.instance.dcplx_trans) for p in self.cell_ports)
 
     def __repr__(self) -> str:
-        return repr({v: self.__getitem__(v) for v in self.cell_ports.get_all().keys()})
+        """String representation.
 
-    def get_all(self) -> dict[str, Port | DCplxPort]:
-        return {v: self.__getitem__(v) for v in self.cell_ports.get_all().keys()}
+        Creates a copy and uses the `__repr__` of
+        :py:class:~`Ports`.
+        """
+        return repr(self.copy())
 
-    def copy(self) -> Ports | CplxPorts:
-        if (
-            not self.instance.instance.is_complex()
-            and not self.instance.cell.ports.complex
-            and not self.instance.cell.complex
-        ):
+    def copy(self) -> Ports:
+        """Creates a copy in the form of :py:class:~`Ports`."""
+        if not self.instance.is_complex():
             return Ports(
-                [
-                    port.copy(trans=self.instance.trans)  # type: ignore[arg-type, misc]
-                    for port in self.cell_ports._ports
-                ]
+                klib=self.instance.klib,
+                ports=[p.copy(self.instance.trans) for p in self.cell_ports._ports],
             )
         else:
-            return CplxPorts(
-                [
-                    port.copy_cplx(
-                        trans=self.instance.cplx_dtrans, dbu=self.instance.cell.klib.dbu
-                    )
-                    for port in self.cell_ports._ports
-                ]
+            return Ports(
+                klib=self.instance.klib,
+                ports=[
+                    p.copy(self.instance.dcplx_trans) for p in self.cell_ports._ports
+                ],
             )
 
 
 @overload
 def autocell(_func: Callable[KCellParams, KCell], /) -> Callable[KCellParams, KCell]:
     ...
 
@@ -2446,31 +2169,39 @@
     set_name: bool = True,
 ) -> Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]:
     ...
 
 
 @logger.catch
 def autocell(
-    _func: Optional[Callable[KCellParams, KCell]] = None,
+    _func: Callable[KCellParams, KCell] | None = None,
     /,
     *,
     set_settings: bool = True,
     set_name: bool = True,
+    check_ports: bool = True,
+    check_instances: bool = True,
 ) -> (
     Callable[KCellParams, KCell]
     | Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]
 ):
-    """Decorator to cache and auto name the celll. This will use :py:func:`functools.cache` to cache the function call.
-    Additionally, if enabled this will set the name and from the args/kwargs of the function and also paste them into a settings dictionary of the :py:class:`~KCell`
+    """Decorator to cache and auto name the celll.
+
+    This will use :py:func:`functools.cache` to cache the function call.
+    Additionally, if enabled this will set the name and from the args/kwargs of the
+    function and also paste them into a settings dictionary of the :py:class:`~KCell`.
 
     Args:
         set_settings: Copy the args & kwargs into the settings dictionary
-        set_name: Auto create the name of the cell to the functionname plus a string created from the args/kwargs
-        maxsize: maximum size of cache, cell parameter sets will be evicted if the cell function is called with more different
-        parameter sets than there are spaces in the cache, in case there are cell calls with existing parameter set calls
+        set_name: Auto create the name of the cell to the functionname plus a
+            string created from the args/kwargs
+        check_ports: Check whether there are any non-90° ports in the cell and throw a
+            warning if there are
+        check_instances: Check for any complex instances. A complex instance is a an
+            instance that has a magnification != 1 or non-90° rotation.
     """
 
     def decorator_autocell(
         f: Callable[KCellParams, KCell]
     ) -> Callable[KCellParams, KCell]:
         sig = signature(f)
 
@@ -2526,69 +2257,73 @@
 
         return wrapper_autocell
 
     return decorator_autocell if _func is None else decorator_autocell(_func)
 
 
 def dict_to_frozen_set(d: dict[str, Any]) -> frozenset[tuple[str, Any]]:
+    """Convert a `dict` to a `frozenset`."""
     return frozenset(d.items())
 
 
 def frozenset_to_dict(fs: frozenset[tuple[str, Hashable]]) -> dict[str, Hashable]:
+    """Convert `frozenset` to `dict`."""
     return dict(fs)
 
 
 def cell(
-    _func: Optional[Callable[..., KCell]] = None,
+    _func: Callable[..., KCell] | None = None,
     *,
     set_settings: bool = True,
     maxsize: int = 512,
 ) -> (
     Callable[KCellParams, KCell]
     | Callable[[Callable[KCellParams, KCell]], Callable[KCellParams, KCell]]
 ):
-    """Convenience alias for :py:func:`~autocell` with `(set_name=False)`"""
+    """Convenience alias for :py:func:`~autocell` with `(set_name=False)`."""
     if _func is None:
         return autocell(set_settings=set_settings, set_name=False)
     else:
         return autocell(_func)
 
 
-def dict2name(prefix: Optional[str] = None, **kwargs: dict[str, Any]) -> str:
-    """returns name from a dict"""
+def dict2name(prefix: str | None = None, **kwargs: dict[str, Any]) -> str:
+    """Returns name from a dict."""
     label = [prefix] if prefix else []
     for key, value in kwargs.items():
         key = join_first_letters(key)
         label += [f"{key.upper()}{clean_value(value)}"]
     _label = "_".join(label)
     return clean_name(_label)
 
 
 def get_component_name(component_type: str, **kwargs: dict[str, Any]) -> str:
+    """Convert a component to a string."""
     name = component_type
 
     if kwargs:
         name += f"_{dict2name(None, **kwargs)}"
 
     return name
 
 
 def join_first_letters(name: str) -> str:
-    """join the first letter of a name separated with underscores (taper_length -> TL)"""
+    """Join the first letter of a name separated with underscores.
+
+    Example::
+
+        "TL" == join_first_letters("taper_length")
+    """
     return "".join([x[0] for x in name.split("_") if x])
 
 
 def clean_value(
     value: float | np.float64 | dict[Any, Any] | KCell | Callable[..., Any]
 ) -> str:
-    """returns more readable value (integer)
-    if number is < 1:
-        returns number units in nm (integer)
-    """
-
+    """Makes sure a value is representable in a limited character_space."""
     try:
         if isinstance(value, int):  # integer
             return str(value)
         elif type(value) in [float, np.float64]:  # float
             return f"{value:.4f}".replace(".", "p").rstrip("0").rstrip("p")
         elif isinstance(value, list):
             return "_".join(clean_value(v) for v in value)
@@ -2603,15 +2338,15 @@
         else:
             return clean_name(str(value))
     except TypeError:  # use the __str__ method
         return clean_name(str(value))
 
 
 def clean_name(name: str) -> str:
-    r"""Ensures that gds cells are composed of [a-zA-Z0-9_\-]::
+    r"""Ensures that gds cells are composed of [a-zA-Z0-9_\-].
 
     FIXME: only a few characters are currently replaced.
         This function has been updated only on case-by-case basis
     """
     replace_map = {
         "=": "",
         ",": "_",
@@ -2625,15 +2360,15 @@
         " ": "_",
     }
     for k, v in list(replace_map.items()):
         name = name.replace(k, v)
     return name
 
 
-DEFAULT_TRANS: dict[str, Union[str, int, float, dict[str, Union[str, int, float]]]] = {
+DEFAULT_TRANS: dict[str, str | int | float | dict[str, str | int | float]] = {
     "x": "E",
     "y": "S",
     "x0": "W",
     "y0": "S",
     "margin": {
         "x": 10000,
         "y": 10000,
@@ -2641,52 +2376,51 @@
         "y0": 0,
     },
     "ref": -2,
 }
 
 
 def update_default_trans(
-    new_trans: dict[str, Union[str, int, float, dict[str, Union[str, int, float]]]]
+    new_trans: dict[str, str | int | float | dict[str, str | int | float]]
 ) -> None:
+    """Allows to change the default transformation for reading a yaml file."""
     DEFAULT_TRANS.update(new_trans)
 
 
 def show(
-    gds: str | KCell | CplxKCell | Path,
+    gds: str | KCell | Path,
     keep_position: bool = True,
     save_options: kdb.SaveLayoutOptions = default_save(),
 ) -> None:
-    """Show GDS in klayout"""
-
+    """Show GDS in klayout."""
     delete = False
 
-    if isinstance(gds, (KCell, CplxKCell)):
+    if isinstance(gds, KCell):
         _mf = "stdin" if mf == "<stdin>" else mf
-        dirpath = Path(gettempdir())
         tf = Path(gettempdir()) / Path(_mf).with_suffix(".gds")
         tf.parent.mkdir(parents=True, exist_ok=True)
         gds.write(str(tf), save_options)
         gds_file = tf
         delete = True
-    elif isinstance(gds, (str, Path)):
+    elif isinstance(gds, str | Path):
         gds_file = Path(gds)
     else:
         raise NotImplementedError(f"unknown type {type(gds)} for streaming to KLayout")
 
     if not gds_file.is_file():
         raise ValueError(f"{gds_file} is not a File")
     data_dict = {
         "gds": str(gds_file),
         "keep_position": keep_position,
     }
     data = json.dumps(data_dict)
     try:
         conn = socket.create_connection(("127.0.0.1", 8082), timeout=0.5)
         data = data + "\n"
-        enc_data = data.encode()  # if hasattr(data, "encode") else data
+        enc_data = data.encode()
         conn.sendall(enc_data)
         conn.settimeout(5)
     except OSError:
         logger.warning("Could not connect to klive server")
     else:
         msg = ""
         try:
@@ -2707,12 +2441,9 @@
     "Port",
     "Ports",
     "autocell",
     "cell",
     "klib",
     "KLib",
     "default_save",
-    "ICplxPort",
-    "DCplxPort",
-    "DPort",
     "LayerEnum",
 ]
```

### Comparing `kfactory-0.5.8/src/kfactory/pcells/circular.py` & `kfactory-0.6.0/src/kfactory/pcells/circular.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,11 @@
-from typing import Optional
+"""Circular bends.
+
+A circular bend has a constant radius.
+"""
 
 import numpy as np
 
 from .. import kdb
 from ..kcell import KCell, LayerEnum, autocell
 from ..utils import Enclosure
 from ..utils.geo import extrude_path
@@ -11,29 +14,29 @@
 
 
 @autocell
 def bend_circular(
     width: float,
     radius: float,
     layer: int | LayerEnum,
-    enclosure: Optional[Enclosure] = None,
+    enclosure: Enclosure | None = None,
     theta: float = 90,
     theta_step: float = 1,
 ) -> KCell:
-    """Circular radius bend
+    """Circular radius bend [um].
 
     Args:
-        width: Width in database units
-        radius: Radius in database units
-        layer: Layer index of the target layer
-        enclosure: :py:class:`kfactory.utils.Enclosure` object to describe the claddings
-    Returns:
-        cell (KCell): Circular Bend KCell
+        width: Width of the core. [um]
+        radius: Radius of the backbone. [um]
+        layer: Layer index of the target layer.
+        enclosure: :py:class:`kfactory.utils.Enclosure` object to describe the
+            claddings.
+        theta: Angle amount of the bend.
+        theta_step: Angle amount per backbone point of the bend.
     """
-
     c = KCell()
     r = radius
     backbone = [
         kdb.DPoint(x, y)
         for x, y in [
             [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
             for _theta in np.linspace(
```

### Comparing `kfactory-0.5.8/src/kfactory/pcells/euler.py` & `kfactory-0.6.0/src/kfactory/pcells/euler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,31 +1,35 @@
-from typing import Optional
+"""Euler bends.
+
+Euler bends are bends with a constantly changing radius
+from zero to a maximum radius and back to 0 at the other
+end.
+"""
 
 import numpy as np
 from scipy.optimize import brentq  # type: ignore[import]
 from scipy.special import fresnel  # type: ignore[import]
 
 from .. import kdb
 from ..kcell import KCell, LayerEnum, autocell
 from ..utils import Enclosure
-from ..utils.geo import extrude_path, extrude_path_dynamic
+from ..utils.geo import extrude_path
 
 __all__ = [
     "euler_bend_points",
     "euler_sbend_points",
     "bend_euler",
     "bend_s_euler",
 ]
 
 
 def euler_bend_points(
     angle_amount: float = 90, radius: float = 100, resolution: float = 150
 ) -> list[kdb.DPoint]:
     """Base euler bend, no transformation, emerging from the origin."""
-
     if angle_amount < 0:
         raise ValueError(f"angle_amount should be positive. Got {angle_amount}")
     # End angle
     eth = angle_amount * np.pi / 180
 
     # If bend is trivial, return a trivial shape
     if eth == 0:
@@ -89,16 +93,15 @@
 
 def euler_endpoint(
     start_point: tuple[float, float] = (0.0, 0.0),
     radius: float = 10.0,
     input_angle: float = 0.0,
     angle_amount: float = 90.0,
 ) -> tuple[float, float]:
-    """Gives the end point of a simple Euler bend as a i3.Coord2"""
-
+    """Gives the end point of a simple Euler bend as a i3.Coord2."""
     th = abs(angle_amount) * np.pi / 180 / 2
     R = radius
     clockwise = angle_amount < 0
 
     (fsin, fcos) = fresnel(np.sqrt(2 * th / np.pi))
 
     a = 2 * np.sqrt(2 * np.pi * th) * (np.cos(th) * fcos + np.sin(th) * fsin)
@@ -111,15 +114,15 @@
 
     return X + start_point[0], Y + start_point[1]
 
 
 def euler_sbend_points(
     offset: float = 5.0, radius: float = 10.0e-6, resolution: float = 150
 ) -> list[kdb.DPoint]:
-    """An Euler s-bend with parallel input and output, separated by an offset"""
+    """An Euler s-bend with parallel input and output, separated by an offset."""
 
     # Function to find root of
     def froot(th: float) -> float:
         end_point = euler_endpoint((0.0, 0.0), radius, 0.0, th)
         return 2 * end_point[1] - abs(offset)
 
     # Get direction
@@ -157,18 +160,28 @@
 
 
 @autocell
 def bend_euler(
     width: float,
     radius: float,
     layer: int | LayerEnum,
-    enclosure: Optional[Enclosure] = None,
+    enclosure: Enclosure | None = None,
     theta: float = 90,
     resolution: float = 150,
 ) -> KCell:
+    """Create a euler bend.
+
+    Args:
+        width: Width of the core. [um]
+        radius: Radius off the backbone. [um]
+        layer: Layer index / LayerEnum of the core.
+        enclosure: Slab/exclude definition. [dbu]
+        theta: Angle of the bend.
+        resolution: Angle resolution for the backbone.
+    """
     c = KCell()
     dbu = c.layout().dbu
     backbone = euler_bend_points(theta, radius=radius, resolution=resolution)
 
     extrude_path(
         target=c,
         layer=layer,
@@ -210,18 +223,28 @@
 
 
 @autocell
 def bend_s_euler(
     offset: float,
     width: float,
     radius: float,
-    layer: int,
-    enclosure: Optional[Enclosure] = None,
+    layer: LayerEnum | int,
+    enclosure: Enclosure | None = None,
     resolution: float = 150,
 ) -> KCell:
+    """Create a euler s-bend.
+
+    Args:
+        offset: Offset between left/right. [um]
+        width: Width of the core. [um]
+        radius: Radius off the backbone. [um]
+        layer: Layer index / LayerEnum of the core.
+        enclosure: Slab/exclude definition. [dbu]
+        resolution: Angle resolution for the backbone.
+    """
     c = KCell()
     dbu = c.layout().dbu
     backbone = euler_sbend_points(
         offset=offset,
         radius=radius,
         resolution=resolution,
     )
```

### Comparing `kfactory-0.5.8/src/kfactory/placer.py` & `kfactory-0.6.0/src/kfactory/placer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,56 +1,61 @@
 import os
 import sys
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Optional, TypeVar, Union
+from typing import Any, TypeVar
 
 from ruamel.yaml import YAML
 from ruamel.yaml.constructor import SafeConstructor
 
 from .kcell import KCell, KLib, Port, Ports
 from .kcell import klib as stdlib
 from .utils import Enclosure
 
 __all__ = ["cells_to_yaml", "cells_from_yaml"]
 
 PathLike = TypeVar("PathLike", str, Path, None)
 
 
 def cells_to_yaml(
-    output: PathLike, cells: Union[list[KCell], KCell]
+    output: PathLike, cells: list[KCell] | KCell
 ) -> None:  # , library: KLib=library):
-    """Convert cell(s) to a yaml representations
+    """Convert cell(s) to a yaml representations.
 
     Args:
         output: A stream or string of a path where to dump the yaml. Can also be set to sys.stdout
         cells: A single :py:class:`~kfactory.kcell.KCell` or a list of them.
+
+
     Returns:
         yaml dump
     """
     yaml = YAML()
     yaml.register_class(KCell)
     yaml.register_class(Port)
     yaml.register_class(Ports)
     yaml.indent(sequence=4, offset=2)
     yaml.dump(cells, output)
 
 
 def get_yaml_obj() -> YAML:
+    """New global yaml object."""
     return YAML()
 
 
 def register_classes(
     yaml: YAML,
     library: KLib = stdlib,
-    additional_classes: Optional[list[object]] = None,
+    additional_classes: list[object] | None = None,
     verbose: bool = False,
 ) -> None:
+    """Register a new KCell class compatible with ruamel yaml."""
+
     class ModKCell(KCell):
-        def __init__(self, name: Optional[str] = None, library: KLib = library):
+        def __init__(self, name: str | None = None, library: KLib = library):
             KCell.__init__(self, name, library)
 
         @classmethod
         def from_yaml(cls, constructor, node):  # type: ignore[no-untyped-def]
             return super().from_yaml(constructor, node, verbose=verbose)
 
     yaml.register_class(ModKCell)
@@ -61,57 +66,72 @@
     if additional_classes is not None:
         for c in additional_classes:
             yaml.register_class(c)
 
 
 def cells_from_yaml(
     inp: Path,
-    library: KLib = stdlib,
-    additional_classes: Optional[list[object]] = None,
+    klib: KLib = stdlib,
+    additional_classes: list[object] | None = None,
     verbose: bool = False,
 ) -> None:
+    """Recreate cells from a yaml file.
+
+    Args:
+        inp: Input file path.
+        klib: KLib to load the cells into.
+        additional_classes: Additional yaml classes that should be registered.
+            This is used for example to enable loading additional yaml files etc.
+        verbose: Print more verbose errors etc.
+    """
     yaml = get_yaml_obj()
     yaml.register_class(
-        include_from_loader(inp.parent, library, additional_classes, verbose)
+        include_from_loader(inp.parent, klib, additional_classes, verbose)
     )
 
     register_classes(
         yaml,
-        library,
+        klib,
         additional_classes,
         verbose,
     )
     yaml.load(inp)
 
 
 def exploded_yaml(
     inp: os.PathLike[Any],
     library: KLib = stdlib,
-    additional_classes: Optional[list[object]] = None,
+    additional_classes: list[object] | None = None,
     verbose: bool = False,
 ) -> Any:
+    """Expanded yaml.
+
+    Expand cross-references. Same syntax as :py:func:~`cells_from_yaml`
+    """
     yaml = YAML(pure=True)
 
     class ModKCell(KCell):
-        def __init__(self, name: Optional[str] = None, library: KLib = library):
+        def __init__(self, name: str | None = None, library: KLib = library):
             KCell.__init__(self, name, library)
 
         @classmethod
         def from_yaml(cls, constructor, node):  # type: ignore[no-untyped-def]
             super().from_yaml(constructor, node, verbose=verbose)
 
     return yaml.dump(yaml.load(inp), sys.stdout)
 
 
 def include_from_loader(
     folder: Path,
     library: KLib,
-    additional_classes: Optional[list[object]],
+    additional_classes: list[object] | None,
     verbose: bool,
 ) -> Any:
+    """Expand ruamel to support the `!include` keyword."""
+
     @dataclass
     class Include:
         filename: str
         yaml_tag: str = "!include"
 
         @classmethod
         def from_yaml(cls, constructor, node):  # type: ignore[no-untyped-def]
```

### Comparing `kfactory-0.5.8/src/kfactory/routing/electrical.py` & `kfactory-0.6.0/src/kfactory/routing/electrical.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,44 @@
-from typing import Callable, Optional
+"""Utilities for automatically routing electrical connections."""
+
+from collections.abc import Callable
 
 from .. import kdb
-from ..kcell import DCplxPort, Instance, KCell, Port
+from ..kcell import Instance, KCell, Port
 from .manhattan import route_manhattan
 
 
 def connect_elec(
     c: KCell,
     start_port: Port,
     end_port: Port,
-    start_straight: Optional[int] = None,
-    end_straight: Optional[int] = None,
+    start_straight: int | None = None,
+    end_straight: int | None = None,
     route_path_function: Callable[..., list[kdb.Point]] = route_manhattan,
-    width: Optional[int] = None,
-    layer: Optional[int] = None,
+    width: int | None = None,
+    layer: int | None = None,
 ) -> None:
+    """Connect two ports with a wire.
+
+    A wire is a path object on a usually metal layer.
+
 
+    Args:
+        c: KCell to place the wire in.
+        start_port: Beginning
+        end_port: End
+        start_straight: Minimum length of straight at start port.
+        end_straight: Minimum length of straight at end port.
+        route_path_function: Function to calculate the path. Signature:
+            `route_path_function(start_port, end_port, bend90_radius, start_straight,
+            end_straight)`
+        width: Overwrite the width of the wire. Calculated by the width of the start
+            port if `None`.
+        layer: Layer to place the wire on. Calculated from the start port if `None`.
+    """
     if width is None:
         width = start_port.width
     if layer is None:
         layer = start_port.layer
     if start_straight is None:
         start_straight = int(width / 2)
     if end_straight is None:
@@ -40,34 +59,31 @@
 
 def connect_L_route(
     c: KCell,
     input_ports: list[Port],
     output_orientation: int = 1,
     wire_spacing: int = 10000,
 ) -> list[Port]:
-    """
+    """Route ports towards a bundle in an L shape.
+
     This function takes a list of input ports and assume they are oriented in the west.
     The output will be a list of ports that have the same y coordinates.
-    The function will produce a L-shape routing to connect input ports to output ports without any crossings.
+    The function will produce a L-shape routing to connect input ports to output ports
+    without any crossings.
     """
     input_ports.sort(key=lambda p: p.y)
 
     y_max = input_ports[-1].y
     y_min = input_ports[0].y
     x_max = max(p.x for p in input_ports)
-    # x_min = min([p.x for p in input_ports])
 
     output_ports = []
     if output_orientation == 1:
         for i, p in enumerate(input_ports[::-1]):
             temp_port = p.copy()
-            # temp_port.trans.disp = kf.kdb.Vector(
-            #     x_max - wire_spacing * (i + 1), y_max + wire_spacing
-            # )
-            # temp_port.trans.angle = 3
             temp_port.trans = kdb.Trans(
                 3, False, x_max - wire_spacing * (i + 1), y_max + wire_spacing
             )
 
             connect_elec(c, p, temp_port)
             temp_port.trans.angle = 1
             output_ports.append(temp_port)
@@ -89,18 +105,27 @@
 
 def connect_bundle(
     c: KCell,
     input_ports: list[Port],
     target_ports: list[Port],
     wire_spacing: int = 10000,
 ) -> None:
-    """
-    This function takes a list of input ports and assume they are all oriented in the same direction (could be any of W, S, E, N).
-    The target ports have the opposite orientation, i.e. if input ports are oriented to north, and target ports should be oriented to south.
-    The function will produce a routing to connect input ports to output ports without any crossings.
+    """Connect multiple input ports to output ports.
+
+    This function takes a list of input ports and assume they are all oriented in the
+    same direction (could be any of W, S, E, N). The target ports have the opposite
+    orientation, i.e. if input ports are oriented to north, and target ports should
+    be oriented to south. The function will produce a routing to connect input ports
+    to output ports without any crossings.
+
+    Args:
+        c: KCell to place the routes in.
+        input_ports; List of start ports.
+        target_ports: List of end ports.
+        wire_spacing: Minimum space between wires. [dbu]
     """
     input_ports.sort(key=lambda p: p.y)
 
     x_max = max(p.x for p in input_ports)
     x_min = min(p.x for p in input_ports)
 
     output_ports = []
@@ -173,78 +198,90 @@
                     start_straight=T_count * wire_spacing,
                     end_straight=abs(target_ports[i].y - output_ports[i].y)
                     - T_count * wire_spacing,
                 )
                 B_count = 0
 
 
-def get_electrical_ports(c: Instance) -> list[Port | DCplxPort]:
-    return [p for p in c.ports.get_all().values() if p.port_type == "electrical"]
+def get_electrical_ports(c: Instance, port_type: str = "electrical") -> list[Port]:
+    """Filter list of an instance by electrical ports."""
+    return [p for p in c.ports if p.port_type == port_type]
 
 
 def connect_wire(c: KCell, input_port: Port, output_port: Port) -> None:
-    """
+    """Connection between two electrical ports *DO NOT USE*.
+
     This function mainly implements a connection between two electrical ports.
     Not finished yet. Don't use.
+
     Args:
-        input port: kf.Port
-        output port: kf.Port
+        c: KCell to place connection in.
+        input_port: Start port.
+        output_port: End port.
     """
     if (input_port.angle + output_port.angle) % 2 == 0:
-        left_corner = (
+        (
             kdb.Point(input_port.x, input_port.y - input_port.width // 2)
             if input_port.angle % 2 == 0
             else kdb.Point(input_port.x - input_port.width // 2, input_port.y)
         )
-        middle_top = (
+        (
             kdb.Point(
                 (input_port.x + output_port.x) // 2,
                 input_port.y + input_port.width // 2,
             )
             if input_port.angle % 2 == 0
             else kdb.Point(
                 input_port.x - input_port.width // 2, (input_port.y + output_port.y)
             )
         )
-        right_corner = (
+        (
             kdb.Point(output_port.x, output_port.y + input_port.width // 2)
             if input_port.angle % 2 == 0
             else kdb.Point(output_port.x + input_port.width // 2, output_port.y)
         )
 
 
 def connect_dual_rails(
     c: KCell,
     start_port: Port,
     end_port: Port,
-    start_straight: Optional[int] = None,
-    end_straight: Optional[int] = None,
+    start_straight: int | None = None,
+    end_straight: int | None = None,
     route_path_function: Callable[..., list[kdb.Point]] = route_manhattan,
-    width: Optional[int] = None,
-    hole_width: Optional[int] = None,
-    layer: Optional[int] = None,
+    width: int | None = None,
+    hole_width: int | None = None,
+    layer: int | None = None,
 ) -> None:
+    """Connect ports with a dual-wire rail.
 
-    if width is None:
-        width = start_port.width
-    if hole_width is None:
-        hole_width = start_port.width // 2
-    if layer is None:
-        layer = start_port.layer
-    if start_straight is None:
-        start_straight = width // 2
-    if end_straight is None:
-        end_straight = width // 2
+    Args:
+        c: KCell to place the connection in.
+        start_port: Start
+        end_port: End
+        start_straight: Minimum straight after the start port.
+        end_straight: Minimum straight before end port.
+        route_path_function: Function to calculate the path. Signature:
+            `route_path_function(start_port, end_port, bend90_radius, start_straight,
+            end_straight)`
+        width: Width of the rail (total). [dbu]
+        hole_width: Width of the space between the rails. [dbu]
+        layer: layer to place the rail in.
+    """
+    _width = width or start_port.width
+    _hole_width = hole_width or start_port.width // 2
+    _layer = layer or start_port.layer
+    _start_straight = start_straight or _width // 2
+    _end_straight = end_straight or _width // 2
 
     pts = route_path_function(
         start_port.copy(),
         end_port.copy(),
         bend90_radius=0,
         start_straight=start_straight,
         end_straight=end_straight,
-        in_dbu=True,
     )
 
-    path = kdb.Path(pts, width)
-    hole_path = kdb.Path(pts, hole_width)
+    path = kdb.Path(pts, _width)
+    hole_path = kdb.Path(pts, _hole_width)
     final_poly = kdb.Region(path.polygon()) - kdb.Region(hole_path.polygon())
-    c.shapes(layer).insert(final_poly)
+    c.shapes(_layer).insert(final_poly)
```

### Comparing `kfactory-0.5.8/src/kfactory/routing/manhattan.py` & `kfactory-0.6.0/src/kfactory/routing/manhattan.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union
+"""Can calculate manhattan routes based on ports/transformations."""
 
 import numpy as np
 
 from .. import kdb
 from ..config import logger
 from ..kcell import KLib, Port
 from ..utils.geo import clean_points
@@ -14,15 +14,29 @@
     port1: kdb.DTrans,
     port2: kdb.DTrans,
     bend90_radius: float,
     bend180_radius: float,
     start_straight: float,
     end_straight: float,
     layout: KLib | kdb.Layout,
-) -> List[kdb.Point]:
+) -> list[kdb.Point]:
+    """Calculate manhattan route using um based points.
+
+    Args:
+        port1: Transformation of start port.
+        port2: Transformation of end port.
+        bend90_radius: The radius or (symmetrical) dimension of 90° bend. [um]
+        bend180_radius: The distance between the two ports of the 180° bend. [um]
+        start_straight: Minimum straight after the starting port. [um]
+        end_straight: Minimum straight before the end port. [um]
+        layout: Layout/KLib object where to get the dbu info from.
+
+    Returns:
+        route: Calculated route in points in dbu.
+    """
     return route_manhattan_180(
         port1.to_itype(layout.dbu),
         port2.to_itype(layout.dbu),
         int(bend90_radius / layout.dbu),
         int(bend180_radius / layout.dbu),
         int(start_straight / layout.dbu),
         int(end_straight / layout.dbu),
@@ -32,16 +46,28 @@
 def route_manhattan_180(
     port1: Port | kdb.Trans,
     port2: Port | kdb.Trans,
     bend90_radius: int,
     bend180_radius: int,
     start_straight: int,
     end_straight: int,
-) -> List[kdb.Point]:
-    """Calculates a  hopefully minimal distance manhattan route (no s-bends)"""
+) -> list[kdb.Point]:
+    """Calculate manhattan route using um based points.
+
+    Args:
+        port1: Transformation of start port.
+        port2: Transformation of end port.
+        bend90_radius: The radius or (symmetrical) dimension of 90° bend. [dbu]
+        bend180_radius: The distance between the two ports of the 180° bend. [dbu]
+        start_straight: Minimum straight after the starting port. [dbu]
+        end_straight: Minimum straight before the end port. [dbu]
+
+    Returns:
+        route: Calculated route in points in dbu.
+    """
     t1 = port1.dup() if isinstance(port1, kdb.Trans) else port1.trans.dup()
     t2 = port2.dup() if isinstance(port2, kdb.Trans) else port2.trans.dup()
 
     _p = kdb.Point(0, 0)
 
     p1 = t1 * _p
     p2 = t2 * _p
@@ -70,15 +96,16 @@
     match (tv.x, tv.y, (t2.angle - t1.angle) % 4):
         case (x, y, 0) if x > 0 and abs(y) == bend180_radius:
             if end_straight > 0:
                 t2 *= kdb.Trans(0, False, end_straight, 0)
             pts = [t1.disp.to_p(), t2.disp.to_p()]
             pts[1:1] = [pts[1] + (t2 * kdb.Vector(0, tv.y))]
             raise NotImplementedError(
-                "`case (x, y, 0) if x > 0 and abs(y) == bend180_radius` not supported yet"
+                "`case (x, y, 0) if x > 0 and abs(y) == bend180_radius`"
+                " not supported yet"
             )
         case (x, 0, 2):
             if start_straight > 0:
                 t1 *= kdb.Trans(0, False, start_straight, 0)
             if end_straight > 0:
                 t2 *= kdb.Trans(0, False, end_straight, 0)
             pts = [t1.disp.to_p(), t2.disp.to_p()]
@@ -98,50 +125,77 @@
         case _:
             return route_manhattan(
                 t1.dup(),
                 t2.dup(),
                 bend90_radius,
                 start_straight=0,
                 end_straight=end_straight,
-                in_dbu=True,
             )
     raise NotImplementedError(
-        "Case not supportedt yet. Please open an issue if you believe this is an error and needs to be implemented ;)"
+        "Case not supportedt yet. Please open an issue if you believe this is an error"
+        " and needs to be implemented ;)"
     )
 
 
 def droute_manhattan(
     port1: kdb.DTrans,
     port2: kdb.DTrans,
     bend90_radius: int,
     start_straight: int,
     end_straight: int,
     layout: KLib | kdb.Layout,
-) -> List[kdb.Point]:
+) -> list[kdb.Point]:
+    """Calculate manhattan route using um based points.
+
+    Doesn't use any non-90° bends.
+
+    Args:
+        port1: Transformation of start port.
+        port2: Transformation of end port.
+        bend90_radius: The radius or (symmetrical) dimension of 90° bend. [um]
+        start_straight: Minimum straight after the starting port. [um]
+        end_straight: Minimum straight before the end port. [um]
+        layout: Layout/KLib object where to get the dbu info from.
+
+    Returns:
+        route: Calculated route in points in dbu.
+    """
     return route_manhattan(
         port1.to_itype(layout.dbu),
         port2.to_itype(layout.dbu),
         int(bend90_radius / layout.dbu),
         int(start_straight / layout.dbu),
         int(end_straight / layout.dbu),
     )
 
 
 def route_manhattan(
-    port1: Union[Port, kdb.Trans],
-    port2: Union[Port, kdb.Trans],
+    port1: Port | kdb.Trans,
+    port2: Port | kdb.Trans,
     bend90_radius: int,
     start_straight: int,
     end_straight: int,
-    in_dbu: bool = True,
-    layout: Optional[KLib | kdb.Layout] = None,
     max_tries: int = 20,
-) -> List[kdb.Point]:
-    """Calculates a hopefully minimal distance manhattan route (no s-bends)"""
+) -> list[kdb.Point]:
+    """Calculate manhattan route using um based points.
 
+    Doesn't use any non-90° bends.
+
+    Args:
+        port1: Transformation of start port.
+        port2: Transformation of end port.
+        bend90_radius: The radius or (symmetrical) dimension of 90° bend. [dbu]
+        start_straight: Minimum straight after the starting port. [dbu]
+        end_straight: Minimum straight before the end port. [dbu]
+        max_tries: Maximum number of tries to calculate a manhattan route before
+        giving up
+
+    Returns:
+        route: Calculated route in points in dbu.
+    """
     t1 = port1.dup() if isinstance(port1, kdb.Trans) else port1.trans.dup()
     t2 = port2.dup() if isinstance(port2, kdb.Trans) else port2.trans.dup()
     _p = kdb.Point(0, 0)
 
     p1 = t1 * _p
     p2 = t2 * _p
     tv = t1.inverted() * (t2.disp - t1.disp)
@@ -168,15 +222,16 @@
         (t2 * kdb.Trans(0, False, end_straight, 0)).disp.to_p(),
     )
     match (box.width(), box.height()):
         case (x, y) if (x < bend90_radius and y <= 2 * bend90_radius) or (
             x <= 2 * bend90_radius and y < bend90_radius
         ):
             logger.warning(
-                f"Potential collision in routing due to small distance between the port in relation to bend radius {x=}/{bend90_radius}, {y=}/{bend90_radius}",
+                "Potential collision in routing due to small distance between the port "
+                f"in relation to bend radius {x=}/{bend90_radius}, {y=}/{bend90_radius}"
             )
 
     # we want a straight start and have to add a bend radius if
     t1 *= kdb.Trans(start_straight + bend90_radius, 0)
     tv = t1.inverted() * (t2.disp - t1.disp)
 
     points = [p1]
@@ -188,27 +243,15 @@
             end_points = [p2]
         else:
             end_points = [t2 * _p, p2]
     else:
         t2 *= kdb.Trans(end_straight + bend90_radius, 0)
         end_points = [t2 * _p, p2]
 
-        # TODO: This works but in some cases makes wrong routes
-        # match (tv.x, tv.y):
-        #     # case (x, y) if -bend90_radius < x < bend90_radius and abs(y) >= bend90_radius:
-        #     #     end_points = [ t2 * _p, p2]
-        #     case (x, y) if -bend90_radius < x < 0:
-        #         # end_points = [t2 * _p, p2]
-        #         t2 *= kdb.Trans(int(np.sign(x)), False, 0, 2 * bend90_radius + abs(x))
-        #         end_points.insert(0, t2 * _p)
-        #     case (x, y) if 0 <= x < bend90_radius:
-        #         t2 *= kdb.Trans(-int(np.sign(x)), False, 0, 2 * bend90_radius)
-        #         end_points.insert(0, t2 * _p)
-
-    v = t1.inverted() * (t2.disp - t1.disp)
+    t1.inverted() * (t2.disp - t1.disp)
 
     for i in range(max_tries):
         tv = t1.inverted() * (t2.disp - t1.disp)
         if tv.abs() == 0 and (t2.angle - t1.angle) % 4 == 2:
             break
         if (t2.angle - t1.angle) % 4 == 2 and tv.x > 0 and tv.y == 0:
             break
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `kfactory-0.5.8/src/kfactory/routing/optical.py` & `kfactory-0.6.0/src/kfactory/routing/optical.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,76 @@
-from typing import Callable, List, Optional, Sequence, Union
+"""Optical routing allows the creation of photonic (or any route using bends)."""
+
+from collections.abc import Callable, Sequence
 
 from .. import kdb
-from ..kcell import DCplxPort, KCell, Port
-from ..utils.geo import vec_angle  # , clean_points
+from ..config import logger
+from ..kcell import KCell, Port
 from .manhattan import route_manhattan
 
 
+def vec_angle(v: kdb.Vector) -> int:
+    """Determine vector angle in increments of 90°."""
+    if v.x != 0 and v.y != 0:
+        raise NotImplementedError("only manhattan vectors supported")
+
+    match (v.x, v.y):
+        case (x, 0) if x > 0:
+            return 0
+        case (x, 0) if x < 0:
+            return 2
+        case (0, y) if y > 0:
+            return 1
+        case (0, y) if y < 0:
+            return 3
+        case _:
+            logger.warning(f"{v} is not a manhattan, cannot determine direction")
+    return -1
+
+
 def route_loopback(
-    p1: Union[Port, kdb.Trans],
-    p2: Union[Port, kdb.Trans],
+    p1: Port | kdb.Trans,
+    p2: Port | kdb.Trans,
     bend90_radius: int,
-    bend180_radius: Optional[int] = None,
+    bend180_radius: int | None = None,
     start_straight: int = 0,
     end_straight: int = 0,
-    in_dbu: bool = True,
     d_loop: int = 200000,
-) -> List[kdb.Point]:
+) -> list[kdb.Point]:
+    r"""Create a loopback on two parallel ports.
 
+        ╭----╮            ╭----╮
+        |    |            |    |
+        |  -----        -----  |
+        |  port1        port2  |
+        ╰----------------------╯
+
+
+    Args:
+        p1: Start port.
+        p2: End port.
+        bend90_radius: Radius of 90° bend. [dbu]
+        bend180_radius: Optional use of 180° bend, distance between two parallel ports.
+            [dbu]
+        start_straight: Minimal straight segment after `p1`.
+        end_straight: Minimal straight segment before `p2`.
+        d_loop: Distance of the (vertical) offset of the back of the ports
+
+    Returns:
+        points: List of the calculated points (starting/ending at p1/p2).
+    """
     t1 = p1 if isinstance(p1, kdb.Trans) else p1.trans
     t2 = p2 if isinstance(p2, kdb.Trans) else p2.trans
 
     if (t1.angle != t2.angle) and (
         (t1.disp.x == t2.disp.x) or (t1.disp.y == t2.disp.y)
     ):
         raise ValueError(
-            "for a standard loopback the ports must point in the same direction and have to be parallel"
+            "for a standard loopback the ports must point in the same direction and"
+            "have to be parallel"
         )
 
     pz = kdb.Point(0, 0)
 
     if (
         start_straight > 0
         and bend180_radius is None
@@ -74,88 +116,86 @@
             start_straight=start_straight + d_loop,
             end_straight=0,
         )
         + pts_end
     )  # end_straight=end_straight# + d_loop,
 
 
+@logger.catch
 def connect(
     c: KCell,
     p1: Port,
     p2: Port,
     straight_factory: Callable[[int, int], KCell],
     bend90_cell: KCell,
-    bend180_cell: Optional[KCell] = None,
-    taper_cell: Optional[KCell] = None,
+    bend180_cell: KCell | None = None,
+    taper_cell: KCell | None = None,
     start_straight: int = 0,
     end_straight: int = 0,
     route_path_function: Callable[
         ...,
-        List[kdb.Point],
+        list[kdb.Point],
     ] = route_manhattan,
     port_type: str = "optical",
     allow_small_routes: int = False,
     different_port_width: int = False,
 ) -> None:
     """Bend 90 part."""
-
     if p1.width != p2.width and not different_port_width:
         raise ValueError(
-            f"The ports have different widths {p1.width=} {p2.width=}. If this is intentional, add `different_port_width=True` to override this."
+            f"The ports have different widths {p1.width=} {p2.width=}. If this is"
+            "intentional, add `different_port_width=True` to override this."
         )
 
     p1 = p1.copy()
     p1.trans.mirror = False
     p2 = p2.copy()
     p2.trans.mirror = False
 
     # determine bend90_radius
-    bend90_ports = [
-        p for p in bend90_cell.ports.get_all().values() if p.port_type == port_type
-    ]
-    if len(bend90_ports) != 2:
-        raise AttributeError(
-            f"{bend90_cell.name} should have 2 ports but has {len(bend90_ports)} ports"
-        )
-    if abs((bend90_ports[0].trans.angle - bend90_ports[1].trans.angle) % 4) != 1:
-        raise AttributeError(
-            f"{bend90_cell.name} bend ports should be 90° apart from each other"
-        )
+    bend90_ports = [p for p in bend90_cell.ports if p.port_type == port_type]
+
+    assert (
+        len(bend90_ports) == 2
+    ), f"{bend90_cell.name} should have 2 ports but has {len(bend90_ports)} ports"
+    assert (
+        abs((bend90_ports[0].trans.angle - bend90_ports[1].trans.angle) % 4) == 1
+    ), f"{bend90_cell.name} bend ports should be 90° apart from each other"
     if (bend90_ports[1].trans.angle - bend90_ports[0].trans.angle) % 4 == 3:
         b90p1 = bend90_ports[1]
         b90p2 = bend90_ports[0]
     else:
         b90p1 = bend90_ports[0]
         b90p2 = bend90_ports[1]
 
     b90c = kdb.Trans(
         b90p1.trans.rot,
         b90p1.trans.is_mirror(),
         b90p1.trans.disp.x if b90p1.trans.angle % 2 else b90p2.trans.disp.x,
         b90p2.trans.disp.y if b90p1.trans.angle % 2 else b90p1.trans.disp.y,
     )
 
-    start_port: Port | DCplxPort = p1.copy()
-    end_port: Port | DCplxPort = p2.copy()
+    start_port: Port = p1.copy()
+    end_port: Port = p2.copy()
     b90r = int(
         max((b90p1.trans.disp - b90c.disp).abs(), (b90p2.trans.disp - b90c.disp).abs())
     )
 
     if bend180_cell is not None:
         # Bend 180 is available
-        bend180_ports = [
-            p for p in bend180_cell.ports.get_all().values() if p.port_type == port_type
-        ]
+        bend180_ports = [p for p in bend180_cell.ports if p.port_type == port_type]
         if len(bend180_ports) != 2:
             raise AttributeError(
-                f"{bend180_cell.name} should have 2 ports but has {len(bend180_ports)} ports"
+                f"{bend180_cell.name} should have 2 ports but has {len(bend180_ports)}"
+                " ports"
             )
         if abs((bend180_ports[0].trans.angle - bend180_ports[1].trans.angle) % 4) != 0:
             raise AttributeError(
-                f"{bend180_cell.name} bend ports for bend180 should be 0° apart from each other"
+                f"{bend180_cell.name} bend ports for bend180 should be 0° apart from"
+                " each other"
             )
         d = 1 if bend180_ports[0].trans.angle in [0, 3] else -1
         b180p1, b180p2 = list(
             sorted(
                 bend180_ports,
                 key=lambda port: (d * port.trans.disp.x, d * port.trans.disp.y),
             )
@@ -174,33 +214,33 @@
         )
 
         if len(pts) > 2:
             if (vec := pts[1] - pts[0]).abs() == b180r:
                 match (p1.trans.angle - vec_angle(vec)) % 4:
                     case 1:
                         bend180 = c << bend180_cell
-                        bend180.connect(b180p1.name, p1)
+                        bend180.align(b180p1.name, p1)
                         start_port = bend180.ports[b180p2.name]
                         pts = pts[1:]
                     case 3:
                         bend180 = c << bend180_cell
-                        bend180.connect(b180p2.name, p1)
+                        bend180.align(b180p2.name, p1)
                         start_port = bend180.ports[b180p1.name]
                         pts = pts[1:]
             if (vec := pts[-1] - pts[-2]).abs() == b180r:
                 match ((vec_angle(vec) - p2.trans.angle) % 4):
                     case 1:
                         bend180 = c << bend180_cell
-                        bend180.connect(b180p1.name, p2)
+                        bend180.align(b180p1.name, p2)
                         end_port = bend180.ports[b180p2.name]
                         pts = pts[:-1]
                     case 3:
                         bend180 = c << bend180_cell
                         # bend180.mirror = True
-                        bend180.connect(b180p2.name, p2)
+                        bend180.align(b180p2.name, p2)
                         end_port = bend180.ports[b180p1.name]
                         pts = pts[:-1]
 
             if len(pts) > 3:
                 # TODO 180 stuff
                 pt1, pt2, pt3 = pts[:3]
                 j = 0
@@ -213,18 +253,18 @@
                     ang1 = vec_angle(vecp)
                     ang2 = vec_angle(vec)
                     ang3 = vec_angle(vecn)
 
                     if vecp == vec and ang2 - ang1 == 0:
                         bend180 = c << bend180_cell
                         if start_port.name == b180p2.name:
-                            bend180.connect(b180p1.name, start_port)
+                            bend180.align(b180p1.name, start_port)
                             start_port = bend180.ports[b180p2.name]
                         else:
-                            bend180.connect(b180p2.name, start_port)
+                            bend180.align(b180p2.name, start_port)
                             start_port = bend180.ports[b180p1.name]
                         j = i - 1
                     elif (
                         vec.abs() == b180r
                         and (ang2 - ang1) % 4 == 1
                         and (ang3 - ang2) % 4 == 1
                     ):
@@ -232,15 +272,15 @@
                         bend180.transform(
                             kdb.Trans((ang1 + 2) % 4, False, pt2.x, pt2.y)
                             * b180p1.trans.inverted()
                         )
                         place90(
                             c,
                             start_port.copy(),
-                            bend180.port[b180p1.name],
+                            bend180.ports[b180p1.name],
                             pts[j : i - 2],
                             straight_factory,
                             bend90_cell,
                             taper_cell,
                         )
                         j = i - 1
                         start_port = bend180.ports[b180p2.name]
@@ -253,15 +293,15 @@
                         bend180.transform(
                             kdb.Trans((ang1 + 2) % 4, False, pt2.x, pt2.y)
                             * b180p2.trans.inverted()
                         )
                         place90(
                             c,
                             start_port.copy(),
-                            bend180.port[b180p2.name],
+                            bend180.ports[b180p2.name],
                             pts[j : i - 2],
                             straight_factory,
                             bend90_cell,
                             taper_cell,
                         )
                         j = i - 1
                         start_port = bend180.ports[b180p1.name]
@@ -277,15 +317,14 @@
             pts,
             straight_factory,
             bend90_cell,
             taper_cell,
         )
 
     else:
-
         start_port = p1.copy()
         end_port = p2.copy()
         pts = route_path_function(
             start_port,
             end_port,
             bend90_radius=b90r,
             start_straight=start_straight,
@@ -293,123 +332,158 @@
         )
 
         place90(c, p1.copy(), p2.copy(), pts, straight_factory, bend90_cell, taper_cell)
 
 
 def place90(
     c: KCell,
-    p1: Port | DCplxPort,
-    p2: Port | DCplxPort,
+    p1: Port,
+    p2: Port,
     pts: Sequence[kdb.Point],
     straight_factory: Callable[..., KCell],
     bend90_cell: KCell,
-    taper_cell: Optional[KCell] = None,
+    taper_cell: KCell | None = None,
     port_type: str = "optical",
     min_straight_taper: int = 1000,
     allow_small_routes: bool = False,
 ) -> None:
+    """Place bends and straight waveguides based on a sequence of points.
+
+    This version will not take any non-90° bends. If the taper is not `None`, tapers
+    will be added to straights that fulfill the minimum length.
 
+    This function will throw an error in case it cannot place bends due to too small
+    routings, E.g. two corner are too close for two bends to be safely placed.
+
+
+    Args:
+        c: Cell in which the route should be placed.
+        p1: Start port.
+        p2: End port.
+        pts: The points
+        straight_factory: A function which takes two keyword arguments `width`
+            and `length`. It returns a :py:class:~`KCell` with two named ports with
+            port_type `port_type` and matching layer as the `bend90_cell` ports.
+        bend90_cell: Bend to use in corners of the `pts`. Must have two named ports on
+            `port_type`
+        taper_cell: Optional taper cell to use if straights and bends should have a
+            different width on the connection layer. Must have two named ports on
+            `port_type` and share the port layer with `bend90_cell` and
+            `straight_factory`.
+        port_type: Filter the port type by this to e.g. ignore potential electrical
+            ports.
+        min_straight_taper: Do not put tapers on a straight if its length
+            is below this minimum length.
+        allow_small_routes: Don't throw an error if two corners cannot be safely placed
+            due to small space and place them anyway.
+    """
     if not pts:
         # Nothing to be placed
         return
     w = p1.width
     old_pt = pts[0]
     old_bend_port = p1
-    bend90_ports = [
-        p for p in bend90_cell.ports.get_all().values() if p.port_type == port_type
-    ]
+    bend90_ports = [p for p in bend90_cell.ports if p.port_type == port_type]
 
     if len(bend90_ports) != 2:
         raise AttributeError(
             f"{bend90_cell.name} should have 2 ports but has {len(bend90_ports)} ports"
+            f"with {port_type=}"
         )
     if abs((bend90_ports[0].trans.angle - bend90_ports[1].trans.angle) % 4) != 1:
         raise AttributeError(
             f"{bend90_cell.name} bend ports should be 90° apart from each other"
         )
 
     if (bend90_ports[1].trans.angle - bend90_ports[0].trans.angle) % 4 == 3:
         b90p1 = bend90_ports[1]
         b90p2 = bend90_ports[0]
     else:
         b90p1 = bend90_ports[0]
         b90p2 = bend90_ports[1]
+    assert b90p1.name is not None, logger.error(
+        "bend90_cell needs named ports, {}", b90p1
+    )
+    assert b90p2.name is not None, logger.error(
+        "bend90_cell needs named ports, {}", b90p2
+    )
     b90c = kdb.Trans(
         b90p1.trans.rot,
         b90p1.trans.is_mirror(),
         b90p1.trans.disp.x if b90p1.trans.angle % 2 else b90p2.trans.disp.x,
         b90p2.trans.disp.y if b90p1.trans.angle % 2 else b90p1.trans.disp.y,
     )
     b90r = max(
         (b90p1.trans.disp - b90c.disp).abs(), (b90p2.trans.disp - b90c.disp).abs()
     )
     if taper_cell is not None:
-        taper_ports = list(taper_cell.ports.get_all().values())
-        taper_ports = [p for p in taper_ports if p.port_type == "optical"]
+        taper_ports = [p for p in taper_cell.ports if p.port_type == "optical"]
         if (
             len(taper_ports) != 2
             or (taper_ports[1].trans.angle + 2) % 4 != taper_ports[0].trans.angle
         ):
             raise AttributeError(
-                "Taper must have only two optical ports that are 180° oriented to each other"
+                "Taper must have only two optical ports that are 180° oriented to each"
+                " other"
             )
         if taper_ports[1].width == b90p1.width:
             taperp2, taperp1 = taper_ports
         elif taper_ports[0].width == b90p1.width:
             taperp1, taperp2 = taper_ports
         else:
             raise AttributeError(
-                "At least one optical ports of the taper must be the same width as the bend's ports"
+                "At least one optical ports of the taper must be the same width as"
+                " the bend's ports"
             )
 
     if len(pts) == 2:
         length = (pts[1] - pts[0]).abs()
         if (
             taper_cell is None
             or length
             < (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 + min_straight_taper
         ):
             wg = c << straight_factory(width=w, length=(pts[1] - pts[0]).abs())
-            _p1, _p2 = (
-                v for v in wg.ports.get_all().values() if v.port_type == port_type
-            )
-            wg.connect(_p1.name, p1)
+            wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
+            wg.align(wg_p1, p1)
         else:
             t1 = c << taper_cell
-            t1.connect(taperp1.name, p1)
+            t1.align(taperp1.name, p1)
             if length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 != 0:
                 wg = c << straight_factory(
                     width=taperp2.width,
                     length=length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2,
                 )
-                _p1, _p2 = (
-                    v for v in wg.ports.get_all().values() if v.port_type == port_type
-                )
-                wg.connect(_p1.name, t1, taperp2.name)
+                wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
+                wg.align(wg_p1, t1, taperp2.name)
                 t2 = c << taper_cell
-                t2.connect(taperp2.name, wg, _p2.name)
+                t2.align(taperp2.name, wg_p2)
             else:
                 t2 = c << taper_cell
-                t2.connect(taperp2.name, t1, taperp2.name)
+                t2.align(taperp2.name, t1, taperp2.name)
         return
     for i in range(1, len(pts) - 1):
         pt = pts[i]
         new_pt = pts[i + 1]
 
         if (pt.distance(old_pt) < b90r) and not allow_small_routes:
             raise ValueError(
-                f"distance between points {str(old_pt)} and {str(pt)} is too small to safely place bends {pt.to_s()=}, {old_pt.to_s()=}, {pt.distance(old_pt)=} < {b90r=}"
+                f"distance between points {str(old_pt)} and {str(pt)} is too small to"
+                f" safely place bends {pt.to_s()=}, {old_pt.to_s()=},"
+                f" {pt.distance(old_pt)=} < {b90r=}"
             )
         elif (
             pt.distance(old_pt) < 2 * b90r
             and i not in [1, len(pts) - 1]
             and not allow_small_routes
         ):
             raise ValueError(
-                f"distance between points {str(old_pt)} and {str(pt)} is too small to safely place bends {str(pt)=}, {str(old_pt)=}, {pt.distance(old_pt)=} < {2 * b90r=}"
+                f"distance between points {str(old_pt)} and {str(pt)} is too small to"
+                f" safely place bends {str(pt)=}, {str(old_pt)=},"
+                f" {pt.distance(old_pt)=} < {2 * b90r=}"
             )
 
         vec = pt - old_pt
         vec_n = new_pt - pt
 
         bend90 = c << bend90_cell
         mirror = (vec_angle(vec_n) - vec_angle(vec)) % 4 != 3
@@ -419,70 +493,58 @@
             )
         ang = (vec_angle(vec) + 2) % 4
         if ang is None:
             raise ValueError(
                 f"The vector between manhattan points is not manhattan {old_pt}, {pt}"
             )
         bend90.transform(kdb.Trans(ang, mirror, pt.x, pt.y) * b90c.inverted())
-        length = (bend90.ports[b90p1.name].trans.disp - old_bend_port.trans.disp).abs()  # type: ignore[operator]
+        length = (bend90.ports[b90p1.name].trans.disp - old_bend_port.trans.disp).abs()
         if length > 0:
             if (
                 taper_cell is None
                 or length
                 < (taperp1.trans.disp - taperp2.trans.disp).abs() * 2
                 + min_straight_taper
             ):
                 wg = c << straight_factory(width=w, length=length)
-                _p1, _p2 = (
-                    v for v in wg.ports.get_all().values() if v.port_type == port_type
-                )
-                wg.connect(_p1.name, bend90, b90p1.name)
+                wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
+                wg.align(wg_p1, bend90, b90p1.name)
             else:
                 t1 = c << taper_cell
-                t1.connect(taperp1.name, bend90, b90p1.name)
+                t1.align(taperp1.name, bend90, b90p1.name)
                 if length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 != 0:
                     wg = c << straight_factory(
                         width=taperp2.width,
                         length=length
                         - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2,
                     )
-                    _p1, _p2 = (
-                        v
-                        for v in wg.ports.get_all().values()
-                        if v.port_type == port_type
-                    )
-                    wg.connect(_p1.name, t1, taperp2.name)
+                    wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
+                    wg.align(wg_p1.name, t1, taperp2.name)
                     t2 = c << taper_cell
-                    t2.connect(taperp2.name, wg, _p2.name)
+                    t2.align(taperp2.name, wg, wg_p2.name)
                 else:
                     t2 = c << taper_cell
-                    t2.connect(taperp2.name, t1, taperp2.name)
+                    t2.align(taperp2.name, t1, taperp2.name)
         old_pt = pt
         old_bend_port = bend90.ports[b90p2.name]
-    length = (
-        bend90.ports[b90p2.name].trans.disp - p2.trans.disp  # type:ignore[operator]
-    ).abs()
+    length = (bend90.ports[b90p2.name].trans.disp - p2.trans.disp).abs()
     if length > 0:
         if (
             taper_cell is None
             or length
             < (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 + min_straight_taper
         ):
             wg = c << straight_factory(width=w, length=length)
-            _p1, _p2 = (
-                v for v in wg.ports.get_all().values() if v.port_type == port_type
-            )
-            wg.connect(_p1.name, bend90, b90p2.name)
+            wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
+            wg.align(wg_p1.name, bend90, b90p2.name)
         else:
             t1 = c << taper_cell
-            t1.connect(taperp1.name, bend90, b90p2.name)
+            t1.align(taperp1.name, bend90, b90p2.name)
             if length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2 != 0:
                 wg = c << straight_factory(
                     width=taperp2.width,
                     length=length - (taperp1.trans.disp - taperp2.trans.disp).abs() * 2,
                 )
-                _p1, _p2 = (
-                    v for v in wg.ports.get_all().values() if v.port_type == port_type
-                )
-                wg.connect(_p1.name, t1, taperp2.name)
+                wg_p1, wg_p2 = (v for v in wg.ports if v.port_type == port_type)
+                wg.align(wg_p1.name, t1, taperp2.name)
                 t2 = c << taper_cell
-                t2.connect(taperp2.name, wg, _p2.name)
+                t2.align(taperp2.name, wg, wg_p2.name)
```

### Comparing `kfactory-0.5.8/src/kfactory/utils/geo.py` & `kfactory-0.6.0/src/kfactory/utils/geo/enclosure.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,56 +1,59 @@
-from enum import Enum
+from collections.abc import Callable, Sequence
+from enum import IntEnum
 from hashlib import sha1
-from typing import Any, Callable, List, Optional, Sequence, TypeGuard, cast, overload
+from typing import Any, Optional, TypeGuard
 
 import numpy as np
-from numpy.typing import ArrayLike
-from pydantic import BaseModel, PrivateAttr
+from pydantic import BaseModel, Field, PrivateAttr
 
-from .. import kdb
-from ..config import logger
-from ..kcell import KCell, LayerEnum
+from ... import kdb
+from ...kcell import KCell, LayerEnum
 
 __all__ = [
+    "Enclosure",
     "extrude_path",
     "extrude_path_points",
-    "extrude_path_dynamic_points",
     "extrude_path_dynamic",
-    "path_pts_to_polygon",
-    "Enclosure",
-    "Direction",
+    "extrude_path_dynamic_points",
 ]
 
 
-def vec_angle(v: kdb.Vector) -> int:
-    """Determine vector angle in increments of 90°"""
-    if v.x != 0 and v.y != 0:
-        raise NotImplementedError("only manhattan vectors supported")
-
-    match (v.x, v.y):
-        case (x, 0) if x > 0:
-            return 0
-        case (x, 0) if x < 0:
-            return 2
-        case (0, y) if y > 0:
-            return 1
-        case (0, y) if y < 0:
-            return 3
-        case _:
-            logger.warning(f"{v} is not a manhattan, cannot determine direction")
-    return -1
+class Direction(IntEnum):
+    X = 1
+    Y = 2
+    BOTH = 3
 
 
 def is_callable_widths(
     widths: Callable[[float], float] | list[float]
 ) -> TypeGuard[Callable[[float], float]]:
     return callable(widths)
 
 
-def clean_points(points: List[kdb.Point]) -> List[kdb.Point]:
+def path_pts_to_polygon(
+    pts_top: list[kdb.DPoint], pts_bot: list[kdb.DPoint]
+) -> kdb.DPolygon:
+    pts_bot.reverse()
+    return kdb.DPolygon(pts_top + pts_bot)
+
+
+def is_Region(r: object) -> TypeGuard[kdb.Region]:
+    return isinstance(r, kdb.Region)
+
+
+def is_int(r: object) -> TypeGuard[int]:
+    return isinstance(r, int)
+
+
+def is_callable(r: object) -> TypeGuard[Callable[[float], float]]:
+    return callable(r)
+
+
+def clean_points(points: list[kdb.Point]) -> list[kdb.Point]:
     if len(points) < 2:
         return points
     if len(points) == 2:
         return points if points[1] != points[0] else points[:1]
     p_p = points[0]
     p = points[1]
 
@@ -68,76 +71,30 @@
 
     for i in reversed(del_points):
         del points[i]
 
     return points
 
 
-def simplify(points: list[kdb.Point], tolerance: float) -> list[kdb.Point]:
-    simple_pts: list[kdb.Point] = [points[0]]
-    if len(points) < 3:
-        return points
-
-    start = 0
-    last = len(points) - 1
-
-    e = kdb.Edge(points[0], points[-1])
-    dists = [e.distance_abs(p) for p in points]
-    ind_dist = int(np.argmax(dists))
-    maxd = dists[ind_dist]
-
-    return (
-        [points[0], points[-1]]
-        if maxd <= tolerance
-        else (
-            simplify(points[: ind_dist + 1], tolerance)
-            + simplify(points[ind_dist:], tolerance)[1:]
-        )
-    )
-
-
-def dsimplify(points: list[kdb.DPoint], tolerance: float) -> list[kdb.DPoint]:
-    if len(points) < 3:
-        return points
-    simple_pts: list[kdb.DPoint] = [points[0]]
-
-    start = 0
-    last = len(points) - 1
-
-    e = kdb.DEdge(points[0], points[-1])
-    dists = [e.distance_abs(p) for p in points]
-    ind_dist = int(np.argmax(dists))
-    maxd = dists[ind_dist]
-
-    return (
-        [points[0], points[-1]]
-        if maxd <= tolerance
-        else (
-            dsimplify(points[: ind_dist + 1], tolerance)
-            + dsimplify(points[ind_dist:], tolerance)[1:]
-        )
-    )
-
-
 def extrude_path_points(
     path: list[kdb.DPoint],
     width: float,
-    start_angle: Optional[float] = None,
-    end_angle: Optional[float] = None,
+    start_angle: float | None = None,
+    end_angle: float | None = None,
 ) -> tuple[list[kdb.DPoint], list[kdb.DPoint]]:
-    """
-    Extrude a path from a list of points and a static width
+    """Extrude a path from a list of points and a static width.
 
     Args:
         path: list of floating-points points
         width: width in µm
-        start_angle: optionally specify a custom starting angle if `None` will be autocalculated from the first two elements
-        end_angle: optionally specify a custom ending angle if `None` will be autocalculated from the last two elements
+        start_angle: optionally specify a custom starting angle if `None` will
+            be autocalculated from the first two elements
+        end_angle: optionally specify a custom ending angle if `None`
+            will be autocalculated from the last two elements
     """
-
     start = path[1] - path[0]
     end = path[-1] - path[-2]
     if start_angle is None:
         start_angle = np.rad2deg(np.arctan2(start.y, start.x))
     if end_angle is None:
         end_angle = np.rad2deg(np.rad2deg(np.arctan2(end.y, end.x)))
 
@@ -171,35 +128,37 @@
 
 def extrude_path(
     target: KCell,
     layer: LayerEnum | int,
     path: list[kdb.DPoint],
     width: float,
     enclosure: Optional["Enclosure"] = None,
-    start_angle: Optional[float] = None,
-    end_angle: Optional[float] = None,
+    start_angle: float | None = None,
+    end_angle: float | None = None,
 ) -> None:
-    """
-    Extrude a path from a list of points and a static width
+    """Extrude a path from a list of points and a static width.
 
     Args:
         target: the cell where to insert the shapes to (and get the database unit from)
         layer: the main layer that should be extruded
         path: list of floating-points points
         width: width in µm
-        enclosure: optoinal enclosure object, specifying necessary layers.this will extrude around the `layer`
-        start_angle: optionally specify a custom starting angle if `None` will be autocalculated from the first two elements
-        end_angle: optionally specify a custom ending angle if `None` will be autocalculated from the last two elements
+        enclosure: optoinal enclosure object, specifying necessary
+            layers.this will extrude around the `layer`
+        start_angle: optionally specify a custom starting angle if `None`
+            will be autocalculated from the first two elements
+        end_angle: optionally specify a custom ending angle if `None` will be
+            autocalculated from the last two elements
     """
     layer_list = {layer: LayerSection(sections=[Section(d_max=0)])}
     if enclosure is not None:
         if layer not in enclosure.layer_sections:
             layer_list |= enclosure.layer_sections
         else:
-            ls = layer_list[layer].sections.copy()
+            layer_list[layer].sections.copy()
             layer_list = enclosure.layer_sections.copy()
             for section in layer_list[layer].sections:
                 layer_list[layer].add_section(section)
 
     for layer, layer_sec in layer_list.items():
         reg = kdb.Region()
         for section in layer_sec.sections:
@@ -227,25 +186,27 @@
             reg.insert(_r)
         target.shapes(layer).insert(reg.merge())
 
 
 def extrude_path_dynamic_points(
     path: list[kdb.DPoint],
     widths: Callable[[float], float] | list[float],
-    start_angle: Optional[float] = None,
-    end_angle: Optional[float] = None,
+    start_angle: float | None = None,
+    end_angle: float | None = None,
 ) -> tuple[list[kdb.DPoint], list[kdb.DPoint]]:
-    """
-    Extrude a profile with a list of points and a list of widths
+    """Extrude a profile with a list of points and a list of widths.
 
     Args:
         path: list of floating-points points
-        width: function (from t==0 to t==1) defining a width profile for the path | list with width for the profile (needs same length as path)
-        start_angle: optionally specify a custom starting angle if `None` will be autocalculated from the first two elements
-        end_angle: optionally specify a custom ending angle if `None` will be autocalculated from the last two elements
+        widths: function (from t==0 to t==1) defining a width profile for the path
+            | list with width for the profile (needs same length as path)
+        start_angle: optionally specify a custom starting angle if `None` will be
+            autocalculated from the first two elements
+        end_angle: optionally specify a custom ending angle if `None` will be
+            autocalculated from the last two elements
     """
     start = path[1] - path[0]
     end = path[-1] - path[-2]
     if start_angle is None:
         start_angle = np.rad2deg(np.arctan2(start.y, start.x))
     if end_angle is None:
         end_angle = np.rad2deg(np.rad2deg(np.arctan2(end.y, end.x)))
@@ -253,34 +214,34 @@
     p_start = path[0]
     p_end = path[-1]
 
     start_trans = kdb.DCplxTrans(1, start_angle, False, p_start.x, p_start.y)
     end_trans = kdb.DCplxTrans(1, end_angle, False, p_end.x, p_end.y)
 
     if callable(widths):
-        l = sum(((p2 - p1).abs() for p2, p1 in zip(path[:-1], path[1:])))
+        length = sum(((p2 - p1).abs() for p2, p1 in zip(path[:-1], path[1:])))
         z: float = 0
-        ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths(z / l) / 2))
+        ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths(z / length) / 2))
         vector_top = [start_trans * ref_vector]
         vector_bot = [start_trans * kdb.DCplxTrans.R180 * ref_vector]
         p_old = path[0]
         p = path[1]
         z += (p - p_old).abs()
         for point in path[2:]:
-            ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths(z / l) / 2))
+            ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths(z / length) / 2))
             p_new = point
             v = p_new - p_old
             angle = np.rad2deg(np.arctan2(v.y, v.x))
             transformation = kdb.DCplxTrans(1, angle, False, p.x, p.y)
             vector_top.append(transformation * ref_vector)
             vector_bot.append(transformation * kdb.DCplxTrans.R180 * ref_vector)
             z += (p_new - p).abs()
             p_old = p
             p = p_new
-        ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths(z / l) / 2))
+        ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths(z / length) / 2))
     else:
         ref_vector = kdb.DCplxTrans(kdb.DVector(0, widths[0] / 2))
         vector_top = [start_trans * ref_vector]
         vector_bot = [start_trans * kdb.DCplxTrans.R180 * ref_vector]
         p_old = path[0]
         p = path[1]
         for point, w in zip(path[2:], widths[1:-1]):
@@ -302,36 +263,41 @@
 
 def extrude_path_dynamic(
     target: KCell,
     layer: LayerEnum | int,
     path: list[kdb.DPoint],
     widths: Callable[[float], float] | list[float],
     enclosure: Optional["Enclosure"] = None,
-    start_angle: Optional[float] = None,
-    end_angle: Optional[float] = None,
+    start_angle: float | None = None,
+    end_angle: float | None = None,
 ) -> None:
-    """
-    Extrude a path with dynamic width from a list of points and a list of widths and add an enclosure if specified
+    """Extrude a path with dynamic width.
+
+    Extrude from a list of points and a list of widths and add an enclosure if
+        specified.
 
     Args:
         target: the cell where to insert the shapes to (and get the database unit from)
         layer: the main layer that should be extruded
         path: list of floating-points points
-        width: function (from t==0 to t==1) defining a width profile for the path | list with width for the profile (needs same length as path)
-        enclosure: optoinal enclosure object, specifying necessary layers.this will extrude around the `layer`
-        start_angle: optionally specify a custom starting angle if `None` will be autocalculated from the first two elements
-        end_angle: optionally specify a custom ending angle if `None` will be autocalculated from the last two elements
+        widths: function (from t==0 to t==1) defining a width profile for the path |
+            list with width for the profile (needs same length as path)
+        enclosure: optoinal enclosure object, specifying necessary layers.this will
+            extrude around the `layer`
+        start_angle: optionally specify a custom starting angle if `None` will be
+            autocalculated from the first two elements
+        end_angle: optionally specify a custom ending angle if `None` will be
+            autocalculated from the last two elements
     """
-
     layer_list = {layer: LayerSection(sections=[Section(d_max=0)])}
     if enclosure is not None:
         if layer not in enclosure.layer_sections:
             layer_list.update(enclosure.layer_sections)
         else:
-            ls = layer_list[layer].sections.copy()
+            layer_list[layer].sections.copy()
             layer_list = enclosure.layer_sections.copy()
             for section in layer_list[layer].sections:
                 layer_list[layer].add_section(section)
     if is_callable_widths(widths):
         for layer, layer_sec in layer_list.items():
             reg = kdb.Region()
             for section in layer_sec.sections:
@@ -394,49 +360,24 @@
                             )
                         ).to_itype(target.klib.dbu)
                     )
                 reg.insert(_r)
             target.shapes(layer).insert(reg.merge())
 
 
-def path_pts_to_polygon(
-    pts_top: list[kdb.DPoint], pts_bot: list[kdb.DPoint]
-) -> kdb.DPolygon:
-    pts_bot.reverse()
-    return kdb.DPolygon(pts_top + pts_bot)
-
-
-def is_Region(r: object) -> TypeGuard[kdb.Region]:
-    return isinstance(r, kdb.Region)
-
-
-def is_int(r: object) -> TypeGuard[int]:
-    return isinstance(r, int)
-
-
-def is_callable(r: object) -> TypeGuard[Callable[[float], float]]:
-    return callable(r)
-
-
-class Direction(Enum):
-    X = 1
-    Y = 2
-    BOTH = 3
-
-
 class Section(BaseModel):
-    d_min: Optional[int] = None
+    d_min: int | None = None
     d_max: int
 
     def __hash__(self) -> int:
         return hash((self.d_min, self.d_max))
 
 
 class LayerSection(BaseModel):
-    sections: list[Section] = []
+    sections: list[Section] = Field(default=[])
 
     def add_section(self, sec: Section) -> None:
         if not self.sections:
             self.sections.append(sec)
         else:
             i = 0
             if sec.d_min is not None:
@@ -452,32 +393,32 @@
 
     def __hash__(self) -> int:
         return hash(tuple((s.d_min, s.d_max) for s in self.sections))
 
 
 class Enclosure(BaseModel):
     layer_sections: dict[LayerEnum | int, LayerSection]
-    _name: Optional[str] = PrivateAttr(default=None)
+    _name: str | None = PrivateAttr(default=None)
     warn: bool = True
 
-    main_layer: Optional[LayerEnum | int]
+    main_layer: LayerEnum | int | None
 
     yaml_tag: str = "!Enclosure"
 
     class Config:
         validate_assignment = True
 
     def __init__(
         self,
         sections: Sequence[
             tuple[LayerEnum | int, int] | tuple[LayerEnum | int, int, int]
         ] = [],
-        name: Optional[str] = None,
+        name: str | None = None,
         warn: bool = True,
-        main_layer: Optional[LayerEnum | int] = None,
+        main_layer: LayerEnum | int | None = None,
     ):
         super().__init__(
             warn=warn,
             layer_sections={},
             main_layer=main_layer,
         )
 
@@ -525,15 +466,15 @@
             d[layer] = LayerSection(sections=[sec])
 
         self.layer_sections = d  # trick pydantic to validate
 
     def minkowski_region(
         self,
         r: kdb.Region,
-        d: Optional[int],
+        d: int | None,
         shape: Callable[[int], list[kdb.Point] | kdb.Box | kdb.Edge | kdb.Polygon],
     ) -> kdb.Region:
         if d is None:
             return kdb.Region()
         elif d == 0:
             return r.dup()
         elif d > 0:
@@ -553,15 +494,15 @@
                 )
             bbox_r = kdb.Region(r.bbox().enlarged(bbox_maxsize))
             return r - (bbox_r - r).minkowski_sum(_shape)
 
     def apply_minkowski_enc(
         self,
         c: KCell,
-        ref: Optional[int | kdb.Region],  # layer index or the region
+        ref: int | kdb.Region | None,  # layer index or the region
         direction: Direction = Direction.BOTH,
     ) -> None:
         match direction:
             case Direction.BOTH:
 
                 def box(d: int) -> kdb.Box:
                     return kdb.Box(-d, -d, d, d)
@@ -581,27 +522,25 @@
                     return kdb.Edge(-d, 0, d, 0)
 
                 self.apply_minkowski_custom(c, ref=ref, shape=edge)
 
             case _:
                 raise ValueError("Undefined direction")
 
-    def apply_minkowski_y(
-        self, c: KCell, ref: Optional[int | kdb.Region] = None
-    ) -> None:
+    def apply_minkowski_y(self, c: KCell, ref: int | kdb.Region | None = None) -> None:
         return self.apply_minkowski_enc(c, ref=ref, direction=Direction.Y)
 
-    def apply_minkowski_x(self, c: KCell, ref: Optional[int | kdb.Region]) -> None:
+    def apply_minkowski_x(self, c: KCell, ref: int | kdb.Region | None) -> None:
         return self.apply_minkowski_enc(c, ref=ref, direction=Direction.X)
 
     def apply_minkowski_custom(
         self,
         c: KCell,
         shape: Callable[[int], kdb.Edge | kdb.Polygon | kdb.Box],
-        ref: Optional[int | kdb.Region] = None,
+        ref: int | kdb.Region | None = None,
     ) -> None:
         if ref is None:
             ref = self.main_layer
 
         if ref is None:
             raise ValueError(
                 "The enclosure doesn't have  a reference `main_layer` defined. Therefore the layer must be defined in calls"
@@ -616,28 +555,28 @@
                     - self.minkowski_region(r, section.d_min, shape)
                 )
 
     def apply_custom(
         self,
         c: KCell,
         shape: Callable[
-            [int, Optional[int]], kdb.Edge | kdb.Polygon | kdb.Box | kdb.Region
+            [int, int | None], kdb.Edge | kdb.Polygon | kdb.Box | kdb.Region
         ],
     ) -> None:
         for layer, layersec in self.layer_sections.items():
             for sec in layersec.sections:
                 c.shapes(layer).insert(shape(sec.d_max, sec.d_min))
 
     def apply_bbox(self, c: KCell, ref: int | kdb.Region) -> None:
         if is_int(ref):
             _ref = c.bbox_per_layer(ref)
         elif is_Region(ref):
             _ref = ref.bbox()
 
-        def bbox_reg(d_max: int, d_min: Optional[int] = None) -> kdb.Region:
+        def bbox_reg(d_max: int, d_min: int | None = None) -> kdb.Region:
             reg_max = kdb.Region(_ref)
             reg_max.size(d_max)
             if d_min is None:
                 return reg_max
             reg_min = kdb.Region(_ref)
             reg_min.size(d_min)
             return reg_max - reg_min
@@ -659,30 +598,52 @@
             list_to_hash.append([str(layer), str(layer_section.sections)])
         return sha1(str(list_to_hash).encode("UTF-8")).hexdigest()[-8:]
 
     def extrude_path(
         self,
         c: KCell,
         path: list[kdb.DPoint],
-        main_layer: Optional[int | LayerEnum],
+        main_layer: int | LayerEnum | None,
         width: float,
     ) -> None:
+        """Extrude a path and add it to a main layer.
+
+        Args:
+            c: The cell where to insert the path to
+            path: Backbone of the path. [um]
+            main_layer: Layer index where to put the main part of the path.
+            width: Width of the core of the path
+        """
         if main_layer is None:
             raise ValueError(
-                "The enclosure doesn't have  a reference `main_layer` defined. Therefore the layer must be defined in calls"
+                "The enclosure doesn't have  a reference `main_layer` defined."
+                " Therefore the layer must be defined in calls"
             )
         extrude_path(target=c, layer=main_layer, path=path, width=width, enclosure=self)
 
     def extrude_path_dynamic(
         self,
         c: KCell,
         path: list[kdb.DPoint],
-        main_layer: Optional[int | LayerEnum],
+        main_layer: int | LayerEnum | None,
         widths: Callable[[float], float] | list[float],
     ) -> None:
+        """Extrude a path and add it to a main layer.
+
+        Supports a dynamic width of the path defined by a function
+        returning the width for the interval [0,1], or as a list of
+        widths of the same lengths as the points.
+
+        Args:
+            c: The cell where to insert the path to
+            path: Backbone of the path. [um]
+            main_layer: Layer index where to put the main part of the path.
+            widths: Width of the core of the path
+        """
         if main_layer is None:
             raise ValueError(
-                "The enclosure doesn't have  a reference `main_layer` defined. Therefore the layer must be defined in calls"
+                "The enclosure doesn't have  a reference `main_layer` defined."
+                " Therefore the layer must be defined in calls"
             )
         extrude_path_dynamic(
             target=c, layer=main_layer, path=path, widths=widths, enclosure=self
         )
```

### Comparing `kfactory-0.5.8/src/kfactory/widgets/interactive.py` & `kfactory-0.6.0/src/kfactory/widgets/interactive.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 try:
     from pathlib import Path
-    from threading import Timer
-    from time import time
-    from typing import Any, Callable, Optional
+    from typing import Any
 
     import klayout.lay as lay
     from ipyevents import Event  # type: ignore[import]
-    from IPython.display import clear_output, display  # type: ignore[import]
+    from IPython.display import display  # type: ignore[import]
     from ipytree import Node, Tree  # type: ignore[import]
     from ipywidgets import (  # type: ignore[import]
-        HTML,
         Accordion,
         AppLayout,
         Box,
         Button,
         HBox,
         Image,
         Label,
@@ -23,15 +20,15 @@
         Tab,
         ToggleButtons,
         VBox,
     )
 
     from .. import kdb, lay
     from ..config import logger
-    from ..kcell import CplxKCell, KCell, KLib
+    from ..kcell import KCell
 
 except ImportError as e:
     print("You need install jupyter notebook plugin with `pip install kfactory[ipy]`")
     raise e
 
 
 def display_kcell(kc: KCell) -> None:
@@ -41,26 +38,26 @@
     lw = LayoutWidget(cell=cell_dup)
     display(lw.widget)
 
 
 class LayoutWidget:
     def __init__(
         self,
-        cell: KCell | CplxKCell,
-        layer_properties: Optional[str] = None,
+        cell: KCell,
+        layer_properties: str | None = None,
         hide_unused_layers: bool = True,
         with_layer_selector: bool = True,
     ):
         self.debug = Output()
 
         self.hide_unused_layers = hide_unused_layers
 
         self.layout_view = lay.LayoutView()
         self.layout_view.show_layout(cell.klib, False)
-        self.layer_properties: Optional[Path] = None
+        self.layer_properties: Path | None = None
         if layer_properties is not None:
             self.layer_properties = Path(layer_properties)
             if self.layer_properties.exists() and self.layer_properties.is_file():
                 self.layer_properties = self.layer_properties
                 self.layout_view.load_layer_props(str(self.layer_properties))
         self.show_cell(cell)
         png_data = self.layout_view.get_screenshot_pixels().to_png_data()
@@ -133,21 +130,19 @@
             if props == button.layer_props:
                 props.visible = not props.visible
                 props.name = button.name
                 button.layer_props = props
                 break
         self.refresh()
 
-    def build_layer_toggle(
-        self, prop_iter: lay.LayerPropertiesIterator
-    ) -> Optional[HBox]:
+    def build_layer_toggle(self, prop_iter: lay.LayerPropertiesIterator) -> HBox | None:
         props = prop_iter.current()
         layer_color = f"#{props.eff_fill_color():06x}"
         # Would be nice to use LayoutView.icon_for_layer() rather than simple colored box
-        button_layout = Layout(
+        Layout(
             width="5px",
             height="20px",
             border=f"solid 2px {layer_color}",
             display="block",
         )
 
         # prop_iter.current().visible = False
@@ -244,15 +239,14 @@
 
     def build_selector(self, max_height: float) -> Tab:
         """Builds a widget for toggling layer displays.
 
         Args:
             max_height: Maximum height to set for the widget (likely the height of the pixel buffer).
         """
-
         all_boxes = []
 
         prop_iter = self.layout_view.begin_layers()
         while not prop_iter.at_end():
             if layer_toggle := self.build_layer_toggle(prop_iter):
                 all_boxes.append(layer_toggle)
             prop_iter.next()
@@ -272,15 +266,15 @@
         selector_tabs = Tab([selector, tree])
         selector_tabs.set_title(0, "Layers")
         selector_tabs.set_title(1, "Cells")
         # selector_tabs.titles = ("Layers",)
 
         return selector_tabs
 
-    def load_layout(self, filepath: str, layer_properties: Optional[str]) -> None:
+    def load_layout(self, filepath: str, layer_properties: str | None) -> None:
         """Loads a GDS layout.
 
         Args:
             filepath: path for the GDS layout.
             layer_properties: Optional path for the layer_properties klayout file (lyp).
         """
         self.layout_view.load_layout(filepath)
@@ -320,15 +314,15 @@
         return buttons
 
     def on_select_cell(self, event: Event) -> None:
         self.show_cell(
             self.layout_view.active_cellview().layout().cell(event["owner"].name)
         )
 
-        max_height = self.layout_view.viewport_height()
+        self.layout_view.viewport_height()
 
         all_boxes = []
         prop_iter = self.layout_view.begin_layers()
         while not prop_iter.at_end():
             if layer_toggle := self.build_layer_toggle(prop_iter):
                 all_boxes.append(layer_toggle)
             prop_iter.next()
@@ -347,30 +341,32 @@
         self.layout_view.send_wheel_event(-delta, False, kdb.DPoint(x, y), buttons)
         self.refresh()
 
     def on_mouse(self, event: Event) -> None:
         self.layout_view.timer()  # type: ignore[attr-defined]
         x = event["relativeX"]
         y = event["relativeY"]
-        moved_x = event["movementX"]
-        moved_y = event["movementY"]
         buttons = self._get_modifier_buttons(event)
 
-        if event["event"] == "mousedown":
-            self.layout_view.send_mouse_press_event(
-                kdb.DPoint(float(x), float(y)), buttons
-            )
-        elif event["event"] == "mouseup":
-            self.layout_view.send_mouse_release_event(
-                kdb.DPoint(float(x), float(y)), buttons
-            )
-        elif event["event"] == "mousemove":
-            self.layout_view.send_mouse_move_event(
-                kdb.DPoint(float(x), float(y)), buttons
-            )
+        match event["event"]:
+            case "mousedown":
+                # if event["event"] == "mousedown":
+                self.layout_view.send_mouse_press_event(
+                    kdb.DPoint(float(x), float(y)), buttons
+                )
+            # elif event["event"] == "mouseup":
+            case "mouseup":
+                self.layout_view.send_mouse_release_event(
+                    kdb.DPoint(float(x), float(y)), buttons
+                )
+            # elif event["event"] == "mousemove":
+            case "mousemove":
+                self.layout_view.send_mouse_move_event(
+                    kdb.DPoint(float(x), float(y)), buttons
+                )
         self.refresh()
         self.layout_view.timer()  # type: ignore[attr-defined]
 
     def on_mouse_enter(self, event: Event) -> None:
         self.layout_view.timer()  # type: ignore[attr-defined]
         self.layout_view.send_enter_event()
         self.refresh()
```

### Comparing `kfactory-0.5.8/src/kfactory.egg-info/PKG-INFO` & `kfactory-0.6.0/src/kfactory.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kfactory
-Version: 0.5.8
+Version: 0.6.0
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
 
-# KFactory 0.5.8
+# KFactory 0.6.0
 
 Kfactory is a [gdsfactory](https://github.com/gdsfactory/gdsfactory)-like tool. It is built with [KLayout](https://klayout.de) as a backend instead of gdstk, but aims to offer the similar featuers.
 
 Features similar to gdsfactory:
 
 - [x] Cells & decorator for caching & storing cells
 - [x] Simple routing (point to point and simpl bundle routes for electrical routes)
```

### Comparing `kfactory-0.5.8/tests/conftest.py` & `kfactory-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/tests/test_cplxcells.py` & `kfactory-0.6.0/tests/test_cplxcells.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,49 +1,44 @@
 import kfactory as kf
-import pytest
-import warnings
-from random import randint
-
-from typing import Callable
 
 
 @kf.autocell
 def simple_cplx_cell(layer: kf.LayerEnum) -> kf.KCell:
-    c = kf.CplxKCell()
+    c = kf.KCell()
 
     hh = 2.5
 
     dct = kf.kdb.DCplxTrans(1, 30, False, 2.5, 2.5)
     dbox = kf.kdb.DPolygon(kf.kdb.DBox(0, -hh, 10, hh)).transformed(dct)
 
-    p1 = kf.DCplxPort(
-        width=hh * 2,
+    p1 = kf.Port(
+        dwidth=hh * 2,
         layer=layer,
         name="o1",
-        trans=dct * kf.kdb.DCplxTrans.R180,
+        dcplx_trans=dct * kf.kdb.DCplxTrans.R180,
     )
-    p2 = kf.DCplxPort(
-        width=hh * 2,
+    p2 = kf.Port(
+        dwidth=hh * 2,
         layer=layer,
         name="o2",
-        trans=dct * kf.kdb.DCplxTrans(kf.kdb.DVector(10, 0)),
+        dcplx_trans=dct * kf.kdb.DCplxTrans(kf.kdb.DVector(10, 0)),
     )
 
     c.add_port(p1)
     c.add_port(p2)
 
     c.shapes(layer).insert(dbox)
 
     c.draw_ports()
     return c
 
 
 def test_cell(LAYER: kf.LayerEnum):
-    c = simple_cplx_cell(LAYER.WG)
+    simple_cplx_cell(LAYER.WG)
 
 
 def test_connected_cell(LAYER: kf.LayerEnum):
-    c = kf.CplxKCell()
+    c = kf.KCell()
     layer = LAYER.WG
     sckc1 = c << simple_cplx_cell(layer)
     sckc2 = c << simple_cplx_cell(layer)
-    sckc2.connect("o1", sckc1, "o1")
+    sckc2.align("o1", sckc1, "o1")
```

### Comparing `kfactory-0.5.8/tests/test_enclosure.py` & `kfactory-0.6.0/tests/test_enclosure.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,47 +27,42 @@
 
     enclosure.apply_minkowski_enc(c, layer)
 
     return c
 
 
 def test_enclosure(LAYER):
-
     enc = kf.utils.Enclosure([(LAYER.WG, 500, -250)])
 
 
 def test_enc(LAYER, wg_enc):
-
     enc = wg_enc
 
     mmi_enc(LAYER.WG, wg_enc)
 
 
 def test_neg_enc(LAYER):
-
     enc = kf.utils.Enclosure([(LAYER.WGCLAD, -1500, 1000)])
 
     mmi_enc(LAYER.WG, enc)
 
 
 def test_layer_multi_enc(LAYER):
-
     enc = kf.utils.Enclosure(
         [
             (LAYER.WGCLAD, -5000, -5400),
             (LAYER.WGCLAD, -4000, -3900),
             (LAYER.WGCLAD, -100, 100),
             (LAYER.WGCLAD, -500, -400),
         ]
     )
     mmi_enc(LAYER.WG, enc)
 
 
 def test_layer_merge_enc(LAYER):
-
     enc = kf.utils.Enclosure(
         [
             (LAYER.WGCLAD, -5000, -3000),
             (LAYER.WGCLAD, -4000, -2000),
             (LAYER.WGCLAD, -2000, 1000),
         ]
     )
```

### Comparing `kfactory-0.5.8/tests/test_extrude.py` & `kfactory-0.6.0/tests/test_extrude.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/tests/test_ports.py` & `kfactory-0.6.0/tests/test_ports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import kfactory as kf
 import pytest
-import warnings
 import re
 
 
 @kf.autocell
 def waveguide(width: int, length: int, layer: int) -> kf.KCell:
     c = kf.KCell()
 
@@ -23,36 +22,36 @@
 def wg(LAYER):
     return waveguide(1000, 20000, LAYER.WG)
 
 
 @pytest.fixture()
 @kf.autocell
 def wg_floating_off_grid(LAYER):
-    c = kf.KCell()
-    dbu = c.klib.dbu
-
-    p1 = kf.kcell.DPort(
-        width=10 + dbu / 2,
-        name="o1",
-        trans=kf.kdb.DTrans(2, False, dbu / 2, 0),
-        layer=LAYER.WG,
-    )
-    p2 = kf.kcell.DPort(
-        width=10 + dbu / 2,
-        name="o2",
-        trans=kf.kdb.DTrans(0, False, 20 + dbu, 0),
-        layer=LAYER.WG,
-    )
-    c.shapes(LAYER.WG).insert(kf.kdb.DBox(p1.x, -p1.width / 2, p2.x, p1.width / 2))
+    with pytest.raises(AssertionError):
+        c = kf.KCell()
+        dbu = c.klib.dbu
+
+        p1 = kf.kcell.Port(
+            dwidth=10 + dbu / 2,
+            name="o1",
+            dcplx_trans=kf.kdb.DCplxTrans(1, 180, False, dbu / 2, 0),
+            layer=LAYER.WG,
+        )
+        p2 = kf.kcell.Port(
+            dwidth=10 + dbu / 2,
+            name="o2",
+            dcplx_trans=kf.kdb.DCplxTrans(1, 0, False, 20 + dbu, 0),
+            layer=LAYER.WG,
+        )
+        c.shapes(LAYER.WG).insert(kf.kdb.DBox(p1.x, -p1.width / 2, p2.x, p1.width / 2))
 
-    kf.config.filter.regex = f"Port ({re.escape(str(p1))}|{re.escape(str(p2))}) is not an integer based port, converting to integer based"
-    c.add_port(p1)
-    c.add_port(p2)
+        c.add_port(p1)
+        c.add_port(p2)
 
-    kf.config.filter.regex = None
+        kf.config.filter.regex = None
 
     return c
 
 
 def test_waveguide(LAYER):
     waveguide(1000, 20000, LAYER.WG)
 
@@ -64,52 +63,52 @@
     assert c.settings["width"] == 1000
     assert c.name == "waveguide_W1000_L20000_LWG"
 
 
 def test_connect_cplx_port(LAYER):
     c = kf.KCell()
     wg1 = c << waveguide(1000, 20000, LAYER.WG)
-    port = kf.kcell.DCplxPort(
-        width=1000,
+    port = kf.kcell.Port(
+        dwidth=1,
         layer=LAYER.WG,
         name="cplxp1",
-        trans=kf.kdb.DCplxTrans(1, 30, False, 5, 10),
+        dcplx_trans=kf.kdb.DCplxTrans(1, 30, False, 5, 10),
     )
-    wg1.connect_cplx("o1", port)
+    wg1.align("o1", port)
 
 
 def test_connect_cplx_inst(LAYER):
     c = kf.KCell()
 
     wg1 = c << waveguide(1000, 20000, LAYER.WG)
     wg2 = c << waveguide(1000, 20000, LAYER.WG)
     wg1.transform(kf.kdb.DCplxTrans(1, 30, False, 5, 10))
-    wg2.connect_cplx("o1", wg1, "o2")
+    wg2.align("o1", wg1, "o2")
     kf.config.filter.regex = f"Port ({re.escape(str(wg1.ports['o1']))}|{re.escape(str(wg2.ports['o2']))}) is not an integer based port, converting to integer based"
 
     c.add_port(wg1.ports["o1"])
     c.add_port(wg2.ports["o2"])
 
     kf.config.filter.regex = None
     c.flatten()
 
 
-def test_floating(wg_floating_off_grid):
-    c = kf.KCell()
+# def test_floating(wg_floating_off_grid):
+#     c = kf.KCell()
 
-    wg1 = c << wg_floating_off_grid
-    wg2 = c << wg_floating_off_grid
-    wg2.connect("o2", wg1, "o1")
+#     wg1 = c << wg_floating_off_grid
+#     wg2 = c << wg_floating_off_grid
+#     wg2.align("o2", wg1, "o1")
 
 
 def test_connect_integer(wg):
     c = kf.KCell()
 
     wg1 = c << wg
     wg2 = c << wg
-    wg2.connect("o1", wg2, "o1")
+    wg2.align("o1", wg1, "o1")
 
     assert wg2.ports["o1"].trans == kf.kdb.Trans(0, False, 0, 0)
 
 
 # if __name__ == "__main__":
 #     test_waveguide()
```

### Comparing `kfactory-0.5.8/tests/test_rename.py` & `kfactory-0.6.0/tests/test_rename.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/tests/test_routing.py` & `kfactory-0.6.0/tests/test_routing.py`

 * *Files identical despite different names*

### Comparing `kfactory-0.5.8/tests/test_spiral.py` & `kfactory-0.6.0/tests/test_spiral.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,33 +88,34 @@
             [np.sin(_theta / 180 * np.pi) * r, (-np.cos(_theta / 180 * np.pi) + 1) * r]
             for _theta in np.linspace(
                 0, theta, int(theta // theta_step + 0.5), endpoint=True
             )
         ]
     ]
     kf.utils.geo.extrude_path(c, layer, backbone, width, enclosure, 0, theta)
-    dp1 = kf.kcell.DPort(width=width, layer=layer, name="W0", trans=kf.kdb.DTrans.R180)
+    dp1 = kf.kcell.Port(
+        dwidth=width, layer=layer, name="W0", dcplx_trans=kf.kdb.DCplxTrans.R180
+    )
     warnings.filterwarnings("ignore")
     c.add_port(dp1)
 
     match theta:
         case 90:
-
-            dp2 = kf.DPort(
+            dp2 = kf.Port(
                 name="N0",
                 layer=layer,
-                width=width,
-                trans=kf.kdb.DTrans(1, False, radius, radius),
+                dwidth=width,
+                dcplx_trans=kf.kdb.DCplxTrans(1, 90, False, radius, radius),
             )
         case 180:
-            dp2 = kf.DPort(
+            dp2 = kf.Port(
                 name="N0",
                 layer=layer,
-                width=width,
-                trans=kf.kdb.DTrans(0, False, 0, 2 * radius),
+                dwidth=width,
+                dcplx_trans=kf.kdb.DTrans(1, 0, False, 0, 2 * radius),
             )
         case _:
             raise ValueError("only support 90/180° bends")
     c.add_port(dp2)
     warnings.filterwarnings("default")
     return c
 
@@ -128,30 +129,32 @@
     p = kf.Port(name="start", trans=kf.kdb.Trans.R0, width=1000, layer=LAYER.WG)
 
     for _ in range(10):
         r = r1 + r2
         r2 = r1
         r1 = r
         b = c << bend_circular(width=1000, radius=r2, layer=LAYER.WG)
-        b.connect("W0", p)
+        b.align("W0", p)
         p = b.ports["N0"]
 
 
 def test_dspiral(LAYER):
     c = kf.KCell()
 
     r1 = 1
     r2 = 0
 
-    p = kf.DPort(name="start", trans=kf.kdb.DTrans.R0, width=1, layer=LAYER.WG)
+    p = kf.Port(
+        name="start", dcplx_trans=kf.kdb.DCplxTrans.R0, dwidth=1, layer=LAYER.WG
+    )
 
     kf.config.filter.level = "ERROR"
 
     for _ in range(10):
         r = r1 + r2
         r2 = r1
         r1 = r
         b = c << dbend_circular(width=1, radius=r2, layer=LAYER.WG)
-        b.connect_cplx("W0", p)
+        b.align("W0", p)
         p = b.ports["N0"]
 
     kf.config.filter.level = "DEBUG"
```

