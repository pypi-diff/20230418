# Comparing `tmp/cbcflow-0.1.1.tar.gz` & `tmp/cbcflow-0.1.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.1.1.tar", last modified: Thu Apr 13 23:01:39 2023, max compression
+gzip compressed data, was "cbcflow-0.1.2a1.tar", last modified: Tue Apr 18 03:29:43 2023, max compression
```

## Comparing `cbcflow-0.1.1.tar` & `cbcflow-0.1.2a1.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.022657 cbcflow-0.1.1/
--rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.1/.gitattributes
--rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-13 22:27:45.000000 cbcflow-0.1.1/.gitignore
--rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-13 21:35:01.000000 cbcflow-0.1.1/.gitlab-ci.yml
--rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-13 22:57:24.000000 cbcflow-0.1.1/CHANGELOG.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-13 22:57:24.000000 cbcflow-0.1.1/LICENSE.md
--rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-13 22:57:24.000000 cbcflow-0.1.1/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     3037 2023-04-13 23:01:39.022657 cbcflow-0.1.1/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.1/README.md
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.000990 cbcflow-0.1.1/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/Makefile
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/requirements.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.000990 cbcflow-0.1.1/docs/source/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.000990 cbcflow-0.1.1/docs/source/_templates/
--rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/actionitems.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/adding-to-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/asimov.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/conf.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/configuration.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/development-setup.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.000990 cbcflow-0.1.1/docs/source/example_mini_schema/
--rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/example_mini_schema/example.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/example_mini_schema/schema_doc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/example_mini_schema/schema_doc.html
--rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/example_mini_schema/schema_doc.min.js
--rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/gwosc.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/index.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.011823 cbcflow-0.1.1/docs/source/libraries_images/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.011823 cbcflow-0.1.1/docs/source/libraries_images/.ipynb_checkpoints/
--rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_1.png
--rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_2.png
--rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_3.png
--rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_4.png
--rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_5.png
--rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_6.png
--rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_7.png
--rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/libraries_images/part_8.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/library-index-labelling.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/library-indices.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/library-setup.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/monitor-usage.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/reading-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.1/docs/source/schema-visualization.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    15260 2023-04-13 22:27:13.000000 cbcflow-0.1.1/docs/source/updating-metadata-from-the-command-line.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/updating-metadata-with-the-python-api.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-13 21:35:01.000000 cbcflow-0.1.1/docs/source/what-is-metadata.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.011823 cbcflow-0.1.1/examples/
--rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.1/examples/initial_example.md
--rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.1/pyproject.toml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.011823 cbcflow-0.1.1/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.1/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88914 2023-04-13 21:35:01.000000 cbcflow-0.1.1/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-13 21:35:01.000000 cbcflow-0.1.1/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     1375 2023-04-13 23:01:39.022657 cbcflow-0.1.1/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.1/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.000990 cbcflow-0.1.1/src/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.011823 cbcflow-0.1.1/src/cbcflow/
--rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      160 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow/_version.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     7295 2023-04-13 22:08:53.000000 cbcflow-0.1.1/src/cbcflow/cbcflow.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/configuration.py
--rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/gracedb.py
--rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/monitor.py
--rw-r--r--   0 greg      (1000) greg      (1000)     6997 2023-04-13 22:08:53.000000 cbcflow-0.1.1/src/cbcflow/parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/process.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.022657 cbcflow-0.1.1/src/cbcflow/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88914 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.1/src/cbcflow/schema.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4189 2023-04-13 21:59:09.000000 cbcflow-0.1.1/src/cbcflow/utils.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.022657 cbcflow-0.1.1/src/cbcflow.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     3037 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3060 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      355 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow.egg-info/entry_points.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-13 23:01:38.000000 cbcflow-0.1.1/src/cbcflow.egg-info/top_level.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.022657 cbcflow-0.1.1/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.022657 cbcflow-0.1.1/tests/files_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/cbc-meta-data-example.json
--rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/test-file-for-linking-1.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/test-file-for-linking-2.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/update_json_1.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/update_json_2.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/update_yaml_1.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/files_for_testing/update_yaml_2.yaml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-13 23:01:39.022657 cbcflow-0.1.1/tests/library_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/library_for_testing/library.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/library_for_testing/testing-library-index.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.1/tests/test_database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.1/tests/test_metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.1/tests/test_parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.1/tests/test_schema.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/
+-rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/.gitattributes
+-rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/.gitignore
+-rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/.gitlab-ci.yml
+-rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/.pre-commit-config.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/CHANGELOG.md
+-rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/LICENSE.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/README.md
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/
+-rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/Makefile
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/requirements.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/source/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/source/_templates/
+-rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/actionitems.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/adding-to-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/asimov.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/conf.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/configuration.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/development-setup.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/source/example_mini_schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/example.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.html
+-rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.min.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/gwosc.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/index.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/docs/source/libraries_images/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_1.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_2.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_3.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_4.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_5.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_6.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_7.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_8.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/library-index-labelling.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/library-indices.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/library-setup.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/monitor-usage.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/reading-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/schema-visualization.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/docs/source/updating-metadata-from-the-command-line.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/updating-metadata-with-the-python-api.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/what-is-metadata.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/examples/
+-rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/examples/initial_example.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/pyproject.toml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88914 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     1375 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.2a1/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/src/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/src/cbcflow/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      162 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow/_version.py
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     7347 2023-04-18 03:21:14.000000 cbcflow-0.1.2a1/src/cbcflow/cbcflow.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/configuration.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/gracedb.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/monitor.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     7734 2023-04-18 03:21:14.000000 cbcflow-0.1.2a1/src/cbcflow/parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/process.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/src/cbcflow/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-18 03:29:42.000000 cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88914 2023-04-18 03:29:42.000000 cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:29:42.000000 cbcflow-0.1.2a1/src/cbcflow/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/schema.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     4189 2023-04-13 21:59:09.000000 cbcflow-0.1.2a1/src/cbcflow/utils.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/src/cbcflow.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3060 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      355 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/entry_points.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/top_level.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/tests/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/tests/files_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/cbc-meta-data-example.json
+-rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_json_1.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_json_2.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_1.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_2.yaml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/tests/library_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/library_for_testing/library.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/library_for_testing/testing-library-index.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/test_database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/test_metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.2a1/tests/test_parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/tests/test_schema.py
```

### Comparing `cbcflow-0.1.1/.gitlab-ci.yml` & `cbcflow-0.1.2a1/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/.pre-commit-config.yaml` & `cbcflow-0.1.2a1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/LICENSE.md` & `cbcflow-0.1.2a1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/PKG-INFO` & `cbcflow-0.1.2a1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.1
+Version: 0.1.2a1
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/meta-data
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.1.1/README.md` & `cbcflow-0.1.2a1/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/Makefile` & `cbcflow-0.1.2a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.1.2a1/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.1.2a1/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/actionitems.rst` & `cbcflow-0.1.2a1/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/adding-to-the-schema.rst` & `cbcflow-0.1.2a1/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/conf.py` & `cbcflow-0.1.2a1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/configuration.rst` & `cbcflow-0.1.2a1/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/development-setup.rst` & `cbcflow-0.1.2a1/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/example_mini_schema/example.schema` & `cbcflow-0.1.2a1/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/index.rst` & `cbcflow-0.1.2a1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries.rst` & `cbcflow-0.1.2a1/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_1.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_2.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_3.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_4.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_5.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_6.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_7.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/libraries_images/part_8.png` & `cbcflow-0.1.2a1/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/library-index-labelling.rst` & `cbcflow-0.1.2a1/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/library-indices.rst` & `cbcflow-0.1.2a1/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/library-setup.rst` & `cbcflow-0.1.2a1/docs/source/library-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/monitor-usage.rst` & `cbcflow-0.1.2a1/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/reading-the-schema.rst` & `cbcflow-0.1.2a1/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.1.2a1/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 Command Line Interface
 ==========================
 
 For many users, the main tool for interacting with ``cbcflow`` metadata are the suite of command line tools.
 These allow you to:
