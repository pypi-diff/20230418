# Comparing `tmp/PySR3-0.3.4.tar.gz` & `tmp/PySR3-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySR3-0.3.4.tar", last modified: Tue Mar 21 17:33:44 2023, max compression
+gzip compressed data, was "PySR3-0.3.5.tar", last modified: Tue Apr 18 00:43:22 2023, max compression
```

## Comparing `PySR3-0.3.4.tar` & `PySR3-0.3.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.703921 PySR3-0.3.4/
--rw-r--r--   0 aksh       (501) staff       (20)    35148 2021-08-18 22:29:02.000000 PySR3-0.3.4/LICENSE
--rw-r--r--   0 aksh       (501) staff       (20)      165 2023-03-21 17:28:48.000000 PySR3-0.3.4/MANIFEST.in
--rw-r--r--   0 aksh       (501) staff       (20)      641 2023-03-21 17:33:44.703652 PySR3-0.3.4/PKG-INFO
--rw-r--r--   0 aksh       (501) staff       (20)    10769 2022-12-31 18:56:23.000000 PySR3-0.3.4/README.md
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.693327 PySR3-0.3.4/docs/
--rw-r--r--   0 aksh       (501) staff       (20)     6148 2022-12-28 17:27:09.000000 PySR3-0.3.4/docs/.DS_Store
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.694336 PySR3-0.3.4/docs/.ipynb_checkpoints/
--rw-r--r--   0 aksh       (501) staff       (20)    65486 2022-12-31 18:52:41.000000 PySR3-0.3.4/docs/.ipynb_checkpoints/models_overview-checkpoint.ipynb
--rw-r--r--   0 aksh       (501) staff       (20)   105478 2022-12-31 18:54:38.000000 PySR3-0.3.4/docs/.ipynb_checkpoints/quickstart-checkpoint.ipynb
--rw-r--r--   0 aksh       (501) staff       (20)      634 2021-08-18 22:29:02.000000 PySR3-0.3.4/docs/Makefile
--rw-r--r--   0 aksh       (501) staff       (20)     2014 2021-09-06 21:01:26.000000 PySR3-0.3.4/docs/community_guidelines.ipynb
--rw-r--r--   0 aksh       (501) staff       (20)     2817 2021-09-06 21:01:09.000000 PySR3-0.3.4/docs/conf.py
--rw-r--r--   0 aksh       (501) staff       (20)      603 2023-01-03 22:16:08.000000 PySR3-0.3.4/docs/index.rst
--rw-r--r--   0 aksh       (501) staff       (20)      795 2021-08-18 22:29:02.000000 PySR3-0.3.4/docs/make.bat
--rw-r--r--   0 aksh       (501) staff       (20)    65486 2022-12-31 18:52:41.000000 PySR3-0.3.4/docs/models_overview.ipynb
--rw-r--r--   0 aksh       (501) staff       (20)   105478 2022-12-31 18:54:38.000000 PySR3-0.3.4/docs/quickstart.ipynb
--rwxr-xr-x   0 aksh       (501) staff       (20)      247 2021-09-06 21:01:09.000000 PySR3-0.3.4/docs/regenerate_docs.sh
--rw-r--r--   0 aksh       (501) staff       (20)   149060 2021-09-06 21:01:09.000000 PySR3-0.3.4/docs/sr3_mixed_intuition.png
--rw-r--r--   0 aksh       (501) staff       (20)       83 2021-09-06 21:01:09.000000 PySR3-0.3.4/requirements.txt
--rw-r--r--   0 aksh       (501) staff       (20)       38 2023-03-21 17:33:44.704013 PySR3-0.3.4/setup.cfg
--rw-r--r--   0 aksh       (501) staff       (20)     1314 2022-12-19 20:25:13.000000 PySR3-0.3.4/setup.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.687972 PySR3-0.3.4/src/
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.695996 PySR3-0.3.4/src/PySR3.egg-info/
--rw-r--r--   0 aksh       (501) staff       (20)      641 2023-03-21 17:33:44.000000 PySR3-0.3.4/src/PySR3.egg-info/PKG-INFO
--rw-r--r--   0 aksh       (501) staff       (20)     1284 2023-03-21 17:33:44.000000 PySR3-0.3.4/src/PySR3.egg-info/SOURCES.txt
--rw-r--r--   0 aksh       (501) staff       (20)        1 2023-03-21 17:33:44.000000 PySR3-0.3.4/src/PySR3.egg-info/dependency_links.txt
--rw-r--r--   0 aksh       (501) staff       (20)        1 2023-03-21 17:33:44.000000 PySR3-0.3.4/src/PySR3.egg-info/not-zip-safe
--rw-r--r--   0 aksh       (501) staff       (20)      205 2023-03-21 17:33:44.000000 PySR3-0.3.4/src/PySR3.egg-info/requires.txt
--rw-r--r--   0 aksh       (501) staff       (20)        6 2023-03-21 17:33:44.000000 PySR3-0.3.4/src/PySR3.egg-info/top_level.txt
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.697701 PySR3-0.3.4/src/pysr3/
--rw-r--r--   0 aksh       (501) staff       (20)     1852 2023-03-21 17:29:47.000000 PySR3-0.3.4/src/pysr3/__about__.py
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.4/src/pysr3/__init__.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.698774 PySR3-0.3.4/src/pysr3/linear/
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.4/src/pysr3/linear/__init__.py
--rw-r--r--   0 aksh       (501) staff       (20)    29909 2022-12-31 18:37:42.000000 PySR3-0.3.4/src/pysr3/linear/models.py
--rw-r--r--   0 aksh       (501) staff       (20)    11335 2022-12-20 20:16:57.000000 PySR3-0.3.4/src/pysr3/linear/oracles.py
--rw-r--r--   0 aksh       (501) staff       (20)     5441 2022-12-20 19:53:33.000000 PySR3-0.3.4/src/pysr3/linear/problems.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.700499 PySR3-0.3.4/src/pysr3/lme/
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.4/src/pysr3/lme/__init__.py
--rw-r--r--   0 aksh       (501) staff       (20)     6237 2022-12-21 04:47:12.000000 PySR3-0.3.4/src/pysr3/lme/model_selectors.py
--rw-r--r--   0 aksh       (501) staff       (20)    61961 2022-12-31 18:32:09.000000 PySR3-0.3.4/src/pysr3/lme/models.py
--rw-r--r--   0 aksh       (501) staff       (20)    59805 2022-12-19 20:25:13.000000 PySR3-0.3.4/src/pysr3/lme/oracles.py
--rw-r--r--   0 aksh       (501) staff       (20)     7675 2021-09-06 21:01:09.000000 PySR3-0.3.4/src/pysr3/lme/priors.py
--rw-r--r--   0 aksh       (501) staff       (20)    40739 2022-12-21 04:47:12.000000 PySR3-0.3.4/src/pysr3/lme/problems.py
--rw-r--r--   0 aksh       (501) staff       (20)     1936 2022-12-19 20:25:13.000000 PySR3-0.3.4/src/pysr3/logger.py
--rw-r--r--   0 aksh       (501) staff       (20)     4763 2021-09-07 23:08:16.000000 PySR3-0.3.4/src/pysr3/priors.py
--rw-r--r--   0 aksh       (501) staff       (20)    20759 2022-12-31 18:37:42.000000 PySR3-0.3.4/src/pysr3/regularizers.py
--rw-r--r--   0 aksh       (501) staff       (20)     6783 2022-12-19 20:25:13.000000 PySR3-0.3.4/src/pysr3/solvers.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.700841 PySR3-0.3.4/tests/
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-08-18 22:29:02.000000 PySR3-0.3.4/tests/__init__.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.701257 PySR3-0.3.4/tests/linear/
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.4/tests/linear/__init__.py
--rw-r--r--   0 aksh       (501) staff       (20)     8400 2022-12-31 18:46:48.000000 PySR3-0.3.4/tests/linear/test_LinearModels.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.702529 PySR3-0.3.4/tests/lme/
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.4/tests/lme/__init__.py
--rw-r--r--   0 aksh       (501) staff       (20)    13132 2022-12-19 20:25:13.000000 PySR3-0.3.4/tests/lme/test_LMEModels.py
--rw-r--r--   0 aksh       (501) staff       (20)    16047 2022-12-19 20:25:13.000000 PySR3-0.3.4/tests/lme/test_LMEOracle.py
--rw-r--r--   0 aksh       (501) staff       (20)     7068 2021-09-07 23:09:05.000000 PySR3-0.3.4/tests/lme/test_LMEProblem.py
--rw-r--r--   0 aksh       (501) staff       (20)     2472 2022-12-19 20:25:13.000000 PySR3-0.3.4/tests/lme/test_select_covariates.py
-drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-03-21 17:33:44.703252 PySR3-0.3.4/tests/test_core/
--rw-r--r--   0 aksh       (501) staff       (20)        0 2021-08-18 22:29:02.000000 PySR3-0.3.4/tests/test_core/__init__.py
--rw-r--r--   0 aksh       (501) staff       (20)      458 2021-09-06 21:01:09.000000 PySR3-0.3.4/tests/test_core/test_Priors.py
--rw-r--r--   0 aksh       (501) staff       (20)      212 2021-09-06 21:01:09.000000 PySR3-0.3.4/tests/test_core/test_Regularizers.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.682565 PySR3-0.3.5/
+-rw-r--r--   0 aksh       (501) staff       (20)    35148 2021-08-18 22:29:02.000000 PySR3-0.3.5/LICENSE
+-rw-r--r--   0 aksh       (501) staff       (20)      165 2023-03-21 17:28:48.000000 PySR3-0.3.5/MANIFEST.in
+-rw-r--r--   0 aksh       (501) staff       (20)      641 2023-04-18 00:43:22.682315 PySR3-0.3.5/PKG-INFO
+-rw-r--r--   0 aksh       (501) staff       (20)    10769 2022-12-31 18:56:23.000000 PySR3-0.3.5/README.md
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.663585 PySR3-0.3.5/docs/
+-rw-r--r--   0 aksh       (501) staff       (20)     6148 2023-03-28 21:13:04.000000 PySR3-0.3.5/docs/.DS_Store
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.666169 PySR3-0.3.5/docs/.ipynb_checkpoints/
+-rw-r--r--   0 aksh       (501) staff       (20)    65486 2022-12-31 18:52:41.000000 PySR3-0.3.5/docs/.ipynb_checkpoints/models_overview-checkpoint.ipynb
+-rw-r--r--   0 aksh       (501) staff       (20)   105478 2022-12-31 18:54:38.000000 PySR3-0.3.5/docs/.ipynb_checkpoints/quickstart-checkpoint.ipynb
+-rw-r--r--   0 aksh       (501) staff       (20)      634 2021-08-18 22:29:02.000000 PySR3-0.3.5/docs/Makefile
+-rw-r--r--   0 aksh       (501) staff       (20)     2073 2023-03-29 00:06:19.000000 PySR3-0.3.5/docs/community_guidelines.ipynb
+-rw-r--r--   0 aksh       (501) staff       (20)     2817 2021-09-06 21:01:09.000000 PySR3-0.3.5/docs/conf.py
+-rw-r--r--   0 aksh       (501) staff       (20)      603 2023-01-03 22:16:08.000000 PySR3-0.3.5/docs/index.rst
+-rw-r--r--   0 aksh       (501) staff       (20)      795 2021-08-18 22:29:02.000000 PySR3-0.3.5/docs/make.bat
+-rw-r--r--   0 aksh       (501) staff       (20)    65486 2022-12-31 18:52:41.000000 PySR3-0.3.5/docs/models_overview.ipynb
+-rw-r--r--   0 aksh       (501) staff       (20)   105478 2023-04-18 00:41:28.000000 PySR3-0.3.5/docs/quickstart.ipynb
+-rwxr-xr-x   0 aksh       (501) staff       (20)      247 2021-09-06 21:01:09.000000 PySR3-0.3.5/docs/regenerate_docs.sh
+-rw-r--r--   0 aksh       (501) staff       (20)   149060 2021-09-06 21:01:09.000000 PySR3-0.3.5/docs/sr3_mixed_intuition.png
+-rw-r--r--   0 aksh       (501) staff       (20)       83 2021-09-06 21:01:09.000000 PySR3-0.3.5/requirements.txt
+-rw-r--r--   0 aksh       (501) staff       (20)       38 2023-04-18 00:43:22.682680 PySR3-0.3.5/setup.cfg
+-rw-r--r--   0 aksh       (501) staff       (20)     1314 2022-12-19 20:25:13.000000 PySR3-0.3.5/setup.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.653096 PySR3-0.3.5/src/
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.669228 PySR3-0.3.5/src/PySR3.egg-info/
+-rw-r--r--   0 aksh       (501) staff       (20)      641 2023-04-18 00:43:22.000000 PySR3-0.3.5/src/PySR3.egg-info/PKG-INFO
+-rw-r--r--   0 aksh       (501) staff       (20)     1284 2023-04-18 00:43:22.000000 PySR3-0.3.5/src/PySR3.egg-info/SOURCES.txt
+-rw-r--r--   0 aksh       (501) staff       (20)        1 2023-04-18 00:43:22.000000 PySR3-0.3.5/src/PySR3.egg-info/dependency_links.txt
+-rw-r--r--   0 aksh       (501) staff       (20)        1 2023-03-21 17:33:44.000000 PySR3-0.3.5/src/PySR3.egg-info/not-zip-safe
+-rw-r--r--   0 aksh       (501) staff       (20)      205 2023-04-18 00:43:22.000000 PySR3-0.3.5/src/PySR3.egg-info/requires.txt
+-rw-r--r--   0 aksh       (501) staff       (20)        6 2023-04-18 00:43:22.000000 PySR3-0.3.5/src/PySR3.egg-info/top_level.txt
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.671822 PySR3-0.3.5/src/pysr3/
+-rw-r--r--   0 aksh       (501) staff       (20)     1852 2023-04-06 22:24:53.000000 PySR3-0.3.5/src/pysr3/__about__.py
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.5/src/pysr3/__init__.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.673785 PySR3-0.3.5/src/pysr3/linear/
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.5/src/pysr3/linear/__init__.py
+-rw-r--r--   0 aksh       (501) staff       (20)    29909 2022-12-31 18:37:42.000000 PySR3-0.3.5/src/pysr3/linear/models.py
+-rw-r--r--   0 aksh       (501) staff       (20)    11335 2022-12-20 20:16:57.000000 PySR3-0.3.5/src/pysr3/linear/oracles.py
+-rw-r--r--   0 aksh       (501) staff       (20)     5441 2022-12-20 19:53:33.000000 PySR3-0.3.5/src/pysr3/linear/problems.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.677410 PySR3-0.3.5/src/pysr3/lme/
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.5/src/pysr3/lme/__init__.py
+-rw-r--r--   0 aksh       (501) staff       (20)     6237 2022-12-21 04:47:12.000000 PySR3-0.3.5/src/pysr3/lme/model_selectors.py
+-rw-r--r--   0 aksh       (501) staff       (20)    63162 2023-04-05 21:14:19.000000 PySR3-0.3.5/src/pysr3/lme/models.py
+-rw-r--r--   0 aksh       (501) staff       (20)    59893 2023-04-05 21:17:43.000000 PySR3-0.3.5/src/pysr3/lme/oracles.py
+-rw-r--r--   0 aksh       (501) staff       (20)     7675 2021-09-06 21:01:09.000000 PySR3-0.3.5/src/pysr3/lme/priors.py
+-rw-r--r--   0 aksh       (501) staff       (20)    40739 2022-12-21 04:47:12.000000 PySR3-0.3.5/src/pysr3/lme/problems.py
+-rw-r--r--   0 aksh       (501) staff       (20)     1936 2022-12-19 20:25:13.000000 PySR3-0.3.5/src/pysr3/logger.py
+-rw-r--r--   0 aksh       (501) staff       (20)     4763 2021-09-07 23:08:16.000000 PySR3-0.3.5/src/pysr3/priors.py
+-rw-r--r--   0 aksh       (501) staff       (20)    20759 2022-12-31 18:37:42.000000 PySR3-0.3.5/src/pysr3/regularizers.py
+-rw-r--r--   0 aksh       (501) staff       (20)     6783 2022-12-19 20:25:13.000000 PySR3-0.3.5/src/pysr3/solvers.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.678189 PySR3-0.3.5/tests/
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-08-18 22:29:02.000000 PySR3-0.3.5/tests/__init__.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.678606 PySR3-0.3.5/tests/linear/
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.5/tests/linear/__init__.py
+-rw-r--r--   0 aksh       (501) staff       (20)     8400 2022-12-31 18:46:48.000000 PySR3-0.3.5/tests/linear/test_LinearModels.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.680765 PySR3-0.3.5/tests/lme/
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-09-06 21:01:09.000000 PySR3-0.3.5/tests/lme/__init__.py
+-rw-r--r--   0 aksh       (501) staff       (20)    13132 2022-12-19 20:25:13.000000 PySR3-0.3.5/tests/lme/test_LMEModels.py
+-rw-r--r--   0 aksh       (501) staff       (20)    16047 2022-12-19 20:25:13.000000 PySR3-0.3.5/tests/lme/test_LMEOracle.py
+-rw-r--r--   0 aksh       (501) staff       (20)     7068 2021-09-07 23:09:05.000000 PySR3-0.3.5/tests/lme/test_LMEProblem.py
+-rw-r--r--   0 aksh       (501) staff       (20)     2472 2022-12-19 20:25:13.000000 PySR3-0.3.5/tests/lme/test_select_covariates.py
+drwxr-xr-x   0 aksh       (501) staff       (20)        0 2023-04-18 00:43:22.681777 PySR3-0.3.5/tests/test_core/
+-rw-r--r--   0 aksh       (501) staff       (20)        0 2021-08-18 22:29:02.000000 PySR3-0.3.5/tests/test_core/__init__.py
+-rw-r--r--   0 aksh       (501) staff       (20)      458 2021-09-06 21:01:09.000000 PySR3-0.3.5/tests/test_core/test_Priors.py
+-rw-r--r--   0 aksh       (501) staff       (20)      212 2021-09-06 21:01:09.000000 PySR3-0.3.5/tests/test_core/test_Regularizers.py
```

### Comparing `PySR3-0.3.4/LICENSE` & `PySR3-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/PKG-INFO` & `PySR3-0.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySR3
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Library for Sparse Relaxed Regularized Regression.
 Home-page: https://github.com/aksholokhov/pysr3
 Author: Aleksei Sholokhov
 Author-email: aksh@uw.edu
 License: GNU GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `PySR3-0.3.4/README.md` & `PySR3-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/.DS_Store` & `PySR3-0.3.5/docs/.DS_Store`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/.ipynb_checkpoints/models_overview-checkpoint.ipynb` & `PySR3-0.3.5/docs/.ipynb_checkpoints/models_overview-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/.ipynb_checkpoints/quickstart-checkpoint.ipynb` & `PySR3-0.3.5/docs/.ipynb_checkpoints/quickstart-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/Makefile` & `PySR3-0.3.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/community_guidelines.ipynb` & `PySR3-0.3.5/docs/community_guidelines.ipynb`

 * *Files 15% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9881944444444444%*

 * *Differences: {"'cells'": "{0: {'metadata': {delete: ['pycharm']}, 'source': {insert: [(3, 'if you fixed a bug "*

 * *            'or developed an extension. If you experience any issues please open a new issue on '*

 * *            "the Issues page, and we will do our best to help.\\n')], delete: [3]}}}"}*

```diff
@@ -1,22 +1,19 @@
 {
     "cells": [
         {
             "cell_type": "markdown",
             "metadata": {
-                "collapsed": true,
-                "pycharm": {
-                    "name": "#%% md\n"
-                }
+                "collapsed": true
             },
             "source": [
                 "# Community Guidelines\n",
                 "\n",
                 "We encourage the broader community to contribute to `pysr3`! Please submit a pull request on GitHub\n",
-                "if you fixed a bug or developed an extension.\n",
+                "if you fixed a bug or developed an extension. If you experience any issues please open a new issue on the Issues page, and we will do our best to help.\n",
                 "\n",
                 "As a  community, we follow the list of rules below:\n",
                 "\n",
                 "1. We adhere to [sklearn's interfaces and standards](https://scikit-learn.org/stable/developers/develop.html)\n",
                 "   * Please use `sklearn.utils.estimator_checks.check_estimator` to ensure that your contributions don't break this compatibility.\n",
                 "2. For comments and docstrings, we use [numpy dostring standards](https://numpydoc.readthedocs.io/en/latest/format.html#docstring-standard)\n",
                 "3. For version numbers, we use [Semantic Versioning](https://semver.org/).\n",
```

### Comparing `PySR3-0.3.4/docs/conf.py` & `PySR3-0.3.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/index.rst` & `PySR3-0.3.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/make.bat` & `PySR3-0.3.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/models_overview.ipynb` & `PySR3-0.3.5/docs/models_overview.ipynb`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/quickstart.ipynb` & `PySR3-0.3.5/docs/quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/docs/sr3_mixed_intuition.png` & `PySR3-0.3.5/docs/sr3_mixed_intuition.png`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/setup.py` & `PySR3-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/PySR3.egg-info/PKG-INFO` & `PySR3-0.3.5/src/PySR3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySR3
-Version: 0.3.4
+Version: 0.3.5
 Summary: Python Library for Sparse Relaxed Regularized Regression.
 Home-page: https://github.com/aksholokhov/pysr3
 Author: Aleksei Sholokhov
 Author-email: aksh@uw.edu
 License: GNU GPLv3
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `PySR3-0.3.4/src/PySR3.egg-info/SOURCES.txt` & `PySR3-0.3.5/src/PySR3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/__about__.py` & `PySR3-0.3.5/src/pysr3/__about__.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,14 @@
 __uri__ = "https://github.com/aksholokhov/pysr3"
 __classifiers__ = [
                       "Programming Language :: Python :: 3",
                       'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
                       "Operating System :: OS Independent",
                   ],
 
-__version__ = "0.3.4"
+__version__ = "0.3.5"
 
 __author__ = "Aleksei Sholokhov"
 __email__ = "aksh@uw.edu"
 
 __license__ = "GNU GPLv3"
 __copyright__ = f"Copyright 2020-2021 {__author__}"
```

### Comparing `PySR3-0.3.4/src/pysr3/linear/models.py` & `PySR3-0.3.5/src/pysr3/linear/models.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/linear/oracles.py` & `PySR3-0.3.5/src/pysr3/linear/oracles.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/linear/problems.py` & `PySR3-0.3.5/src/pysr3/linear/problems.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/lme/model_selectors.py` & `PySR3-0.3.5/src/pysr3/lme/model_selectors.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/lme/models.py` & `PySR3-0.3.5/src/pysr3/lme/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -578,14 +578,15 @@
                  tol_solver: float = 1e-5,
                  initializer: str = "None",
                  max_iter_oracle: int = 10000,
                  max_iter_solver: int = 10000,
                  stepping: str = "fixed",
                  ell: float = 40,
                  elastic_eps: float = 1e-4,
+                 central_path_neighbourhood_target=0.5,
                  logger_keys: Set = ('converged',),
                  warm_start_oracle=True,
                  practical=False,
                  update_prox_every=1,
                  fixed_step_len=None,
                  take_only_positive_part=True,
                  take_expected_value=False,
@@ -606,14 +607,18 @@
             one step of EM algorithm
         max_iter_solver: int
             maximal number of iterations for PGD solver
         stepping: str
             step-size policy for PGD. Can be either "line-search" or "fixed"
         ell: float
             level of SR3-relaxation
+        elastic_eps: float
+            regularizer coefficient for ||beta|| and ||gamma||. Safeguards against infinite solutions.
+        central_path_neighbourhood_target: float
+            how close to the central path MSR3-fast algorithm needs to finish Newton iterations and make a projection
         logger_keys: List[str]
             list of keys for the parameters that the logger should track
         warm_start_oracle: bool
             if fitting should be started from the current model's coefficients.
             Used for fine-tuning and iterative fitting.
         practical: bool
             whether to use SR3-Practical method, which works faster at the expense of accuracy
@@ -641,14 +646,15 @@
         self.prior = prior
         self.ell = ell
         self.elastic_eps = elastic_eps
         self.practical = practical
         self.take_only_positive_part = take_only_positive_part
         self.take_expected_value = take_expected_value
         self.update_prox_every = update_prox_every
+        self.central_path_neighbourhood_target = central_path_neighbourhood_target
 
     def instantiate(self):
         """
         Instantiates the model: creates all internal entities such as oracle, regularizer, and solver
 
         Returns
         -------
@@ -665,15 +671,17 @@
                                fixed_step_len=fixed_step_len)
         oracle = LinearLMEOracleSR3(None, lb=self.ell, lg=self.ell,
                                     tol_inner=self.tol_oracle,
                                     n_iter_inner=self.max_iter_oracle,
                                     warm_start=self.warm_start_oracle,
                                     take_only_positive_part=self.take_only_positive_part,
                                     take_expected_value=self.take_expected_value,
-                                    prior=self.prior)
+                                    prior=self.prior,
+                                    central_path_neighbourhood_target=self.central_path_neighbourhood_target
+                                    )
         dummy_regularizer = DummyRegularizer()
         elastic_regularizer = ElasticRegularizer(other_regularizer=dummy_regularizer, eps=self.elastic_eps)
         regularizer = PositiveQuadrantRegularizer(other_regularizer=elastic_regularizer)
         return oracle, regularizer, solver
 
     def get_information_criterion(self, x, y, columns_labels=None, ic="muller_ic"):
         """
@@ -822,14 +830,15 @@
                  tol_solver: float = 1e-5,
                  initializer: str = "None",
                  max_iter_oracle: int = 1000,
                  max_iter_solver: int = 1000,
                  stepping: str = "fixed",
                  ell: float = 40,
                  elastic_eps: float = 1e-4,
+                 central_path_neighbourhood_target=0.5,
                  nnz_tbeta: int = 1,
                  nnz_tgamma: int = 1,
                  logger_keys: Set = ('converged',),
                  warm_start_oracle=True,
                  practical=False,
                  take_only_positive_part=True,
                  take_expected_value=False,
@@ -893,14 +902,15 @@
                          take_only_positive_part=take_only_positive_part,
                          take_expected_value=take_expected_value,
                          update_prox_every=update_prox_every,
                          logger_keys=logger_keys,
                          fixed_step_len=fixed_step_len,
                          ell=ell,
                          elastic_eps=elastic_eps,
+                         central_path_neighbourhood_target=central_path_neighbourhood_target,
                          prior=prior)
         self.nnz_tbeta = nnz_tbeta
         self.nnz_tgamma = nnz_tgamma
 
     def instantiate(self):
         """
         Instantiates the model: creates all internal entities such as oracle, regularizer, and solver
@@ -1008,14 +1018,15 @@
                  lam: float = 1,
                  logger_keys: Set = ('converged',),
                  warm_start_oracle=True,
                  practical=False,
                  take_only_positive_part=True,
                  take_expected_value=False,
                  update_prox_every=1,
+                 central_path_neighbourhood_target=0.5,
                  fixed_step_len=None,
                  prior=None,
                  **kwargs):
         """
         Initializes the model
 
         Parameters
@@ -1063,14 +1074,15 @@
                          initializer=initializer,
                          max_iter_oracle=max_iter_oracle,
                          max_iter_solver=max_iter_solver,
                          stepping=stepping,
                          warm_start_oracle=warm_start_oracle,
                          practical=practical,
                          take_only_positive_part=take_only_positive_part,
+                         central_path_neighbourhood_target=central_path_neighbourhood_target,
                          take_expected_value=take_expected_value,
                          update_prox_every=update_prox_every,
                          logger_keys=logger_keys,
                          fixed_step_len=fixed_step_len,
                          ell=ell,
                          elastic_eps=elastic_eps,
                          prior=prior)
@@ -1180,14 +1192,15 @@
                  max_iter_oracle: int = 10000,
                  max_iter_solver: int = 10000,
                  stepping: str = "fixed",
                  ell: float = 40.0,
                  rho: float = 0.3,
                  lam: float = 1.0,
                  elastic_eps: float = 1e-4,
+                 central_path_neighbourhood_target: float = 0.5,
                  logger_keys: Set = ('converged',),
                  warm_start_oracle=True,
                  practical=False,
                  take_only_positive_part=True,
                  take_expected_value=False,
                  update_prox_every=1,
                  fixed_step_len=None,
@@ -1249,14 +1262,15 @@
                          take_only_positive_part=take_only_positive_part,
                          take_expected_value=take_expected_value,
                          update_prox_every=update_prox_every,
                          logger_keys=logger_keys,
                          fixed_step_len=fixed_step_len,
                          ell=ell,
                          elastic_eps=elastic_eps,
+                         central_path_neighbourhood_target=central_path_neighbourhood_target,
                          prior=prior)
         self.lam = lam
         self.rho = rho
 
     def instantiate(self):
         """
         Instantiates the model: creates all internal entities such as oracle, regularizer, and solver
@@ -1366,14 +1380,15 @@
                  max_iter_solver: int = 10000,
                  stepping: str = "fixed",
                  ell: float = 40.0,
                  rho: float = 3.7,  # as per recommendation from (Fan, Li, 2001), p. 1351
                  sigma: float = 0.5,  # same
                  lam: float = 1.0,
                  elastic_eps: float = 1e-4,
+                 central_path_neighbourhood_target: float = 0.5,
                  logger_keys: Set = ('converged',),
                  warm_start_oracle=True,
                  practical=False,
                  take_only_positive_part=True,
                  take_expected_value=False,
                  update_prox_every=1,
                  fixed_step_len=None,
@@ -1437,14 +1452,15 @@
                          take_only_positive_part=take_only_positive_part,
                          take_expected_value=take_expected_value,
                          update_prox_every=update_prox_every,
                          logger_keys=logger_keys,
                          fixed_step_len=fixed_step_len,
                          ell=ell,
                          elastic_eps=elastic_eps,
+                         central_path_neighbourhood_target=central_path_neighbourhood_target,
                          prior=prior)
         self.lam = lam
         self.rho = rho
         self.sigma = sigma
 
     def instantiate(self):
         """
```

### Comparing `PySR3-0.3.4/src/pysr3/lme/oracles.py` & `PySR3-0.3.5/src/pysr3/lme/oracles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1001,15 +1001,15 @@
     """
        Implements Sparse Relaxed Regularized Regression (SR3) for Linear Mixed-Effects Model.
        The problem should be provided as LMEProblem.
 
        """
 
     def __init__(self, problem: Optional[LMEProblem], lb=0.1, lg=0.1, warm_start=True, take_only_positive_part=True,
-                 take_expected_value=False, **kwargs):
+                 take_expected_value=False, central_path_neighbourhood_target=0.5, **kwargs):
         """
         Creates an oracle on top of the given problem. The problem should be in the form of LinearLMEProblem.
 
         Parameters
         ----------
         problem: LMEProblem
             The set of data and answers. See the docs for LinearLMEProblem for more details.
@@ -1022,14 +1022,15 @@
         super().__init__(problem, **kwargs)
         self.lb = lb
         self.lg = lg
         self.warm_start = warm_start
         self.warm_start_ip = {}
         self.take_only_positive_part = take_only_positive_part
         self.take_expected_value = take_expected_value
+        self.central_path_neighbourhood_target = central_path_neighbourhood_target
 
     def loss(self, beta: np.ndarray, gamma: np.ndarray, tbeta: np.ndarray = None, tgamma: np.ndarray = None, **kwargs):
         """
         Returns the loss function value ℒ(β, 𝛄) + lb/2*||β - tβ||^2 + lg/2*||𝛄 - t𝛄||^2
 
         Parameters
         ----------
