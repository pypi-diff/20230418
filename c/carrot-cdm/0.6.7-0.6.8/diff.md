# Comparing `tmp/carrot-cdm-0.6.7.tar.gz` & `tmp/carrot-cdm-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carrot-cdm-0.6.7.tar", last modified: Mon Feb 27 15:23:47 2023, max compression
+gzip compressed data, was "carrot-cdm-0.6.8.tar", last modified: Tue Apr 18 07:23:55 2023, max compression
```

## Comparing `carrot-cdm-0.6.7.tar` & `carrot-cdm-0.6.8.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.103530 carrot-cdm-0.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-27 15:23:47.103530 carrot-cdm-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/analyses/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/analyses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/analyses/example_serology.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/cdm/
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/cdm/classes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/cdm/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/cdm/objects/versions/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/death.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/measurement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/observation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/specimen.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cdm/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.095530 carrot-cdm-0.6.7/carrot/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.099530 carrot-cdm-0.6.7/carrot/cli/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/airflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/display.py
--rw-r--r--   0 runner    (1001) docker     (123)    41561 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/etl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/get.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/pseudonymise.py
--rw-r--r--   0 runner    (1001) docker     (123)    38742 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/cli/subcommands/search.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.099530 carrot-cdm-0.6.7/carrot/io/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/io/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.099530 carrot-cdm-0.6.7/carrot/io/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/io/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/io/plugins/bclink.py
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/io/plugins/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/io/plugins/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.099530 carrot-cdm-0.6.7/carrot/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/bash_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/bclink_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.099530 carrot-cdm-0.6.7/carrot/tools/extract/
--rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/extract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/extract/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4747 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/mappingrules.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9921 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/omopcdm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/carrot/tools/rules_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 15:23:47.103530 carrot-cdm-0.6.7/carrot_cdm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-02-27 15:23:47.000000 carrot-cdm-0.6.7/carrot_cdm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-02-27 15:23:47.000000 carrot-cdm-0.6.7/carrot_cdm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 15:23:47.000000 carrot-cdm-0.6.7/carrot_cdm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-02-27 15:23:47.000000 carrot-cdm-0.6.7/carrot_cdm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-02-27 15:23:47.000000 carrot-cdm-0.6.7/carrot_cdm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-27 15:23:47.000000 carrot-cdm-0.6.7/carrot_cdm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 15:23:47.103530 carrot-cdm-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-02-27 15:23:45.000000 carrot-cdm-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/analyses/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/analyses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/analyses/example_serology.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33784 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     1257 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/objects/versions/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1420 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/death.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/measurement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/observation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/specimen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cdm/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.106208 carrot-cdm-0.6.8/carrot/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/cli/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/airflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41561 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/pseudonymise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44828 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2071 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/cli/subcommands/search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6117 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/io/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/bclink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/io/plugins/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3104 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/bash_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19345 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/bclink_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot/tools/extract/
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/extract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/extract/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/mappingrules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4875 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/omopcdm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/carrot/tools/rules_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/carrot_cdm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 07:23:55.000000 carrot-cdm-0.6.8/carrot_cdm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 07:23:55.110209 carrot-cdm-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-04-18 07:23:54.000000 carrot-cdm-0.6.8/setup.py
```

### Comparing `carrot-cdm-0.6.7/LICENSE` & `carrot-cdm-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/PKG-INFO` & `carrot-cdm-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.6.7
+Version: 0.6.8
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: calmacx@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.6.7/carrot/analyses/example_serology.py` & `carrot-cdm-0.6.8/carrot/analyses/example_serology.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/__init__.py` & `carrot-cdm-0.6.8/carrot/cdm/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/decorators.py` & `carrot-cdm-0.6.8/carrot/cdm/decorators.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/model.py` & `carrot-cdm-0.6.8/carrot/cdm/model.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/__init__.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/common.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/condition_occurrence.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import pandas as pd
 from ...common import DestinationTable, DestinationField
 
 class ConditionOccurrence(DestinationTable):
     """
     CDM Condition Occurrence object class
     """
