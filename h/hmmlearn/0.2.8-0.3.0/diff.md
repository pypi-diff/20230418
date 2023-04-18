# Comparing `tmp/hmmlearn-0.2.8.tar.gz` & `tmp/hmmlearn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hmmlearn-0.2.8.tar", last modified: Mon Sep 26 19:23:19 2022, max compression
+gzip compressed data, was "hmmlearn-0.3.0.tar", last modified: Tue Apr 18 18:56:35 2023, max compression
```

## Comparing `hmmlearn-0.2.8.tar` & `hmmlearn-0.3.0.tar`

### file list

```diff
@@ -1,66 +1,74 @@
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.496702 hmmlearn-0.2.8/
--rw-r--r--   0 antony    (1000) users      (100)       15 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/.codecov.yml
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.483369 hmmlearn-0.2.8/.github/
--rw-r--r--   0 antony    (1000) users      (100)     1128 2021-10-21 19:42:31.000000 hmmlearn-0.2.8/.github/ISSUE_TEMPLATE.md
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.483369 hmmlearn-0.2.8/.github/workflows/
--rw-r--r--   0 antony    (1000) users      (100)     3434 2022-09-26 18:56:25.000000 hmmlearn-0.2.8/.github/workflows/build.yml
--rw-r--r--   0 antony    (1000) users      (100)      199 2019-12-15 20:47:22.000000 hmmlearn-0.2.8/.gitignore
--rw-r--r--   0 antony    (1000) users      (100)       86 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/.readthedocs.yaml
--rw-r--r--   0 antony    (1000) users      (100)      502 2022-05-24 20:16:02.000000 hmmlearn-0.2.8/AUTHORS.rst
--rw-r--r--   0 antony    (1000) users      (100)     5970 2022-09-26 16:14:20.000000 hmmlearn-0.2.8/CHANGES.rst
--rw-r--r--   0 antony    (1000) users      (100)     1527 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/LICENSE.txt
--rw-r--r--   0 antony    (1000) users      (100)     2463 2022-09-26 19:23:19.496702 hmmlearn-0.2.8/PKG-INFO
--rw-r--r--   0 antony    (1000) users      (100)     1775 2021-11-06 21:15:34.000000 hmmlearn-0.2.8/README.rst
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.483369 hmmlearn-0.2.8/doc/
--rw-r--r--   0 antony    (1000) users      (100)       29 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/doc/.gitignore
--rw-r--r--   0 antony    (1000) users      (100)      588 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/doc/Makefile
--rw-r--r--   0 antony    (1000) users      (100)      750 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/doc/make.bat
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.486703 hmmlearn-0.2.8/doc/source/
--rw-r--r--   0 antony    (1000) users      (100)    19968 2021-01-23 18:03:57.000000 hmmlearn-0.2.8/doc/source/GMMHMM.rst
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.486703 hmmlearn-0.2.8/doc/source/_static/
--rw-r--r--   0 antony    (1000) users      (100)       84 2021-08-22 20:54:59.000000 hmmlearn-0.2.8/doc/source/_static/hide_some_gallery_elements.css
--rw-r--r--   0 antony    (1000) users      (100)      910 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/doc/source/api.rst
--rw-r--r--   0 antony    (1000) users      (100)       31 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/doc/source/changelog.rst
--rw-r--r--   0 antony    (1000) users      (100)     1356 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/doc/source/conf.py
--rw-r--r--   0 antony    (1000) users      (100)      651 2021-07-04 19:25:41.000000 hmmlearn-0.2.8/doc/source/index.rst
--rw-r--r--   0 antony    (1000) users      (100)     8642 2022-09-26 15:33:07.000000 hmmlearn-0.2.8/doc/source/tutorial.rst
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.490036 hmmlearn-0.2.8/examples/
--rw-r--r--   0 antony    (1000) users      (100)       33 2016-01-24 02:48:31.000000 hmmlearn-0.2.8/examples/README.txt
--rw-r--r--   0 antony    (1000) users      (100)     5194 2022-09-26 15:24:39.000000 hmmlearn-0.2.8/examples/plot_casino.py
--rw-r--r--   0 antony    (1000) users      (100)     3891 2022-07-04 22:09:09.000000 hmmlearn-0.2.8/examples/plot_hmm_sampling_and_decoding.py
--rw-r--r--   0 antony    (1000) users      (100)     4372 2022-09-26 15:33:16.000000 hmmlearn-0.2.8/examples/plot_multinomial_hmm.py
--rw-r--r--   0 antony    (1000) users      (100)     4286 2022-07-04 22:09:09.000000 hmmlearn-0.2.8/examples/plot_poisson_hmm.py
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.480036 hmmlearn-0.2.8/lib/
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.493369 hmmlearn-0.2.8/lib/hmmlearn/
--rw-r--r--   0 antony    (1000) users      (100)       16 2019-01-31 20:31:01.000000 hmmlearn-0.2.8/lib/hmmlearn/.gitignore
--rw-r--r--   0 antony    (1000) users      (100)      457 2022-05-16 22:18:33.000000 hmmlearn-0.2.8/lib/hmmlearn/__init__.py
--rw-r--r--   0 antony    (1000) users      (100)     3672 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/lib/hmmlearn/_utils.py
--rw-r--r--   0 antony    (1000) users      (100)      176 2022-09-26 19:23:18.000000 hmmlearn-0.2.8/lib/hmmlearn/_version.py
--rw-r--r--   0 antony    (1000) users      (100)    31925 2022-09-26 15:34:11.000000 hmmlearn-0.2.8/lib/hmmlearn/base.py
--rw-r--r--   0 antony    (1000) users      (100)    55635 2022-09-26 15:34:11.000000 hmmlearn-0.2.8/lib/hmmlearn/hmm.py
--rw-r--r--   0 antony    (1000) users      (100)     3978 2022-07-04 22:09:21.000000 hmmlearn-0.2.8/lib/hmmlearn/stats.py
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.496702 hmmlearn-0.2.8/lib/hmmlearn/tests/
--rw-r--r--   0 antony    (1000) users      (100)     1961 2022-07-10 19:14:47.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/__init__.py
--rw-r--r--   0 antony    (1000) users      (100)      313 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/conftest.py
--rw-r--r--   0 antony    (1000) users      (100)     9367 2022-07-10 19:14:47.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_base.py
--rw-r--r--   0 antony    (1000) users      (100)     6023 2022-07-10 19:14:47.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_categorical_hmm.py
--rw-r--r--   0 antony    (1000) users      (100)    13826 2022-09-26 15:34:11.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_gaussian_hmm.py
--rw-r--r--   0 antony    (1000) users      (100)     4088 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_gmm_hmm.py
--rw-r--r--   0 antony    (1000) users      (100)    14112 2022-07-04 22:09:09.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_gmm_hmm_multisequence.py
--rw-r--r--   0 antony    (1000) users      (100)     9410 2022-07-10 19:14:47.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_gmm_hmm_new.py
--rw-r--r--   0 antony    (1000) users      (100)     6662 2022-07-10 19:14:47.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_multinomial_hmm.py
--rw-r--r--   0 antony    (1000) users      (100)     2843 2022-07-10 19:14:47.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_poisson_hmm.py
--rw-r--r--   0 antony    (1000) users      (100)     1472 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/lib/hmmlearn/tests/test_utils.py
--rw-r--r--   0 antony    (1000) users      (100)     3011 2022-09-26 15:34:11.000000 hmmlearn-0.2.8/lib/hmmlearn/utils.py
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.493369 hmmlearn-0.2.8/lib/hmmlearn.egg-info/
--rw-r--r--   0 antony    (1000) users      (100)     2463 2022-09-26 19:23:18.000000 hmmlearn-0.2.8/lib/hmmlearn.egg-info/PKG-INFO
--rw-r--r--   0 antony    (1000) users      (100)     1342 2022-09-26 19:23:19.000000 hmmlearn-0.2.8/lib/hmmlearn.egg-info/SOURCES.txt
--rw-r--r--   0 antony    (1000) users      (100)        1 2022-09-26 19:23:18.000000 hmmlearn-0.2.8/lib/hmmlearn.egg-info/dependency_links.txt
--rw-r--r--   0 antony    (1000) users      (100)      125 2022-09-26 19:23:19.000000 hmmlearn-0.2.8/lib/hmmlearn.egg-info/requires.txt
--rw-r--r--   0 antony    (1000) users      (100)       10 2022-09-26 19:23:19.000000 hmmlearn-0.2.8/lib/hmmlearn.egg-info/top_level.txt
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.496702 hmmlearn-0.2.8/scripts/
--rw-r--r--   0 antony    (1000) users      (100)     8715 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/scripts/benchmark.py
--rw-r--r--   0 antony    (1000) users      (100)      220 2022-09-26 19:23:19.496702 hmmlearn-0.2.8/setup.cfg
--rw-r--r--   0 antony    (1000) users      (100)     2660 2022-05-17 21:24:13.000000 hmmlearn-0.2.8/setup.py
-drwxr-xr-x   0 antony    (1000) users      (100)        0 2022-09-26 19:23:19.496702 hmmlearn-0.2.8/src/
--rw-r--r--   0 antony    (1000) users      (100)    11273 2022-07-04 22:09:21.000000 hmmlearn-0.2.8/src/_hmmc.cpp
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.442906 hmmlearn-0.3.0/
+-rw-r--r--   0 antony     (501) staff       (20)       15 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/.codecov.yml
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.422745 hmmlearn-0.3.0/.github/
+-rw-r--r--   0 antony     (501) staff       (20)     1128 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/.github/ISSUE_TEMPLATE.md
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.423073 hmmlearn-0.3.0/.github/workflows/
+-rw-r--r--   0 antony     (501) staff       (20)     1165 2023-04-18 18:00:19.000000 hmmlearn-0.3.0/.github/workflows/build.yml
+-rw-r--r--   0 antony     (501) staff       (20)      199 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/.gitignore
+-rw-r--r--   0 antony     (501) staff       (20)       86 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/.readthedocs.yaml
+-rw-r--r--   0 antony     (501) staff       (20)      502 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/AUTHORS.rst
+-rw-r--r--   0 antony     (501) staff       (20)     6532 2023-04-18 15:13:23.000000 hmmlearn-0.3.0/CHANGES.rst
+-rw-r--r--   0 antony     (501) staff       (20)     1527 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/LICENSE.txt
+-rw-r--r--   0 antony     (501) staff       (20)     2538 2023-04-18 18:56:35.443002 hmmlearn-0.3.0/PKG-INFO
+-rw-r--r--   0 antony     (501) staff       (20)     1824 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/README.rst
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.424804 hmmlearn-0.3.0/doc/
+-rw-r--r--   0 antony     (501) staff       (20)       29 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/.gitignore
+-rw-r--r--   0 antony     (501) staff       (20)      588 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/Makefile
+-rw-r--r--   0 antony     (501) staff       (20)      750 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/make.bat
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.427563 hmmlearn-0.3.0/doc/source/
+-rw-r--r--   0 antony     (501) staff       (20)    19968 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/source/GMMHMM.rst
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.428013 hmmlearn-0.3.0/doc/source/_static/
+-rw-r--r--   0 antony     (501) staff       (20)       84 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/source/_static/hide_some_gallery_elements.css
+-rw-r--r--   0 antony     (501) staff       (20)     1838 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/source/api.rst
+-rw-r--r--   0 antony     (501) staff       (20)       31 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/source/changelog.rst
+-rw-r--r--   0 antony     (501) staff       (20)     1356 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/source/conf.py
+-rw-r--r--   0 antony     (501) staff       (20)      651 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/doc/source/index.rst
+-rw-r--r--   0 antony     (501) staff       (20)     8750 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/doc/source/tutorial.rst
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.430457 hmmlearn-0.3.0/examples/
+-rw-r--r--   0 antony     (501) staff       (20)       33 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/examples/README.txt
+-rw-r--r--   0 antony     (501) staff       (20)     5194 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/examples/plot_casino.py
+-rw-r--r--   0 antony     (501) staff       (20)     2656 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/examples/plot_gaussian_model_selection.py
+-rw-r--r--   0 antony     (501) staff       (20)     3891 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/examples/plot_hmm_sampling_and_decoding.py
+-rw-r--r--   0 antony     (501) staff       (20)     4372 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/examples/plot_multinomial_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)     4249 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/examples/plot_poisson_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)     6567 2023-02-27 18:04:22.000000 hmmlearn-0.3.0/examples/plot_variational_inference.py
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.418558 hmmlearn-0.3.0/lib/
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.435299 hmmlearn-0.3.0/lib/hmmlearn/
+-rw-r--r--   0 antony     (501) staff       (20)       16 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/.gitignore
+-rw-r--r--   0 antony     (501) staff       (20)      457 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/__init__.py
+-rw-r--r--   0 antony     (501) staff       (20)    15957 2023-02-06 16:53:57.000000 hmmlearn-0.3.0/lib/hmmlearn/_emissions.py
+-rw-r--r--   0 antony     (501) staff       (20)     3559 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/_kl_divergence.py
+-rw-r--r--   0 antony     (501) staff       (20)     3256 2023-02-10 09:51:52.000000 hmmlearn-0.3.0/lib/hmmlearn/_utils.py
+-rw-r--r--   0 antony     (501) staff       (20)      160 2023-04-18 18:56:35.000000 hmmlearn-0.3.0/lib/hmmlearn/_version.py
+-rw-r--r--   0 antony     (501) staff       (20)    48667 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/lib/hmmlearn/base.py
+-rw-r--r--   0 antony     (501) staff       (20)    42047 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/lib/hmmlearn/hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)     3978 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/stats.py
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.442021 hmmlearn-0.3.0/lib/hmmlearn/tests/
+-rw-r--r--   0 antony     (501) staff       (20)     3791 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/__init__.py
+-rw-r--r--   0 antony     (501) staff       (20)      313 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/conftest.py
+-rw-r--r--   0 antony     (501) staff       (20)     9365 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_base.py
+-rw-r--r--   0 antony     (501) staff       (20)     6565 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_categorical_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)    14766 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_gaussian_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)     4024 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_gmm_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)    14112 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_gmm_hmm_multisequence.py
+-rw-r--r--   0 antony     (501) staff       (20)    10208 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_gmm_hmm_new.py
+-rw-r--r--   0 antony     (501) staff       (20)     1707 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_kl_divergence.py
+-rw-r--r--   0 antony     (501) staff       (20)     6802 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_multinomial_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)     3642 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_poisson_hmm.py
+-rw-r--r--   0 antony     (501) staff       (20)     1472 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_utils.py
+-rw-r--r--   0 antony     (501) staff       (20)    11429 2023-02-27 18:04:22.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_variational_categorical.py
+-rw-r--r--   0 antony     (501) staff       (20)    21354 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/lib/hmmlearn/tests/test_variational_gaussian.py
+-rw-r--r--   0 antony     (501) staff       (20)     1831 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/lib/hmmlearn/utils.py
+-rw-r--r--   0 antony     (501) staff       (20)    34109 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/lib/hmmlearn/vhmm.py
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.437223 hmmlearn-0.3.0/lib/hmmlearn.egg-info/
+-rw-r--r--   0 antony     (501) staff       (20)     2538 2023-04-18 18:56:35.000000 hmmlearn-0.3.0/lib/hmmlearn.egg-info/PKG-INFO
+-rw-r--r--   0 antony     (501) staff       (20)     1642 2023-04-18 18:56:35.000000 hmmlearn-0.3.0/lib/hmmlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 antony     (501) staff       (20)        1 2023-04-18 18:56:35.000000 hmmlearn-0.3.0/lib/hmmlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 antony     (501) staff       (20)      134 2023-04-18 18:56:35.000000 hmmlearn-0.3.0/lib/hmmlearn.egg-info/requires.txt
+-rw-r--r--   0 antony     (501) staff       (20)       10 2023-04-18 18:56:35.000000 hmmlearn-0.3.0/lib/hmmlearn.egg-info/top_level.txt
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.442393 hmmlearn-0.3.0/scripts/
+-rw-r--r--   0 antony     (501) staff       (20)     8715 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/scripts/benchmark.py
+-rw-r--r--   0 antony     (501) staff       (20)      181 2023-04-18 18:56:35.443393 hmmlearn-0.3.0/setup.cfg
+-rw-r--r--   0 antony     (501) staff       (20)     2672 2023-02-06 15:22:19.000000 hmmlearn-0.3.0/setup.py
+drwxr-xr-x   0 antony     (501) staff       (20)        0 2023-04-18 18:56:35.442691 hmmlearn-0.3.0/src/
+-rw-r--r--   0 antony     (501) staff       (20)    11210 2023-04-14 22:11:59.000000 hmmlearn-0.3.0/src/_hmmc.cpp
```

### Comparing `hmmlearn-0.2.8/.github/ISSUE_TEMPLATE.md` & `hmmlearn-0.3.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/CHANGES.rst` & `hmmlearn-0.3.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 hmmlearn Changelog
 ==================
 
 Here you can see the full list of changes between each hmmlearn release.
 
+Version 0.3.0
+-------------
+
+Released on April 18th, 2023.
+
+- Introduce learning HMMs with Variational Inference.  Support
+  Gaussian and Categorical Emissions.  This feature is provisional and subject
+  to further changes.
+- Deprecated support for inputs of shape other than ``(n_samples, 1)`` for
+  categorical HMMs.
+- Removed the deprecated ``iter_from_X_lengths`` and ``log_mask_zero``;
+  ``lengths`` arrays that do not sum up to the entire array length are no
+  longer supported.
+- Support variable ``n_trials`` in ``MultinomialHMM``, except for sampling.
+
 Version 0.2.8
 -------------
 
 Released on September 26th, 2022.
 
 - The ``PoissonHMM`` class was added with an example use case.
 - For ``MultinomialHMM``, parameters after ``transmat_prior`` are now