@@ -1307,15 +1308,15 @@
                                                                  update_prox_every=update_prox_every,
                                                                  **kwargs)
         return self.beta_gamma_to_x(tbeta, tgamma)
 
     def find_optimal_parameters_ip(self, beta: np.ndarray, gamma: np.ndarray, tbeta=None, tgamma=None,
                                    regularizer=None, increase_lambdas=False,
                                    line_search=False, prox_step_len=1.0, update_prox_every=1, logger=None,
-                                   central_path_neighbourhood_target=0.5, mu_decay=0.5,
+                                   mu_decay=0.5,
                                    **kwargs):
         losses_kkt = []
         if len(tgamma) == 0:
             beta = self.optimal_beta(gamma=tgamma, tbeta=tbeta)
             gamma = tgamma
             return beta, gamma, tbeta, tgamma, losses_kkt
 
@@ -1404,15 +1405,15 @@
             # x[x <= 1e-18] = 0  # killing effective zeros
             v = x[:q]
             beta = x[q:-q]
             gamma = x[-q:]
 
             iteration += 1
 
-            if np.linalg.norm(gamma * v - gamma.dot(v) / q) > central_path_neighbourhood_target * gamma.dot(v) / q:
+            if np.linalg.norm(gamma * v - gamma.dot(v) / q) > self.central_path_neighbourhood_target * gamma.dot(v) / q:
                 # do correction steps without tightening the barrier relaxation
                 continue
             else:
                 # adjust barrier relaxation
                 mu = mu_decay * v.dot(gamma) / q
                 # figure out which mu the problem actually got solved for
                 mu_effective = v.dot(gamma) / q
```

### Comparing `PySR3-0.3.4/src/pysr3/lme/priors.py` & `PySR3-0.3.5/src/pysr3/lme/priors.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/lme/problems.py` & `PySR3-0.3.5/src/pysr3/lme/problems.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/logger.py` & `PySR3-0.3.5/src/pysr3/logger.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/priors.py` & `PySR3-0.3.5/src/pysr3/priors.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/regularizers.py` & `PySR3-0.3.5/src/pysr3/regularizers.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/src/pysr3/solvers.py` & `PySR3-0.3.5/src/pysr3/solvers.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/tests/linear/test_LinearModels.py` & `PySR3-0.3.5/tests/linear/test_LinearModels.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/tests/lme/test_LMEModels.py` & `PySR3-0.3.5/tests/lme/test_LMEModels.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/tests/lme/test_LMEOracle.py` & `PySR3-0.3.5/tests/lme/test_LMEOracle.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/tests/lme/test_LMEProblem.py` & `PySR3-0.3.5/tests/lme/test_LMEProblem.py`

 * *Files identical despite different names*

### Comparing `PySR3-0.3.4/tests/lme/test_select_covariates.py` & `PySR3-0.3.5/tests/lme/test_select_covariates.py`

 * *Files identical despite different names*