-    
+
     name = 'condition_occurrence'
     def __init__(self,name=None):
         self.condition_occurrence_id       = DestinationField(dtype="Integer"   , required=True , pk=True)
         self.person_id                     = DestinationField(dtype="Integer"   , required=True )
         self.condition_concept_id          = DestinationField(dtype="Integer"   , required=True )
         self.condition_start_date          = DestinationField(dtype="Date"      , required=False )
         self.condition_start_datetime      = DestinationField(dtype="Timestamp" , required=True )
@@ -19,33 +19,32 @@
         self.stop_reason                   = DestinationField(dtype="Text20"    , required=False )
         self.provider_id                   = DestinationField(dtype="Integer"   , required=False )
         self.visit_occurrence_id           = DestinationField(dtype="Integer"   , required=False )
         self.condition_source_value        = DestinationField(dtype="Text50"    , required=False )
         self.condition_source_concept_id   = DestinationField(dtype="Integer"   , required=False )
         self.condition_status_source_value = DestinationField(dtype="Text50"    , required=False )
         self.condition_status_concept_id   = DestinationField(dtype="Integer"   , required=False )
-        
+
         if name is None:
             name = hex(id(self))
         super().__init__(name,self.name)
 
-        
+
     def get_df(self,**kwargs):
         """
         Overload/append the creation of the dataframe, specifically for the condition_occurrence objects
         * condition_concept_id is required to be not null
           this can happen when spawning multiple rows from a person
           we just want to keep the ones that have actually been filled
-        
+
         Returns:
            pandas.Dataframe: output dataframe
         """
 
         df = super().get_df(**kwargs)
         if self.automatically_fill_missing_columns == True:
             if df['condition_start_date'].isnull().all():
                 df['condition_start_date'] = self.tools.get_date(df['condition_start_datetime'])
 
             if df['condition_end_date'].isnull().all():
                 df['condition_end_date'] = self.tools.get_date(df['condition_end_datetime'])
         return df