```

### Comparing `hmmlearn-0.2.8/LICENSE.txt` & `hmmlearn-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/PKG-INFO` & `hmmlearn-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmlearn
-Version: 0.2.8
+Version: 0.3.0
 Summary: Hidden Markov Models in Python with scikit-learn like API
 Home-page: https://github.com/hmmlearn/hmmlearn
 Maintainer: Antony Lee
 License: new BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved
 Classifier: Intended Audience :: Developers
@@ -14,35 +14,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
+License-File: AUTHORS.rst
 
 hmmlearn
 ========
 
 | |GitHub| |PyPI|
 | |Read the Docs| |Build| |CodeCov|
 
 .. |GitHub|
    image:: https://img.shields.io/badge/github-hmmlearn%2Fhmmlearn-brightgreen
    :target: https://github.com/hmmlearn/hmmlearn
 .. |PyPI|
-   image:: https://img.shields.io/pypi/v/hmmlearn.svg
+   image:: https://img.shields.io/pypi/v/hmmlearn.svg?color=brightgreen
    :target: https://pypi.python.org/pypi/hmmlearn
 .. |Read the Docs|
    image:: https://readthedocs.org/projects/hmmlearn/badge/?version=latest
    :target: http://hmmlearn.readthedocs.io/en/latest/?badge=latest
 .. |Build|
-   image:: https://img.shields.io/github/workflow/status/hmmlearn/hmmlearn/build
+   image:: https://img.shields.io/github/actions/workflow/status/hmmlearn/hmmlearn/build.yml?branch=main
    :target: https://github.com/hmmlearn/hmmlearn/actions
 .. |CodeCov|
-   image:: https://codecov.io/gh/hmmlearn/hmmlearn/master.svg
+   image:: https://img.shields.io/codecov/c/github/hmmlearn/hmmlearn
    :target: https://codecov.io/gh/hmmlearn/hmmlearn
 
 hmmlearn is a set of algorithms for **unsupervised** learning and inference
 of Hidden Markov Models. For supervised learning learning of HMMs and similar
 models see seqlearn_.
 
 .. _seqlearn: https://github.com/larsmans/seqlearn
```

### Comparing `hmmlearn-0.2.8/README.rst` & `hmmlearn-0.3.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 | |GitHub| |PyPI|
 | |Read the Docs| |Build| |CodeCov|
 
 .. |GitHub|
    image:: https://img.shields.io/badge/github-hmmlearn%2Fhmmlearn-brightgreen
    :target: https://github.com/hmmlearn/hmmlearn
 .. |PyPI|
-   image:: https://img.shields.io/pypi/v/hmmlearn.svg
+   image:: https://img.shields.io/pypi/v/hmmlearn.svg?color=brightgreen
    :target: https://pypi.python.org/pypi/hmmlearn
 .. |Read the Docs|
    image:: https://readthedocs.org/projects/hmmlearn/badge/?version=latest
    :target: http://hmmlearn.readthedocs.io/en/latest/?badge=latest
 .. |Build|
-   image:: https://img.shields.io/github/workflow/status/hmmlearn/hmmlearn/build
+   image:: https://img.shields.io/github/actions/workflow/status/hmmlearn/hmmlearn/build.yml?branch=main
    :target: https://github.com/hmmlearn/hmmlearn/actions
 .. |CodeCov|
-   image:: https://codecov.io/gh/hmmlearn/hmmlearn/master.svg
+   image:: https://img.shields.io/codecov/c/github/hmmlearn/hmmlearn
    :target: https://codecov.io/gh/hmmlearn/hmmlearn
 
 hmmlearn is a set of algorithms for **unsupervised** learning and inference
 of Hidden Markov Models. For supervised learning learning of HMMs and similar
 models see seqlearn_.
 
 .. _seqlearn: https://github.com/larsmans/seqlearn
```

### Comparing `hmmlearn-0.2.8/doc/Makefile` & `hmmlearn-0.3.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/doc/make.bat` & `hmmlearn-0.3.0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/doc/source/GMMHMM.rst` & `hmmlearn-0.3.0/doc/source/GMMHMM.rst`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/doc/source/api.rst` & `hmmlearn-0.3.0/doc/source/api.rst`

 * *Files 15% similar despite different names*

```diff
@@ -12,22 +12,38 @@
 -------------
 
 ConvergenceMonitor
 ~~~~~~~~~~~~~~~~~~
 
 .. autoclass:: hmmlearn.base.ConvergenceMonitor
 
+_AbstractHMM
+~~~~~~~~~~~~
+
+.. autoclass:: hmmlearn.base._AbstractHMM
+   :exclude-members: set_params, get_params, _get_param_names
+   :private-members:
+   :no-inherited-members:
+
 BaseHMM
-~~~~~~~~
+~~~~~~~
 
 .. autoclass:: hmmlearn.base.BaseHMM
    :exclude-members: set_params, get_params, _get_param_names
    :private-members:
    :no-inherited-members:
 
+VariationalBaseHMM
+~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: hmmlearn.base.VariationalBaseHMM
+   :exclude-members: set_params, get_params, _get_param_names
+   :private-members:
+   :no-inherited-members:
+
 hmmlearn.hmm
 ------------
 
 GaussianHMM
 ~~~~~~~~~~~
 
 .. autoclass:: hmmlearn.hmm.GaussianHMM
@@ -40,7 +56,35 @@
    :exclude-members: set_params, get_params
 
 MultinomialHMM
 ~~~~~~~~~~~~~~
 
 .. autoclass:: hmmlearn.hmm.MultinomialHMM
    :exclude-members: set_params, get_params
+
+CategoricalHMM
+~~~~~~~~~~~~~~
+
+.. autoclass:: hmmlearn.hmm.CategoricalHMM
+   :exclude-members: set_params, get_params
+
+PoissonHMM
+~~~~~~~~~~
+
+.. autoclass:: hmmlearn.hmm.PoissonHMM
+   :exclude-members: set_params, get_params
+
+
+hmmlearn.vhmm
+-------------
+
+VariationalCategoricalHMM
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: hmmlearn.vhmm.VariationalCategoricalHMM
+   :exclude-members: set_params, get_params
+
+VariationalGaussianHMM
+~~~~~~~~~~~~~~~~~~~~~~
+
+.. autoclass:: hmmlearn.vhmm.VariationalGaussianHMM
+   :exclude-members: set_params, get_params
```

### Comparing `hmmlearn-0.2.8/doc/source/conf.py` & `hmmlearn-0.3.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/doc/source/index.rst` & `hmmlearn-0.3.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/doc/source/tutorial.rst` & `hmmlearn-0.3.0/doc/source/tutorial.rst`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,21 @@
 
 Available models
 ----------------
 
 .. autosummary::
    :nosignatures:
 
+   hmm.CategoricalHMM
    hmm.GaussianHMM
    hmm.GMMHMM
    hmm.MultinomialHMM
+   hmm.PoissonHMM
+   vhmm.VariationalCategoricalHMM
+   vhmm.VariationalGaussianHMM
 
 :ref:`Read on <customizing>` for details on how to implement a HMM with a
 custom emission probability.
 
 Building HMM and generating samples
 -----------------------------------
 
@@ -89,15 +93,15 @@
 If any of the required parameters are missing, :meth:`~.BaseHMM.sample`
 will raise an exception:
 
 >>> model = hmm.GaussianHMM(n_components=3)
 >>> X, Z = model.sample(100)
 Traceback (most recent call last):
     ...
-sklearn.exceptions.NotFittedError: This GaussianHMM instance is not fitted yet. Call 'fit' with appropriate arguments before using this method.
+sklearn.exceptions.NotFittedError: This GaussianHMM instance is not fitted yet. Call 'fit' with appropriate arguments before using this estimator.
 
 Fixing parameters
 -----------------
 
 Each HMM parameter has a character code which can be used to customize its
 initialization and estimation.  The EM algorithm needs a starting point to
 proceed, thus prior to training each parameter is assigned a value
```

### Comparing `hmmlearn-0.2.8/examples/plot_casino.py` & `hmmlearn-0.3.0/examples/plot_casino.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/examples/plot_hmm_sampling_and_decoding.py` & `hmmlearn-0.3.0/examples/plot_hmm_sampling_and_decoding.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/examples/plot_multinomial_hmm.py` & `hmmlearn-0.3.0/examples/plot_multinomial_hmm.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
   categories instead of the binary success/failure outcome; a Categorical HMM
   has the emission probabilities for each component parametrized by Categorical
   distributions.
 
 - a Multinomial__ distribution models the outcome of ``n_trials`` independent
   rolls of die, each with ``n_features`` possible values; i.e.
 
-  - when ``n_trials = 1`` and ``n_features = 1``, it is a Bernoulli
+  - when ``n_trials = 1`` and ``n_features = 2``, it is a Bernoulli
     distribution,
   - when ``n_trials > 1`` and ``n_features = 2``, it is a Binomial
     distribution,
   - when ``n_trials = 1`` and ``n_features > 2``, it is a Categorical
     distribution.
 
 The emission probabilities for each component of a Multinomial HMM are
```

### Comparing `hmmlearn-0.2.8/examples/plot_poisson_hmm.py` & `hmmlearn-0.3.0/examples/plot_poisson_hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,13 @@
 prop_per_state = model.predict_proba(earthquakes[:, None]).mean(axis=0)
 
 # earthquake counts to plot
 bins = sorted(np.unique(earthquakes))
 
 fig, ax = plt.subplots()
 ax.hist(earthquakes, bins=bins, density=True)
-ax.plot(bins, np.dot(poisson.pmf(bins, model.lambdas_).T,
-                     prop_per_state[:, None]))
+ax.plot(bins, poisson.pmf(bins, model.lambdas_).T @ prop_per_state)
 ax.set_title('Histogram of Earthquakes with Fitted Poisson States')
 ax.set_xlabel('Number of Earthquakes')
 ax.set_ylabel('Proportion')
 
 plt.show()
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/_utils.py` & `hmmlearn-0.3.0/lib/hmmlearn/_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """Private utilities."""
 
 import warnings
 
 import numpy as np
-from sklearn.utils.validation import NotFittedError
+
+
+def logdet(a):
+    sign, logdet = np.linalg.slogdet(a)
+    if (sign < 0).any():
+        warnings.warn("invalid value encountered in log", RuntimeWarning)
+        return np.where(sign < 0, np.nan, logdet)
+    else:
+        return logdet
 
 
 def split_X_lengths(X, lengths):
     if lengths is None:
         return [X]
     else:
         cs = np.cumsum(lengths)
         n_samples = len(X)
-        if cs[-1] > n_samples:
+        if cs[-1] != n_samples:
             raise ValueError(
-                f"more than {n_samples} samples in lengths array {lengths}")
-        elif cs[-1] != n_samples:
-            warnings.warn(
-                f"less that {n_samples} samples in lengths array {lengths}; "
-                f"support for silently dropping samples is deprecated and "
-                f"will be removed", DeprecationWarning, stacklevel=3)
+                f"lengths array {lengths} doesn't sum to {n_samples} samples")
         return np.split(X, cs)[:-1]
 
 
 # Copied from scikit-learn 0.19.
 def _validate_covars(covars, covariance_type, n_components):
     """Do basic checks on matrix covariance sizes and values."""
     from scipy import linalg
@@ -75,16 +78,7 @@
         cv = np.tile(np.diag(tied_cv), (n_components, 1))
     elif covariance_type == 'full':
         cv = np.tile(tied_cv, (n_components, 1, 1))
     else:
         raise ValueError("covariance_type must be one of " +
                          "'spherical', 'tied', 'diag', 'full'")
     return cv
-
-
-# Adapted from scikit-learn 0.21.
-def check_is_fitted(estimator, attribute):
-    if not hasattr(estimator, attribute):
-        raise NotFittedError(
-            "This %s instance is not fitted yet. Call 'fit' with "
-            "appropriate arguments before using this method."
-            % type(estimator).__name__)
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/base.py` & `hmmlearn-0.3.0/lib/hmmlearn/base.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 import string
 import sys
 from collections import deque
 
 import numpy as np
 from scipy import linalg, special
 from sklearn.base import BaseEstimator
-from sklearn.utils import check_array, check_random_state
+from sklearn.utils.validation import (
+    check_array, check_is_fitted, check_random_state)
 
-from . import _hmmc, _utils
+from . import _hmmc, _kl_divergence as _kl, _utils
 from .utils import normalize, log_normalize
 
 
 _log = logging.getLogger(__name__)
 #: Supported decoder algorithms.
 DECODER_ALGORITHMS = frozenset(("viterbi", "map"))
 
@@ -48,15 +49,15 @@
     >>>
     >>> model = hmm.GaussianHMM(n_components=2, tol=5, verbose=True)
     >>> model.monitor_ = ThresholdMonitor(model.monitor_.tol,
     ...                                   model.monitor_.n_iter,
     ...                                   model.monitor_.verbose)
     """
 
-    _template = "{iter:>10d} {log_prob:>16.4f} {delta:>+16.4f}"
+    _template = "{iter:>10d} {log_prob:>16.8f} {delta:>+16.8f}"
 
     def __init__(self, tol, n_iter, verbose):
         """
         Parameters
         ----------
         tol : double
             Convergence threshold.  EM has converged either if the maximum
@@ -72,15 +73,15 @@
         self.verbose = verbose
         self.history = deque()
         self.iter = 0
 
     def __repr__(self):
         class_name = self.__class__.__name__
         params = sorted(dict(vars(self), history=list(self.history)).items())
