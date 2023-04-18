# Comparing `tmp/xemc3-0.2.2.tar.gz` & `tmp/xemc3-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xemc3-0.2.2.tar", last modified: Fri Oct 28 09:42:02 2022, max compression
+gzip compressed data, was "xemc3-0.2.3.tar", last modified: Tue Apr 18 07:17:53 2023, max compression
```

## Comparing `xemc3-0.2.2.tar` & `xemc3-0.2.3.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.176960 xemc3-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (121)      144 2022-10-28 09:41:48.000000 xemc3-0.2.2/.codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.156960 xemc3-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.164960 xemc3-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      701 2022-10-28 09:41:48.000000 xemc3-0.2.2/.github/workflows/black-fix.yml
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-10-28 09:41:48.000000 xemc3-0.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-10-28 09:41:48.000000 xemc3-0.2.2/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (121)      658 2022-10-28 09:41:48.000000 xemc3-0.2.2/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2797 2022-10-28 09:41:48.000000 xemc3-0.2.2/.github/workflows/test-python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      347 2022-10-28 09:41:48.000000 xemc3-0.2.2/.github/workflows/zenodo.yml
--rw-r--r--   0 runner    (1001) docker     (121)      460 2022-10-28 09:41:48.000000 xemc3-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-10-28 09:41:48.000000 xemc3-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)      259 2022-10-28 09:41:48.000000 xemc3-0.2.2/.zenodo.json
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-10-28 09:41:48.000000 xemc3-0.2.2/COPYING
--rw-r--r--   0 runner    (1001) docker     (121)     1337 2022-10-28 09:41:48.000000 xemc3-0.2.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-28 09:42:02.176960 xemc3-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      974 2022-10-28 09:41:48.000000 xemc3-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.164960 xemc3-0.2.2/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/citing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      447 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)      649 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/cli.rst.in.py
--rw-r--r--   0 runner    (1001) docker     (121)     5932 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.168960 xemc3-0.2.2/docs/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     7270 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/evaluate_at.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/get_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     3901 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/heatflux.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     3697 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/info.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)    12317 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1281 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/load1.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/load2.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples/setup_plt.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/examples.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.168960 xemc3-0.2.2/docs/exercises/
--rw-r--r--   0 runner    (1001) docker     (121)     1275 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/exercises/get_data.py
--rw-r--r--   0 runner    (1001) docker     (121)     8773 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/exercises/introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (121)     1220 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3525 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/xarray.rst
--rw-r--r--   0 runner    (1001) docker     (121)      596 2022-10-28 09:41:48.000000 xemc3-0.2.2/docs/xemc3.rst
--rw-r--r--   0 runner    (1001) docker     (121)       84 2022-10-28 09:41:48.000000 xemc3-0.2.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-10-28 09:41:48.000000 xemc3-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      523 2022-10-28 09:41:48.000000 xemc3-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2102 2022-10-28 09:42:02.180960 xemc3-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-10-28 09:41:48.000000 xemc3-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.168960 xemc3-0.2.2/xemc3/
--rw-r--r--   0 runner    (1001) docker     (121)      881 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-28 09:42:01.000000 xemc3-0.2.2/xemc3/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.172960 xemc3-0.2.2/xemc3/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1495 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/cli/_common.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1465 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/cli/append_time.py
--rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/cli/to_archive.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      887 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/cli/to_netcdf.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3698 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/cli/xdivertor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.172960 xemc3-0.2.2/xemc3/core/
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20081 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)    10779 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/depo.py
--rw-r--r--   0 runner    (1001) docker     (121)     4847 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/evaluate_at.py
--rw-r--r--   0 runner    (1001) docker     (121)    63885 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/load.py
--rw-r--r--   0 runner    (1001) docker     (121)     3550 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/plot_2d.py
--rw-r--r--   0 runner    (1001) docker     (121)    10401 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/plot_3d.py
--rw-r--r--   0 runner    (1001) docker     (121)     6485 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.172960 xemc3-0.2.2/xemc3/load/
--rw-r--r--   0 runner    (1001) docker     (121)      740 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/load/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.176960 xemc3-0.2.2/xemc3/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9211 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/gen_ds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_average.py
--rw-r--r--   0 runner    (1001) docker     (121)       43 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)    15461 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_load_real.py
--rw-r--r--   0 runner    (1001) docker     (121)     1874 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     4413 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/test/test_write_load.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.176960 xemc3-0.2.2/xemc3/tools/
--rw-r--r--   0 runner    (1001) docker     (121)     9653 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/tools/run_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.176960 xemc3-0.2.2/xemc3/write/
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      682 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/write/fortran.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-28 09:41:48.000000 xemc3-0.2.2/xemc3/write/nc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-28 09:42:02.168960 xemc3-0.2.2/xemc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2123 2022-10-28 09:42:02.000000 xemc3-0.2.2/xemc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1639 2022-10-28 09:42:02.000000 xemc3-0.2.2/xemc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-28 09:42:02.000000 xemc3-0.2.2/xemc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-10-28 09:42:02.000000 xemc3-0.2.2/xemc3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-28 09:42:02.000000 xemc3-0.2.2/xemc3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-10-28 09:42:02.000000 xemc3-0.2.2/xemc3.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-04-18 07:17:39.000000 xemc3-0.2.3/.codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.167501 xemc3-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/black-fix.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/test-python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-18 07:17:39.000000 xemc3-0.2.3/.github/workflows/zenodo.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 07:17:39.000000 xemc3-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-04-18 07:17:39.000000 xemc3-0.2.3/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-18 07:17:39.000000 xemc3-0.2.3/.zenodo.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-18 07:17:39.000000 xemc3-0.2.3/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)     1337 2023-04-18 07:17:39.000000 xemc3-0.2.3/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-18 07:17:53.175501 xemc3-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-04-18 07:17:39.000000 xemc3-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/citing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/cli.rst.in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/docs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     7270 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/evaluate_at.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3901 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/heatflux.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/info.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    12317 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/load1.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/load2.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples/setup_plt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/examples.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/docs/exercises/
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/exercises/get_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8773 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/exercises/introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/xarray.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-18 07:17:39.000000 xemc3-0.2.3/docs/xemc3.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-18 07:17:39.000000 xemc3-0.2.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-18 07:17:39.000000 xemc3-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-18 07:17:39.000000 xemc3-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-04-18 07:17:53.175501 xemc3-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 07:17:39.000000 xemc3-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/xemc3/
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 07:17:52.000000 xemc3-0.2.3/xemc3/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/xemc3/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1465 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/append_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/to_archive.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      887 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/to_netcdf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3698 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/cli/xdivertor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/depo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/evaluate_at.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63885 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/plot_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/plot_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6485 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/load/
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/load/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9211 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/gen_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_average.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15461 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_load_real.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/test/test_write_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/tools/run_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.175501 xemc3-0.2.3/xemc3/write/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/write/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:39.000000 xemc3-0.2.3/xemc3/write/nc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:17:53.171501 xemc3-0.2.3/xemc3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 07:17:53.000000 xemc3-0.2.3/xemc3.egg-info/top_level.txt
```

### Comparing `xemc3-0.2.2/.github/workflows/black-fix.yml` & `xemc3-0.2.3/.github/workflows/black-fix.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/.github/workflows/coverage.yml` & `xemc3-0.2.3/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/.github/workflows/python_publish.yml` & `xemc3-0.2.3/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/.github/workflows/test-python-package.yml` & `xemc3-0.2.3/.github/workflows/test-python-package.yml`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/COPYING` & `xemc3-0.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/Makefile` & `xemc3-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/PKG-INFO` & `xemc3-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.2/README.md` & `xemc3-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/cli.rst.in.py` & `xemc3-0.2.3/docs/cli.rst.in.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/conf.py` & `xemc3-0.2.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/evaluate_at.ipynb` & `xemc3-0.2.3/docs/examples/evaluate_at.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/get_data.py` & `xemc3-0.2.3/docs/examples/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/heatflux.ipynb` & `xemc3-0.2.3/docs/examples/heatflux.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/info.ipynb` & `xemc3-0.2.3/docs/examples/info.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/introduction.ipynb` & `xemc3-0.2.3/docs/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/load1.ipynb` & `xemc3-0.2.3/docs/examples/load1.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/examples/load2.ipynb` & `xemc3-0.2.3/docs/examples/load2.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/exercises/get_data.py` & `xemc3-0.2.3/docs/exercises/get_data.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/exercises/introduction.ipynb` & `xemc3-0.2.3/docs/exercises/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/index.rst` & `xemc3-0.2.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/introduction.rst` & `xemc3-0.2.3/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/xarray.rst` & `xemc3-0.2.3/docs/xarray.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/docs/xemc3.rst` & `xemc3-0.2.3/docs/xemc3.rst`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/requirements.txt` & `xemc3-0.2.3/requirements.txt`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/setup.cfg` & `xemc3-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/__init__.py` & `xemc3-0.2.3/xemc3/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/cli/_common.py` & `xemc3-0.2.3/xemc3/cli/_common.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/cli/append_time.py` & `xemc3-0.2.3/xemc3/cli/append_time.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/cli/to_archive.py` & `xemc3-0.2.3/xemc3/cli/to_archive.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/cli/to_netcdf.py` & `xemc3-0.2.3/xemc3/cli/to_netcdf.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/cli/xdivertor.py` & `xemc3-0.2.3/xemc3/cli/xdivertor.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/core/dataset.py` & `xemc3-0.2.3/xemc3/core/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             The data to be set. See the xarray documentation for what
             is accepted.
         """
         return self._set(var, data)
 
     def _get_alt_name(self, var_name, suffix=""):
         var_suffix = ["_bounds", "", "_plus1"]
-        var_prefix = ["", "_plate_", "plate_"]
+        var_prefix = ["plate_", "_plate_", ""]
         for extra_suffix in var_suffix:
             for prefix in var_prefix:
                 cur = prefix + var_name + extra_suffix + suffix
                 if cur in self.data:
                     return cur
         assert False, f"Didn't find variable for {var_name} coordinate!"
```