-
```

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/death.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/death.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/drug_exposure.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/measurement.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/measurement.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/observation.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/observation.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/person.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/person.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/procedure_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/specimen.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/specimen.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py` & `carrot-cdm-0.6.8/carrot/cdm/objects/versions/v5_3_1/visit_occurrence.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cdm/operations.py` & `carrot-cdm-0.6.8/carrot/cdm/operations.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/cli.py` & `carrot-cdm-0.6.8/carrot/cli/cli.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/airflow.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/airflow.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/display.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/display.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/etl.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/etl.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/generate.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/generate.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/get.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/get.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/info.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/info.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/pseudonymise.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/pseudonymise.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/run.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/run.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 import pandas as pd
 import inspect
 import os, time
+import datetime
 import fnmatch
 import sys
 import click
 import json
 import yaml
 import glob
 import copy
 import subprocess
+import cProfile, pstats
 import carrot
 import carrot.tools as tools
 
 @click.group(help="Commands for mapping data to the OMOP CommonDataModel (CDM).")
 def run():
     pass
 
@@ -599,148 +601,195 @@
 @click.option("--write-mode",
               default='w',
               type=click.Choice(['w','a']),
               help="force write-mode on output files")
 @click.option("--person-file",
               required=True,
               help="File containing person_ids in the first column")
+@click.option("--omop-config",
+              required=True,
+              help="File containing json configfor omop outputs")
 @click.option("--saved-person-id-filename",
               default='person_ids.tsv',
               required=False,
               help="Person id file used to save state between runs")
+@click.option("--use-input-person-ids",
+              required=True,
+              default='No',
+              help="Use person ids as input without generating new integers")
 @click.argument("input-dir",
                 required=False,
                 nargs=-1)
-def mapstream(rules, output_folder, write_mode, person_file, saved_person_id_filename, input_dir):
+def mapstream(rules, output_folder, write_mode, person_file, omop_config, saved_person_id_filename, use_input_person_ids, input_dir):
     """
     Map to output using input streams
     """
+    #profiler = cProfile.Profile()
+    #profiler.enable()
     if os.path.isdir(input_dir[0]) == False:
         print("Not a directory {0}".format(input_dir[0]))
         sys.exit(1)
 
     starttime = time.time()
-    omopcdm = tools.omopcdm.OmopCDM()
-    mappingrules = tools.mappingrules.MappingRules(rules)
+    metrics = tools.metrics.Metrics()
+    omopcdm = tools.omopcdm.OmopCDM(omop_config)
+    mappingrules = tools.mappingrules.MappingRules(rules, omop_config)
     nowtime = time.time()
+
     print("--------------------------------------------------------------------------------")
     print("Loaded mapping rules from: {0} after {1:.5f} secs".format(rules, (nowtime - starttime)))
     output_files = mappingrules.get_all_outfile_names()
     record_numbers = {}
     for output_file in output_files:
         record_numbers[output_file] = 0
 
     fhd = {}
     tgtcolmaps = {}
 
     try:
+        # TODO: add in person_ids.tsv existence testing and reload
         fhp = open(person_file, mode="r")
-        person_lookup = load_person_ids(fhp, mappingrules)
+        person_lookup, rejected_person_count = load_person_ids(fhp, mappingrules, use_input_person_ids)
         fhp.close()
+        fhpout = open(output_folder + "/person_ids.tsv", mode="w")
+        fhpout.write("SOURCE_SUBJECT\tTARGET_SUBJECT\n")
+        for person_id, person_assigned_id in person_lookup.items():
+            fhpout.write("{0}\t{1}\n".format(str(person_id), str(person_assigned_id)))
+        fhpout.close()
         for tgtfile in output_files:
             fhd[tgtfile] = open(output_folder + "/" + tgtfile + ".tsv", mode=write_mode)
             if write_mode == 'w':
                 outhdr = omopcdm.get_omop_column_list(tgtfile)
                 fhd[tgtfile].write("\t".join(outhdr) + "\n")
             tgtcolmaps[tgtfile] = omopcdm.get_omop_column_map(tgtfile)
 
     except IOError as e:
         print("I/O error({0}): {1}".format(e.errno, e.strerror))
         exit()
 
+    print("person_id stats: total loaded {0}, reject count {1}".format(len(person_lookup), rejected_person_count))
+
     input_files = fnmatch.filter(os.listdir(input_dir[0]), '*.csv')
     rejidcounts = {}
     rejdatecounts = {}
     src_tgt_counts = {}
 
     for srcfilename in input_files:
         rejidcounts[srcfilename] = 0
         rejdatecounts[srcfilename] = 0
 
 
     for srcfilename in input_files:
-        rcount = 0
         outcounts = {}
         rejcounts = {}
+        rcount = 0
+
         try:
             fh = open(input_dir[0] + "/" + srcfilename, mode='r')
         except IOError as e:
             print("I/O error({0}): {1}".format(e.errno, e.strerror))
             exit()
 
         tgtfiles, src_to_tgt = mappingrules.parse_rules_src_to_tgt(srcfilename)
+        infile_datetime_source, infile_person_id_source = mappingrules.get_infile_date_person_id(srcfilename)
         for tgtfile in tgtfiles:
             outcounts[tgtfile] = 0
             rejcounts[tgtfile] = 0
         datacolsall = []
         hdrdata = fh.readline().strip().split(",")
         dflist = mappingrules.get_infile_data_fields(srcfilename)
         for colname in hdrdata:
             datacolsall.append(colname)
         inputcolmap = omopcdm.get_column_map(hdrdata)
+        pers_id_col = inputcolmap[infile_person_id_source]
+        datetime_col = inputcolmap[infile_datetime_source]
         print("--------------------------------------------------------------------------------")
         print("Processing input: {0}".format(srcfilename))
 #        print("Processing input: {0}, All input cols = {1}, Data cols = {2}".format(srcfilename, str(datacolsall), str(dflist)))
 
         for inputline in fh:
             indata = inputline.strip().split(",")
+            key = srcfilename + "~all~all"
+            metrics.increment_key_count(key, "input_count")
             rcount += 1
+            strdate = indata[datetime_col].split(" ")[0]
+            fulldate = parse_date(strdate)
+            if fulldate != None:
+                #fulldate = "{0}-{1:02}-{2:02}".format(dt.year, dt.month, dt.day)
+                indata[datetime_col] = fulldate
+            else:
+                metrics.increment_key_count(key, "invalid_date_fields")
+                continue
+
             for tgtfile in tgtfiles:
                 tgtcolmap = tgtcolmaps[tgtfile]
                 count_key = srcfilename + "~" + tgtfile
-                date_col_data = omopcdm.get_omop_date_column_data(tgtfile)
+                date_col_data = omopcdm.get_omop_date_fields(tgtfile)
+                date_component_data = omopcdm.get_omop_date_field_components(tgtfile)
                 auto_num_col = omopcdm.get_omop_auto_number_field(tgtfile)
                 pers_id_col = omopcdm.get_omop_person_id_field(tgtfile)
 
                 datacols = datacolsall
                 if tgtfile in dflist:
                     datacols = dflist[tgtfile]
 
                 for datacol in datacols:
-                    built_records, outrecords = get_target_records(tgtfile, tgtcolmap, src_to_tgt, datacol, indata, inputcolmap, srcfilename, date_col_data)
+                    built_records, outrecords, metrics = get_target_records(tgtfile, tgtcolmap, src_to_tgt, datacol, indata, inputcolmap, srcfilename, date_col_data, date_component_data, metrics)
                     if built_records == True:
                         for outrecord in outrecords:
-                            outcounts[tgtfile] += 1
-                            record_numbers[tgtfile] += 1
                             if auto_num_col != None:
                                 outrecord[tgtcolmap[auto_num_col]] = str(record_numbers[tgtfile])
                             if (outrecord[tgtcolmap[pers_id_col]]) in person_lookup:
                                 outrecord[tgtcolmap[pers_id_col]] = person_lookup[outrecord[tgtcolmap[pers_id_col]]]
+                                outcounts[tgtfile] += 1
+                                key = srcfilename + "~all~all"
+                                metrics.increment_key_count(key, "output_count")
+                                key = "all~" + tgtfile + "~all"
+                                metrics.increment_key_count(key, "output_count")
+                                key = srcfilename + "~" + tgtfile + "~all"
+                                metrics.increment_key_count(key, "output_count")
+                                key = srcfilename + "~" + tgtfile + "~" + datacol
+                                metrics.increment_key_count(key, "output_count")
                                 fhd[tgtfile].write("\t".join(outrecord) + "\n")
                             else:
+                                key = srcfilename + "~" + tgtfile + "~all"
+                                metrics.increment_key_count(key, "invalid_person_ids")
                                 rejidcounts[srcfilename] += 1
-                    else:
-                        rejcounts[tgtfile] += 1
 
         fh.close()
+
         nowtime= time.time()
-        print("INPUT file data : {0}: in count {1}, time since start {2:.5} secs".format(srcfilename, str(rcount), (nowtime - starttime)))
+        print("INPUT file data : {0}: input count {1}, time since start {2:.5} secs".format(srcfilename, str(rcount), (nowtime - starttime)))
         for outtablename, count in outcounts.items():
-            print("TARGET: {0}: o/p by field count {1}, reject o/p by field count {2}".format(outtablename, str(count), str(rejcounts[outtablename])))
+            print("TARGET: {0}: output count {1}".format(outtablename, str(count)))
 
     print("--------------------------------------------------------------------------------")
-    print("Rejected input records due to unmatched person_id counts:")
-    for srcfilename, count in rejidcounts.items():
-        print("{0},{1}".format(srcfilename, str(count)))
-    print("--------------------------------------------------------------------------------")
-    print("Rejected input records due to invalid date counts:")
-    for srcfilename, count in rejdatecounts.items():
-        print("{0}, count {1}".format(srcfilename, str(count)))
+    data_summary = metrics.get_mapstream_summary()
+    try:
+        dsfh = open(output_folder + "/summary_mapstream.tsv", mode="w")
+        dsfh.write(data_summary)
+        dsfh.close()
+    except IOError as e:
+        print("I/O error({0}): {1}".format(e.errno, e.strerror))
+        print("Unable to write summary.tsv")
 
-    print("--------------------------------------------------------------------------------")
     nowtime = time.time()
     print("Elapsed time = {0:.5f} secs".format(nowtime - starttime))
+    #profiler.disable()
+    #stats = pstats.Stats(profiler).sort_stats('ncalls')
+    #stats.print_stats()
 
-def get_target_records(tgtfilename, tgtcolmap, rulesmap, srcfield, srcdata, srccolmap, srcfilename, date_col_data):
+def get_target_records(tgtfilename, tgtcolmap, rulesmap, srcfield, srcdata, srccolmap, srcfilename, date_col_data, date_component_data, metrics):
     build_records = False
     tgtrecords = []
 
+    srckey = srcfilename + "~" + srcfield + "~" + tgtfilename
+    summarykey = srcfilename + "~" + tgtfilename + "~" + srcfield
     if valid_value(str(srcdata[srccolmap[srcfield]])):
         srcfullkey = srcfilename + "~" + srcfield + "~" + str(srcdata[srccolmap[srcfield]]) + "~" + tgtfilename
-        srckey = srcfilename + "~" + srcfield + "~" + tgtfilename
         dictkeys = []
         if srcfullkey in rulesmap:
             build_records = True
             dictkeys.append(srcfullkey)
         if srckey in rulesmap:
             build_records = True
             dictkeys.append(srckey)
@@ -752,72 +801,178 @@
                     for infield, outfield_list in out_data_elem.items():
                         for output_col_data in outfield_list:
                             if "~" in output_col_data:
                                 outcol, term = output_col_data.split("~")
                                 tgtarray[tgtcolmap[outcol]] = term
                             else:
                                 tgtarray[tgtcolmap[output_col_data]] = srcdata[srccolmap[infield]]
-                            if output_col_data in date_col_data:
-                                if valid_date_value(srcdata[srccolmap[infield]].split(" ")[0]):
-                                    tgtarray[tgtcolmap[date_col_data[output_col_data]]] = srcdata[srccolmap[infield]].split(" ")[0]
+                            if output_col_data in date_component_data:
+                                strdate = srcdata[srccolmap[infield]].split(" ")[0]
+                                dt = get_datetime_value(strdate)
+                                if dt != None:
+                                    year_field = date_component_data[output_col_data]["year"]
+                                    month_field = date_component_data[output_col_data]["month"]
+                                    day_field = date_component_data[output_col_data]["day"]
+                                    #print("DATE Fieldnames {0} {1} {2}".format(year_field, month_field, day_field))
+                                    tgtarray[tgtcolmap[year_field]] = str(dt.year)
+                                    tgtarray[tgtcolmap[month_field]] = str(dt.month)
+                                    tgtarray[tgtcolmap[day_field]] = str(dt.day)
+                                    fulldate = "{0}-{1:02}-{2:02}".format(dt.year, dt.month, dt.day)
+                                    tgtarray[tgtcolmap[output_col_data]] = fulldate
                                 else:
+                                    metrics.increment_key_count(summarykey, "invalid_date_fields")
                                     valid_data_elem = False
+                            elif output_col_data in date_col_data:
+                                fulldate = srcdata[srccolmap[infield]]
+                                tgtarray[tgtcolmap[output_col_data]] = fulldate
+                                tgtarray[tgtcolmap[date_col_data[output_col_data]]] = fulldate
                     if valid_data_elem == True:
                         tgtrecords.append(tgtarray)
-    return build_records, tgtrecords
+    else:
+        metrics.increment_key_count(summarykey, "invalid_source_fields")
+
+
+    return build_records, tgtrecords, metrics
 
 def valid_value(item):
     """
     Check if an item is non blank (null)
     """
     if item.strip() == "":
         return(False)
     return(True)
 
 def valid_date_value(item):
     """
-    Check if a date item is non null and parses (crudely)
+    Check if a date item is non null and parses as ISO (YYYY-MM-DD), reverse-ISO
+    or dd/mm/yyyy or mm/dd/yyyy
     """
     if item.strip() == "":
         return(False)
-    dparts = item.split("-")
-    if len(dparts) < 3:
+    if not valid_iso_date(item) and not valid_reverse_iso_date(item) and not valid_uk_date(item):
+        #print("Bad date : {0}".format(item))
         return(False)
-    if dparts[0] == "" or dparts[1] == "" or dparts[2] == "":
+    return(True)
+
+def get_datetime_value(item):
+    """
+    Check if a date item is non null and parses as ISO (YYYY-MM-DD), reverse-ISO
+    or dd/mm/yyyy or mm/dd/yyyy
+    """
+    dt = None
+    # Does the date parse as an ISO date?
+    try:
+        dt = datetime.datetime.strptime(item, "%Y-%m-%d")
+    except ValueError:
+        pass
+    if dt != None:
+      return(dt)
+
+    # Does the date parse as a reverse ISO date?
+    try:
+        dt = datetime.datetime.strptime(item, "%d-%m-%Y")
+    except ValueError:
+        pass
+
+    if dt != None:
+      return(dt)
+
+    # Does the date parse as a UK old-style date?
+    try:
+        dt = datetime.datetime.strptime(item, "%d/%m/%Y")
+    except ValueError:
+        pass
+
+    if dt != None:
+      return(dt)
+
+    return None
+
+def parse_date(item):
+    """
+    Crude hand-coded check on date format
+    """
+    datedata = item.split("-")
+    if len(datedata) != 3:
+        datedata = item.split("/")
+    if len(datedata) != 3:
+        return None
+    if len(datedata[2]) == 4:
+        return("{0}-{1}-{2}".format(datedata[2], datedata[1], datedata[0]))
+    return("{0}-{1}-{2}".format(datedata[0], datedata[1], datedata[2]))
+
+
+def valid_iso_date(item):
+    """
+    Check if a date item is non null and parses as ISO (YYYY-MM-DD)
+    """
+    try:
+        datetime.datetime.strptime(item, "%Y-%m-%d")
+    except ValueError:
+        return(False)
+
+    return(True)
+
+def valid_reverse_iso_date(item):
+    """
+    Check if a date item is non null and parses as reverse ISO (DD-MM-YYYY)
+    """
+    try:
+        datetime.datetime.strptime(item, "%d-%m-%Y")
+    except ValueError:
+        return(False)
+
+    return(True)
+
+def valid_uk_date(item):
+    """
+    Check if a date item is non null and parses as UK format (DD/MM/YYYY)
+    """
+    try:
+        datetime.datetime.strptime(item, "%d/%m/%Y")
+    except ValueError:
         return(False)
+
     return(True)
 
-def load_person_ids(fh, mappingrules, delim=",", remap=True):
+def load_person_ids(fh, mappingrules, use_input_person_ids, person_number=1, delim=","):
     person_ids = {}
     person_columns = {}
-    person_col_number = 0
-    person_number = 1
+    person_col_in_hdr_number = 0
+    reject_count = 0
 
     phdr = fh.readline()
     personhdr = phdr.strip().split(delim)
     print(personhdr)
 
     # Make a dictionary of column names vs their positions
     for col in personhdr:
-        person_columns[col] = person_col_number
-        person_col_number += 1
+        person_columns[col] = person_col_in_hdr_number
+        person_col_in_hdr_number += 1
 
     birth_datetime_source, person_id_source = mappingrules.get_person_source_field_info("person")
+    print("Load Person Data {0}, {1}".format(birth_datetime_source, person_id_source))
     person_col = 0
 
     for line in fh:
         persondata = line.strip().split(delim)
         if not valid_value(persondata[person_columns[person_id_source]]):
+            reject_count += 1
             continue
         if not valid_date_value(persondata[person_columns[birth_datetime_source]]):
+            reject_count += 1
             continue
-        person_ids[persondata[person_col]] = str(person_number)
-        person_number += 1
+        if persondata[person_col] not in person_ids:
+            if use_input_person_ids == "N":
+                person_ids[persondata[person_col]] = str(person_number)
+                person_number += 1
+            else:
+                person_ids[persondata[person_col]] = str(persondata[person_col])
 
-    return person_ids
+    return person_ids, reject_count
 
 @click.command(help="Perform OMOP Mapping given a python configuration file.")
 @click.option("--rules",
               help="input json file containing all the mapping rules to be applied")
 @click.option("--pyconf","--conf",
               required=True,
               help="Run with a python configuration file")
```