-        return (f"{class_name}(\n"
+        return ("{}(\n".format(class_name)
                 + "".join(map("    {}={},\n".format, *zip(*params)))
                 + ")")
 
     def _reset(self):
         """Reset the monitor's state."""
         self.iter = 0
         self.history.clear()
@@ -101,69 +102,47 @@
             in the current iteration.
         """
         if self.verbose:
             delta = log_prob - self.history[-1] if self.history else np.nan
             message = self._template.format(
                 iter=self.iter + 1, log_prob=log_prob, delta=delta)
             print(message, file=sys.stderr)
+
+        # Allow for some wiggleroom based on precision.
+        precision = np.finfo(float).eps ** (1/2)
+        if self.history and (log_prob - self.history[-1]) < -precision:
+            delta = log_prob - self.history[-1]
+            _log.warning(f"Model is not converging.  Current: {log_prob}"
+                         f" is not greater than {self.history[-1]}."
+                         f" Delta is {delta}")
         self.history.append(log_prob)
         self.iter += 1
 
     @property
     def converged(self):
         """Whether the EM algorithm converged."""
         # XXX we might want to check that ``log_prob`` is non-decreasing.
         return (self.iter == self.n_iter or
                 (len(self.history) >= 2 and
                  self.history[-1] - self.history[-2] < self.tol))
 
 
-class BaseHMM(BaseEstimator):
+class _AbstractHMM(BaseEstimator):
     """
-    Base class for Hidden Markov Models.
-
-    This class allows for easy evaluation of, sampling from, and maximum a
-    posteriori estimation of the parameters of a HMM.
-
-    Attributes
-    ----------
-    monitor_ : ConvergenceMonitor
-        Monitor object used to check the convergence of EM.
-    startprob_ : array, shape (n_components, )
-        Initial state occupation distribution.
-    transmat_ : array, shape (n_components, n_components)
-        Matrix of transition probabilities between states.
-
-    Notes
-    -----
-    Normally, one should use a subclass of `.BaseHMM`, with its specialization
-    towards a given emission model.  In rare cases, the base class can also be
-    useful in itself, if one simply wants to generate a sequence of states
-    using `.BaseHMM.sample`.  In that case, the feature matrix will have zero
-    features.
+    Base class for Hidden Markov Models learned via Expectation-Maximization
+    and Variational Bayes.
     """
 
-    def __init__(self, n_components=1,
-                 startprob_prior=1.0, transmat_prior=1.0,
-                 algorithm="viterbi", random_state=None,
-                 n_iter=10, tol=1e-2, verbose=False,
-                 params=string.ascii_letters,
-                 init_params=string.ascii_letters,
-                 implementation="log"):
+    def __init__(self, n_components, algorithm, random_state, n_iter,
+                 tol, verbose, params, init_params, implementation):
         """
         Parameters
         ----------
         n_components : int
             Number of states in the model.
-        startprob_prior : array, shape (n_components, ), optional
-            Parameters of the Dirichlet prior distribution for
-            :attr:`startprob_`.
-        transmat_prior : array, shape (n_components, n_components), optional
-            Parameters of the Dirichlet prior distribution for each row
-            of the transition probabilities :attr:`transmat_`.
         algorithm : {"viterbi", "map"}, optional
             Decoder algorithm.
         random_state: RandomState or an int seed, optional
             A random number generator instance.
         n_iter : int, optional
             Maximum number of iterations to perform.
         tol : float, optional
@@ -180,36 +159,24 @@
             subclass-specific emission parameters.  Defaults to all parameters.
         implementation: string, optional
             Determines if the forward-backward algorithm is implemented with
             logarithms ("log"), or using scaling ("scaling").  The default is
             to use logarithms for backwards compatability.  However, the
             scaling implementation is generally faster.
         """
+
         self.n_components = n_components
         self.params = params
         self.init_params = init_params
-        self.startprob_prior = startprob_prior
-        self.transmat_prior = transmat_prior
         self.algorithm = algorithm
-        self.random_state = random_state
         self.n_iter = n_iter
         self.tol = tol
         self.verbose = verbose
         self.implementation = implementation
-        self.monitor_ = ConvergenceMonitor(self.tol, self.n_iter, self.verbose)
-
-    def get_stationary_distribution(self):
-        """Compute the stationary distribution of states."""
-        # The stationary distribution is proportional to the left-eigenvector
-        # associated with the largest eigenvalue (i.e., 1) of the transition
-        # matrix.
-        _utils.check_is_fitted(self, "transmat_")
-        eigvals, eigvecs = linalg.eig(self.transmat_.T)
-        eigvec = np.real_if_close(eigvecs[:, np.argmax(eigvals)])
-        return eigvec / eigvec.sum()
+        self.random_state = random_state
 
     def score_samples(self, X, lengths=None):
         """
         Compute the log probability under the model and compute posteriors.
 
         Parameters
         ----------
@@ -262,15 +229,15 @@
         """
         Helper for `score` and `score_samples`.
 
         Compute the log probability under the model, as well as posteriors if
         *compute_posteriors* is True (otherwise, an empty array is returned
         for the latter).
         """
-        _utils.check_is_fitted(self, "startprob_")
+        check_is_fitted(self, "startprob_")
         self._check()
 
         X = check_array(X)
         impl = {
             "scaling": self._score_scaling,
             "log": self._score_log,
         }[self.implementation]
@@ -349,15 +316,15 @@
 
         See Also
         --------
         score_samples : Compute the log probability under the model and
             posteriors.
         score : Compute the log probability under the model.
         """
-        _utils.check_is_fitted(self, "startprob_")
+        check_is_fitted(self, "startprob_")
         self._check()
 
         algorithm = algorithm or self.algorithm
         if algorithm not in DECODER_ALGORITHMS:
             raise ValueError(f"Unknown decoder {algorithm!r}")
 
         decoder = {
@@ -441,15 +408,15 @@
         --------
         ::
 
             # generate samples continuously
             _, Z = model.sample(n_samples=10)
             X, Z = model.sample(n_samples=10, currstate=Z[-1])
         """
-        _utils.check_is_fitted(self, "startprob_")
+        check_is_fitted(self, "startprob_")
         self._check()
 
         if random_state is None:
             random_state = self.random_state
         random_state = check_random_state(random_state)
 
         transmat_cdf = np.cumsum(self.transmat_, axis=1)
@@ -459,16 +426,16 @@
             currstate = (startprob_cdf > random_state.rand()).argmax()
 
         state_sequence = [currstate]
         X = [self._generate_sample_from_state(
             currstate, random_state=random_state)]
 
         for t in range(n_samples - 1):
-            currstate = (transmat_cdf[currstate] > random_state.rand()) \
-                .argmax()
+            currstate = (
+                (transmat_cdf[currstate] > random_state.rand()).argmax())
             state_sequence.append(currstate)
             X.append(self._generate_sample_from_state(
                 currstate, random_state=random_state))
 
         return np.atleast_2d(X), np.array(state_sequence, dtype=int)
 
     def fit(self, X, lengths=None):
@@ -490,68 +457,45 @@
 
         Returns
         -------
         self : object
             Returns self.
         """
         X = check_array(X)
-        self._init(X)
-        self._check()
 
+        if lengths is None:
+            lengths = np.asarray([X.shape[0]])
+
+        self._init(X, lengths)
+        self._check()
         self.monitor_._reset()
 
-        impl = {
-            "scaling": self._fit_scaling,
-            "log": self._fit_log,
-        }[self.implementation]
         for iter in range(self.n_iter):
-            stats = self._initialize_sufficient_statistics()
-            curr_log_prob = 0
-            for sub_X in _utils.split_X_lengths(X, lengths):
-                lattice, log_prob, posteriors, fwdlattice, bwdlattice = \
-                        impl(sub_X)
-                # Derived HMM classes will implement the following method to
-                # update their probability distributions, so keep
-                # a single call to this method for simplicity.
-                self._accumulate_sufficient_statistics(
-                    stats, sub_X, lattice, posteriors, fwdlattice,
-                    bwdlattice)
-                curr_log_prob += log_prob
+            stats, curr_logprob = self._do_estep(X, lengths)
+
+            # Compute lower bound before updating model parameters
+            lower_bound = self._compute_lower_bound(curr_logprob)
 
             # XXX must be before convergence check, because otherwise
             #     there won't be any updates for the case ``n_iter=1``.
             self._do_mstep(stats)
-
-            self.monitor_.report(curr_log_prob)
+            self.monitor_.report(lower_bound)
             if self.monitor_.converged:
                 break
 
-        if (self.transmat_.sum(axis=1) == 0).any():
-            _log.warning("Some rows of transmat_ have zero sum because no "
-                         "transition from the state was ever observed.")
-
+            if (self.transmat_.sum(axis=1) == 0).any():
+                _log.warning("Some rows of transmat_ have zero sum because no "
+                             "transition from the state was ever observed.")
         return self
 
     def _fit_scaling(self, X):
-        frameprob = self._compute_likelihood(X)
-        log_prob, fwdlattice, scaling_factors = _hmmc.forward_scaling(
-            self.startprob_, self.transmat_, frameprob)
-        bwdlattice =  _hmmc.backward_scaling(
-            self.startprob_, self.transmat_, frameprob, scaling_factors)
-        posteriors = self._compute_posteriors_scaling(fwdlattice, bwdlattice)
-        return frameprob, log_prob, posteriors, fwdlattice, bwdlattice
+        raise NotImplementedError("Must be overridden in subclass")
 
     def _fit_log(self, X):
-        log_frameprob = self._compute_log_likelihood(X)
-        log_prob, fwdlattice = _hmmc.forward_log(
-            self.startprob_, self.transmat_, log_frameprob)
-        bwdlattice = _hmmc.backward_log(
-            self.startprob_, self.transmat_, log_frameprob)
-        posteriors = self._compute_posteriors_log(fwdlattice, bwdlattice)
-        return log_frameprob, log_prob, posteriors, fwdlattice, bwdlattice
+        raise NotImplementedError("Must be overridden in subclass")
 
     def _compute_posteriors_scaling(self, fwdlattice, bwdlattice):
         posteriors = fwdlattice * bwdlattice
         normalize(posteriors, axis=1)
         return posteriors
 
     def _compute_posteriors_log(self, fwdlattice, bwdlattice):
@@ -572,50 +516,34 @@
                     "overwritten during initialization because 'init_params' "
                     "contains %r", name, code)
             return True
         if not hasattr(self, name):
             return True
         return False
 
+    def _check_and_set_n_features(self, X):
+        _, n_features = X.shape
+        if hasattr(self, "n_features"):
+            if self.n_features != n_features:
+                raise ValueError(
+                    f"Unexpected number of dimensions, got {n_features} but "
+                    f"expected {self.n_features}")
+        else:
+            self.n_features = n_features
+
     def _get_n_fit_scalars_per_param(self):
         """
         Return a mapping of fittable parameter names (as in ``self.params``)
         to the number of corresponding scalar parameters that will actually be
         fitted.
 
         This is used to detect whether the user did not pass enough data points
         for a non-degenerate fit.
         """
-
-    def _init(self, X):
-        """
-        Initialize model parameters prior to fitting.
-
-        Parameters
-        ----------
-        X : array-like, shape (n_samples, n_features)
-            Feature matrix of individual samples.
-        """
-        init = 1. / self.n_components
-        random_state = check_random_state(self.random_state)
-        if self._needs_init("s", "startprob_"):
-            self.startprob_ = random_state.dirichlet(
-                np.full(self.n_components, init))
-        if self._needs_init("t", "transmat_"):
-            self.transmat_ = random_state.dirichlet(
-                np.full(self.n_components, init), size=self.n_components)
-        n_fit_scalars_per_param = self._get_n_fit_scalars_per_param()
-        if n_fit_scalars_per_param is not None:
-            n_fit_scalars = sum(
-                n_fit_scalars_per_param[p] for p in self.params)
-            if X.size < n_fit_scalars:
-                _log.warning(
-                    "Fitting a model with %d free scalar parameters with only "
-                    "%d data points will result in a degenerate solution.",
-                    n_fit_scalars, X.size)
+        raise NotImplementedError("Must be overridden in subclass")
 
     def _check_sum_1(self, name):
         """Check that an array describes one or more distributions."""
         s = getattr(self, name).sum(axis=-1)
         if not np.allclose(s, 1):
             raise ValueError(
                 f"{name} must sum to 1 (got {s:.4f})" if s.ndim == 0 else
@@ -628,24 +556,15 @@
 
         Raises
         ------
         ValueError
             If any of the parameters are invalid, e.g. if :attr:`startprob_`
             don't sum to 1.
         """
-        self.startprob_ = np.asarray(self.startprob_)
-        if len(self.startprob_) != self.n_components:
-            raise ValueError("startprob_ must have length n_components")
-        self._check_sum_1("startprob_")
-
-        self.transmat_ = np.asarray(self.transmat_)
-        if self.transmat_.shape != (self.n_components, self.n_components):
-            raise ValueError(
-                "transmat_ must have shape (n_components, n_components)")
-        self._check_sum_1("transmat_")
+        raise NotImplementedError("Must be overridden in subclass")
 
     def _compute_likelihood(self, X):
         """
         Compute per-component probability under the model.
 
         Parameters
         ----------
@@ -655,16 +574,18 @@
         Returns
         -------
         log_prob : array, shape (n_samples, n_components)
             Log probability of each sample in ``X`` for each of the
             model states.
         """
         if (self._compute_log_likelihood  # prevent recursion
-                != BaseHMM._compute_log_likelihood.__get__(self)):
-            return np.exp(self._compute_log_likelihood(X))
+                != __class__._compute_log_likelihood.__get__(self)):
+            # Probabilities equal to zero do occur, and exp(-LARGE) = 0 is OK.
+            with np.errstate(under="ignore"):
+                return np.exp(self._compute_log_likelihood(X))
         else:
             raise NotImplementedError("Must be overridden in subclass")
 
     def _compute_log_likelihood(self, X):
         """
         Compute per-component emission log probability under the model.
 
@@ -676,17 +597,17 @@
         Returns
         -------
         log_prob : array, shape (n_samples, n_components)
             Emission log probability of each sample in ``X`` for each of the
             model states, i.e., ``log(p(X|state))``.
         """
         if (self._compute_likelihood  # prevent recursion
-                != BaseHMM._compute_likelihood.__get__(self)):
-            likelihood = self._compute_likelihood(X)
+                != __class__._compute_likelihood.__get__(self)):
             # Probabilities equal to zero do occur, and log(0) = -inf is OK.
+            likelihood = self._compute_likelihood(X)
             with np.errstate(divide="ignore"):
                 return np.log(likelihood)
         else:
             raise NotImplementedError("Must be overridden in subclass")
 
     def _generate_sample_from_state(self, state, random_state):
         """
@@ -704,16 +625,14 @@
         -------
         X : array, shape (n_features, )
             A random sample from the emission distribution corresponding
             to a given component.
         """
         return ()
 
-    # Methods used by self.fit()
-
     def _initialize_sufficient_statistics(self):
         """
         Initialize sufficient statistics required for M-step.
 
         The method is *pure*, meaning that it doesn't change the state of
         the instance.  For extensibility computed statistics are stored
         in a dictionary.
@@ -813,14 +732,155 @@
         Perform the M-step of EM algorithm.
 
         Parameters
         ----------
         stats : dict
             Sufficient statistics updated from all available samples.
         """
+
+    def _do_estep(self, X, lengths):
+        impl = {
+            "scaling": self._fit_scaling,
+            "log": self._fit_log,
+        }[self.implementation]
+
+        stats = self._initialize_sufficient_statistics()
+        self._estep_begin()
+        curr_logprob = 0
+        for sub_X in _utils.split_X_lengths(X, lengths):
+            lattice, logprob, posteriors, fwdlattice, bwdlattice = impl(sub_X)
+            # Derived HMM classes will implement the following method to
+            # update their probability distributions, so keep
+            # a single call to this method for simplicity.
+            self._accumulate_sufficient_statistics(
+                stats, sub_X, lattice, posteriors, fwdlattice,
+                bwdlattice)
+            curr_logprob += logprob
+        return stats, curr_logprob
+
+    def _estep_begin(self):
+        pass
+
+    def _compute_lower_bound(self, curr_logprob):
+        raise NotImplementedError("Must be overridden in subclass")
+
+
+class BaseHMM(_AbstractHMM):
+    """
+    Base class for Hidden Markov Models learned from Expectation-Maximization.
+
+    This class allows for easy evaluation of, sampling from, and maximum a
+    posteriori estimation of the parameters of a HMM.
+
+    Attributes
+    ----------
+    monitor_ : ConvergenceMonitor
+        Monitor object used to check the convergence of EM.
+    startprob_ : array, shape (n_components, )
+        Initial state occupation distribution.
+    transmat_ : array, shape (n_components, n_components)
+        Matrix of transition probabilities between states.
+
+    Notes
+    -----
+    Normally, one should use a subclass of `.BaseHMM`, with its specialization
+    towards a given emission model.  In rare cases, the base class can also be
+    useful in itself, if one simply wants to generate a sequence of states
+    using `.BaseHMM.sample`.  In that case, the feature matrix will have zero
+    features.
+    """
+
+    def __init__(self, n_components=1,
+                 startprob_prior=1.0, transmat_prior=1.0,
+                 algorithm="viterbi", random_state=None,
+                 n_iter=10, tol=1e-2, verbose=False,
+                 params=string.ascii_letters,
+                 init_params=string.ascii_letters,
+                 implementation="log"):
+        """
+        Parameters
+        ----------
+        n_components : int
+            Number of states in the model.
+        startprob_prior : array, shape (n_components, ), optional
+            Parameters of the Dirichlet prior distribution for
+            :attr:`startprob_`.
+        transmat_prior : array, shape (n_components, n_components), optional
+            Parameters of the Dirichlet prior distribution for each row
+            of the transition probabilities :attr:`transmat_`.
+        algorithm : {"viterbi", "map"}, optional
+            Decoder algorithm.
+        random_state: RandomState or an int seed, optional
+            A random number generator instance.
+        n_iter : int, optional
+            Maximum number of iterations to perform.
+        tol : float, optional
+            Convergence threshold. EM will stop if the gain in log-likelihood
+            is below this value.
+        verbose : bool, optional
+            Whether per-iteration convergence reports are printed to
+            :data:`sys.stderr`.  Convergence can also be diagnosed using the
+            :attr:`monitor_` attribute.
+        params, init_params : string, optional
+            The parameters that get updated during (``params``) or initialized
+            before (``init_params``) the training.  Can contain any combination
+            of 's' for startprob, 't' for transmat, and other characters for
+            subclass-specific emission parameters.  Defaults to all parameters.
+        implementation: string, optional
+            Determines if the forward-backward algorithm is implemented with
+            logarithms ("log"), or using scaling ("scaling").  The default is
+            to use logarithms for backwards compatability.  However, the
+            scaling implementation is generally faster.
+        """
+        super().__init__(
+            n_components=n_components, algorithm=algorithm,
+            random_state=random_state, n_iter=n_iter, tol=tol,
+            verbose=verbose, params=params, init_params=init_params,
+            implementation=implementation)
+        self.startprob_prior = startprob_prior
+        self.transmat_prior = transmat_prior
+        self.monitor_ = ConvergenceMonitor(self.tol, self.n_iter, self.verbose)
+
+    def get_stationary_distribution(self):
+        """Compute the stationary distribution of states."""
+        # The stationary distribution is proportional to the left-eigenvector
+        # associated with the largest eigenvalue (i.e., 1) of the transition
+        # matrix.
+        check_is_fitted(self, "transmat_")
+        eigvals, eigvecs = linalg.eig(self.transmat_.T)
+        eigvec = np.real_if_close(eigvecs[:, np.argmax(eigvals)])
+        return eigvec / eigvec.sum()
+
+    def _fit_scaling(self, X):
+        frameprob = self._compute_likelihood(X)
+        log_prob, fwdlattice, scaling_factors = _hmmc.forward_scaling(
+            self.startprob_, self.transmat_, frameprob)
+        bwdlattice = _hmmc.backward_scaling(
+            self.startprob_, self.transmat_, frameprob, scaling_factors)
+        posteriors = self._compute_posteriors_scaling(fwdlattice, bwdlattice)
+        return frameprob, log_prob, posteriors, fwdlattice, bwdlattice
+
+    def _fit_log(self, X):
+        log_frameprob = self._compute_log_likelihood(X)
+        log_prob, fwdlattice = _hmmc.forward_log(
+            self.startprob_, self.transmat_, log_frameprob)
+        bwdlattice = _hmmc.backward_log(
+            self.startprob_, self.transmat_, log_frameprob)
+        posteriors = self._compute_posteriors_log(fwdlattice, bwdlattice)
+        return log_frameprob, log_prob, posteriors, fwdlattice, bwdlattice
+
+    def _do_mstep(self, stats):
+        """
+        Perform the M-step of EM algorithm.
+
+        Parameters
+        ----------
+        stats : dict
+            Sufficient statistics updated from all available samples.
+        """
         # If a prior is < 1, `prior - 1 + starts['start']` can be negative.  In
         # that case maximization of (n1+e1) log p1 + ... + (ns+es) log ps under
         # the conditions sum(p) = 1 and all(p >= 0) show that the negative
         # terms can just be set to zero.
         # The ``np.where`` calls guard against updating forbidden states
         # or transitions in e.g. a left-right HMM.
         if 's' in self.params:
@@ -829,9 +889,360 @@
             self.startprob_ = np.where(self.startprob_ == 0, 0, startprob_)
             normalize(self.startprob_)
         if 't' in self.params:
             transmat_ = np.maximum(self.transmat_prior - 1 + stats['trans'], 0)
             self.transmat_ = np.where(self.transmat_ == 0, 0, transmat_)
             normalize(self.transmat_, axis=1)
 
+    def _compute_lower_bound(self, curr_logprob):
+        return curr_logprob
+
+    def _init(self, X, lengths=None):
+        """
+        Initialize model parameters prior to fitting.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            Feature matrix of individual samples.
+        """
+        self._check_and_set_n_features(X)
+        init = 1. / self.n_components
+        random_state = check_random_state(self.random_state)
+        if self._needs_init("s", "startprob_"):
+            self.startprob_ = random_state.dirichlet(
+                np.full(self.n_components, init))
+        if self._needs_init("t", "transmat_"):
+            self.transmat_ = random_state.dirichlet(
+                np.full(self.n_components, init), size=self.n_components)
+        n_fit_scalars_per_param = self._get_n_fit_scalars_per_param()
+        if n_fit_scalars_per_param is not None:
+            n_fit_scalars = sum(
+                n_fit_scalars_per_param[p] for p in self.params)
+            if X.size < n_fit_scalars:
+                _log.warning(
+                    "Fitting a model with %d free scalar parameters with only "
+                    "%d data points will result in a degenerate solution.",
+                    n_fit_scalars, X.size)
+
+    def _check_sum_1(self, name):
+        """Check that an array describes one or more distributions."""
+        s = getattr(self, name).sum(axis=-1)
+        if not np.allclose(s, 1):
+            raise ValueError(
+                f"{name} must sum to 1 (got {s:.4f})" if s.ndim == 0 else
+                f"{name} rows must sum to 1 (got {s})" if s.ndim == 1 else
+                "Expected 1D or 2D array")
+
+    def _check(self):
+        """
+        Validate model parameters prior to fitting.
+
+        Raises
+        ------
+        ValueError
+            If any of the parameters are invalid, e.g. if :attr:`startprob_`
+            don't sum to 1.
+        """
+        self.startprob_ = np.asarray(self.startprob_)
+        if len(self.startprob_) != self.n_components:
+            raise ValueError("startprob_ must have length n_components")
+        self._check_sum_1("startprob_")
+
+        self.transmat_ = np.asarray(self.transmat_)
+        if self.transmat_.shape != (self.n_components, self.n_components):
+            raise ValueError(
+                "transmat_ must have shape (n_components, n_components)")
+        self._check_sum_1("transmat_")
+
+    def aic(self, X, lengths=None):
+        """
+        Akaike information criterion for the current model on the input X.
+
+        AIC = -2*logLike + 2 * num_free_params
+
+        https://en.wikipedia.org/wiki/Akaike_information_criterion
+
+        Parameters
+        ----------
+        X : array of shape (n_samples, n_dimensions)
+            The input samples.
+        lengths : array-like of integers, shape (n_sequences, )
+            Lengths of the individual sequences in ``X``. The sum of
+            these should be ``n_samples``.
+
+        Returns
+        -------
+        aic : float
+            The lower the better.
+        """
+        n_params = sum(self._get_n_fit_scalars_per_param().values())
+        return -2 * self.score(X, lengths=lengths) + 2 * n_params
+
+    def bic(self, X, lengths=None):
+        """
+        Bayesian information criterion for the current model on the input X.
+
+        BIC = -2*logLike + num_free_params * log(num_of_data)
+
+        https://en.wikipedia.org/wiki/Bayesian_information_criterion
+
+        Parameters
+        ----------
+        X : array of shape (n_samples, n_dimensions)
+            The input samples.
+        lengths : array-like of integers, shape (n_sequences, )
+            Lengths of the individual sequences in ``X``. The sum of
+            these should be ``n_samples``.
+
+        Returns
+        -------
+        bic : float
+            The lower the better.
+        """
+        n_params = sum(self._get_n_fit_scalars_per_param().values())
+        return -2 * self.score(X, lengths=lengths) + n_params * np.log(len(X))
 
 _BaseHMM = BaseHMM  # Backcompat name, will be deprecated in the future.
+
+
+class VariationalBaseHMM(_AbstractHMM):
+
+    def __init__(self, n_components=1,
+                 startprob_prior=None, transmat_prior=None,
+                 algorithm="viterbi", random_state=None,
+                 n_iter=100, tol=1e-6, verbose=False,
+                 params="ste", init_params="ste",
+                 implementation="log"):
+        super().__init__(
+            n_components=n_components, algorithm=algorithm,
+            random_state=random_state, n_iter=n_iter, tol=tol,
+            verbose=verbose, params=params, init_params=init_params,
+            implementation=implementation)
+
+        self.startprob_prior = startprob_prior
+        self.transmat_prior = transmat_prior
+        self.monitor_ = ConvergenceMonitor(
+            self.tol, self.n_iter, self.verbose)
+
+    def _init(self, X, lengths=None):
+        """
+        Initialize model parameters prior to fitting.
+
+        Parameters
+        ----------
+        X : array-like, shape (n_samples, n_features)
+            Feature matrix of individual samples.
+        lengths : array-like of integers, shape (n_sequences, )
+            Lengths of the individual sequences in ``X``. The sum of
+            these should be ``n_samples``.
+        """
+        self._check_and_set_n_features(X)
+        nc = self.n_components
+        uniform_prior = 1 / nc
+        random_state = check_random_state(self.random_state)
+        if (self._needs_init("s", "startprob_posterior_")
+                or self._needs_init("s", "startprob_prior_")):
+            if self.startprob_prior is None:
+                startprob_init = uniform_prior
+            else:
+                startprob_init = self.startprob_prior
+
+            self.startprob_prior_ = np.full(nc, startprob_init)
+            self.startprob_posterior_ = random_state.dirichlet(
+                np.full(nc, uniform_prior)) * len(lengths)
+
+        if (self._needs_init("t", "transmat_posterior_")
+                or self._needs_init("t", "transmat_prior_")):
+            if self.transmat_prior is None:
+                transmat_init = uniform_prior
+            else:
+                transmat_init = self.transmat_prior
+            self.transmat_prior_ = np.full(
+                (nc, nc), transmat_init)
+            self.transmat_posterior_ = random_state.dirichlet(
+                np.full(nc, uniform_prior), size=nc)
+            self.transmat_posterior_ *= sum(lengths) / nc
+
+        n_fit_scalars_per_param = self._get_n_fit_scalars_per_param()
+        if n_fit_scalars_per_param is not None:
+            n_fit_scalars = sum(
+                n_fit_scalars_per_param[p] for p in self.params)
+            if X.size < n_fit_scalars:
+                _log.warning(
+                    "Fitting a model with %d free scalar parameters with only "
+                    "%d data points will result in a degenerate solution.",
+                    n_fit_scalars, X.size)
+
+    # For Variational Inference, we compute the forward/backward algorithm
+    # using subnormalized probabilities.
+    def _fit_scaling(self, X):
+        frameprob = self._compute_subnorm_likelihood(X)
+        logprob, fwdlattice, scaling_factors = _hmmc.forward_scaling(
+            self.startprob_subnorm_, self.transmat_subnorm_, frameprob)
+
+        bwdlattice = _hmmc.backward_scaling(
+            self.startprob_subnorm_, self.transmat_subnorm_,
+            frameprob, scaling_factors)
+        posteriors = self._compute_posteriors_scaling(fwdlattice, bwdlattice)
+        return frameprob, logprob, posteriors, fwdlattice, bwdlattice
+
+    def _fit_log(self, X):
+        framelogprob = self._compute_subnorm_log_likelihood(X)
+        logprob, fwdlattice = _hmmc.forward_log(
+            self.startprob_subnorm_, self.transmat_subnorm_, framelogprob)
+        bwdlattice = _hmmc.backward_log(
+            self.startprob_subnorm_, self.transmat_subnorm_, framelogprob)
+        posteriors = self._compute_posteriors_log(fwdlattice, bwdlattice)
+        return framelogprob, logprob, posteriors, fwdlattice, bwdlattice
+
+    def _check(self):
+        """
+        Validate model parameters prior to fitting.
+
+        Raises
+        ------
+        ValueError
+            If any of the parameters are invalid, e.g. if :attr:`startprob_`
+            don't sum to 1.
+        """
+        nc = self.n_components
+
+        self.startprob_prior_ = np.asarray(self.startprob_prior_)
+        if len(self.startprob_prior_) != nc:
+            raise ValueError("startprob_prior_ must have length n_components")
+        self.startprob_posterior_ = np.asarray(self.startprob_posterior_)
+        if len(self.startprob_posterior_) != nc:
+            raise ValueError("startprob_posterior_ must have length "
+                             "n_components")
+
+        self.transmat_prior_ = np.asarray(self.transmat_prior_)
+        if self.transmat_prior_.shape != (nc, nc):
+            raise ValueError("transmat_prior_ must have shape "
+                             "(n_components, n_components)")
+        self.transmat_posterior_ = np.asarray(self.transmat_posterior_)
+        if self.transmat_posterior_.shape != (nc, nc):
+            raise ValueError("transmat_posterior_ must have shape "
+                             "(n_components, n_components)")
+
+    def _compute_subnorm_likelihood(self, X):
+        if (self._compute_subnorm_log_likelihood !=  # prevent recursion
+                __class__._compute_subnorm_log_likelihood.__get__(self)):
+            return np.exp(self._compute_subnorm_log_likelihood(X))
+        else:
+            raise NotImplementedError("Must be overridden in subclass")
+
+    def _compute_subnorm_log_likelihood(self, X):
+        if (self._compute_subnorm_likelihood !=  # prevent recursion
+                __class__._compute_subnorm_likelihood.__get__(self)):
+            return np.log(self._compute_subnorm_likelihood(X))
+        else:
+            raise NotImplementedError("Must be overridden in subclass")
+
+    def _accumulate_sufficient_statistics_scaling(
+            self, stats, X, lattice, posteriors, fwdlattice, bwdlattice):
+        """
+        Implementation of `_accumulate_sufficient_statistics`
+        for ``implementation = "log"``.
+        """
+        stats['nobs'] += 1
+        if 's' in self.params:
+            stats['start'] += posteriors[0]
+        if 't' in self.params:
+            n_samples, n_components = lattice.shape
+            # when the sample is of length 1, it contains no transitions
+            # so there is no reason to update our trans. matrix estimate
+            if n_samples <= 1:
+                return
+
+            xi_sum = _hmmc.compute_scaling_xi_sum(fwdlattice,
+                                                  self.transmat_subnorm_,
+                                                  bwdlattice, lattice)
+            stats['trans'] += xi_sum
+
+    def _accumulate_sufficient_statistics_log(
+            self, stats, X, lattice, posteriors, fwdlattice, bwdlattice):
+        """
+        Implementation of `_accumulate_sufficient_statistics`
+        for ``implementation = "log"``.
+        """
+        stats['nobs'] += 1
+        if 's' in self.params:
+            stats['start'] += posteriors[0]
+        if 't' in self.params:
+            n_samples, n_components = lattice.shape
+            # when the sample is of length 1, it contains no transitions
+            # so there is no reason to update our trans. matrix estimate
+            if n_samples <= 1:
+                return
+
+            log_xi_sum = _hmmc.compute_log_xi_sum(
+                fwdlattice, self.transmat_subnorm_, bwdlattice,
+                lattice)
+            with np.errstate(under="ignore"):
+                stats['trans'] += np.exp(log_xi_sum)
+
+    def _estep_begin(self):
+        """
+        Update the subnormalized model parameters.  Called at the beginning of
+        each iteration of fit()
+        """
+        startprob_log_subnorm = (
+            special.digamma(self.startprob_posterior_)
+            - special.digamma(self.startprob_posterior_.sum()))
+        self.startprob_subnorm_ = np.exp(startprob_log_subnorm)
+
+        transmat_log_subnorm = (
+            special.digamma(self.transmat_posterior_)
+            - special.digamma(self.transmat_posterior_.sum(axis=1)[:, None]))
+        self.transmat_subnorm_ = np.exp(transmat_log_subnorm)
+
+    def _do_mstep(self, stats):
+        """
+        Perform the M-step of EM algorithm.
+
+        Parameters
+        ----------
+        stats : dict
+            Sufficient statistics updated from all available samples.
+        """
+        if 's' in self.params:
+            self.startprob_posterior_ = self.startprob_prior_ + stats['start']
+            # For compatability in _AbstractHMM
+            self.startprob_ = (self.startprob_posterior_
+                               / self.startprob_posterior_.sum())
+        if 't' in self.params:
+            self.transmat_posterior_ = self.transmat_prior_ + stats['trans']
+            # For compatability in _AbstractHMM
+            self.transmat_ = (self.transmat_posterior_
+                              / self.transmat_posterior_.sum(axis=1)[:, None])
+
+    def _compute_lower_bound(self, curr_logprob):
+        """
+        Compute the Variational Lower Bound of the model as currently
+        configured.
+
+        Following the pattern elsewhere, derived implementations should call
+        this method to get the contribution of the current log_prob,
+        transmat, and startprob towards the lower bound
+
+        Parameters
+        ----------
+        curr_logprob : float
+                       The current log probability of the data as computed at
+                       the subnormalized model parameters.
+
+        Returns
+        -------
+        lower_bound: float
+                     Returns the computed lower bound contribution of the
+                     log_prob, startprob, and transmat.
+        """
+        # Get the contribution from the state transitions,
+        # initial probabilities, and the likelihood of the sequences
+        startprob_lower_bound = -_kl.kl_dirichlet(
+            self.startprob_posterior_, self.startprob_prior_)
+        transmat_lower_bound = 0
+        for i in range(self.n_components):
+            transmat_lower_bound -= _kl.kl_dirichlet(
+                self.transmat_posterior_[i], self.transmat_prior_[i])
+        return startprob_lower_bound + transmat_lower_bound + curr_logprob
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/hmm.py` & `hmmlearn-0.3.0/lib/hmmlearn/hmm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,159 @@
 """
 The :mod:`hmmlearn.hmm` module implements hidden Markov models.
 """
 
-import functools
-import inspect
 import logging
 
 import numpy as np
-from scipy import linalg, special
-from scipy.stats import multinomial, poisson
+from scipy import linalg
 from sklearn import cluster
 from sklearn.utils import check_random_state
 
-from . import _utils
-from .stats import log_multivariate_normal_density
+from . import _emissions, _utils
 from .base import BaseHMM
-from .utils import fill_covars, log_normalize, normalize
+from .utils import fill_covars, normalize
 
 
 __all__ = [
     "GMMHMM", "GaussianHMM", "CategoricalHMM", "MultinomialHMM", "PoissonHMM",
 ]
 
 
 _log = logging.getLogger(__name__)
 COVARIANCE_TYPES = frozenset(("spherical", "diag", "full", "tied"))
 
 
-def _check_and_set_n_features(model, X):
-    _, n_features = X.shape
-    if hasattr(model, "n_features"):
-        if model.n_features != n_features:
+class CategoricalHMM(_emissions.BaseCategoricalHMM, BaseHMM):
+    """
+    Hidden Markov Model with categorical (discrete) emissions.
+
+    Attributes
+    ----------
+    n_features : int
+        Number of possible symbols emitted by the model (in the samples).
+
+    monitor_ : ConvergenceMonitor
+        Monitor object used to check the convergence of EM.
+
+    startprob_ : array, shape (n_components, )
+        Initial state occupation distribution.
+
+    transmat_ : array, shape (n_components, n_components)
+        Matrix of transition probabilities between states.
+
+    emissionprob_ : array, shape (n_components, n_features)
+        Probability of emitting a given symbol when in each state.
+
+    Examples
+    --------
+    >>> from hmmlearn.hmm import CategoricalHMM
+    >>> CategoricalHMM(n_components=2)  #doctest: +ELLIPSIS
+    CategoricalHMM(algorithm='viterbi',...
+    """
+
+    def __init__(self, n_components=1, startprob_prior=1.0,
+                 transmat_prior=1.0, *, emissionprob_prior=1.0,
+                 n_features=None, algorithm="viterbi",
+                 random_state=None, n_iter=10, tol=1e-2,
+                 verbose=False, params="ste", init_params="ste",
+                 implementation="log"):
+        """
+        Parameters
+        ----------
+        n_components : int
+            Number of states.
+
+        startprob_prior : array, shape (n_components, ), optional
+            Parameters of the Dirichlet prior distribution for
+            :attr:`startprob_`.
+
+        transmat_prior : array, shape (n_components, n_components), optional
+            Parameters of the Dirichlet prior distribution for each row
+            of the transition probabilities :attr:`transmat_`.
+
+        emissionprob_prior : array, shape (n_components, n_features), optional
+            Parameters of the Dirichlet prior distribution for
+            :attr:`emissionprob_`.
+
+        n_features: int, optional
+            The number of categorical symbols in the HMM.  Will be inferred
+            from the data if not set.
+
+        algorithm : {"viterbi", "map"}, optional
+            Decoder algorithm.
+
+        random_state: RandomState or an int seed, optional
+            A random number generator instance.
+
+        n_iter : int, optional
+            Maximum number of iterations to perform.
+
+        tol : float, optional
+            Convergence threshold. EM will stop if the gain in log-likelihood
+            is below this value.
+
+        verbose : bool, optional
+            Whether per-iteration convergence reports are printed to
+            :data:`sys.stderr`.  Convergence can also be diagnosed using the
+            :attr:`monitor_` attribute.
+
+        params, init_params : string, optional
+            The parameters that get updated during (``params``) or initialized
+            before (``init_params``) the training.  Can contain any
+            combination of 's' for startprob, 't' for transmat, and 'e' for
+            emissionprob.  Defaults to all parameters.
+
+        implementation : string, optional
+            Determines if the forward-backward algorithm is implemented with
+            logarithms ("log"), or using scaling ("scaling").  The default is
+            to use logarithms for backwards compatability.
+        """
+        BaseHMM.__init__(self, n_components,
+                         startprob_prior=startprob_prior,
+                         transmat_prior=transmat_prior,
+                         algorithm=algorithm,
+                         random_state=random_state,
+                         n_iter=n_iter, tol=tol, verbose=verbose,
+                         params=params, init_params=init_params,
+                         implementation=implementation)
+        self.emissionprob_prior = emissionprob_prior
+        self.n_features = n_features
+
+    def _init(self, X, lengths=None):
+        super()._init(X, lengths)
+
+        self.random_state = check_random_state(self.random_state)
+
+        if self._needs_init('e', 'emissionprob_'):
+            self.emissionprob_ = self.random_state.rand(
+                self.n_components, self.n_features)
+            normalize(self.emissionprob_, axis=1)
+
+    def _check(self):
+        super()._check()
+
+        self.emissionprob_ = np.atleast_2d(self.emissionprob_)
+        if self.n_features is None:
+            self.n_features = self.emissionprob_.shape[1]
+        if self.emissionprob_.shape != (self.n_components, self.n_features):
             raise ValueError(
-                f"Unexpected number of dimensions, got {n_features} but "
-                f"expected {model.n_features}")
-    else:
-        model.n_features = n_features
+                f"emissionprob_ must have shape"
+                f"({self.n_components}, {self.n_features})")
+        self._check_sum_1("emissionprob_")
 
