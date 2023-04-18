# Comparing `tmp/geo-espresso-0.2.2.dev0.tar.gz` & `tmp/geo-espresso-0.2.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geo-espresso-0.2.2.dev0.tar", last modified: Thu Apr 13 00:25:58 2023, max compression
+gzip compressed data, was "geo-espresso-0.2.2.dev1.tar", last modified: Tue Apr 18 04:23:21 2023, max compression
```

## Comparing `geo-espresso-0.2.2.dev0.tar` & `geo-espresso-0.2.2.dev1.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.059305 geo-espresso-0.2.2.dev0/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3526 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-13 00:25:58.059305 geo-espresso-0.2.2.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.023305 geo-espresso-0.2.2.dev0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.023305 geo-espresso-0.2.2.dev0/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.023305 geo-espresso-0.2.2.dev0/docs/source/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_ext/generate_contrib_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.023305 geo-espresso-0.2.2.dev0/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/contrib_edit1.png
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork.png
--rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork2.png
--rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork3.png
--rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork4.png
--rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/contrib_pr1.png
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/espresso_arch.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/inlab_logo_60px.png
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.023305 geo-espresso-0.2.2.dev0/docs/source/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.023305 geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/exception.rst
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/function.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (123)     5033 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.027305 geo-espresso-0.2.2.dev0/docs/source/contributor_guide/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/contributor_guide/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/contributor_guide/github.rst
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/contributor_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13396 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/contributor_guide/new_contrib.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6476 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/contributor_guide/setup.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.027305 geo-espresso-0.2.2.dev0/docs/source/developer_guide/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/build.rst
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/deploy.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/develop.rst
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/licence.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/repository.rst
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/developer_guide/sphinx.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.027305 geo-espresso-0.2.2.dev0/docs/source/user_guide/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.027305 geo-espresso-0.2.2.dev0/docs/source/user_guide/api/
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/api/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.027305 geo-espresso-0.2.2.dev0/docs/source/user_guide/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/contrib/_index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2809 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5403 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/docs/source/user_guide/why.rst
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 00:25:58.059305 geo-espresso-0.2.2.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5145 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.019305 geo-espresso-0.2.2.dev0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.031305 geo-espresso-0.2.2.dev0/src/espresso/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_espresso_problem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.031305 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.031305 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.031305 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/
--rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat
--rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat
--rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
--rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/fmst/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/fmst/compile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/fmst/src/
--rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/waveTracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/_gravity_density.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/data/gravmodel1.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/metadata.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_machine/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/check_requires.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/criteria.py
--rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/report.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/run_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_machine/doc_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/doc_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/doc_utils/gen_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.035305 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.039305 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     5362 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.039305 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/data/testdata.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/example_name.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/create_new_contrib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.039305 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     4385 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.039305 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.043305 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/
--rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.py
--rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.py
--rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.043305 geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/_pumping_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.043305 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     8122 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RF.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.047305 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/
--rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/dpythag.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     5500 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/dsvdcmp.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/four1.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/priorvalue.f90
--rwxr-xr-x   0 runner    (1001) docker     (123)    13138 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/qlayer.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/ran3.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/rfi_param.inc
--rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/svbksb.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/theo.f
--rwxr-xr-x   0 runner    (1001) docker     (123)     4197 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/theo_noise.f
--rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/whichcell.f90
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7793 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/_receiver_function.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8649 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/rf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.047305 geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/_simple_regression.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.051305 geo-espresso-0.2.2.dev0/src/espresso/_slug_test/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_slug_test/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_slug_test/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_slug_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_slug_test/_slug_test.py
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-13 00:25:57.000000 geo-espresso-0.2.2.dev0/src/espresso/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.051305 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/_xray_tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.055305 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/csiro_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/example1.dat
--rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/example2.dat
--rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/example3.dat
--rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/inlab_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/list_problems.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.055305 geo-espresso-0.2.2.dev0/src/espresso/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/utils/data_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/utils/file_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-13 00:25:38.000000 geo-espresso-0.2.2.dev0/src/espresso/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 00:25:58.055305 geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5337 2023-04-13 00:25:57.000000 geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6919 2023-04-13 00:25:58.000000 geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 00:25:57.000000 geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-13 00:25:57.000000 geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-13 00:25:57.000000 geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.668932 geo-espresso-0.2.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/source/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_ext/generate_contrib_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    16996 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/contrib_edit1.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork.png
+-rw-r--r--   0 runner    (1001) docker     (123)    82278 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork2.png
+-rw-r--r--   0 runner    (1001) docker     (123)    22274 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork3.png
+-rw-r--r--   0 runner    (1001) docker     (123)    35166 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36057 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/contrib_pr1.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/espresso_arch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4783 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/inlab_logo_60px.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/source/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/exception.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/function.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5477 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.648932 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/github.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10779 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/new_contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/setup.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/submit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/contributor_guide/video.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/docs/source/developer_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    96856 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/build.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/ci.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/deploy.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/develop.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/licence.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/developer_guide/repository.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4586 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/docs/source/user_guide/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/docs/source/user_guide/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/api/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/changelog.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/docs/source/user_guide/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/contrib/_index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6336 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/docs/source/user_guide/why.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 04:23:21.668932 geo-espresso-0.2.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4830 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.644932 geo-espresso-0.2.2.dev1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/src/espresso/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11486 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_espresso_problem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10364 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.652932 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)    38400 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/
+-rw-r--r--   0 runner    (1001) docker     (123)     2700 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    37500 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat
+-rw-r--r--   0 runner    (1001) docker     (123)  1350000 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat
+-rw-r--r--   0 runner    (1001) docker     (123)     7500 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/fmst/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1115 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/fmst/compile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/fmst/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    57221 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/waveTracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21254 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/_gravity_density.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/data/gravmodel1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/metadata.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.644932 geo-espresso-0.2.2.dev1/src/espresso/_machine/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/check_requires.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/criteria.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15212 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/run_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_machine/doc_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/doc_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4482 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/doc_utils/gen_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.656932 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/data/testdata.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/example_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/create_new_contrib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.660932 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11984 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.660932 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7052 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.660932 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)   125288 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101422 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2101 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146169 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.660932 geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14893 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/_pumping_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.660932 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/
+-rw-r--r--   0 runner    (1001) docker     (123)     3025 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8122 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RF.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.660932 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      442 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/dpythag.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5500 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/dsvdcmp.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/four1.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      326 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/priorvalue.f90
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13138 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/qlayer.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1514 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/ran3.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      343 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/rfi_param.inc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      619 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/svbksb.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4110 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/theo.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4197 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/theo_noise.f
+-rwxr-xr-x   0 runner    (1001) docker     (123)      963 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/whichcell.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7286 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/_receiver_function.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8649 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/rf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12826 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/_simple_regression.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/src/espresso/_slug_test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_slug_test/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_slug_test/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_slug_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9990 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_slug_test/_slug_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 04:23:21.000000 geo-espresso-0.2.2.dev1/src/espresso/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11218 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/_xray_tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55535 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/csiro_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)   510434 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/example1.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   166740 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/example2.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   233604 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/example3.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   312372 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/inlab_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/list_problems.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/src/espresso/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/utils/data_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/utils/file_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-18 04:23:02.000000 geo-espresso-0.2.2.dev1/src/espresso/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 04:23:21.664932 geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5434 2023-04-18 04:23:21.000000 geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-18 04:23:21.000000 geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 04:23:21.000000 geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-18 04:23:21.000000 geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 04:23:21.000000 geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/top_level.txt
```

### Comparing `geo-espresso-0.2.2.dev0/.gitignore` & `geo-espresso-0.2.2.dev1/.gitignore`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/CHANGELOG.md` & `geo-espresso-0.2.2.dev1/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Change Log
 
+## v0.2.2.dev1 (18/04/2023)
+
+### Changed examples
+
+- Fix installation of receiver function under SKBUILD
+
 ## v0.2.2.dev0 (13/04/2023)
 
 ### New examples
 
 - [#106](https://github.com/inlab-geo/espresso/pull/106) Receiver function
 
 ### Changed examples
```