### Comparing `carrot-cdm-0.6.7/carrot/cli/subcommands/search.py` & `carrot-cdm-0.6.8/carrot/cli/subcommands/search.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/io/common.py` & `carrot-cdm-0.6.8/carrot/io/common.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/io/plugins/bclink.py` & `carrot-cdm-0.6.8/carrot/io/plugins/bclink.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/io/plugins/local.py` & `carrot-cdm-0.6.8/carrot/io/plugins/local.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/io/plugins/sql.py` & `carrot-cdm-0.6.8/carrot/io/plugins/sql.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/__init__.py` & `carrot-cdm-0.6.8/carrot/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/bash_helpers.py` & `carrot-cdm-0.6.8/carrot/tools/bash_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/bclink_helpers.py` & `carrot-cdm-0.6.8/carrot/tools/bclink_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/dag.py` & `carrot-cdm-0.6.8/carrot/tools/dag.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/extract/__init__.py` & `carrot-cdm-0.6.8/carrot/tools/extract/__init__.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/extract/templates.py` & `carrot-cdm-0.6.8/carrot/tools/extract/templates.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/file_helpers.py` & `carrot-cdm-0.6.8/carrot/tools/file_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/logger.py` & `carrot-cdm-0.6.8/carrot/tools/logger.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/mappingrules.py` & `carrot-cdm-0.6.8/carrot/tools/mappingrules.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import os
 import json
 from .omopcdm import OmopCDM
 
 class MappingRules:
 