+
 #. Print the contents of a metadata file
 #. Pull GraceDB information into a metadata file
 #. Update a metadata file using a series of flags
 #. Update a metadata file by writing a file containing many changes
+
 This documentation will go over how to use each of those, and also provide an introduction to updating metadata in general.
 
 This page assumes that you have read :doc:`what-is-metadata` and :doc:`reading-the-schema` already -
 if you haven't it is strongly encouraged that you do so first.
 
 The Tutorial Library
 --------------------
@@ -136,14 +138,16 @@
 
 .. code-block::
 
   cbcflow_update_from_flags S230409it --ParameterEstimation-Analysts-add "Name"
 
 where naturally "Name" is your name!
 
+Note: the commands get be quite long and cumbersome. To help, if you follow the :doc:`configuration` guide and set up ``argcomplete``, you can use the <TAB> key to help when you can't recmember the full command.
+
 Now, we also want to make some changes to a result.
 All of these are modifying a field that's not an array, so all of them will use ``set``.
 For our ``UID``, we have ``--ParameterEstimation-Results-UID-set``, and lets call our result "Tutorial1".
 Notice that the ending of this flag is ``-UID-set``: this is one of the two magic combinations in ``cbcflow``.
 This designates that this flag is setting which analysis we modify, and so must always be included if we want to modify that analysis.
 Moreover, if this specific combination appears at the end of a command, you know that is what it *must* mean.
 