+    def _do_mstep(self, stats):
+        super()._do_mstep(stats)
+        if 'e' in self.params:
+            self.emissionprob_ = np.maximum(
+                self.emissionprob_prior - 1 + stats['obs'], 0)
+            normalize(self.emissionprob_, axis=1)
 
-class GaussianHMM(BaseHMM):
+
+class GaussianHMM(_emissions.BaseGaussianHMM, BaseHMM):
     """
     Hidden Markov Model with Gaussian emissions.
 
     Attributes
     ----------
     n_features : int
         Dimensionality of the Gaussian emissions.
@@ -145,20 +256,20 @@
 
         params, init_params : string, optional
             The parameters that get updated during (``params``) or initialized
             before (``init_params``) the training.  Can contain any combination
             of 's' for startprob, 't' for transmat, 'm' for means, and 'c' for
             covars.  Defaults to all parameters.
 
-        implementation: string, optional
+        implementation : string, optional
             Determines if the forward-backward algorithm is implemented with
             logarithms ("log"), or using scaling ("scaling").  The default is
             to use logarithms for backwards compatability.
         """
-        BaseHMM.__init__(self, n_components,
+        super().__init__(n_components,
                          startprob_prior=startprob_prior,
                          transmat_prior=transmat_prior, algorithm=algorithm,
                          random_state=random_state, n_iter=n_iter,
                          tol=tol, params=params, verbose=verbose,
                          init_params=init_params,
                          implementation=implementation)
         self.covariance_type = covariance_type
@@ -177,36 +288,21 @@
     @covars_.setter
     def covars_(self, covars):
         covars = np.array(covars, copy=True)
         _utils._validate_covars(covars, self.covariance_type,
                                 self.n_components)
         self._covars_ = covars
 
-    def _get_n_fit_scalars_per_param(self):
-        nc = self.n_components
-        nf = self.n_features
-        return {
-            "s": nc - 1,
-            "t": nc * (nc - 1),
-            "m": nc * nf,
-            "c": {
-                "spherical": nc,
-                "diag": nc * nf,
-                "full": nc * nf * (nf + 1) // 2,
-                "tied": nf * (nf + 1) // 2,
-            }[self.covariance_type],
-        }
-
-    def _init(self, X):
-        _check_and_set_n_features(self, X)
-        super()._init(X)
+    def _init(self, X, lengths=None):
+        super()._init(X, lengths)
 
         if self._needs_init("m", "means_"):
             kmeans = cluster.KMeans(n_clusters=self.n_components,
-                                    random_state=self.random_state)
+                                    random_state=self.random_state,
+                                    n_init=1)  # sklearn <1.4 backcompat.
             kmeans.fit(X)
             self.means_ = kmeans.cluster_centers_
         if self._needs_init("c", "covars_"):
             cv = np.cov(X.T) + self.min_covar * np.eye(X.shape[1])
             if not cv.shape:
                 cv.shape = (1, 1)
             self.covars_ = \
@@ -219,49 +315,19 @@
         self.means_ = np.asarray(self.means_)
         self.n_features = self.means_.shape[1]
 
         if self.covariance_type not in COVARIANCE_TYPES:
             raise ValueError(
                 f"covariance_type must be one of {COVARIANCE_TYPES}")
 
-    def _compute_log_likelihood(self, X):
-        return log_multivariate_normal_density(
-            X, self.means_, self._covars_, self.covariance_type)
-
-    def _generate_sample_from_state(self, state, random_state):
-        return random_state.multivariate_normal(
-            self.means_[state], self.covars_[state])
-
-    def _initialize_sufficient_statistics(self):
-        stats = super()._initialize_sufficient_statistics()
-        stats['post'] = np.zeros(self.n_components)
-        stats['obs'] = np.zeros((self.n_components, self.n_features))
-        stats['obs**2'] = np.zeros((self.n_components, self.n_features))
-        if self.covariance_type in ('tied', 'full'):
-            stats['obs*obs.T'] = np.zeros((self.n_components, self.n_features,
-                                           self.n_features))
-        return stats
-
-    def _accumulate_sufficient_statistics(self, stats, obs, lattice,
-                                          posteriors, fwdlattice, bwdlattice):
-        super()._accumulate_sufficient_statistics(
-            stats, obs, lattice, posteriors, fwdlattice, bwdlattice)
-
-        if 'm' in self.params or 'c' in self.params:
-            stats['post'] += posteriors.sum(axis=0)
-            stats['obs'] += np.dot(posteriors.T, obs)
+    def _needs_sufficient_statistics_for_mean(self):
+        return 'm' in self.params
 
-        if 'c' in self.params:
-            if self.covariance_type in ('spherical', 'diag'):
-                stats['obs**2'] += np.dot(posteriors.T, obs ** 2)
-            elif self.covariance_type in ('tied', 'full'):
-                # posteriors: (nt, nc); obs: (nt, nf); obs: (nt, nf)
-                # -> (nc, nf, nf)
-                stats['obs*obs.T'] += np.einsum(
-                    'ij,ik,il->jkl', posteriors, obs, obs)
+    def _needs_sufficient_statistics_for_covars(self):
+        return 'c' in self.params
 
     def _do_mstep(self, stats):
         super()._do_mstep(stats)
 
         means_prior = self.means_prior
         means_weight = self.means_weight
 
@@ -305,403 +371,15 @@
                     self._covars_ = ((covars_prior + c_n.sum(axis=0)) /
                                      (cvweight + stats['post'].sum()))
                 elif self.covariance_type == 'full':
                     self._covars_ = ((covars_prior + c_n) /
                                      (cvweight + stats['post'][:, None, None]))
 
 
-class MultinomialHMM(BaseHMM):
-    """
-    Hidden Markov Model with multinomial emissions
-
-    Attributes
-    ----------
-    n_features : int
-        Number of possible symbols emitted by the model (in the samples).
-
-    monitor_ : ConvergenceMonitor
-        Monitor object used to check the convergence of EM.
-
-    startprob_ : array, shape (n_components, )
-        Initial state occupation distribution.
-
-    transmat_ : array, shape (n_components, n_components)
-        Matrix of transition probabilities between states.
-
-    emissionprob_ : array, shape (n_components, n_features)
-        Probability of emitting a given symbol when in each state.
-
-    Examples
-    --------
-    >>> from hmmlearn.hmm import MultinomialHMM
-    """
-
-    def __init__(self, n_components=1, n_trials=None,
-                 startprob_prior=1.0, transmat_prior=1.0,
-                 algorithm="viterbi", random_state=None,
-                 n_iter=10, tol=1e-2, verbose=False,
-                 params="ste", init_params="ste",
-                 implementation="log"):
-        """
-        Parameters
-        ----------
-        n_components : int
-            Number of states
-
-        n_trials : int
-            Number of trials
-            for now assume all samples have the same n_trials
-
-        startprob_prior : array, shape (n_components, ), optional
-            Parameters of the Dirichlet prior distribution for
-            :attr:`startprob_`.
-
-        transmat_prior : array, shape (n_components, n_components), optional
-            Parameters of the Dirichlet prior distribution for each row
-            of the transition probabilities :attr:`transmat_`.
-
-        algorithm : {"viterbi", "map"}, optional
-            Decoder algorithm.
-
-        random_state: RandomState or an int seed, optional
-            A random number generator instance.
-
-        n_iter : int, optional
-            Maximum number of iterations to perform.
-
-        tol : float, optional
-            Convergence threshold. EM will stop if the gain in log-likelihood
-            is below this value.
-
-        verbose : bool, optional
-            Whether per-iteration convergence reports are printed to
-            :data:`sys.stderr`.  Convergence can also be diagnosed using the
-            :attr:`monitor_` attribute.
-
-        params, init_params : string, optional
-            The parameters that get updated during (``params``) or initialized
-            before (``init_params``) the training.  Can contain any
-            combination of 's' for startprob, 't' for transmat, and 'e' for
-            emissionprob.  Defaults to all parameters.
-
-        implementation: string, optional
-            Determines if the forward-backward algorithm is implemented with
-            logarithms ("log"), or using scaling ("scaling").  The default is
-            to use logarithms for backwards compatability.
-        """
-        BaseHMM.__init__(self, n_components,
-                         startprob_prior=startprob_prior,
-                         transmat_prior=transmat_prior,
-                         algorithm=algorithm,
-                         random_state=random_state,
-                         n_iter=n_iter, tol=tol, verbose=verbose,
-                         params=params, init_params=init_params,
-                         implementation=implementation)
-        self.n_trials = n_trials
-
-        _log.warning(
-            "MultinomialHMM has undergone major changes. "
-            "The previous version was implementing a CategoricalHMM "
-            "(a special case of MultinomialHMM). "
-            "This new implementation follows the standard definition for "
-            "a Multinomial distribution (e.g. as in "
-            "https://en.wikipedia.org/wiki/Multinomial_distribution). "
-            "See these issues for details:\n"
-            "https://github.com/hmmlearn/hmmlearn/issues/335\n"
-            "https://github.com/hmmlearn/hmmlearn/issues/340")
-
-    def _get_n_fit_scalars_per_param(self):
-        nc = self.n_components
-        nf = self.n_features
-        return {
-            "s": nc - 1,
-            "t": nc * (nc - 1),
-            "e": nc * (nf - 1),
-        }
-
-    def _check_and_set_multinomial_n_features_n_trials(self, X):
-        """
-        Check if ``X`` is a sample from a multinomial distribution, i.e. an
-        array of non-negative integers, summing up to n_trials.
-        """
-        n_samples, n_features = X.shape
-        self.n_features = n_features
-
-        if not np.issubdtype(X.dtype, np.integer) or X.min() < 0:
-            raise ValueError("Symbol counts should be nonnegative integers")
-
-        sample_n_trials = X.sum(axis=1)[0]
-        if self.n_trials is None:
-            self.n_trials = sample_n_trials
-
-        if not (X.sum(axis=1) == self.n_trials).all():
-            raise ValueError("Total count for each sample should add up to "
-                             "the number of trials")
-
-    def _init(self, X):
-        self._check_and_set_multinomial_n_features_n_trials(X)
-        super()._init(X)
-        self.random_state = check_random_state(self.random_state)
-        if 'e' in self.init_params:
-            self.emissionprob_ = self.random_state \
-                .rand(self.n_components, self.n_features)
-            normalize(self.emissionprob_, axis=1)
-
-    def _check(self):
-        super()._check()
-        self.emissionprob_ = np.atleast_2d(self.emissionprob_)
-        n_features = getattr(self, "n_features", self.emissionprob_.shape[1])
-        if self.emissionprob_.shape != (self.n_components, n_features):
-            raise ValueError(
-                "emissionprob_ must have shape (n_components, n_features)")
-        else:
-            self.n_features = n_features
-
-    def _compute_likelihood(self, X):
-        probs = []
-        for component in range(self.n_components):
-            score = multinomial.pmf(
-                X, n=self.n_trials, p=self.emissionprob_[component, :])
-            probs.append(score)
-        return np.vstack(probs).T
-
-    def _compute_log_likelihood(self, X):
-        logprobs = []
-        for component in range(self.n_components):
-            score = multinomial.logpmf(
-                X, n=self.n_trials, p=self.emissionprob_[component, :])
-            logprobs.append(score)
-        return np.vstack(logprobs).T
-
-    def _generate_sample_from_state(self, state, random_state):
-        sample = multinomial.rvs(
-            n=self.n_trials, p=self.emissionprob_[state, :],
-            size=1, random_state=self.random_state)
-        return sample.squeeze(0)  # shape (1, nf) -> (nf,)
-
-    def _initialize_sufficient_statistics(self):
-        stats = super()._initialize_sufficient_statistics()
-        stats['obs'] = np.zeros((self.n_components, self.n_features))
-        return stats
-
-    def _accumulate_sufficient_statistics(self, stats, X, framelogprob,
-                                          posteriors, fwdlattice, bwdlattice):
-        super()._accumulate_sufficient_statistics(
-            stats, X, framelogprob, posteriors, fwdlattice, bwdlattice)
-        if 'e' in self.params:
-            stats['obs'] += np.dot(posteriors.T, X)
-
-    def _do_mstep(self, stats):
-        super()._do_mstep(stats)
-        if 'e' in self.params:
-            self.emissionprob_ = (
-                stats['obs'] / stats['obs'].sum(axis=1, keepdims=True))
-
-
-_CATEGORICALHMM_DOC_SUFFIX = """
-
-Notes
------
-Unlike other HMM classes, `CategoricalHMM` ``X`` arrays have shape
-``(n_samples, 1)`` (instead of ``(n_samples, n_features)``).  Consider using
-`sklearn.preprocessing.LabelEncoder` to transform your input to the right
-format.
-"""
-
-
-def _categoricalhmm_fix_docstring_shape(func):
-    doc = inspect.getdoc(func)
-    if doc is None:
-        wrapper = func
-    else:
-        wrapper = functools.wraps(func)(
-            lambda *args, **kwargs: func(*args, **kwargs))
-        wrapper.__doc__ = (
-            doc.replace("(n_samples, n_features)", "(n_samples, 1)")
-            + _CATEGORICALHMM_DOC_SUFFIX)
-    return wrapper
-
-
-class CategoricalHMM(BaseHMM):
-    """
-    Hidden Markov Model with categorical (discrete) emissions.
-
-    Attributes
-    ----------
-    n_features : int
-        Number of possible symbols emitted by the model (in the samples).
-
-    monitor_ : ConvergenceMonitor
-        Monitor object used to check the convergence of EM.
-
-    startprob_ : array, shape (n_components, )
-        Initial state occupation distribution.
-
-    transmat_ : array, shape (n_components, n_components)
-        Matrix of transition probabilities between states.
-
-    emissionprob_ : array, shape (n_components, n_features)
-        Probability of emitting a given symbol when in each state.
-
-    Examples
-    --------
-    >>> from hmmlearn.hmm import CategoricalHMM
-    >>> CategoricalHMM(n_components=2)  #doctest: +ELLIPSIS
-    CategoricalHMM(algorithm='viterbi',...
-    """
-
-    def __init__(self, n_components=1, startprob_prior=1.0,
-                 transmat_prior=1.0, *, emissionprob_prior=1.0,
-                 algorithm="viterbi", random_state=None,
-                 n_iter=10, tol=1e-2, verbose=False,
-                 params="ste", init_params="ste",
-                 implementation="log"):
-        """
-        Parameters
-        ----------
-        n_components : int
-            Number of states.
-
-        startprob_prior : array, shape (n_components, ), optional
-            Parameters of the Dirichlet prior distribution for
-            :attr:`startprob_`.
-
-        transmat_prior : array, shape (n_components, n_components), optional
-            Parameters of the Dirichlet prior distribution for each row
-            of the transition probabilities :attr:`transmat_`.
-
-        emissionprob_prior : array, shape (n_components, n_features), optional
-            Parameters of the Dirichlet prior distribution for
-            :attr:`emissionprob_`.
-
-        algorithm : {"viterbi", "map"}, optional
-            Decoder algorithm.
-
-        random_state: RandomState or an int seed, optional
-            A random number generator instance.
-
-        n_iter : int, optional
-            Maximum number of iterations to perform.
-
-        tol : float, optional
-            Convergence threshold. EM will stop if the gain in log-likelihood
-            is below this value.
-
-        verbose : bool, optional
-            Whether per-iteration convergence reports are printed to
-            :data:`sys.stderr`.  Convergence can also be diagnosed using the
-            :attr:`monitor_` attribute.
-
-        params, init_params : string, optional
-            The parameters that get updated during (``params``) or initialized
-            before (``init_params``) the training.  Can contain any
-            combination of 's' for startprob, 't' for transmat, and 'e' for
-            emissionprob.  Defaults to all parameters.
-
-        implementation: string, optional
-            Determines if the forward-backward algorithm is implemented with
-            logarithms ("log"), or using scaling ("scaling").  The default is
-            to use logarithms for backwards compatability.
-        """
-        BaseHMM.__init__(self, n_components,
-                         startprob_prior=startprob_prior,
-                         transmat_prior=transmat_prior,
-                         algorithm=algorithm,
-                         random_state=random_state,
-                         n_iter=n_iter, tol=tol, verbose=verbose,
-                         params=params, init_params=init_params,
-                         implementation=implementation)
-        self.emissionprob_prior = emissionprob_prior
-
-    score_samples, score, decode, predict, predict_proba, sample, fit = map(
-        _categoricalhmm_fix_docstring_shape, [
-            BaseHMM.score_samples,
-            BaseHMM.score,
-            BaseHMM.decode,
-            BaseHMM.predict,
-            BaseHMM.predict_proba,
-            BaseHMM.sample,
-            BaseHMM.fit,
-        ])
-
-    def _get_n_fit_scalars_per_param(self):
-        nc = self.n_components
-        nf = self.n_features
-        return {
-            "s": nc - 1,
-            "t": nc * (nc - 1),
-            "e": nc * (nf - 1),
-        }
-
-    def _init(self, X):
-        self._check_and_set_categorical_n_features(X)
-        super()._init(X)
-        self.random_state = check_random_state(self.random_state)
-
-        if self._needs_init('e', 'emissionprob_'):
-            self.emissionprob_ = self.random_state.rand(
-                self.n_components, self.n_features)
-            normalize(self.emissionprob_, axis=1)
-
-    def _check(self):
-        super()._check()
-
-        self.emissionprob_ = np.atleast_2d(self.emissionprob_)
-        n_features = getattr(self, "n_features", self.emissionprob_.shape[1])
-        if self.emissionprob_.shape != (self.n_components, n_features):
-            raise ValueError(
-                "emissionprob_ must have shape (n_components, n_features)")
-        self._check_sum_1("emissionprob_")
-        self.n_features = n_features
-
-    def _compute_likelihood(self, X):
-        return self.emissionprob_[:, np.concatenate(X)].T
-
-    def _generate_sample_from_state(self, state, random_state):
-        cdf = np.cumsum(self.emissionprob_[state, :])
-        return [(cdf > random_state.rand()).argmax()]
-
-    def _initialize_sufficient_statistics(self):
-        stats = super()._initialize_sufficient_statistics()
-        stats['obs'] = np.zeros((self.n_components, self.n_features))
-        return stats
-
-    def _accumulate_sufficient_statistics(self, stats, X, lattice,
-                                          posteriors, fwdlattice, bwdlattice):
-        super()._accumulate_sufficient_statistics(
-            stats, X, lattice, posteriors, fwdlattice, bwdlattice)
-        if 'e' in self.params:
-            np.add.at(stats['obs'].T, np.concatenate(X), posteriors)
-
-    def _do_mstep(self, stats):
-        super()._do_mstep(stats)
-        if 'e' in self.params:
-            self.emissionprob_ = np.maximum(
-                self.emissionprob_prior - 1 + stats['obs'], 0)
-            normalize(self.emissionprob_, axis=1)
-
-    def _check_and_set_categorical_n_features(self, X):
-        """
-        Check if ``X`` is a sample from a categorical distribution, i.e. an
-        array of non-negative integers.
-        """
-        if not np.issubdtype(X.dtype, np.integer):
-            raise ValueError("Symbols should be integers")
-        if X.min() < 0:
-            raise ValueError("Symbols should be nonnegative")
-        if hasattr(self, "n_features"):
-            if self.n_features - 1 < X.max():
-                raise ValueError(
-                    f"Largest symbol is {X.max()} but the model only emits "
-                    f"symbols up to {self.n_features - 1}")
-        else:
-            self.n_features = X.max() + 1
-
-
-class GMMHMM(BaseHMM):
+class GMMHMM(_emissions.BaseGMMHMM):
     """
     Hidden Markov Model with Gaussian mixture emissions.
 
     Attributes
     ----------
     monitor_ : ConvergenceMonitor
         Monitor object used to check the convergence of EM.
@@ -809,15 +487,15 @@
         params, init_params : string, optional
             The parameters that get updated during (``params``) or initialized
             before (``init_params``) the training.  Can contain any combination
             of 's' for startprob, 't' for transmat, 'm' for means, 'c'
             for covars, and 'w' for GMM mixing weights.  Defaults to all
             parameters.
 
-        implementation: string, optional
+        implementation : string, optional
             Determines if the forward-backward algorithm is implemented with
             logarithms ("log"), or using scaling ("scaling").  The default is
             to use logarithms for backwards compatability.
         """
         BaseHMM.__init__(self, n_components,
                          startprob_prior=startprob_prior,
                          transmat_prior=transmat_prior,
@@ -830,54 +508,38 @@
         self.n_mix = n_mix
         self.weights_prior = weights_prior
         self.means_prior = means_prior
         self.means_weight = means_weight
         self.covars_prior = covars_prior
         self.covars_weight = covars_weight
 
-    def _get_n_fit_scalars_per_param(self):
-        nc = self.n_components
-        nf = self.n_features
-        nm = self.n_mix
-        return {
-            "s": nc - 1,
-            "t": nc * (nc - 1),
-            "m": nc * nm * nf,
-            "c": {
-                "spherical": nc * nm,
-                "diag": nc * nm * nf,
-                "full": nc * nm * nf * (nf + 1) // 2,
-                "tied": nc * nf * (nf + 1) // 2,
-            }[self.covariance_type],
-            "w": nm - 1,
-        }
-
-    def _init(self, X):
-        _check_and_set_n_features(self, X)
-        super()._init(X)
+    def _init(self, X, lengths=None):
+        super()._init(X, lengths=None)
         nc = self.n_components
         nf = self.n_features
         nm = self.n_mix
 
         def compute_cv():
             return np.cov(X.T) + self.min_covar * np.eye(nf)
 
         # Default values for covariance prior parameters
         self._init_covar_priors()
         self._fix_priors_shape()
 
         main_kmeans = cluster.KMeans(n_clusters=nc,
-                                     random_state=self.random_state)
+                                     random_state=self.random_state,
+                                     n_init=10)  # sklearn >=1.2 compat.
         cv = None  # covariance matrix
         labels = main_kmeans.fit_predict(X)
         main_centroid = np.mean(main_kmeans.cluster_centers_, axis=0)
         means = []
         for label in range(nc):
             kmeans = cluster.KMeans(n_clusters=nm,
-                                    random_state=self.random_state)
+                                    random_state=self.random_state,
+                                    n_init=10)  # sklearn >=1.2 compat.
             X_cluster = X[np.where(labels == label)]
             if X_cluster.shape[0] >= nm:
                 kmeans.fit(X_cluster)
                 means.append(kmeans.cluster_centers_)
             else:
                 if cv is None:
                     cv = compute_cv()