### Comparing `geo-espresso-0.2.2.dev0/LICENCE` & `geo-espresso-0.2.2.dev1/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/PKG-INFO` & `geo-espresso-0.2.2.dev1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.2.2.dev0
+Version: 0.2.2.dev1
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: doc
 License-File: LICENCE
 
 # Espresso
 
 [![PyPI version](https://img.shields.io/pypi/v/geo-espresso?logo=pypi&style=flat-square&color=bde0fe&labelColor=f8f9fa)](https://pypi.org/project/geo-espresso/)
 [![build](https://img.shields.io/github/actions/workflow/status/inlab-geo/espresso/build_wheels.yml?branch=main&logo=githubactions&style=flat-square&color=ccd5ae&labelColor=f8f9fa)](https://github.com/inlab-geo/espresso/actions/workflows/build_wheels.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/geo-espresso?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://geo-espresso.readthedocs.io/en/latest/?badge=latest)
@@ -44,15 +43,15 @@
 to another requires changing one line of code. 
 
 The Espresso project is a community effort - if you think it sounds useful,
 please consider contributing an example or two from your own research. The project
 is currently being coordinated by InLab, with support from the CoFI development
 team.
 
-For more information, please visit our documentation (coming soon).
+For more information, please visit [our documentation](geo-espresso.readthedocs.io).
 
 
 ## Installation
 
 ```console
 $ pip install geo-espresso
 ```
@@ -65,50 +64,45 @@
 
 Once installed, each test problem can be imported using the following command:
 
 ```python
 from espresso import <testproblem>
 ```
 
-Replace ``<testproblem>`` with one of the following currently available problems:
-
-- `SimpleRegression`
-- `XrayTomography`
-- `FmmTomography`
-- `PumpingTest`
-- `SlugTest`
-- `GravityDensity`
+Replace ``<testproblem>`` with an actual problem class in Espresso, such as
+`SimpleRegression` and `FmWavefrontTracker`. See 
+[here](https://geo-espresso.readthedocs.io/en/latest/user_guide/contrib/index.html) 
+for a full list of problems Espresso currently includes.
 
 Once a problem is imported, its main functions can be called using the same 
 structure for each problem. For instance:
 
 ```python
-from espresso import GravityDensity
+from espresso import FmWavefrontTracker
 
-problem = GravityDensity(example_number=1)
+problem = FmWavefrontTracker(example_number=1)
 model = problem.good_model
 data = problem.data
 pred = problem.forward(model)
 fig_model = problem.plot_model(model)
-fig_data = problem.plot_data(data, pred)
 ```
 
 You can access related metadata programatically:
 
 ```python
-print(GravityDensity.problem_title)
-print(GravityDensity.problem_short_description)
-print(GravityDensity.author_names)
+print(FmWavefrontTracker.metadata["problem_title"])
+print(FmWavefrontTracker.metadata["problem_short_description"])
+print(FmWavefrontTracker.metadata["author_names"])
 ```
 
 Other problem-specific parameters can be accessed through the problem instance. For instance:
 
 ```python
-print(problem.m)
-print(problem.rec_coords)
+print(problem.extent)
+print(problem.model_shape)
 ```
 
 Which additional values are set is highly problem-specific and we suggest to 
 consult the 
 [Espresso Documentation on the problems](https://geo-espresso.readthedocs.io/en/latest/user_guide/contrib/index.html).
```

### Comparing `geo-espresso-0.2.2.dev0/README.md` & `geo-espresso-0.2.2.dev1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 to another requires changing one line of code. 
 
 The Espresso project is a community effort - if you think it sounds useful,
 please consider contributing an example or two from your own research. The project
 is currently being coordinated by InLab, with support from the CoFI development
 team.
 
-For more information, please visit our documentation (coming soon).
+For more information, please visit [our documentation](geo-espresso.readthedocs.io).
 
 
 ## Installation
 
 ```console
 $ pip install geo-espresso
 ```
@@ -38,50 +38,45 @@
 
 Once installed, each test problem can be imported using the following command:
 
 ```python
 from espresso import <testproblem>
 ```
 
-Replace ``<testproblem>`` with one of the following currently available problems:
-
-- `SimpleRegression`
-- `XrayTomography`
-- `FmmTomography`
-- `PumpingTest`
-- `SlugTest`
-- `GravityDensity`
+Replace ``<testproblem>`` with an actual problem class in Espresso, such as
+`SimpleRegression` and `FmWavefrontTracker`. See 
+[here](https://geo-espresso.readthedocs.io/en/latest/user_guide/contrib/index.html) 
+for a full list of problems Espresso currently includes.
 
 Once a problem is imported, its main functions can be called using the same 
 structure for each problem. For instance:
 
 ```python
-from espresso import GravityDensity
+from espresso import FmWavefrontTracker
 
-problem = GravityDensity(example_number=1)
+problem = FmWavefrontTracker(example_number=1)
 model = problem.good_model
 data = problem.data
 pred = problem.forward(model)
 fig_model = problem.plot_model(model)
-fig_data = problem.plot_data(data, pred)
 ```
 
 You can access related metadata programatically:
 
 ```python
-print(GravityDensity.problem_title)
-print(GravityDensity.problem_short_description)
-print(GravityDensity.author_names)
+print(FmWavefrontTracker.metadata["problem_title"])
+print(FmWavefrontTracker.metadata["problem_short_description"])
+print(FmWavefrontTracker.metadata["author_names"])
 ```
 
 Other problem-specific parameters can be accessed through the problem instance. For instance:
 
 ```python
-print(problem.m)
-print(problem.rec_coords)
+print(problem.extent)
+print(problem.model_shape)
 ```
 
 Which additional values are set is highly problem-specific and we suggest to 
 consult the 
 [Espresso Documentation on the problems](https://geo-espresso.readthedocs.io/en/latest/user_guide/contrib/index.html).
```

### Comparing `geo-espresso-0.2.2.dev0/docs/Makefile` & `geo-espresso-0.2.2.dev1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_ext/generate_contrib_docs.py` & `geo-espresso-0.2.2.dev1/docs/source/_ext/generate_contrib_docs.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/contrib_edit1.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/contrib_edit1.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork2.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork2.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork3.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork3.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/contrib_fork4.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/contrib_fork4.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/contrib_pr1.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/contrib_pr1.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/espresso_arch.svg` & `geo-espresso-0.2.2.dev1/docs/source/_static/espresso_arch.svg`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/inlab_logo_60px.png` & `geo-espresso-0.2.2.dev1/docs/source/_static/inlab_logo_60px.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_static/style.css` & `geo-espresso-0.2.2.dev1/docs/source/_static/style.css`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-/* ALL: links color */
-:root {
-    --pst-color-link: 141, 66, 76
-}
+/* https://github.com/pydata/pydata-sphinx-theme/blob/master/src/pydata_sphinx_theme/theme/pydata_sphinx_theme/layout.html */
+/* https://github.com/executablebooks/sphinx-book-theme/blob/master/src/sphinx_book_theme/theme/sphinx_book_theme/layout.html */
 
-/* ALL: text font size */
+/* ALL: color, text font size */
+html[data-theme="light"] {
+    --pst-color-primary: #E29578;
+}
 p {
     font-size: 1rem;
 }
 
 
 /* APV modifications */
 /* Mainly designed to get FAQ looking good */
@@ -26,76 +27,48 @@
 
 div.contents {
     padding: 1em 1em 1em;
 }
 div.contents>ul>li>p>a {
     font-size: 100%;
 }
-
-
 /* End APV modifications */
 
 
 /* TOP LEFT: logo + project title */
 div.navbar-brand-box a.navbar-brand img {
     max-height: 10vh !important;
 }
 span.project-version {
-    color: #649A69;
+    color: var(--pst-color-primary);
     font-size: 0.8em;
     font-weight: 600;
     margin-left: 3px;
 }
 
-/* TOP RIGHT: three little logos */
-/* .topbar .topbar-main button.topbarbtn {
-    font-size: 1.2em;
-}
-[aria-label] {
-    position: relative;
-}
-div.dropdown-buttons-trigger div.dropdown-buttons button.topbarbtn {
-    font-size: .85em !important;
-} */
-
 /* LEFT: side bar font size */
 .bd-sidenav a.reference.internal {
     font-size: 0.8rem;
 }
 
-/* HOME: inference tree */
+/* Mermaid */
 div.mermaid:not([data-processed]) {
     display: none;
 }
 div.mermaid {
     transition: transform .2s;
 }
 div.mermaid:hover {
     transform: translateX(15%) scale(1.3);
 }
 
 
 /* HOME: panel button */
-.btn-outline-primary:hover {
-    color: #8D424C;
-    background-color: #FFD883;
-    border-color: #FFD883;
-}
-.btn-outline-primary {
-    /* color: rgb(51, 125, 222); */
-    /* color: #99582a; */
-    border-color: #FFD883;
-}
-.card-body {
-    display: flex;
-    flex-direction: column;
-    justify-content: space-between;
-}
-.card:hover {
-    border: 1px solid #8D424C;
+.card-border:hover {
+    border: 1.5px solid var(--pst-color-primary) !important;
 }
 
 /* API: class/method name */
 span.sig-name {
     color: #99582a;
 }
 code.xref {
@@ -107,20 +80,14 @@
 table.autosummary p {
     font-size: 0.8rem;
 }
 table.autosummary span {
     font-size: 1rem;
 }
 
-/* Sphinx gallery */
-div.sphx-glr-download {
-    height: 0px;
-    visibility: hidden;
-}
-
 /* TOC .. contents:: */
 #developer-notes section div.contents {
     border: 0;
     background-color: transparent;
     padding: 0;
 }
 #developer-notes section div.contents ul {
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/class.rst` & `geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/_templates/autosummary/module.rst` & `geo-espresso-0.2.2.dev1/docs/source/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/conf.py` & `geo-espresso-0.2.2.dev1/docs/source/conf.py`

 * *Files 11% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 extensions = [
     "sphinx.ext.autodoc",
     "sphinx.ext.autosummary",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.doctest",
     "sphinx.ext.mathjax",
-    "sphinx_panels",
+    "sphinx_design",
     "sphinx_togglebutton",
     "sphinx_copybutton",
     "sphinx.ext.napoleon",
     "myst_nb",
     # "sphinx_gallery.gen_gallery",
     "sphinxcontrib.mermaid",
     "generate_contrib_docs",                # our own extension
@@ -87,55 +87,64 @@
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3/", None),
     "scipy": ("https://docs.scipy.org/doc/scipy/", None),
     "numpy": ("https://numpy.org/doc/stable/", None),
     "matplotlib": ("https://matplotlib.org/stable", None),
 }
 
-# Disable including boostrap CSS for sphinx_panels since it's already included
-# with sphinx-book-theme
-panels_add_bootstrap_css = False
-panels_css_variables = {
-    "tabs-color-label-inactive": "hsla(231, 99%, 66%, 0.5)",
-}
-
 # settings for the sphinx-copybutton extension
 copybutton_prompt_text = ">>> "
 
 
 # -- Options for HTML output -------------------------------------------------
 html_title = f'{project} <span class="project-version">{version}</span>'
 html_short_title = project
-# html_logo = "_static/???"
 html_favicon = "_static/inlab_logo_60px.png"
 
 html_theme = "sphinx_book_theme"
 html_theme_options = {
     "repository_url": "https://github.com/inlab-geo/espresso",
     "repository_branch": "main",
-    "path_to_docs": "docs",
+    "path_to_docs": "docs/source/",
     "launch_buttons": {
         "notebook_interface": "classic",
         "inlab_url": "http://www.inlab.edu.au/",
     },
     "extra_footer": "",
     "home_page_in_toc": True,
     "use_repository_button": True,
     "use_edit_page_button": True,
+    "use_source_button": True,
     "use_issues_button": True,
+    "use_download_button": True,
+    "use_sidenotes": True,
+    "icon_links": [
+        {
+            "name": "GitHub",
+            "url": "https://github.com/inlab-geo/geo-espresso",
+            "icon": "https://img.shields.io/badge/GitHub-espresso-171515?logo=github&labelColor=f8f9fa&style=flat-square&logoColor=171515",
+            "type": "url",
+        },
+        {
+            "name": "Version",
+            "url": "https://pypi.org/project/geo-espresso/",
+            "icon": "https://img.shields.io/pypi/v/geo-espresso?logo=pypi&style=flat-square&color=83C5BE&labelColor=f8f9fa&label=latest",
+            "type": "url",
+        },
+    ],
 }
 
 html_static_path = ["_static"]
 html_css_files = ["style.css"]
 html_context = {
     "display_github": True, # Integrate GitHub
     "github_user": "inlab-geo", # Username
-    "github_repo": "cofi", # Repo name
+    "github_repo": "espresso", # Repo name
     "github_version": "main", # Version
-    "conf_py_path": "", # Path in the checkout to the docs root
+    "conf_py_path": "/source/", # Path in the checkout to the docs root
 }
 
 
 # -- myst-nb settings ---------------------------------------------------------
 myst_enable_extensions = [
     "amsmath",
     "colon_fence",
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/contributor_guide/new_contrib.rst` & `geo-espresso-0.2.2.dev1/docs/source/contributor_guide/new_contrib.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,225 +1,182 @@
-===============================
-Creating a new Espresso problem
-===============================
+==================
+Create new example
+==================
 
 👋 Everyone is welcomed to contribute with their own forward code. We aim to reduce the
-barrier of contributing so don't worry if you are not familiar with those technical
-stuff like git operations - we are here to help.
+barrier of contributing so don't worry if you are not familiar with some technical
+stuff - we are here to help.
 
-There are generally three steps involved in submiting your code:
 
-- **Download** - :ref:`get a copy of Espresso <get_own_copy>`
-- **Edit** - :ref:`add in your own Espresso problem <add_contrib>`
-- **Upload** - :ref:`submit your changes to our main repository <submit_changes>`
-
-It's important to note that after you've uploaded your contribution, you can still edit 
-it with the same "pull request" workflow.
-
-In the following paragraphs, we list out detailed steps on how to contribute a new 
-example. Again, feel free to `contact us <../user_guide/faq.html>`_ when in doubt.
-
-In case you prefer an alternative guide, we've also prepared a demo video below. If 
-your browser fails to load the video, head to 
-`this link <https://dl.dropbox.com/s/j1xdl0q7zj039cl/%28with%20clicks%29%20how-to-contribute-an-example-in-espresso.mp4?dl=0>`_ 
-to watch it.
-
-.. raw:: html
-
-    <iframe width="560" height="315" src="https://www.dropbox.com/s/j1xdl0q7zj039cl/%28with%20clicks%29%20how-to-contribute-an-example-in-espresso.mp4?dl=0&raw=1" frameborder="0" allowfullscreen></iframe>
-
-.. _get_own_copy:
-
-Get your own copy of Espresso
+Add your own Espresso problem
 -----------------------------
 
-#. Open your browser and go to the Espresso `repository`_.
-#. Ensure you have a GitHub account and it's signed in. If not, click the "Sign Up"
-   button on the top right and fill in the necessary information to sign up an account.
-#. Now click the "Fork" button on the top right.
-
-   .. figure:: ../_static/contrib_fork.png
-    :align: center
-
-#. Leave everything by default and click the green "Create fork" button.
+#. A new contribution to Espresso has to conform to a consistent
+   file structure. The simplest way to ensure that a new contribution includes
+   all files is to start the creation of a new problem from the template. Run the 
+   following command from the the path to Espresso:
 
-   .. figure:: ../_static/contrib_fork2.png
-    :align: center
-
-#. Now you will be redirected to your own "fork" of the Espresso repository.
+   .. code-block:: bash
 
-   This fork is your own version of Espresso, and you can make changes however you 
-   want. We will later demonstrate that after you make your own changes, you are
-   able to "contribute" back to the main repository.
+        python espresso_machine/new_contribution/create_new_contrib.py <problem-name>
 
-   .. figure:: ../_static/contrib_fork3.png
-    :align: center
+   Replacing :code:`problem-name` with your Espresso problem name in snake case 
+   (e.g. :code:`gravity_density`, :code:`polynomial_regression`). Remember to choose a 
+   sensible, unique name for your contribution that makes it easy to understand what 
+   the example is about.
 
-#. We will clone your fork into your local machine. Click the green "Code" button first, 
-   and then copy the content under the "HTTPS" tab.
+#. Navigate to folder :code:`<path-to-espresso>/contrib/<problem-name>`, and you'll see template 
+   files needed for a new contribution. Each Espresso example is organised around a
+   central class object that contains, at minimum, a set of functions with names
+   that are shared by all examples.
 
-   .. figure:: ../_static/contrib_fork4.png
+   .. figure:: ../_static/contrib_edit1.png
     :align: center
 
-#. Clone your fork to somewhere in your computer.
+#. Now the folder is all yours, get started with the following checklist.
 
-   - For **MacOS** and **Linux** users, open your "Terminal" app, change your working 
-     directory into somehwere you'd like to place the Espresso code, then run the 
-     :code:`git clone` command as following.
-   - For **Windows** users, please install `git <https://git-scm.com/downloads>`_ first, 
-     and open "Git Bash" to run the following commands. In the steps afterwards, it's
-     always "Git Bash" when we refer to a "terminal" if you are on Windows.
+   .. dropdown:: Checklist and tips
+      :icon: tasklist
+      :open:
 
-   .. code-block:: console
+      - ``contrib/<problem-name>/README.md``
 
-    cd <path-to-espresso>
-    git clone <url-you-copied-in-step-6>
-    cd espresso
-    git remote add upstream https://github.com/inlab-geo/espresso
-    git fetch upstream
+        - Document anything you'd like to add for this problem, such as the what the 
+          problem is about and some brief intro of the theory behind.
+        - This will be automatically rendered into :doc:`../user_guide/contrib/index`.
 
-   .. admonition:: Instructions for first-time GitHub users
-      :class: dropdown, attention
-
-      If this is the first time you clone a GitHub repository, it's very likely that you 
-      will need a personal access token as your password. 
+      - ``contrib/<problem-name>/LICENCE``
       
-      **Option 1** - Check out this page:
-      `creating a personal access token <https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token>`_
-      for how to create a personal access token, and use it as your password when you are
-      asked to enter it in the terminal.
+        - We use a 2-clause BSD licence as the default one. Feel free to replace it
+          with a licence that suits you best.
 
-      **Option 2** - Alternatively, set up SSH key and upload your public key to your 
-      GitHub account. Follow instructions in this page:
-      `Generating a new SSH key and adding it to the ssh-agent <https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent>`_
-      for how to set up SSH keys with GitHub.
+      - ``contrib/<problem-name>/<problem-name>.py``
 
-#. Open :code:`<path-to-espresso>/espresso` folder with your favourite code editor. 
-   You will see a copy of Espresso in front of you, cheers ☕️! 
+        - The development will be centered around the autogenerated class 
+          ``ProblemName``. It is a subclass of 
+          :doc:`EspressoProblem <../user_guide/api/generated/espresso.EspressoProblem>`
+          so you might find the API reference helpful.
+        - All standard attributes have been declared in the template but are left for 
+          you to implement. You'll see that some are required (with ``TODO``) and 
+          others are optional.
+        - If you would like to load data from files, please use our 
+          :doc:`utility functions <../user_guide/api/generated/espresso.utils>`
+          to get the absolute path before calling your loading function.
+        - Apart from the standard attributes, there are many more functions and values 
+          that a new contribution can contain, for examples:
+
+          - inversion_suggestion: a string containing inversion suggestions
+          - reg_param_suggestion: a sensible value for regularization parameter
+          - dx: spatial resolution in x-direction
+          - dt: temporal resolution
+          - nt: number of time steps
+          - The possibilities are endless! Whatever information you find helpful is
+            probably also helpful for the users. Simply attach them to the problem 
+            class as additional attributes.
+         
+        - We aim to follow `Python PEP8 style conventions <https://peps.python.org/pep-0008/>`_
+          to make source code readable. Though not strictly enforced, we recommend
+          `Black formatter <https://github.com/psf/black#installation-and-usage>`_ and
+          `PyLint <https://github.com/pylint-dev/pylint#install>`_ to maintain a good 
+          coding style.
+         
+      - ``setup.py``, in particular the ``INSTALL_REQUIRES`` variable, if needed.
+   
+#. Test running your code. 
 
+   .. dropdown:: Troubleshooting: issue with relative import
+      :icon: tools
 
-.. _add_contrib:
+      Note that you might see an error if you have any relative import in the main Python 
+      file:
 
-Add your own Espresso problem
------------------------------
+      .. code-block:: python
 
-#. Let's now ensure that you have a correct environment set up. Python >= 3.6 is required,
-   and see this 
-   `environment_contrib.yml <https://github.com/inlab-geo/espresso/blob/main/envs/environment_contrib.yml>`_ 
-   file for a list of required packages.
-
-   .. toggle::
-        
-        - Choose a Python environment manager first. 
-          `mamba <https://mamba.readthedocs.io/en/latest/>`_ /
-          `conda <https://docs.conda.io/en/latest/>`_ is recommended as it can set 
-          up system-wide dependencies as well, but feel free to use the one you are most 
-          familiar with.
-
-        - Python >= 3.6 is required.
-
-        - If you use `mamba <https://mamba.readthedocs.io/en/latest/>`_ /
-          `conda <https://docs.conda.io/en/latest/>`_, run 
-          :code:`conda create -f envs/environment_contrib.yml` under the project root folder.
-          Otherwise, make sure you have the list of packages in 
-          `environment_contrib.yml <https://github.com/inlab-geo/espresso/blob/main/envs/environment_contrib.yml>`_
-          in the virtual environment with your preferred tool.
+         # file: <problem-name>.py
 
-#. Install Espresso core library - this enables you to access the base class for an Espresso problem
-   :code:`EspressoProblem` and some utility functions to help the development.
+         from .lib import *
 
-   Run the following in your terminal, with :code:`<path-to-espresso>/` as your working directory.
+      In this case, use ``contrib`` as your working directory and import your contribution
+      in the following example way:
 
-   .. code-block:: bash
+      .. code-block:: pycon
 
-      pip install .
-
-#. Create a folder for your new contribution under :code:`contrib/<problem-name>`,
-   by running the following in your terminal:
-
-   .. code-block:: bash
+         $ pwd                                        # check you are in the right folder
+         <path-to-espresso>/contrib
+         $ python
+         >>> from example_name import ExampleName     # ...and import this way
+      
+      Or the following example if you are running a file:
 
-        python <path-to-espresso>/espresso_machine/new_contribution/create_new_contrib.py <problem-name>
+      .. code-block:: python
 
-   Replacing :code:`path-to-espresso` with your path to the espresso folder you've just cloned,
-   and :code:`problem-name` with your Espresso problem name, with lower case words connected
-   by underscores (e.g. :code:`gravity_density`, :code:`polynomial_regression`).
+         # file: contrib/tmp.py                       # create tmp file in the right folder
+         from example_name import ExampleName         # ...and import this way
 
-#. Navigate to folder :code:`<path-to-espresso>/contrib/<problem-name>`, and you'll see template 
-   files.
+#. Validate your code with Espresso by running:
 
-   .. figure:: ../_static/contrib_edit1.png
-    :align: center
+   .. code-block:: console
 
-#. Read instructions in the :code:`README.md` file, and you will know what to do next 🧑🏽‍💻👩🏻‍💻👨‍💻
+      $ python espresso_machine/build_package/build.py --pre --post -c <example_name>
 
-   #. You should already have all the "pre-requisites" installed if you've gone through 
-      the steps above.
+   which includes the following steps:
 
-   #. See a list of "Checklists". These are pretty much all the things you've
-      got to do to complete this contribution.
+   - Validate all required and standard attributes that you've implemented
+   - Build your contribution into a temporary source code folder ``_esp_build``
+   - Install your local development Espresso version
+   - Validate all required and standard attributes from the installed package
+   - Check that packages needed to run your code are listed by Espresso
 
-   #. When you'd like to perform a quick local test by running your own code, run
-      :code:`python espresso_machine/build_package/validate.py -c <problem-name>`
+   Read on the :ref:`appendix sections <appendix>` in this page for how an Espresso 
+   example is validated and how Espresso is built, and continue with the 
+   :doc:`../developer_guide/index` further details the whole infrastructure (i.e. the 
+   ``espresso_machine``).
 
-   #. When you think you've finished the coding, run
-      :code:`python espresso_machine/build_package/build.py --validate`
 
+Jupyter Notebook
+----------------
 
-.. _submit_changes:
+Additionally, we encourage you to add a Jupyter Notebook with an identical name
+into the folder Jupyter Notebooks that contains the following:
 
-Submit your changes
--------------------
+1. An extensive description of the new Espresso Problem, containing
+   information about (but not limited to):
 
-#. It's helpful to "commit" your changes when you have any progress. Feel free to make 
-   commits as often as necesary.
-   
-   - Use :code:`git add <file-name-1> <file-name-2>` to choose which files you'd like to 
-     include in the following "commit".
-   - Use :code:`git commit -m "progress in xxx"` to commit your changes.
-   - Use :code:`git push origin <branch-name>` to push your changes onto your GitHub fork,
-     where :code:`<branch-name>` is :code:`main` by default.
+   - the forward calculation (ie. the underlying physics) and how it was implemented.
+   - which inversion method is used (and regularisation) and how it was implemented.
+   - the physical unit of relevant variables, but at least of ``model`` and ``data``.
+   - all changeable parameters, possibly in a list.
 
-   .. seealso::
 
-    Check `this cheatsheet <https://education.github.com/git-cheat-sheet-education.pdf>`_
-    for a good reference of using Git.
+2. An example of the new problem being used, with a reasonable output.
 
-#. After you've commited code changes and pushed your commits up to your fork, open your 
-   fork on GitHub :code:`https://github.com/<your-gh-account>/espresso` in a browser.
 
-#. Find the word "Contribute" on top of the page, click it and choose the green "Open 
-   pull request" button. Follow the prompts and fill in necessary message you'd like us
-   to know.
+.. _appendix:
 
-   .. figure:: ../_static/contrib_pr1.png
-    :align: center
+Appendix I: build steps
+-----------------------
 
-#. Once your pull request is submitted, some automatic checks will be triggered. Rest 
-   assured - we will review your contribution, comment if necessary, and proceed to merge
-   your contribution into our main repository when everything's ready.
+Usage:
 
-#. After your contribution is merged to the main branch, you can request another change
-   with the same workflow anytime you want. Just keep your own fork, edit, commit and 
-   push to your own fork, and raise a pull request from there.
+.. code-block:: console
 
-#. Thanks again, for your contribution to open source 🌟 
+   $ python build.py [--pre] [--post] [--no-install] [-c <example_name>] [--file <file_name>]
 
+For instance, to install your development version locally, run the following in your 
+terminal:
 
-.. _appendix_build_steps:
+.. code-block:: console
 
-Appendix I: installation steps
-------------------------------
+   $ python espresso_machine/build_package/build.py
 
-To install your development version locally, run the following in your terminal:
+Run the following for detailed usage information:
 
 .. code-block:: console
 
-   $ python espresso_machine/build_package/build.py
-
+   $ python espresso_machine/build_package.build.py --help
 
 The following table describes what happens when we package Espresso:
 
 .. list-table:: How Espresso is packaged
    :widths: 10 45 45
    :header-rows: 1
 
@@ -242,44 +199,36 @@
      - Write dynamic version and extra versioningit configs into ``_esp_build/pyproject.toml``
      - ``versioningit``
    * - 6
      - Install package from ``_esp_build/``
      - ``pip install _esp_build``
 
 
-.. _appendix_validation_steps:
-
 Appendix II: validation steps
 -----------------------------
 
-To test whether your new contribution aligns with the Espresso standard, run 
-the following in your terminal:
+Usage:
 
 .. code-block:: console
 
-   $ python espresso_machine/build_package/validate.py -c <contrib-name>
+   $ python validate.py [-h] [--all] [--pre] [--post] [--contrib CONTRIBS] [--file <file_name>]
 
-You can run the validation script before (``--pre`` flag on) and/or after (``--post`` 
-flag on) you install your development version of Espresso. A better workflow is to run 
-both:
+For instance, to test whether your new contribution aligns with the Espresso standard, 
+run the following in your terminal:
 
 .. code-block:: console
 
-   $ python espresso_machine/build_package/validate.py --pre -c <contrib-name>
-   $ python espresso_machine/build_package/build.py
-   $ python espresso_machine/build_package/validate.py --post -c <contrib-name>
-
+   $ python espresso_machine/build_package/validate.py -c <contrib-name>
 
-Or the following for a complete check on all examples (including yours), both before
-and after Espresso installed:
+Or the following for a complete check on all examples (including yours and existing 
+ones for regression test), both before and after Espresso installed:
 
 .. code-block:: console
 
-   $ python espresso_machine/build_package/build.py
-
+   $ python espresso_machine/build_package/validate.py
 
 Anyway, run the following for a detailed usage of this script:
 
 .. code-block:: console
 
    $ python espresso_machine/build_package/validate.py --help
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/developer_guide/repository.rst` & `geo-espresso-0.2.2.dev1/docs/source/developer_guide/repository.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-==============================
-The Espresso Github repository
-==============================
+================
+Folder structure
+================
 
 .. figure:: ../_static/espresso_arch.svg
     :align: center
 
 - Folder **contrib/** contains subfolders for each Espresso problem. Each Espresso
   problem has a self-contained subfolder with :code:`problem_name` as the folder name.
 
@@ -14,19 +14,18 @@
   functions.
 
   - If you'd like to improve base class specification or :code:`espresso.utils`,
     this is the place to edit.
 
   - If you'd like to bump the version, change file :code:`src/espresso/version.py`.
 
+
 - Folder **espresso_machine/** has all the utility scripts to be used by contributors and 
   developers.
 
+
 - Folder **_esp_build/** will contain temporary Python package source files after you
   build :code:`espresso`.
 
   - These are built files, so you never have to change the contents under this folder. 
     If you feel something's wrong in this folder, look for the source from the three 
     folders above.
-
-- Folder **docs/** has all the documentation sources.
-
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/index.rst` & `geo-espresso-0.2.2.dev1/docs/source/index.rst`

 * *Files 17% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 
 .. The following defines the structure of the document. It is hidden so it doesn't
    render into the html, but it cannot be removed!
    We assume that each 'index.rst' document defines its own toctree that can be incorporated.
 
 .. toctree::
     :hidden: 
-    :maxdepth: 1
+    :maxdepth: 2
 
     user_guide/index.rst
 
 .. toctree::
     :hidden:
-    :maxdepth: 1
+    :maxdepth: 2
 
     contributor_guide/index.rst
 
 .. toctree::
     :hidden:
-    :maxdepth: 1
+    :maxdepth: 2
 
     developer_guide/index.rst
 
 
-.. toctree::
-    :hidden:
+.. .. toctree::
+..     :hidden:
     
-    GitHub repository <https://github.com/inlab-geo/espresso/>
-    Issue tracker <https://github.com/inlab-geo/espresso/issues/>
+..     GitHub repository <https://github.com/inlab-geo/espresso/>
+..     Issue tracker <https://github.com/inlab-geo/espresso/issues/>
 
 
 You've just come up with a new optimisation algorithm, inversion strategy, or machine learning-based inference framework. Now you want to see how it performs on a real-world problem... 
 
 Espresso (**E**\ arth **s**\ cience **pr**\ oblems for the **e**\ valuation of **s**\ trategies, **s**\ olvers and **o**\ ptimizers) aims to make this as easy as possible. It provides access to a range of exemplars via a standardized Python interface, including domain-expert--curated datasets and corresponding simulation codes. Swapping from one test problem to the next is just one line of code.
 
 Here's a simple illustration:
@@ -77,38 +77,70 @@
     print("Espresso:", tp.good_model)
 
     # And let's visualise both to see where the differences are:
     my_fig = tp.plot_model(model)
     espresso_fig = tp.plot_model(tp.good_model)
     data_fig = tp.plot_model(tp.data, tp.forward(model))
 
-If this looks interesting, you can:
-
-- Read the :doc:`user_guide/index` for more information about what Espresso provides and how to use it;
-- Contribute your own example problems by following the instructions in the :doc:`contributor_guide/index`;
-- Learn about the infrastructure behind Espresso by looking at the :doc:`developer_guide/index`;
-- Explore the source code on `GitHub <https://github.com/inlab-geo/espresso/>`_;
-- Report a bug or suggest a feature using the `Issue Tracker <https://github.com/inlab-geo/espresso/issues/>`_;
-- Join the conversation on `Slack <https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg>`_.
-
-Espresso is an open-source community effort, currently supported and coordinated by `InLab <http://www.inlab.edu.au/>`_.
-
 
-.. Espresso (**E**\ arth **S**\ cience **PR**\ oblems for the **E**\ valuation of **S**\ trategies,
-.. **S**\ olvers and **O**\ ptimizers) is:
-
-.. - A collection of:
-
-..   - geoscience simulation codes (or 'forward models'), with 
-..   - associated datasets;
-
-.. - Designed for researchers, educators and students working in areas such as inference, inversion, optimisation or machine learning. It aims to:
-
-..   - Provide real-world test problems to support algorithm development;
-..   - Enable benchmarking and comparison of techniques across a range of application areas;
-..   - Support teaching by providing a variety of examples that can be incorporated into lectures, demonstrations and practical exercises.
-
-.. - Accessible via a standardised interface. Testing your algorithm on a new problem means changing just one line of code, and does not require any domain knowledge.
+If this looks interesting, you can:
 
-.. - An open-source community effort, currently coordinated by `InLab <http://www.inlab.edu.au/>`_, with support from the CoFI development team.
+.. grid:: 1 3 3 3
+    :gutter: 3
+    :padding: 2
+
+    .. grid-item-card::
+        :link: user_guide/index.html
+        :text-align: center
+        :class-card: card-border
+
+        *📙 User Guide*
+        ^^^^^^^^^^^^^^^
+        Read about what Espresso provides and how to use it
+
+    .. grid-item-card::
+        :link: contributor_guide/index.html
+        :text-align: center
+        :class-card: card-border
+
+        *📗 Contributor Guide*
+        ^^^^^^^^^^^^^^^^^^^^^^
+        Contribute your own example problems with minimal steps
+
+    .. grid-item-card::
+        :link: developer_guide/index.html
+        :text-align: center
+        :class-card: card-border
+
+        *📘 Developer Guide*
+        ^^^^^^^^^^^^^^^^^^^^
+        Learn about the infrastructure behind Espresso
+
+    .. grid-item-card::
+        :link: https://github.com/inlab-geo/espresso/
+        :text-align: center
+        :class-card: card-border
+
+        *🐍 GitHub Repository*
+        ^^^^^^^^^^^^^^^^^^^^^^
+        Explore the source code on GitHub
+
+    .. grid-item-card::
+        :link: https://github.com/inlab-geo/espresso/issues/
+        :text-align: center
+        :class-card: card-border
+
+        *🐛 Issue Tracker*
+        ^^^^^^^^^^^^^^^^^^
+        Report a bug or suggest a feature by creating an issue
+
+    .. grid-item-card::
+        :link: https://join.slack.com/t/inlab-community/shared_invite/zt-1ejny069z-v5ZyvP2tDjBR42OAu~TkHg
+        :text-align: center
+        :class-card: card-border
+
+        *💬 Join Slack*
+        ^^^^^^^^^^^^^^^
+        Accept this invitation to join the conversation on Slack
 
 
+Espresso is an open-source community effort, currently supported and coordinated by `InLab <http://www.inlab.edu.au/>`_.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/user_guide/examples.rst` & `geo-espresso-0.2.2.dev1/docs/source/user_guide/examples.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 .. highlight:: python
 
-========
-Examples
-========
+==============
+Usage Examples
+==============
 
 This page provides some annotated examples showing how Espresso can be used.
 
 Gradient descent
 ----------------
 
 .. code-block:: python
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/user_guide/faq.rst` & `geo-espresso-0.2.2.dev1/docs/source/user_guide/faq.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,28 @@
-==========================
-Frequently Asked Questions
-==========================
+=========
+User FAQs
+=========
 
 Contents
 ********
 
 .. contents::
     :local:
     :class: toggle:
- 
+
 
 Why doesn't the Espresso API include <feature>?
 -----------------------------------------------
-Our design philosophy centres around having a universal interface that enables users to access a range of test problems without detailed domain knowledge. We think this means we should keep the API as small and tightly-defined as possible, to ensure that it can accommodate the widest range of problems and users.
 
-Nevertheless, we welcome suggestions! You can propose a new API feature by `opening an issue <https://github.com/inlab-geo/espresso/issues>`_.
+- Our design philosophy centres around having a universal interface that enables 
+  users to access a range of test problems without detailed domain knowledge. 
+  We think this means we should keep the API as small and tightly-defined as possible, 
+  to ensure that it can accommodate the widest range of problems and users.
+- Nevertheless, we welcome suggestions! You can propose a new API feature by `opening an issue <https://github.com/inlab-geo/espresso/issues>`_.
 
 I've got an idea for a new test problem!
 ----------------------------------------
-Great! We welcome suggestions and contributions. You can tell us about your idea by `opening an issue <https://github.com/inlab-geo/espresso/issues>`_. You can also have a go at adding the test problem yourself --- take a look at the :doc:`../contributor_guide/index`
+
+- Great! We welcome suggestions and contributions. You can tell us about your idea by 
+  `opening an issue <https://github.com/inlab-geo/espresso/issues>`_. 
+- You can also have a go at adding the test problem yourself --- take a look at the 
+  :doc:`../contributor_guide/index`
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/user_guide/index.rst` & `geo-espresso-0.2.2.dev1/docs/source/user_guide/index.rst`

 * *Files 22% similar despite different names*

```diff
@@ -8,16 +8,25 @@
     why.rst
     installation.rst
     usage.rst
     examples.rst
     contrib/index.rst
     api/index.rst
     faq.rst
+    changelog.md
 
 
-This guide describes how to install and use Espresso, and provides :doc:`detailed information <contrib/index>` about individal test problems. You may also wish to look at:
+This guide describes:
+
+- :doc:`What is Espresso and why <why>`,
+- :doc:`How to install Espresso <installation>`,
+- :doc:`How to use Espresso <usage>` and :doc:`examples <examples>`,
+- :doc:`Reference <contrib/index>` for individal test problems,
+- :doc:`API reference <api/index>`, :doc:`FAQ <faq>`, and :doc:`Release notes <changelog>`
+
+You may also wish to look at:
 
 - The :doc:`../contributor_guide/index`, which explains how you can add a new test problem into Espresso, or improve an existing one;
 - The :doc:`../developer_guide/index`, which describes the infrastructure that runs 'in the background' to build Espresso;
 - Our `Github repository <https://github.com/inlab-geo/espresso/>`_ 
-- The Espresso community on Slack
+- The ``#espresso`` channel on `Slack`_
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/user_guide/installation.rst` & `geo-espresso-0.2.2.dev1/docs/source/user_guide/installation.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,146 +1,200 @@
 ============
 Installation
 ============
 
-.. Pre-requisites should be automagically handled so I'm not sure they need to be listed here?
-.. 
-.. Pre-requisites
-.. --------------
-
-.. Espresso requires Python 3.6+, and the following dependencies:
-
-.. - numpy>=1.18
-.. - scipy>=1.0.0
-.. - matplotlib>=3.1
-.. - tqdm>=4.0
+Install Espresso
+----------------
 
 **Step 1**: (*Optional*) Set up a virtual environment.
 
-We strongly recommend installing Espresso within a `virtual environment <https://docs.python.org/3/tutorial/venv.html>`_. This ensures that Espresso can install the various modules that it needs without the risk of breaking anything else on your system. There are a number of tools that can facilitate this, including `venv`, `virtualenv`, `conda` and `mamba`.
+We strongly recommend installing Espresso within a 
+`virtual environment <https://docs.python.org/3/tutorial/venv.html>`_. 
+This ensures that Espresso can install the various modules that it needs without the 
+risk of breaking anything else on your system. There are a number of tools that can 
+facilitate this, including `venv`, `virtualenv`, `conda` and `mamba`.
 
-.. tabbed:: venv
 
-  Ensure you have `python>=3.6`. Then, you can create a new virtual environment by running the command
+.. dropdown:: Expand for how to manage virtual environments
+  :icon: package
 
-  .. code-block:: console
+  .. tab-set::
 
-    $ python -m venv <path-to-new-env>/<env-name>
+    .. tab-item:: venv
 
-  where :code:`<path-to-new-env>` is your prefered location for storing information about this environment, and :code:`<env-name>` is your preferred name for the virtual environmment. For example,
+      Ensure you have `python>=3.7`. Then, you can create a new virtual environment by 
+      running the command:
 
-  .. code-block:: console
+      .. code-block:: console
 
-    $ python -m venv ~/my_envs/espresso 
+        $ python -m venv <path-to-new-env>/espresso
 
-  will create a virtual environment named :code:`espresso` and store everything within a sub-directory of your home-space named :code:`my_envs`.
+      where :code:`<path-to-new-env>` is your prefered location for storing information 
+      about this environment, and :code:`<env-name>` is your preferred name for the 
+      virtual environmment. For example,
 
-  To 'activate' or 'switch on' the virtual environment, run the command
-  
-  .. code-block:: console
+      .. code-block:: console
 
-    $ source <path-to-new-env>/<env-name>/bin/activate
+        $ python -m venv ~/my_envs/espresso 
 
-  At this point you effectively have a 'clean' Python installation. You can now install and use Espresso, following the instructions at step 2. When you are finished, you can run the command
-  
-  .. code-block:: console
+      will create a virtual environment named :code:`espresso` and store everything 
+      within a sub-directory of your home-space named :code:`my_envs`.
 
-    $ deactivate
+      To 'activate' or 'switch on' the virtual environment, run the command
+    
+      .. code-block:: console
 
-  and your system will return to its default state. If you want to use Espresso again, simply re-run the 'activate' step above; you do not need to repeat the installation process. Alternatively, you can remove Espresso and the virtual environment from your system by running
+        $ source <path-to-new-env>/<env-name>/bin/activate
 
-  .. code-block:: console
+      At this point you effectively have a 'clean' Python installation. You can now 
+      install and use Espresso, following the instructions at step 2. When you are 
+      finished, you can run the command
+      
+      .. code-block:: console
 
-    $ rm -rf <path-to-new-env>/<env-name>
+        $ deactivate
 
-.. tabbed:: virtualenv
+      and your system will return to its default state. If you want to use Espresso 
+      again, simply re-run the 'activate' step above; you do not need to repeat the 
+      installation process. Alternatively, you can remove Espresso and the virtual 
+      environment from your system by running
 
-  You can create a new virtual environment (using Python version 3.10) by running the command
+      .. code-block:: console
 
-  .. code-block:: console
+        $ rm -rf <path-to-new-env>/<env-name>
 
-    $ virtualenv <path-to-new-env>/<env-name> -p=3.10
-  
-  where :code:`<path-to-new-env>` is your prefered location for storing information about this environment, and :code:`<env-name>` is your preferred name for the virtual environmment. For example,
+    .. tab-item:: virtualenv
 
-  .. code-block:: console
+      You can create a new virtual environment (using Python version 3.10) by running 
+      the command
 
-    $ virtualenv ~/my_envs/espresso -p=3.10
+      .. code-block:: console
 
-  will create a virtual environment named :code:`espresso` and store everything within a sub-directory of your home-space named :code:`my_envs`.
+        $ virtualenv <path-to-new-env>/<env-name> -p=3.10
+      
+      where :code:`<path-to-new-env>` is your prefered location for storing information 
+      about this environment, and :code:`<env-name>` is your preferred name for the 
+      virtual environmment. For example,
 
-  To 'activate' or 'switch on' the virtual environment, run the command
+      .. code-block:: console
 
-  .. code-block:: console
+        $ virtualenv ~/my_envs/espresso -p=3.10
 
-    $ source <path-to-new-env>/<env-name>/bin/activate
+      will create a virtual environment named :code:`espresso` and store everything 
+      within a sub-directory of your home-space named :code:`my_envs`.
 
-  At this point you effectively have a 'clean' Python installation. You can now install and use Espresso, following the instructions at step 2. When you are finished, you can run the command
+      To 'activate' or 'switch on' the virtual environment, run the command
 
-  .. code-block:: console
+      .. code-block:: console
 
-    $ deactivate
+        $ source <path-to-new-env>/<env-name>/bin/activate
 
-  and your system will return to its default state. If you want to use Espresso again, simply re-run the 'activate' step above; you do not need to repeat the installation process. Alternatively, you can remove Espresso and the virtual environment from your system by running
+      At this point you effectively have a 'clean' Python installation. You can now 
+      install and use Espresso, following the instructions at step 2. When you are 
+      finished, you can run the command
 
-  .. code-block:: console
+      .. code-block:: console
 
-    $ rm -rf <path-to-new-env>/<env-name>
+        $ deactivate
 
-.. tabbed:: conda / mamba
+      and your system will return to its default state. If you want to use Espresso 
+      again, simply re-run the 'activate' step above; you do not need to repeat the 
+      installation process. Alternatively, you can remove Espresso and the virtual 
+      environment from your system by running
 
-  You can create a new virtual environment (using Python version 3.10) by running the command
+      .. code-block:: console
 
-  .. code-block:: console
+        $ rm -rf <path-to-new-env>/<env-name>
 
-    $ conda create -n <env-name> python=3.10
+    .. tab-item::  conda / mamba
 
-  where :code:`<env-name>` is your preferred name for the virtual environmment. For example,
+      You can create a new virtual environment (using Python version 3.10) by running 
+      the command
 
-  .. code-block:: console
+      .. code-block:: console
 
-    $ conda create -n espresso python=3.10
+        $ conda create -n <env-name> python=3.10
 
-  will create a virtual environment named :code:`espresso`.
-  
-  To 'activate' or 'switch on' the virtual environment, run the command
+      where :code:`<env-name>` is your preferred name for the virtual environmment. 
+      For example,
 
-  .. code-block:: console
+      .. code-block:: console
 
-    $ conda activate <env-name>
+        $ conda create -n espresso python=3.10
 
-  At this point you effectively have a 'clean' Python installation. You can now install and use Espresso, following the instructions at step 2. When you are finished, you can run the command
-  
-  .. code-block:: console
+      will create a virtual environment named :code:`espresso`.
+      
+      To 'activate' or 'switch on' the virtual environment, run the command
 
-    $ conda deactivate
+      .. code-block:: console
 
-  and your system will return to its default state. If you want to use Espresso again, simply re-run the 'activate' step above; you do not need to repeat the installation process. Alternatively, you can remove Espresso and the virtual environment from your system by running
-  
-  .. code-block:: console
+        $ conda activate <env-name>
+
+      At this point you effectively have a 'clean' Python installation. You can now 
+      install and use Espresso, following the instructions at step 2. When you are 
+      finished, you can run the command
+      
+      .. code-block:: console
+
+        $ conda deactivate
+
+      and your system will return to its default state. If you want to use Espresso 
+      again, simply re-run the 'activate' step above; you do not need to repeat the 
+      installation process. Alternatively, you can remove Espresso and the virtual 
+      environment from your system by running
+      
+      .. code-block:: console
+
+        $ conda env remove -n <env-name>
 
-    $ conda env remove -n <env-name>
 
 
 **Step 2**: Install Espresso
 
-.. tabbed:: pip
+.. tab-set::
+
+  .. tab-item:: pip
+
+    Espresso is available on `PyPI <https://pypi.org/project/geo-espresso/>`_, so for most 
+    users installation is as simple as:
+
+    .. code-block:: console
+
+      $ pip install geo-espresso
+
+  .. tab-item:: conda / mamba
+
+    This is work in progress and will be up soon.
+
+    .. Espresso is available on `conda-forge <https://anaconda.org/conda-forge/geo-espresso>`_,
+    .. so you can install it with ``mamba`` or ``conda``:
+
+    .. .. code-block:: console
+
+    ..   $ conda install -c conda-forge geo-espresso
+
+  .. tab-item:: From source
 
-  Espresso is available on `PyPI <https://pypi.org/project/geo-espresso/>`_, so for most users installation is as simple as:
+    You can build Espresso from source. You are most likely to want to do this if you 
+    want to work in 'developer mode', and make changes to Espresso's source code.
 
-  .. code-block:: console
+    .. code-block:: console
 
-    $ pip install geo-espresso
+      $ git clone https://github.com/inlab-geo/espresso.git
+      $ cd espresso
+      $ pip install -e .
 
-.. tabbed:: From source
+    The :code:`-e` flag ensures that the module is installed in editable mode; you can 
+    omit this if you do not intend to make any changes.
 
-  You can build Espresso from source. You are most likely to want to do this if you want to work in 'developer mode', and make changes to Espresso's source code.
 
-  .. code-block:: console
+If all has gone well, you should now be able to successfully :code:`import espresso` 
+within your Python interpreter or script.
 
-    $ git clone https://github.com/inlab-geo/espresso.git
-    $ cd espresso
-    $ pip install -e .
 
-  The :code:`-e` flag ensures that the module is installed in editable mode; you can omit this if you do not intend to make any changes.
+Container support
+-----------------
 
-If all has gone well, you should now be able to successfully :code:`import espresso` within your Python interpreter or script.
+Espresso and the InLab geoscience software ecosystem are now available in the form of 
+a handy container image. We kindly refer you to the 
+`inlab-containers guide <https://github.com/inlab-geo/inlab-containers#getting-started>`_
+to get started.
```

### Comparing `geo-espresso-0.2.2.dev0/docs/source/user_guide/usage.rst` & `geo-espresso-0.2.2.dev1/docs/source/user_guide/usage.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/docs/source/user_guide/why.rst` & `geo-espresso-0.2.2.dev1/docs/source/user_guide/why.rst`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/pyproject.toml` & `geo-espresso-0.2.2.dev1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/setup.py` & `geo-espresso-0.2.2.dev1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -93,27 +93,14 @@
 INSTALL_REQUIRES = [
     "numpy>=1.18",
     "scipy>=1.0.0",
     "matplotlib>=3.1",
     "tqdm>=4.0",
     "mpmath>=1.2.0",
 ]
-EXTRAS_REQUIRE = {
-    "doc": [
-        "sphinx", 
-        "sphinx-book-theme", 
-        "sphinx-panels", 
-        "sphinx-togglebutton",
-        "sphinx-autobuild",
-        "pypandoc",
-        "myst-nb",
-        "sphinxcontrib-mermaid",
-        "sphinx-copybutton",
-    ],
-}
 
 
 ########################## SETUP ######################################################
 class NullIO(io.StringIO):
     def write(self, txt):
        pass
 sys.stdout = NullIO()
@@ -132,15 +119,14 @@
         package_dir=PACKAGE_DIR,
         packages=PACKAGES,
         include_package_data=True,
         cmake_install_dir=CMAKE_INSTALL_DIR,
         cmake_args=CMAKE_ARGS,
         python_requires=PYTHON_REQUIRES,
         install_requires=INSTALL_REQUIRES,
-        extras_require=EXTRAS_REQUIRE,
     )
 except SystemExit as e:
     skbuild_error : skbuild.exceptions.SKBuildError = e.args[0]
     error_message = skbuild_error.args[0]
     error_message += "\n\nHint: search 'error' in current terminal session to find out the details. "
     # error_message += f"Here are some possible reasons that cause failure in building `{PACKAGE_NAME}`:"
     # error_message += "\n\t1. no Fortran compiler found -> install a Fortran compiler and ensure it's included in the path"
```

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/CMakeLists.txt` & `geo-espresso-0.2.2.dev1/src/espresso/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/__init__.py` & `geo-espresso-0.2.2.dev1/src/espresso/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_espresso_problem.py` & `geo-espresso-0.2.2.dev1/src/espresso/_espresso_problem.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/CMakeLists.txt` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/__init__.py` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/_fm_wavefront_tracker.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/cbmod.txt`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_InLab_lrt_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/receivers_crossb_nwt_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_InLab_lrt_s500.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/sources_crossb_nwt_s10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_InLab_lrt_s500_r36.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/datasets/ttimes/ttimes_crossb_nwt_s10_r10.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/fmst/compile` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/fmst/compile`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/fmst/src/fm2dss.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_fm_wavefront_tracker/waveTracker.py` & `geo-espresso-0.2.2.dev1/src/espresso/_fm_wavefront_tracker/waveTracker.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/_gravity_density.py` & `geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/_gravity_density.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_gravity_density/metadata.yml` & `geo-espresso-0.2.2.dev1/src/espresso/_gravity_density/metadata.yml`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/_utils.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/_utils.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/build.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/build.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/check_requires.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/check_requires.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/conftest.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/conftest.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/criteria.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/criteria.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/report.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/report.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/run_examples.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/run_examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,18 +195,18 @@
 
 def run_cmake_if_needed(prob_path, pre_build):
     if pre_build and "CMakeLists.txt" in os.listdir(prob_path):
         build_dir = pathlib.Path(prob_path) / "build"
         build_dir.mkdir(exist_ok=True)
         res1 = subprocess.call(["cmake", ".."], cwd=build_dir)
         if res1:
-            raise ChildProcessError("`cmake ..` failed in example_sub_folder")
+            raise ChildProcessError(f"`cmake ..` failed in {prob_path}/build")
         res2 = subprocess.call(["make"], cwd=build_dir)
         if res2:
-            raise ChildProcessError("`make` failed in example_sub_folder")
+            raise ChildProcessError(f"`make` failed in {prob_path}/build")
 
 
 def run_problems(
     problems, pre_build, timeout=None
 ) -> typing.Iterator[ResultsFromProblem]:
     for (prob_name, prob_path) in problems:
         prob_class_str = _utils.problem_name_to_class(prob_name)
```

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/test_examples.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/test_examples.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/build_package/validate.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/build_package/validate.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/doc_utils/gen_docs.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/doc_utils/gen_docs.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/_template/example_name.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/_template/example_name.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_machine/new_contribution/create_new_contrib.py` & `geo-espresso-0.2.2.dev1/src/espresso/_machine/new_contribution/create_new_contrib.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 with $f$ the frequency defined in Hz, the apparent resistivity $\rho_{app}$ defined in $\Omega m$ and the phase in degrees. 
 
 Details regarding the MT method can be found in Simpson and Bahr (2005) and Chave and Jones (2012).
 
 As mentioned earlier, the penetration of the EM fields depends on the frequency and the electrical conductivity of the Earth. Lower frequencies will penetrate deeper into the Earth, and conductive material will attenuate faster the EM fields. Therefore, depending on the frequency range available (and the composition of the Earth), the MT method can be used to map the distribution of the electrical conductivity into the Earth from tens of meters to hundreds of kilometres. Programs such as AusLAMP (for example Robertson et al., 2016) aims at imaging the Australia lithosphere and upper mantle using long period MT data, while Audio MT (AMT) and Broad Band MT (BBMT) data are used to image the upper crust (for example Simpson et al., 2021 or Jiang et al., 2022). 
 
-#### References:
+### References
 
 *Chave, A. D., & Jones, A. G. (Eds.). (2012). The magnetotelluric method: Theory and practice. Cambridge University Press.*
 
 *Jiang, W., Duan, J., Doublier, M., Clark, A., Schofield, A., Brodie, R. C., & Goodwin, J. (2022). Application of multiscale magnetotelluric data to mineral exploration: An example from the east Tennant region, Northern Australia. Geophysical Journal International, 229(3), 1628-1645.*
 
 *Pedersen, J., & Hermance, J. F. (1986). Least squares inversion of one-dimensional magnetotelluric data: An assessment of procedures employed by Brown University. Surveys in Geophysics, 8(2), 187-231.*
```

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/__init__.py` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/_magnetotelluric_1D.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/data/16-A_KN2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/example_01.py` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/example_01.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/field_MT.py` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/field_MT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.ipynb`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py` & `geo-espresso-0.2.2.dev1/src/espresso/_magnetotelluric_1D/examples/synthetic_AMT.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_pumping_test/_pumping_test.py` & `geo-espresso-0.2.2.dev1/src/espresso/_pumping_test/_pumping_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/CMakeLists.txt` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/CMakeLists.txt`

 * *Files 10% similar despite different names*

```diff
@@ -81,8 +81,12 @@
     LINK_FLAGS  '-Wl,-dylib,-undefined,dynamic_lookup')
   else()
     set_target_properties(${f2py_module_name} PROPERTIES
   LINK_FLAGS  '-Wl,--allow-shlib-undefined')
   endif()
 endif()
 
-install(TARGETS ${f2py_module_name} DESTINATION .)
+if(SKBUILD)
+  install(TARGETS ${f2py_module_name} DESTINATION _receiver_function/build)
+else()
+  install(TARGETS ${f2py_module_name} DESTINATION .)
+endif()
```

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RF.f90` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RF.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/dsvdcmp.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/dsvdcmp.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/four1.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/four1.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/qlayer.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/qlayer.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/ran3.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/ran3.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/svbksb.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/svbksb.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/theo.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/theo.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/theo_noise.f` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/theo_noise.f`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/RFsubs/voro2qmodel.f90`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/__init__.py` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/_receiver_function.py` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/_receiver_function.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,25 +10,18 @@
 
 class ReceiverFunction(EspressoProblem):
     """Forward simulation class
     """
 
     metadata = {
         "problem_title": "Receiver function",                # To be used in docs
-        "problem_short_description": \
-            """
-            'Receiver functions' are a class of seismic data used to study 
-            discontinuities (layering) in the Earth's crust. At each discontinuity, 
-            P-to-S conversions occur, introducing complexity in the waveform. By 
-            deconvolving horizontal- and vertical-channel waveforms from earthquakes 
-            at teleseismic distances, we can isolate information about these 
-            conversions, and hence learn about the crustal structure. This deconvolved 
-            signal is the receiver function, and has a highly non-linear dependence on 
-            the local crustal properties.
-            """,    # 1-3 sentences
+        "problem_short_description": (
+            "'Receiver functions' are a class of seismic data used to study "
+            "discontinuities (layering) in the Earth's crust"
+        ),    # 1-3 sentences
 
         "author_names": ["Malcolm Sambridge","Takuo Shibutani"],    # List of names e.g. author_names = ["Sally Smith", "Mark Brown"]
 
         "contact_name": "Malcolm Sambridge",         # Contact for contributor/maintainer of espresso example
         "contact_email": "Malcolm.Sambridge@anu.edu.au",
 
         "citations": [("Langston, C. A., Structure under Mount Rainer, Washington, inferred from teleseismic body waves, J. Geophys. Res., vol 84, 4749-4762, 1979.",
```

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_receiver_function/rf.py` & `geo-espresso-0.2.2.dev1/src/espresso/_receiver_function/rf.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_simple_regression/_simple_regression.py` & `geo-espresso-0.2.2.dev1/src/espresso/_simple_regression/_simple_regression.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_slug_test/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_slug_test/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_slug_test/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_slug_test/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_slug_test/_slug_test.py` & `geo-espresso-0.2.2.dev1/src/espresso/_slug_test/_slug_test.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/LICENCE` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/LICENCE`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/README.md` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/README.md`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/_xray_tracer.py` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/_xray_tracer.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/csiro_logo.png` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/csiro_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/example1.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/example1.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/example2.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/example2.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/example3.dat` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/example3.dat`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/_xray_tracer/data/inlab_logo.png` & `geo-espresso-0.2.2.dev1/src/espresso/_xray_tracer/data/inlab_logo.png`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/exceptions.py` & `geo-espresso-0.2.2.dev1/src/espresso/exceptions.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/list_problems.py` & `geo-espresso-0.2.2.dev1/src/espresso/list_problems.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,19 @@
     _all_names = [p.__name__ for p in _problems]
     return _all_names
 
 def list_problems(capabilities: list = None):
     """Returns a list of all Espresso problem classes"""
     if capabilities is None:
         return _all_problems
+    elif not isinstance(capabilities, (list, set, tuple)):
+        raise ValueError(
+            "pass in a list of capabilities, e.g. "
+            "`espresso.list_problems(['plot_model'])"
+        )
     else:
         _problem_names = []
         for p, c in _capability_matrix.items():
             ok = True
             for to_check in capabilities:
                 if not (to_check in c and c[to_check] == 1):
                     ok = False
@@ -77,17 +82,17 @@
         "inverse_covariance_matrix": 1,
         "jacobian": 1,
         "plot_model": 1,
         "plot_data": 1,
         "misfit": 1,
         "log_likelihood": 0,
         "log_prior": 0,
+        "set_start_mesh": 1,
         "set_obs_data": 1,
-        "set_start_model": 1,
-        "set_start_mesh": 1
+        "set_start_model": 1
     },
     "SlugTest": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
@@ -114,18 +119,18 @@
         "inverse_covariance_matrix": 0,
         "jacobian": 1,
         "plot_model": 1,
         "plot_data": 0,
         "misfit": 0,
         "log_likelihood": 0,
         "log_prior": 0,
-        "tmp_paths": 1,
+        "exe_fm2dss": 1,
         "clean_tmp_files": 1,
-        "tmp_files": 1,
-        "exe_fm2dss": 1
+        "tmp_paths": 1,
+        "tmp_files": 1
     },
     "GravityDensity": {
         "model_size": 1,
         "data_size": 1,
         "good_model": 1,
         "starting_model": 1,
         "data": 1,
```

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/utils/__init__.py` & `geo-espresso-0.2.2.dev1/src/espresso/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/espresso/utils/data_loader.py` & `geo-espresso-0.2.2.dev1/src/espresso/utils/data_loader.py`

 * *Files identical despite different names*

### Comparing `geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/PKG-INFO` & `geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geo-espresso
-Version: 0.2.2.dev0
+Version: 0.2.2.dev1
 Summary: Earth Science PRoblems for the Evaluation of Strategies, Solvers and Optimizers
 Author: InLab, Espresso development team
 Keywords: inversion,inference,python package,geoscience,geophysics
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python
@@ -18,15 +18,14 @@
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Fortran
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: License :: OSI Approved :: BSD License
 Classifier: License :: Other/Proprietary License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Provides-Extra: doc
 License-File: LICENCE
 
 # Espresso
 
 [![PyPI version](https://img.shields.io/pypi/v/geo-espresso?logo=pypi&style=flat-square&color=bde0fe&labelColor=f8f9fa)](https://pypi.org/project/geo-espresso/)
 [![build](https://img.shields.io/github/actions/workflow/status/inlab-geo/espresso/build_wheels.yml?branch=main&logo=githubactions&style=flat-square&color=ccd5ae&labelColor=f8f9fa)](https://github.com/inlab-geo/espresso/actions/workflows/build_wheels.yml)
 [![Documentation Status](https://img.shields.io/readthedocs/geo-espresso?logo=readthedocs&style=flat-square&color=fed9b7&labelColor=f8f9fa&logoColor=eaac8b)](https://geo-espresso.readthedocs.io/en/latest/?badge=latest)
@@ -44,15 +43,15 @@
 to another requires changing one line of code. 
 
 The Espresso project is a community effort - if you think it sounds useful,
 please consider contributing an example or two from your own research. The project
 is currently being coordinated by InLab, with support from the CoFI development
 team.
 
-For more information, please visit our documentation (coming soon).
+For more information, please visit [our documentation](geo-espresso.readthedocs.io).
 
 
 ## Installation
 
 ```console
 $ pip install geo-espresso
 ```
@@ -65,50 +64,45 @@
 
 Once installed, each test problem can be imported using the following command:
 
 ```python
 from espresso import <testproblem>
 ```
 
-Replace ``<testproblem>`` with one of the following currently available problems:
-
-- `SimpleRegression`
-- `XrayTomography`
-- `FmmTomography`
-- `PumpingTest`
-- `SlugTest`
-- `GravityDensity`
+Replace ``<testproblem>`` with an actual problem class in Espresso, such as
+`SimpleRegression` and `FmWavefrontTracker`. See 
+[here](https://geo-espresso.readthedocs.io/en/latest/user_guide/contrib/index.html) 
+for a full list of problems Espresso currently includes.
 
 Once a problem is imported, its main functions can be called using the same 
 structure for each problem. For instance:
 
 ```python
-from espresso import GravityDensity
+from espresso import FmWavefrontTracker
 
-problem = GravityDensity(example_number=1)
+problem = FmWavefrontTracker(example_number=1)
 model = problem.good_model
 data = problem.data
 pred = problem.forward(model)
 fig_model = problem.plot_model(model)
-fig_data = problem.plot_data(data, pred)
 ```
 
 You can access related metadata programatically:
 
 ```python
-print(GravityDensity.problem_title)
-print(GravityDensity.problem_short_description)
-print(GravityDensity.author_names)
+print(FmWavefrontTracker.metadata["problem_title"])
+print(FmWavefrontTracker.metadata["problem_short_description"])
+print(FmWavefrontTracker.metadata["author_names"])
 ```
 
 Other problem-specific parameters can be accessed through the problem instance. For instance:
 
 ```python
-print(problem.m)
-print(problem.rec_coords)
+print(problem.extent)
+print(problem.model_shape)
 ```
 
 Which additional values are set is highly problem-specific and we suggest to 
 consult the 
 [Espresso Documentation on the problems](https://geo-espresso.readthedocs.io/en/latest/user_guide/contrib/index.html).
```

### Comparing `geo-espresso-0.2.2.dev0/src/geo_espresso.egg-info/SOURCES.txt` & `geo-espresso-0.2.2.dev1/src/geo_espresso.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 CHANGELOG.md
 CMakeLists.txt
 LICENCE
 README.md
 pyproject.toml
 setup.py
 docs/Makefile
-docs/README.md
 docs/environment.yml
 docs/requirements.txt
 docs/source/conf.py
 docs/source/index.rst
 docs/source/_ext/generate_contrib_docs.py
 docs/source/_static/contrib_edit1.png
 docs/source/_static/contrib_fork.png
@@ -24,27 +23,29 @@
 docs/source/_static/style.css
 docs/source/_templates/layout.html
 docs/source/_templates/autosummary/base.rst
 docs/source/_templates/autosummary/class.rst
 docs/source/_templates/autosummary/exception.rst
 docs/source/_templates/autosummary/function.rst
 docs/source/_templates/autosummary/module.rst
-docs/source/contributor_guide/documentation.rst
+docs/source/contributor_guide/faq.rst
 docs/source/contributor_guide/github.rst
 docs/source/contributor_guide/index.rst
 docs/source/contributor_guide/new_contrib.rst
 docs/source/contributor_guide/setup.rst
+docs/source/contributor_guide/submit.rst
+docs/source/contributor_guide/video.rst
 docs/source/developer_guide/build.rst
-docs/source/developer_guide/changelog.md
+docs/source/developer_guide/ci.rst
 docs/source/developer_guide/deploy.rst
 docs/source/developer_guide/develop.rst
 docs/source/developer_guide/index.rst
 docs/source/developer_guide/licence.rst
 docs/source/developer_guide/repository.rst
-docs/source/developer_guide/sphinx.rst
+docs/source/user_guide/changelog.md
 docs/source/user_guide/examples.rst
 docs/source/user_guide/faq.rst
 docs/source/user_guide/index.rst
 docs/source/user_guide/installation.rst
 docs/source/user_guide/usage.rst
 docs/source/user_guide/why.rst
 docs/source/user_guide/api/index.rst
@@ -76,15 +77,14 @@
 src/espresso/_gravity_density/README.md
 src/espresso/_gravity_density/__init__.py
 src/espresso/_gravity_density/_gravity_density.py
 src/espresso/_gravity_density/metadata.yml
 src/espresso/_gravity_density/data/__init__.py
 src/espresso/_gravity_density/data/gravmodel1.txt
 src/espresso/_gravity_density/data/testdata.txt
-src/espresso/_machine/README.md
 src/espresso/_machine/build_package/_utils.py
 src/espresso/_machine/build_package/build.py
 src/espresso/_machine/build_package/check_requires.py
 src/espresso/_machine/build_package/conftest.py
 src/espresso/_machine/build_package/criteria.py
 src/espresso/_machine/build_package/report.py
 src/espresso/_machine/build_package/run_examples.py
```