### Comparing `xemc3-0.2.2/xemc3/core/depo.py` & `xemc3-0.2.3/xemc3/core/depo.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/core/evaluate_at.py` & `xemc3-0.2.3/xemc3/core/evaluate_at.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/core/load.py` & `xemc3-0.2.3/xemc3/core/load.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/core/plot_2d.py` & `xemc3-0.2.3/xemc3/core/plot_2d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/core/plot_3d.py` & `xemc3-0.2.3/xemc3/core/plot_3d.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/core/utils.py` & `xemc3-0.2.3/xemc3/core/utils.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/load/__init__.py` & `xemc3-0.2.3/xemc3/load/__init__.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/gen_ds.py` & `xemc3-0.2.3/xemc3/test/gen_ds.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/test_average.py` & `xemc3-0.2.3/xemc3/test/test_average.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/test_cli.py` & `xemc3-0.2.3/xemc3/test/test_cli.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/test_dataset.py` & `xemc3-0.2.3/xemc3/test/test_dataset.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/test_load_real.py` & `xemc3-0.2.3/xemc3/test/test_load_real.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/test_utils.py` & `xemc3-0.2.3/xemc3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/test/test_write_load.py` & `xemc3-0.2.3/xemc3/test/test_write_load.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/tools/run_wrapper.py` & `xemc3-0.2.3/xemc3/tools/run_wrapper.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3/write/fortran.py` & `xemc3-0.2.3/xemc3/write/fortran.py`

 * *Files identical despite different names*

### Comparing `xemc3-0.2.2/xemc3.egg-info/PKG-INFO` & `xemc3-0.2.3/xemc3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xemc3
-Version: 0.2.2
+Version: 0.2.3
 Summary: Collect data from EMC3 runs in python using xarray
 Home-page: https://github.com/dschwoerer/xemc3
 Author: David Bold
 Author-email: dave@ipp.mpg.de
 License: GPL
 Project-URL: Tracker, https://github.com/dschwoerer/xemc3/issues
 Project-URL: Documentation, https://xemc3.rtfd.io
```

### Comparing `xemc3-0.2.2/xemc3.egg-info/SOURCES.txt` & `xemc3-0.2.3/xemc3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