@@ -264,8 +268,8 @@
       - Path: /path/to/a/file
 
 These can be applied by the same command.
 
 Finally, one may notice one last detail: how can we remove array elements with this?
 For this we can write a negative image file. 
 When applied with the extra flag ``--removal-file``, any element in the array will be removed instead of being added. 
-So, applying the first file above will *remove* the analyst with "Name", instead of adding them.
+So, applying the first file above will *remove* the analyst with "Name", instead of adding them.
```

### Comparing `cbcflow-0.1.1/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.1.2a1/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/docs/source/what-is-metadata.rst` & `cbcflow-0.1.2a1/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/examples/initial_example.md` & `cbcflow-0.1.2a1/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/pyproject.toml` & `cbcflow-0.1.2a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/schema/cbc-meta-data-v1.schema` & `cbcflow-0.1.2a1/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/schema/cbc-meta-data-v2.schema` & `cbcflow-0.1.2a1/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/schema/index-v1.schema` & `cbcflow-0.1.2a1/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/setup.cfg` & `cbcflow-0.1.2a1/setup.cfg`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/setup.py` & `cbcflow-0.1.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/__init__.py` & `cbcflow-0.1.2a1/src/cbcflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/cbcflow.py` & `cbcflow-0.1.2a1/src/cbcflow/cbcflow.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 import jsonschema
 
 from .configuration import config_defaults
 from .gracedb import fetch_gracedb_information
 from .metadata import MetaData
 from .database import LocalLibraryDatabase
-from .parser import get_parser_and_default_data
+from .parser import get_parser_and_default_data, sname_string
 from .process import process_user_input
 from .schema import get_schema
 
 
 def setup_logger() -> "logging.Logger":
     """Setup a logger for CBCFlow"""
     logging.basicConfig(level=logging.INFO)
@@ -100,15 +100,15 @@
 def print_metadata() -> None:
     """Print the metadata for a given event in a given library, as passed in args"""
     # Read in command line arguments
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
 
     parser = argparse.ArgumentParser()
-    parser.add_argument("sname", help="The superevent SNAME")
+    parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     parser.add_argument(
         "--library", default=config_defaults["library"], help="The library"
     )
     args = parser.parse_args()
 
     # Set the sname in the default data
     default_data["Sname"] = args.sname
@@ -129,15 +129,15 @@
     logger = setup_logger()
 
     # Read in command line arguments
     schema = get_schema()
     _, default_data = get_parser_and_default_data(schema)
 
     file_parser = argparse.ArgumentParser()
-    file_parser.add_argument("sname", help="The superevent SNAME")
+    file_parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     file_parser.add_argument(
         "update_file",
         help="The file to update from, either a json or a yaml.\
         The type of file will be inferred from the ending .yaml or .json",
     )
     file_parser.add_argument(
         "--removal-file",
```