@@ -1047,123 +709,14 @@
                         raise ValueError(
                             f"Covariance of state #{i}, mixture #{j} is not "
                             f"positive definite")
                     if min_eigvalsh == 0:
                         _log.warning("Covariance of state #%d, mixture #%d "
                                      "has a null eigenvalue.", i, j)
 
-    def _generate_sample_from_state(self, state, random_state):
-        cur_weights = self.weights_[state]
-        i_gauss = random_state.choice(self.n_mix, p=cur_weights)
-        if self.covariance_type == 'tied':
-            # self.covars_.shape == (n_components, n_features, n_features)
-            # shouldn't that be (n_mix, ...)?
-            covs = self.covars_
-        else:
-            covs = self.covars_[:, i_gauss]
-            covs = fill_covars(covs, self.covariance_type,
-                               self.n_components, self.n_features)
-        return random_state.multivariate_normal(
-            self.means_[state, i_gauss], covs[state]
-        )
-
-    def _compute_log_weighted_gaussian_densities(self, X, i_comp):
-        cur_means = self.means_[i_comp]
-        cur_covs = self.covars_[i_comp]
-        if self.covariance_type == 'spherical':
-            cur_covs = cur_covs[:, None]
-        log_cur_weights = np.log(self.weights_[i_comp])
-
-        return log_multivariate_normal_density(
-            X, cur_means, cur_covs, self.covariance_type
-        ) + log_cur_weights
-
-    def _compute_log_likelihood(self, X):
-        n_samples, _ = X.shape
-        res = np.zeros((n_samples, self.n_components))
-
-        for i in range(self.n_components):
-            log_denses = self._compute_log_weighted_gaussian_densities(X, i)
-            with np.errstate(under="ignore"):
-                res[:, i] = special.logsumexp(log_denses, axis=1)
-
-        return res
-
-    def _initialize_sufficient_statistics(self):
-        stats = super()._initialize_sufficient_statistics()
-        stats['post_mix_sum'] = np.zeros((self.n_components, self.n_mix))
-        stats['post_sum'] = np.zeros(self.n_components)
-
-        if 'm' in self.params:
-            lambdas, mus = self.means_weight, self.means_prior
-            stats['m_n'] = lambdas[:, :, None] * mus
-        if 'c' in self.params:
-            stats['c_n'] = np.zeros_like(self.covars_)
-
-        # These statistics are stored in arrays and updated in-place.
-        # We accumulate chunks of data for multiple sequences (aka
-        # multiple frames) during fitting. The fit(X, lengths) method
-        # in the BaseHMM class will call
-        # _accumulate_sufficient_statistics once per sequence in the
-        # training samples. Data from all sequences needs to be
-        # accumulated and fed into _do_mstep.
-        return stats
-
-    def _accumulate_sufficient_statistics(self, stats, X, lattice,
-                                          post_comp, fwdlattice, bwdlattice):
-        super()._accumulate_sufficient_statistics(
-            stats, X, lattice, post_comp, fwdlattice, bwdlattice
-        )
-
-        n_samples, _ = X.shape
-
-        # Statistics shapes:
-        # post_comp_mix     (n_samples, n_components, n_mix)
-        # samples           (n_samples, n_features)
-        # centered          (n_samples, n_components, n_mix, n_features)
-
-        post_mix = np.zeros((n_samples, self.n_components, self.n_mix))
-        for p in range(self.n_components):
-            log_denses = self._compute_log_weighted_gaussian_densities(X, p)
-            log_normalize(log_denses, axis=-1)
-            with np.errstate(under="ignore"):
-                post_mix[:, p, :] = np.exp(log_denses)
-
-        with np.errstate(under="ignore"):
-            post_comp_mix = post_comp[:, :, None] * post_mix
-
-        stats['post_mix_sum'] += post_comp_mix.sum(axis=0)
-        stats['post_sum'] += post_comp.sum(axis=0)
-
-        if 'm' in self.params:  # means stats
-            stats['m_n'] += np.einsum('ijk,il->jkl', post_comp_mix, X)
-
-        if 'c' in self.params:  # covariance stats
-            centered = X[:, None, None, :] - self.means_
-
-            def outer_f(x):  # Outer product over features.
-                return x[..., :, None] * x[..., None, :]
-
-            if self.covariance_type == 'full':
-                centered_dots = outer_f(centered)
-                c_n = np.einsum('ijk,ijklm->jklm', post_comp_mix,
-                                     centered_dots)
-            elif self.covariance_type == 'diag':
-                centered2 = np.square(centered, out=centered)  # reuse
-                c_n = np.einsum('ijk,ijkl->jkl', post_comp_mix, centered2)
-            elif self.covariance_type == 'spherical':
-                # Faster than (x**2).sum(-1).
-                centered_norm2 = np.einsum('...i,...i', centered, centered)
-                c_n = np.einsum('ijk,ijk->jk', post_comp_mix, centered_norm2)
-            elif self.covariance_type == 'tied':
-                centered_dots = outer_f(centered)
-                c_n = np.einsum('ijk,ijklm->jlm', post_comp_mix, centered_dots)
-
-            stats['c_n'] += c_n
-
     def _do_mstep(self, stats):
         super()._do_mstep(stats)
         nf = self.n_features
         nm = self.n_mix
 
         # Maximizing weights
         if 'w' in self.params:
@@ -1234,15 +787,142 @@
                                 lambdas, centered_means_dots) + psis_t
                 c_n += stats['c_n']
                 c_d = (stats['post_sum'] + nm + nus + nf + 1)[:, None, None]
 
             self.covars_ = c_n / c_d
 
 
-class PoissonHMM(BaseHMM):
+class MultinomialHMM(_emissions.BaseMultinomialHMM):
+    """
+    Hidden Markov Model with multinomial emissions.
+
+    Attributes
+    ----------
+    n_features : int
+        Number of possible symbols emitted by the model (in the samples).
+
+    monitor_ : ConvergenceMonitor
+        Monitor object used to check the convergence of EM.
+
+    startprob_ : array, shape (n_components, )
+        Initial state occupation distribution.
+
+    transmat_ : array, shape (n_components, n_components)
+        Matrix of transition probabilities between states.
+
+    emissionprob_ : array, shape (n_components, n_features)
+        Probability of emitting a given symbol when in each state.
+
+    Examples
+    --------
+    >>> from hmmlearn.hmm import MultinomialHMM
+    """
+
+    def __init__(self, n_components=1, n_trials=None,
+                 startprob_prior=1.0, transmat_prior=1.0,
+                 algorithm="viterbi", random_state=None,
+                 n_iter=10, tol=1e-2, verbose=False,
+                 params="ste", init_params="ste",
+                 implementation="log"):
+        """
+        Parameters
+        ----------
+        n_components : int
+            Number of states.
+
+        n_trials : int or array of int
+            Number of trials (when sampling, all samples must have the same
+            :attr:`n_trials`).
+
+        startprob_prior : array, shape (n_components, ), optional
+            Parameters of the Dirichlet prior distribution for
+            :attr:`startprob_`.
+
+        transmat_prior : array, shape (n_components, n_components), optional
+            Parameters of the Dirichlet prior distribution for each row
+            of the transition probabilities :attr:`transmat_`.
+
+        algorithm : {"viterbi", "map"}, optional
+            Decoder algorithm.
+
+        random_state: RandomState or an int seed, optional
+            A random number generator instance.
+
+        n_iter : int, optional
+            Maximum number of iterations to perform.
+
+        tol : float, optional
+            Convergence threshold. EM will stop if the gain in log-likelihood
+            is below this value.
+
+        verbose : bool, optional
+            Whether per-iteration convergence reports are printed to
+            :data:`sys.stderr`.  Convergence can also be diagnosed using the
+            :attr:`monitor_` attribute.
+
+        params, init_params : string, optional
+            The parameters that get updated during (``params``) or initialized
+            before (``init_params``) the training.  Can contain any
+            combination of 's' for startprob, 't' for transmat, and 'e' for
+            emissionprob.  Defaults to all parameters.
+
+        implementation : string, optional
+            Determines if the forward-backward algorithm is implemented with
+            logarithms ("log"), or using scaling ("scaling").  The default is
+            to use logarithms for backwards compatability.
+        """
+        BaseHMM.__init__(self, n_components,
+                         startprob_prior=startprob_prior,
+                         transmat_prior=transmat_prior,
+                         algorithm=algorithm,
+                         random_state=random_state,
+                         n_iter=n_iter, tol=tol, verbose=verbose,
+                         params=params, init_params=init_params,
+                         implementation=implementation)
+        self.n_trials = n_trials
+
+        _log.warning(
+            "MultinomialHMM has undergone major changes. "
+            "The previous version was implementing a CategoricalHMM "
+            "(a special case of MultinomialHMM). "
+            "This new implementation follows the standard definition for "
+            "a Multinomial distribution (e.g. as in "
+            "https://en.wikipedia.org/wiki/Multinomial_distribution). "
+            "See these issues for details:\n"
+            "https://github.com/hmmlearn/hmmlearn/issues/335\n"
+            "https://github.com/hmmlearn/hmmlearn/issues/340")
+
+    def _init(self, X, lengths=None):
+        super()._init(X, lengths=None)
+        self.random_state = check_random_state(self.random_state)
+        if 'e' in self.init_params:
+            self.emissionprob_ = self.random_state \
+                .rand(self.n_components, self.n_features)
+            normalize(self.emissionprob_, axis=1)
+
+    def _check(self):
+        super()._check()
+        self.emissionprob_ = np.atleast_2d(self.emissionprob_)
+        n_features = getattr(self, "n_features", self.emissionprob_.shape[1])
+        if self.emissionprob_.shape != (self.n_components, n_features):
+            raise ValueError(
+                "emissionprob_ must have shape (n_components, n_features)")
+        else:
+            self.n_features = n_features
+        if self.n_trials is None:
+            raise ValueError("n_trials must be set")
+
+    def _do_mstep(self, stats):
+        super()._do_mstep(stats)
+        if 'e' in self.params:
+            self.emissionprob_ = (
+                stats['obs'] / stats['obs'].sum(axis=1, keepdims=True))
+
+
+class PoissonHMM(_emissions.BasePoissonHMM):
     """
     Hidden Markov Model with Poisson emissions.
 
     Attributes
     ----------
     monitor_ : ConvergenceMonitor
         Monitor object used to check the convergence of EM.
@@ -1304,15 +984,15 @@
 
         params, init_params : string, optional
             The parameters that get updated during (``params``) or initialized
             before (``init_params``) the training.  Can contain any
             combination of 's' for startprob, 't' for transmat, and 'l' for
             lambdas.  Defaults to all parameters.
 
-        implementation: string, optional
+        implementation : string, optional
             Determines if the forward-backward algorithm is implemented with
             logarithms ("log"), or using scaling ("scaling").  The default is
             to use logarithms for backwards compatability.
         """
         BaseHMM.__init__(self, n_components,
                          startprob_prior=startprob_prior,
                          transmat_prior=transmat_prior,
@@ -1320,73 +1000,38 @@
                          random_state=random_state,
                          n_iter=n_iter, tol=tol, verbose=verbose,
                          params=params, init_params=init_params,
                          implementation=implementation)
         self.lambdas_prior = lambdas_prior
         self.lambdas_weight = lambdas_weight
 