-    def __init__(self, rulesfilepath):
+    def __init__(self, rulesfilepath, omopcfgfilepath):
         self.rules_data = self.load_json(rulesfilepath)
-        self.omopcdm = OmopCDM()
+        self.omopcdm = OmopCDM(omopcfgfilepath)
         self.parsed_rules = {}
         self.outfile_names = {}
 
     def load_json(self, f_in):
         """
         """
         if os.path.exists(f_in):
@@ -47,14 +47,33 @@
                         outfielddata = outfield.split("~")
                         if self.omopcdm.is_omop_data_field(outfile, outfielddata[0]):
                             if infield not in data_fields_lists[outfile]:
                                 data_fields_lists[outfile].append(infield)
 
         return data_fields_lists
 
+    def get_infile_date_person_id(self, infilename):
+        outfilenames, outdata = self.parse_rules_src_to_tgt(infilename)
+        datetime_source = ""
+        person_id_source = ""
+
+        for key, outfield_data in outdata.items():
+            keydata = key.split("~")
+            outfile = keydata[-1]
+            for outfield_elem in outfield_data:
+                for infield, outfield_list in outfield_elem.items():
+                    #print("{0}, {1}, {2}".format(outfile, infield, str(outfield_list)))
+                    for outfield in outfield_list:
+                        if outfield in self.omopcdm.get_omop_datetime_fields(outfile):
+                            datetime_source = infield
+                        if outfield == self.omopcdm.get_omop_person_id_field(outfile):
+                            person_id_source = infield
+
+        return datetime_source, person_id_source
+
     def get_person_source_field_info(self, tgtfilename):
         """
         Specific discovery of input data field names for 'person' in these rules
         """
         birth_datetime_source = None
         person_id_source = None
         if tgtfilename in self.rules_data["cdm"]:
```

### Comparing `carrot-cdm-0.6.7/carrot/tools/profiling.py` & `carrot-cdm-0.6.8/carrot/tools/profiling.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot/tools/rules_helpers.py` & `carrot-cdm-0.6.8/carrot/tools/rules_helpers.py`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/carrot_cdm.egg-info/PKG-INFO` & `carrot-cdm-0.6.8/carrot_cdm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carrot-cdm
-Version: 0.6.7
+Version: 0.6.8
 Summary: Python package for performing mapping of ETL to CDM 
 Home-page: https://github.com/HDRUK/CaRROT-CDM
 Author: CO-CONNECT Collaboration
 Author-email: calmacx@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `carrot-cdm-0.6.7/carrot_cdm.egg-info/SOURCES.txt` & `carrot-cdm-0.6.8/carrot_cdm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `carrot-cdm-0.6.7/setup.py` & `carrot-cdm-0.6.8/setup.py`

 * *Files identical despite different names*