### Comparing `cbcflow-0.1.1/src/cbcflow/configuration.py` & `cbcflow-0.1.2a1/src/cbcflow/configuration.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/database.py` & `cbcflow-0.1.2a1/src/cbcflow/database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/gracedb.py` & `cbcflow-0.1.2a1/src/cbcflow/gracedb.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/metadata.py` & `cbcflow-0.1.2a1/src/cbcflow/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/monitor.py` & `cbcflow-0.1.2a1/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/parser.py` & `cbcflow-0.1.2a1/src/cbcflow/parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Parsing tools, and tools for generating default data"""
 import argparse
 import logging
 from typing import Tuple
+import re
 
 import argcomplete
 
 from .configuration import config_defaults
 
 logger = logging.getLogger(__name__)
 
@@ -179,15 +180,15 @@
     =======
     `argparse.ArgumentParser`
         A parser object, associated with this schema
     dict
         The default data associated with this schema
     """
     parser = argparse.ArgumentParser(allow_abbrev=False)
-    parser.add_argument("sname", help="The superevent SNAME")
+    parser.add_argument("sname", help="The superevent SNAME", type=sname_string)
     parser.add_argument(
         "--library", default=config_defaults["library"], help="The library"
     )
     parser.add_argument("--schema-version", help="The schema version to use")
     parser.add_argument(
         "--schema-file",
         help="Explicit path to the schema-file. If None (default) the inbuilt schema is used",
@@ -208,7 +209,34 @@
         help="Do not ask for confirmation",
         action="store_true",
     )
 
     parser, default_data = build_parser_from_schema(parser, schema)
     argcomplete.autocomplete(parser)
     return parser, default_data
+
+
+def sname_string(sname):
+    """Sanitize and check the given sname string
+
+    This will check there is one unique sname in the given string. Other text
+    is ignored (allowing the meta-data filename to be passed) while no match
+    or multiple matches will raise an error
+
+    Parameters
+    ==========
+    sname : str
+        The input sname it sanitize and check
+
+    Returns
+    =======
+    sname
+        The unique sname
+
+    """
+    matches = re.findall("S[0-9]{6}[a-z]+", sname)
+    if len(matches) == 0:
+        raise TypeError("Given sname invalid")
+    elif len(matches) > 1:
+        raise TypeError("Multiple snames given, we can only handle one at a time")
+    else:
+        return matches[0]
```

### Comparing `cbcflow-0.1.1/src/cbcflow/process.py` & `cbcflow-0.1.2a1/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.1.2a1/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/schema.py` & `cbcflow-0.1.2a1/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow/utils.py` & `cbcflow-0.1.2a1/src/cbcflow/utils.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.1.2a1/src/cbcflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.1
+Version: 0.1.2a1
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/meta-data
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.1.1/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.1.2a1/src/cbcflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.1.2a1/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/files_for_testing/update_json_1.json` & `cbcflow-0.1.2a1/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/files_for_testing/update_json_2.json` & `cbcflow-0.1.2a1/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.1.2a1/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/test_database.py` & `cbcflow-0.1.2a1/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/test_metadata.py` & `cbcflow-0.1.2a1/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/test_parser.py` & `cbcflow-0.1.2a1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.1/tests/test_schema.py` & `cbcflow-0.1.2a1/tests/test_schema.py`

 * *Files identical despite different names*