-    def _init(self, X):
-        _check_and_set_n_features(self, X)
-        super()._init(X)
+    def _init(self, X, lengths=None):
+        super()._init(X, lengths)
         self.random_state = check_random_state(self.random_state)
 
         mean_X = X.mean()
         var_X = X.var()
 
         if self._needs_init("l", "lambdas_"):
             # initialize with method of moments based on X
             self.lambdas_ = self.random_state.gamma(
                 shape=mean_X**2 / var_X,
                 scale=var_X / mean_X,  # numpy uses theta = 1 / beta
                 size=(self.n_components, self.n_features))
 
-    def _get_n_fit_scalars_per_param(self):
-        nc = self.n_components
-        nf = self.n_features
-        return {
-            "s": nc - 1,
-            "t": nc * (nc - 1),
-            "l": nc * nf,
-        }
-
     def _check(self):
         super()._check()
 
         self.lambdas_ = np.atleast_2d(self.lambdas_)
         n_features = getattr(self, "n_features", self.lambdas_.shape[1])
         if self.lambdas_.shape != (self.n_components, n_features):
             raise ValueError(
                 "lambdas_ must have shape (n_components, n_features)")
         self.n_features = n_features
 
-    def _generate_sample_from_state(self, state, random_state):
-        return random_state.poisson(self.lambdas_[state])
-
-    def _compute_log_likelihood(self, X):
-        return np.array([np.sum(poisson.logpmf(X, lambdas), axis=1)
-                         for lambdas in self.lambdas_]).T
-
-    def _compute_likelihood(self, X):
-        return np.array([np.prod(poisson.pmf(X, lambdas), axis=1)
-                         for lambdas in self.lambdas_]).T
-
-    def _initialize_sufficient_statistics(self):
-        stats = super()._initialize_sufficient_statistics()
-        stats['post'] = np.zeros(self.n_components)
-        stats['obs'] = np.zeros((self.n_components, self.n_features))
-        return stats
-
-    def _accumulate_sufficient_statistics(self, stats, obs, lattice,
-                                          posteriors, fwdlattice, bwdlattice):
-        super()._accumulate_sufficient_statistics(
-            stats, obs, lattice, posteriors, fwdlattice, bwdlattice)
-        if 'l' in self.params:
-            stats['post'] += posteriors.sum(axis=0)
-            stats['obs'] += np.dot(posteriors.T, obs)
-
     def _do_mstep(self, stats):
         super()._do_mstep(stats)
 
         if 'l' in self.params:
             # Based on: Hyvönen & Tolonen, "Bayesian Inference 2019"
             # section 3.2
             # https://vioshyvo.github.io/Bayesian_inference
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/stats.py` & `hmmlearn-0.3.0/lib/hmmlearn/stats.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_base.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
                                 [0.0408, 0.0150],
                                 [0.0298, 0.0046]])
         assert_allclose(np.exp(fwdlattice), reffwdlattice, 4)
 
     def test_do_forward_pass(self):
         log_prob, fwdlattice = _hmmc.forward_log(
             self.hmm.startprob_, self.hmm.transmat_, self.log_frameprob)
+
         ref_log_prob = -3.3725
         assert round(log_prob, 4) == ref_log_prob
         reffwdlattice = np.array([[0.4500, 0.1000],
                                   [0.3105, 0.0410],
                                   [0.0230, 0.0975],
                                   [0.0408, 0.0150],
                                   [0.0298, 0.0046]])
@@ -236,9 +237,9 @@
     n_components = 10
     h = StubHMM(n_components)
     transmat = np.random.random((n_components, n_components))
     transmat /= np.tile(transmat.sum(axis=1)[:, np.newaxis], (1, n_components))
     h.transmat_ = transmat
     stationary = h.get_stationary_distribution()
     assert stationary.dtype == float
-    assert np.dot(h.get_stationary_distribution().T, h.transmat_) \
-        == pytest.approx(stationary)
+    assert (h.get_stationary_distribution().T @ h.transmat_
+            == pytest.approx(stationary))
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_categorical_hmm.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_categorical_hmm.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,26 +56,44 @@
             [0.23170303, 0.76829697],
             [0.62406281, 0.37593719],
             [0.86397706, 0.13602294],
         ], rtol=0, atol=1e-6)
 
 
 class TestCategoricalHMM:
-    def setup(self):
-        self.n_components = 2
-        self.n_features = 3
+    n_components = 2
+    n_features = 3
 
     def new_hmm(self, impl):
         h = hmm.CategoricalHMM(self.n_components, implementation=impl)
         h.startprob_ = np.array([0.6, 0.4])
         h.transmat_ = np.array([[0.7, 0.3], [0.4, 0.6]])
         h.emissionprob_ = np.array([[0.1, 0.4, 0.5], [0.6, 0.3, 0.1]])
         return h
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
+    def test_n_features(self, implementation):
+        sequences, _ = self.new_hmm(implementation).sample(500)
+        # set n_features
+        model = hmm.CategoricalHMM(
+            n_components=2, implementation=implementation)
+
+        assert_log_likelihood_increasing(model, sequences, [500], 10)
+        assert model.n_features == 3
+
+        # Respect n_features
+        model = hmm.CategoricalHMM(
+            n_components=2,
+            implementation=implementation,
+            n_features=5)
+
+        assert_log_likelihood_increasing(model, sequences, [500], 10)
+        assert model.n_features == 5
+
+    @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_attributes(self, implementation):
         with pytest.raises(ValueError):
             h = self.new_hmm(implementation)
             h.emissionprob_ = []
             h._check()
         with pytest.raises(ValueError):
             h.emissionprob_ = np.zeros((self.n_components - 2,
@@ -130,24 +148,20 @@
         lengths = [10] * 10
         h = self.new_hmm(implementation)
         X, _state_sequence = h.sample(sum(lengths))
 
         # use init_function to initialize paramerters
         h = hmm.CategoricalHMM(self.n_components, params=params,
                                init_params=params)
-        h._init(X)
+        h._init(X, lengths)
 
         assert_log_likelihood_increasing(h, X, lengths, n_iter)
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test__check_and_set_categorical_n_features(self, implementation):
         h = self.new_hmm(implementation)
-        h._check_and_set_categorical_n_features(
-            np.array([[0, 0, 2, 1, 3, 1, 1]]))
-        h._check_and_set_categorical_n_features(
-            np.array([[0, 0, 1, 3, 1]], np.uint8))
+        h._check_and_set_n_features(np.array([[0, 0, 2, 1, 3, 1, 1]]).T)
+        h._check_and_set_n_features(np.array([[0, 0, 1, 3, 1]], np.uint8))
         with pytest.raises(ValueError):  # non-integral
-            h._check_and_set_categorical_n_features(
-                np.array([[0., 2., 1., 3.]]))
+            h._check_and_set_n_features(np.array([[0., 2., 1., 3.]]))
         with pytest.raises(ValueError):  # negative integers
-            h._check_and_set_categorical_n_features(
-                np.array([[0, -2, 1, 3, 1, 1]]))
+            h._check_and_set_n_features(np.array([[0, -2, 1, 3, 1, 1]]))
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_gaussian_hmm.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_gaussian_hmm.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
+from sklearn.utils import check_random_state
 
 from .. import hmm
 from . import assert_log_likelihood_increasing, make_covar_matrix, normalized
 
 
 class GaussianHMMTestMixin:
     covariance_type = None  # set by subclasses
 
     @pytest.fixture(autouse=True)
     def setup(self):
         self.prng = prng = np.random.RandomState(10)
         self.n_components = n_components = 3
         self.n_features = n_features = 3
-        self.startprob = prng.rand(n_components)
-        self.startprob = self.startprob / self.startprob.sum()
-        self.transmat = prng.rand(n_components, n_components)
-        self.transmat /= np.tile(self.transmat.sum(axis=1)[:, np.newaxis],
-                                 (1, n_components))
+        self.startprob = normalized(prng.rand(n_components))
+        self.transmat = normalized(
+            prng.rand(n_components, n_components), axis=1)
         self.means = prng.randint(-20, 20, (n_components, n_features))
         self.covars = make_covar_matrix(
             self.covariance_type, n_components, n_features, random_state=prng)
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_bad_covariance_type(self, implementation):
         with pytest.raises(ValueError):
@@ -45,15 +44,15 @@
         # picks the actual component used to generate the observations.
         h.means_ = 20 * h.means_
 
         gaussidx = np.repeat(np.arange(self.n_components), 5)
         n_samples = len(gaussidx)
         X = (self.prng.randn(n_samples, self.n_features)
              + h.means_[gaussidx])
-        h._init(X)
+        h._init(X, [n_samples])
         ll, posteriors = h.score_samples(X)
         assert posteriors.shape == (n_samples, self.n_components)
         assert_allclose(posteriors.sum(axis=1), np.ones(n_samples))
 
         viterbi_ll, stateseq = h.decode(X)
         assert_allclose(stateseq, gaussidx)
 
@@ -87,14 +86,42 @@
 
         # Mess up the parameters and see if we can re-learn them.
         # TODO: change the params and uncomment the check
         h.fit(X, lengths=lengths)
         # assert_log_likelihood_increasing(h, X, lengths, n_iter)
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
+    def test_criterion(self, implementation):
+        random_state = check_random_state(42)
+        m1 = hmm.GaussianHMM(self.n_components, init_params="",
+            covariance_type=self.covariance_type)
+        m1.startprob_ = self.startprob
+        m1.transmat_ = self.transmat
+        m1.means_ = self.means * 10
+        m1.covars_ = self.covars
+
+        X, _ = m1.sample(2000, random_state=random_state)
+
+        aic = []
+        bic = []
+        ns = [2, 3, 4]
+        for n in ns:
+            h = hmm.GaussianHMM(n, self.covariance_type, n_iter=500,
+                random_state=random_state, implementation=implementation)
+            h.fit(X)
+            aic.append(h.aic(X))
+            bic.append(h.bic(X))
+
+        assert np.all(aic) > 0
+        assert np.all(bic) > 0
+        # AIC / BIC pick the right model occasionally
+        # assert ns[np.argmin(aic)] == self.n_components
+        # assert ns[np.argmin(bic)] == self.n_components
+
+    @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_fit_ignored_init_warns(self, implementation, caplog):
         h = hmm.GaussianHMM(self.n_components, self.covariance_type,
                             implementation=implementation)
         h.startprob_ = self.startprob
         h.fit(np.random.randn(100, self.n_components))
         assert len(caplog.records) == 1, caplog
         assert "will be overwritten" in caplog.records[0].getMessage()
@@ -104,15 +131,15 @@
         h = hmm.GaussianHMM(
             self.n_components, self.covariance_type, init_params="",
             implementation=implementation)
         h.startprob_ = self.startprob
         h.transmat_ = self.transmat
         h.means_ = 20 * self.means
         h.covars_ = np.maximum(self.covars, 0.1)
-        h._init(np.random.randn(5, self.n_components))
+        h._init(np.random.randn(5, self.n_components), 5)
         assert len(caplog.records) == 1
         assert "degenerate solution" in caplog.records[0].getMessage()
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_fit_sequences_of_different_length(self, implementation):
         lengths = [3, 4, 5]
         X = self.prng.rand(sum(lengths), self.n_features)
@@ -265,15 +292,15 @@
     covariance_type = 'diag'
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_covar_is_writeable(self, implementation):
         h = hmm.GaussianHMM(n_components=1, covariance_type="diag",
                             init_params="c", implementation=implementation)
         X = np.random.normal(size=(1000, 5))
-        h._init(X)
+        h._init(X, 1000)
 
         # np.diag returns a read-only view of the array in NumPy 1.9.X.
         # Make sure this doesn't prevent us from fitting an HMM with
         # diagonal covariance matrix. See PR#44 on GitHub for details
         # and discussion.
         assert h._covars_.flags["WRITEABLE"]
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_gmm_hmm.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_gmm_hmm.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,20 +21,17 @@
 
 class GMMHMMTestMixin:
     def setup_method(self, method):
         self.prng = np.random.RandomState(9)
         self.n_components = 3
         self.n_mix = 2
         self.n_features = 2
-        self.startprob = self.prng.rand(self.n_components)
-        self.startprob = self.startprob / self.startprob.sum()
+        self.startprob = normalized(self.prng.rand(self.n_components))
         self.transmat = normalized(
-            self.prng.rand(self.n_components, self.n_components),
-            axis=1)
-
+            self.prng.rand(self.n_components, self.n_components), axis=1)
         self.gmms = []
         for state in range(self.n_components):
             self.gmms.append(create_random_gmm(
                 self.n_mix, self.n_features, self.covariance_type,
                 prng=self.prng))
 
     def test_score_samples_and_decode(self):
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_gmm_hmm_multisequence.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_gmm_hmm_multisequence.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_gmm_hmm_new.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_gmm_hmm_new.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 from numpy.testing import assert_allclose, assert_array_less
 import pytest
+from sklearn.utils import check_random_state
 
 from ..hmm import GMMHMM
 from .test_gmm_hmm import create_random_gmm
 from . import assert_log_likelihood_increasing, normalized
 
 
 def sample_from_parallelepiped(low, high, n_samples, random_state):
@@ -43,37 +44,33 @@
         covs = random_state.uniform(0.1, 5, size=(n_comps, n_mix))
     elif covar_type == "diag":
         covs = random_state.uniform(0.1, 5, size=(n_comps, n_mix, n_features))
     elif covar_type == "tied":
         covs = np.zeros((n_comps, n_features, n_features))
         for i in range(n_comps):
             low = random_state.uniform(-2, 2, (n_features, n_features))
-            covs[i] = np.dot(low.T, low)
+            covs[i] = low.T @ low
     elif covar_type == "full":
         covs = np.zeros((n_comps, n_mix, n_features, n_features))
         for i in range(n_comps):
             for j in range(n_mix):
                 low = random_state.uniform(-2, 2,
                                            size=(n_features, n_features))
-                covs[i, j] = np.dot(low.T, low)
+                covs[i, j] = low.T @ low
 
-    weights = normalized(random_state.uniform(size=(n_comps, n_mix)),
-                         axis=1)
+    weights = normalized(random_state.uniform(size=(n_comps, n_mix)), axis=1)
 
     return covs, means, startprob, transmat, weights
 
 
 class GMMHMMTestMixin:
-    def setup(self):
-        self.implementations = ["log", "scaling"]
-        self.n_components = 3
-        self.n_mix = 2
-        self.n_features = 2
-
-        self.low, self.high = 10, 15
+    n_components = 3
+    n_mix = 2
+    n_features = 2
+    low, high = 10, 15
 
     def new_hmm(self, implementation):
         prng = np.random.RandomState(14)
         covars, means, startprob, transmat, weights = prep_params(
             self.n_components, self.n_mix, self.n_features,
             self.covariance_type, self.low, self.high, prng)
         h = GMMHMM(n_components=self.n_components, n_mix=self.n_mix,
@@ -108,15 +105,15 @@
         assert len(states) == n_samples
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_init(self, implementation):
         n_samples = 1000
         h = self.new_hmm(implementation)
         X, _states = h.sample(n_samples)
-        h._init(X)
+        h._init(X, [n_samples])
         h._check()  # should not raise any errors
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_score_samples_and_decode(self, implementation):
         n_samples = 1000
         h = self.new_hmm(implementation)
         X, states = h.sample(n_samples)
@@ -153,15 +150,15 @@
         n_samples = 1000
         h = self.new_hmm(implementation)
         h.means_ *= 1000  # this will put gaussians very far apart
         X, _states = h.sample(n_samples)
 
         # this should not raise
         # "ValueError: array must not contain infs or NaNs"
-        h._init(X)
+        h._init(X, [1000])
         h.fit(X)
 
     @pytest.mark.xfail
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_fit_zero_variance(self, implementation):
         # Example from issue #2 on GitHub.
         # this data has singular covariance matrix
@@ -176,14 +173,38 @@
             [7.15000000e+02, 1.3000000e+02, 4.09387207e+00, -5.83621216e+01],
             [7.15000000e+02, 6.5000000e+01, -1.21667480e+00, -4.48131409e+01]
         ])
 
         h = self.new_hmm(implementation)
         h.fit(X)
 
+    @pytest.mark.parametrize("implementation", ["scaling", "log"])
+    def test_criterion(self, implementation):
+        random_state = check_random_state(2013)
+        m1 = self.new_hmm(implementation)
+        # Spread the means out to make this easier
+        m1.means_ *= 10
+
+        X, _ = m1.sample(4000, random_state=random_state)
+        aic = []
+        bic = []
+        ns = [2, 3, 4, 5]
+        for n in ns:
+            h = GMMHMM(n, n_mix=2, covariance_type=self.covariance_type,
+                random_state=random_state, implementation=implementation)
+            h.fit(X)
+            aic.append(h.aic(X))
+            bic.append(h.bic(X))
+
+        assert np.all(aic) > 0
+        assert np.all(bic) > 0
+        # AIC / BIC pick the right model occasionally
+        # assert ns[np.argmin(aic)] == self.n_components
+        # assert ns[np.argmin(bic)] == self.n_components
+
 
 class TestGMMHMMWithSphericalCovars(GMMHMMTestMixin):
     covariance_type = 'spherical'
 
 
 class TestGMMHMMWithDiagCovars(GMMHMMTestMixin):
     covariance_type = 'diag'
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_multinomial_hmm.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_multinomial_hmm.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 
 from hmmlearn import hmm
 
 from . import assert_log_likelihood_increasing, normalized
 
 
 class TestMultinomialHMM:
-    def setup(self):
-        self.n_components = 2
-        self.n_features = 4
-        self.n_trials = 5
+    n_components = 2
+    n_features = 4
+    n_trials = 5
 
     def new_hmm(self, impl):
         h = hmm.MultinomialHMM(
             n_components=self.n_components,
             n_trials=self.n_trials,
             implementation=impl)
         h.startprob_ = np.array([.6, .4])
@@ -59,14 +58,20 @@
     def test_sample(self, implementation, n_samples=1000):
         h = self.new_hmm(implementation)
         X, state_sequence = h.sample(n_samples)
         assert X.ndim == 2
         assert len(X) == len(state_sequence) == n_samples
         assert len(np.unique(X)) == self.n_trials + 1
         assert (X.sum(axis=1) == self.n_trials).all()
+        h.n_trials = None
+        with pytest.raises(ValueError):
+            h.sample(n_samples)
+        h.n_trials = [1, 2, 3]
+        with pytest.raises(ValueError):
+            h.sample(n_samples)
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_fit(self, implementation, params='ste', n_iter=5):
         h = self.new_hmm(implementation)
         h.params = params
 
         lengths = np.array([10] * 10)
@@ -76,14 +81,17 @@
         h.startprob_ = normalized(np.random.random(self.n_components))
         h.transmat_ = normalized(
             np.random.random((self.n_components, self.n_components)),
             axis=1)
         h.emissionprob_ = normalized(
             np.random.random((self.n_components, self.n_features)),
             axis=1)
+        # Also mess up trial counts.
+        h.n_trials = None
+        X[::2] *= 2
 
         assert_log_likelihood_increasing(h, X, lengths, n_iter)
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_fit_emissionprob(self, implementation):
         self.test_fit(implementation, 'e')
 
@@ -93,37 +101,37 @@
         h = self.new_hmm(implementation)
         X, _state_sequence = h.sample(sum(lengths))
 
         # use init_function to initialize paramerters
         h = hmm.MultinomialHMM(
             n_components=self.n_components, n_trials=self.n_trials,
             params=params, init_params=params)
-        h._init(X)
+        h._init(X, lengths)
 
         assert_log_likelihood_increasing(h, X, lengths, n_iter)
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test__check_and_set_multinomial_n_features_n_trials(
             self, implementation):
         h = hmm.MultinomialHMM(
             n_components=2, n_trials=None, implementation=implementation)
-        h._check_and_set_multinomial_n_features_n_trials(
+        h._check_and_set_n_features(
             np.array([[0, 2, 3, 0], [1, 0, 2, 2]]))
-        assert h.n_trials == 5
+        assert (h.n_trials == 5).all()
         with pytest.raises(ValueError):  # wrong dimensions
-            h._check_and_set_multinomial_n_features_n_trials(
-                    np.array([[0, 0, 2, 1, 3, 1, 1]]))
+            h._check_and_set_n_features(
+                np.array([[0, 0, 2, 1, 3, 1, 1]]))
         with pytest.raises(ValueError):  # not added up to n_trials
-            h._check_and_set_multinomial_n_features_n_trials(
-                    np.array([[0, 0, 1, 1], [3, 1, 1, 0]]))
+            h._check_and_set_n_features(
+                np.array([[0, 0, 1, 1], [3, 1, 1, 0]]))
         with pytest.raises(ValueError):  # non-integral
-            h._check_and_set_multinomial_n_features_n_trials(
+            h._check_and_set_n_features(
                 np.array([[0., 2., 0., 3.], [0.0, 2.5, 2.5, 0.0]]))
         with pytest.raises(ValueError):  # negative integers
-            h._check_and_set_multinomial_n_features_n_trials(
+            h._check_and_set_n_features(
                 np.array([[0, -2, 1, 6], [5, 6, -6, 0]]))
 
     @pytest.mark.parametrize("implementation", ["scaling", "log"])
     def test_compare_with_categorical_hmm(self, implementation):
         n_components = 2   # ['Rainy', 'Sunny']
         n_features = 3     # ['walk', 'shop', 'clean']
         n_trials = 1
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_poisson_hmm.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_poisson_hmm.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import numpy as np
 from numpy.testing import assert_allclose
 import pytest
+from sklearn.utils import check_random_state
 
 from hmmlearn import hmm
 
 from . import assert_log_likelihood_increasing, normalized
 
 
 class TestPoissonHMM:
-
     n_components = 2
     n_features = 3
 
     def new_hmm(self, impl):
         h = hmm.PoissonHMM(self.n_components, implementation=impl,
                            random_state=0)
         h.startprob_ = np.array([0.6, 0.4])
@@ -70,10 +70,32 @@
         lengths = [10] * 10
         h = self.new_hmm(implementation)
         X, _state_sequence = h.sample(sum(lengths))
 
         # use init_function to initialize paramerters
         h = hmm.PoissonHMM(self.n_components, params=params,
                            init_params=params)
-        h._init(X)
+        h._init(X, lengths)
 
         assert_log_likelihood_increasing(h, X, lengths, n_iter)
+
+    @pytest.mark.parametrize("implementation", ["scaling", "log"])
+    def test_criterion(self, implementation):
+        random_state = check_random_state(412)
+        m1 = self.new_hmm(implementation)
+        X, _ = m1.sample(2000, random_state=random_state)
+
+        aic = []
+        bic = []
+        ns = [2, 3, 4]
+        for n in ns:
+            h = hmm.PoissonHMM(n, n_iter=500,
+                random_state=random_state, implementation=implementation)
+            h.fit(X)
+            aic.append(h.aic(X))
+            bic.append(h.bic(X))
+
+        assert np.all(aic) > 0
+        assert np.all(bic) > 0
+        # AIC / BIC pick the right model occasionally
+        # assert ns[np.argmin(aic)] == 2
+        # assert ns[np.argmin(bic)] == 2
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn/tests/test_utils.py` & `hmmlearn-0.3.0/lib/hmmlearn/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/lib/hmmlearn.egg-info/PKG-INFO` & `hmmlearn-0.3.0/lib/hmmlearn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hmmlearn
-Version: 0.2.8
+Version: 0.3.0
 Summary: Hidden Markov Models in Python with scikit-learn like API
 Home-page: https://github.com/hmmlearn/hmmlearn
 Maintainer: Antony Lee
 License: new BSD
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved
 Classifier: Intended Audience :: Developers
@@ -14,35 +14,36 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE.txt
+License-File: AUTHORS.rst
 
 hmmlearn
 ========
 
 | |GitHub| |PyPI|
 | |Read the Docs| |Build| |CodeCov|
 
 .. |GitHub|
    image:: https://img.shields.io/badge/github-hmmlearn%2Fhmmlearn-brightgreen
    :target: https://github.com/hmmlearn/hmmlearn
 .. |PyPI|
-   image:: https://img.shields.io/pypi/v/hmmlearn.svg
+   image:: https://img.shields.io/pypi/v/hmmlearn.svg?color=brightgreen
    :target: https://pypi.python.org/pypi/hmmlearn
 .. |Read the Docs|
    image:: https://readthedocs.org/projects/hmmlearn/badge/?version=latest
    :target: http://hmmlearn.readthedocs.io/en/latest/?badge=latest
 .. |Build|
-   image:: https://img.shields.io/github/workflow/status/hmmlearn/hmmlearn/build
+   image:: https://img.shields.io/github/actions/workflow/status/hmmlearn/hmmlearn/build.yml?branch=main
    :target: https://github.com/hmmlearn/hmmlearn/actions
 .. |CodeCov|
-   image:: https://codecov.io/gh/hmmlearn/hmmlearn/master.svg
+   image:: https://img.shields.io/codecov/c/github/hmmlearn/hmmlearn
    :target: https://codecov.io/gh/hmmlearn/hmmlearn
 
 hmmlearn is a set of algorithms for **unsupervised** learning and inference
 of Hidden Markov Models. For supervised learning learning of HMMs and similar
 models see seqlearn_.
 
 .. _seqlearn: https://github.com/larsmans/seqlearn
```

### Comparing `hmmlearn-0.2.8/lib/hmmlearn.egg-info/SOURCES.txt` & `hmmlearn-0.3.0/lib/hmmlearn.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,36 +17,44 @@
 doc/source/changelog.rst
 doc/source/conf.py
 doc/source/index.rst
 doc/source/tutorial.rst
 doc/source/_static/hide_some_gallery_elements.css
 examples/README.txt
 examples/plot_casino.py
+examples/plot_gaussian_model_selection.py
 examples/plot_hmm_sampling_and_decoding.py
 examples/plot_multinomial_hmm.py
 examples/plot_poisson_hmm.py
+examples/plot_variational_inference.py
 lib/hmmlearn/.gitignore
 lib/hmmlearn/__init__.py
+lib/hmmlearn/_emissions.py
+lib/hmmlearn/_kl_divergence.py
 lib/hmmlearn/_utils.py
 lib/hmmlearn/_version.py
 lib/hmmlearn/base.py
 lib/hmmlearn/hmm.py
 lib/hmmlearn/stats.py
 lib/hmmlearn/utils.py
+lib/hmmlearn/vhmm.py
 lib/hmmlearn.egg-info/PKG-INFO
 lib/hmmlearn.egg-info/SOURCES.txt
 lib/hmmlearn.egg-info/dependency_links.txt
 lib/hmmlearn.egg-info/requires.txt
 lib/hmmlearn.egg-info/top_level.txt
 lib/hmmlearn/tests/__init__.py
 lib/hmmlearn/tests/conftest.py
 lib/hmmlearn/tests/test_base.py
 lib/hmmlearn/tests/test_categorical_hmm.py
 lib/hmmlearn/tests/test_gaussian_hmm.py
 lib/hmmlearn/tests/test_gmm_hmm.py
 lib/hmmlearn/tests/test_gmm_hmm_multisequence.py
 lib/hmmlearn/tests/test_gmm_hmm_new.py
+lib/hmmlearn/tests/test_kl_divergence.py
 lib/hmmlearn/tests/test_multinomial_hmm.py
 lib/hmmlearn/tests/test_poisson_hmm.py
 lib/hmmlearn/tests/test_utils.py
+lib/hmmlearn/tests/test_variational_categorical.py
+lib/hmmlearn/tests/test_variational_gaussian.py
 scripts/benchmark.py
 src/_hmmc.cpp
```

### Comparing `hmmlearn-0.2.8/scripts/benchmark.py` & `hmmlearn-0.3.0/scripts/benchmark.py`

 * *Files identical despite different names*

### Comparing `hmmlearn-0.2.8/setup.py` & `hmmlearn-0.3.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         "version_scheme": "post-release",
         "local_scheme": "node-and-date",
         "write_to": "lib/hmmlearn/_version.py",
         "fallback_version": "0+unknown",
     },
     install_requires=[
         "numpy>=1.10",  # np.broadcast_to.
-        "scikit-learn>=0.16",  # sklearn.utils.check_array.
+        "scikit-learn>=0.16,!=0.22.0",  # check_array, check_is_fitted.
         "scipy>=0.19",  # scipy.special.logsumexp.
     ],
     extras_require={
         "tests": ["pytest"],
         "docs": [
             "matplotlib",
             "pydata_sphinx_theme",
```

### Comparing `hmmlearn-0.2.8/src/_hmmc.cpp` & `hmmlearn-0.3.0/src/_hmmc.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -59,15 +59,15 @@
     throw std::invalid_argument{"shape mismatch"};
   }
   auto fwdlattice_ = py::array_t<double>{{ns, nc}};
   auto fwd = fwdlattice_.mutable_unchecked<2>();
   auto scaling_ = py::array_t<double>{{ns}};
   auto scaling = scaling_.mutable_unchecked<1>();
   auto log_prob = 0.;
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   std::fill_n(fwd.mutable_data(0, 0), fwd.size(), 0);
   for (auto i = 0; i < nc; ++i) {
     fwd(0, i) = startprob(i) * frameprob(0, i);
   }
   auto sum = std::accumulate(&fwd(0, 0), &fwd(0, nc), 0.);
   if (sum < min_sum) {
     throw std::range_error{"forward pass failed with underflow; "
@@ -113,15 +113,15 @@
   if (log_startprob.shape(0) != nc
       || log_transmat.shape(0) != nc || log_transmat.shape(1) != nc) {
     throw std::invalid_argument{"shape mismatch"};
   }
   auto buf = std::vector<double>(nc);
   auto fwdlattice_ = py::array_t<double>{{ns, nc}};
   auto fwd = fwdlattice_.mutable_unchecked<2>();
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   for (auto i = 0; i < nc; ++i) {
     fwd(0, i) = log_startprob(i) + log_frameprob(0, i);
   }
   for (auto t = 1; t < ns; ++t) {
     for (auto j = 0; j < nc; ++j) {
       for (auto i = 0; i < nc; ++i) {
         buf[i] = fwd(t - 1, i) + log_transmat(i, j);
@@ -147,15 +147,15 @@
   if (startprob.shape(0) != nc
       || transmat.shape(0) != nc || transmat.shape(1) != nc
       || scaling.shape(0) != ns) {
     throw std::invalid_argument{"shape mismatch"};
   }
   auto bwdlattice_ = py::array_t<double>{{ns, nc}};
   auto bwd = bwdlattice_.mutable_unchecked<2>();
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   std::fill_n(bwd.mutable_data(0, 0), bwd.size(), 0);
   for (auto i = 0; i < nc; ++i) {
     bwd(ns - 1, i) = scaling(ns - 1);
   }
   for (auto t = ns - 2; t >= 0; --t) {
     for (auto i = 0; i < nc; ++i) {
       for (auto j = 0; j < nc; ++j) {
@@ -181,15 +181,15 @@
   if (log_startprob.shape(0) != nc
       || log_transmat.shape(0) != nc || log_transmat.shape(1) != nc) {
     throw std::invalid_argument{"shape mismatch"};
   }
   auto buf = std::vector<double>(nc);
   auto bwdlattice_ = py::array_t<double>{{ns, nc}};
   auto bwd = bwdlattice_.mutable_unchecked<2>();
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   for (auto i = 0; i < nc; ++i) {
     bwd(ns - 1, i) = 0;
   }
   for (auto t = ns - 2; t >= 0; --t) {
     for (auto i = 0; i < nc; ++i) {
       for (auto j = 0; j < nc; ++j) {
         buf[j] = log_transmat(i, j) + log_frameprob(t + 1, j) + bwd(t + 1, j);
@@ -215,15 +215,15 @@
       || transmat.shape(0) != nc || transmat.shape(1) != nc
       || bwd.shape(0) != ns || bwd.shape(1) != nc) {
     throw std::invalid_argument{"shape mismatch"};
   }
   auto xi_sum_ = py::array_t<double>{{nc, nc}};
   auto xi_sum = xi_sum_.mutable_unchecked<2>();
   std::fill_n(xi_sum.mutable_data(0, 0), xi_sum.size(), 0);
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   for (auto t = 0; t < ns - 1; ++t) {
     for (auto i = 0; i < nc; ++i) {
       for (auto j = 0; j < nc; ++j) {
         xi_sum(i, j) += fwd(t, i)
                         * transmat(i, j)
                         * frameprob(t + 1, j)
                         * bwd(t + 1, j);
@@ -251,15 +251,15 @@
     throw std::invalid_argument{"shape mismatch"};
   }
   auto log_prob = logsumexp(&fwd(ns - 1, 0), nc);
   auto log_xi_sum_ = py::array_t<double>{{nc, nc}};
   auto log_xi_sum = log_xi_sum_.mutable_unchecked<2>();
   std::fill_n(log_xi_sum.mutable_data(0, 0), log_xi_sum.size(),
               -std::numeric_limits<double>::infinity());
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   for (auto t = 0; t < ns - 1; ++t) {
     for (auto i = 0; i < nc; ++i) {
       for (auto j = 0; j < nc; ++j) {
         auto log_xi = fwd(t, i)
                       + log_transmat(i, j)
                       + log_frameprob(t + 1, j)
                       + bwd(t + 1, j)
@@ -286,15 +286,15 @@
       || log_transmat.shape(0) != nc || log_transmat.shape(1) != nc) {
     throw std::invalid_argument{"shape mismatch"};
   }
   auto state_sequence_ = py::array_t<ssize_t>{{ns}};
   auto viterbi_lattice_ = py::array_t<double>{{ns, nc}};
   auto state_sequence = state_sequence_.mutable_unchecked<1>();
   auto viterbi_lattice = viterbi_lattice_.mutable_unchecked<2>();
-  auto nogil = py::gil_scoped_release{};
+  py::gil_scoped_release nogil;
   for (auto i = 0; i < nc; ++i) {
     viterbi_lattice(0, i) = log_startprob(i) + log_frameprob(0, i);
   }
   for (auto t = 1; t < ns; ++t) {
     for (auto i = 0; i < nc; ++i) {
       auto max = -std::numeric_limits<double>::infinity();
       for (auto j = 0; j < nc; ++j) {
```

