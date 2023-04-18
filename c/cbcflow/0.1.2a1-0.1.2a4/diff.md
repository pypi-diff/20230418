# Comparing `tmp/cbcflow-0.1.2a1.tar.gz` & `tmp/cbcflow-0.1.2a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbcflow-0.1.2a1.tar", last modified: Tue Apr 18 03:29:43 2023, max compression
+gzip compressed data, was "cbcflow-0.1.2a4.tar", last modified: Tue Apr 18 03:42:04 2023, max compression
```

## Comparing `cbcflow-0.1.2a1.tar` & `cbcflow-0.1.2a4.tar`

### file list

```diff
@@ -1,108 +1,109 @@
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/
--rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/.gitattributes
--rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/.gitignore
--rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/.gitlab-ci.yml
--rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/.pre-commit-config.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/CHANGELOG.md
--rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/LICENSE.md
--rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/MANIFEST.in
--rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/README.md
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/
--rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/Makefile
--rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/requirements.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/source/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/source/_templates/
--rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/_templates/custom-class-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/_templates/custom-module-template.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/actionitems.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/adding-to-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/asimov.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/conf.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/configuration.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/development-setup.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/docs/source/example_mini_schema/
--rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/example.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.css
--rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.html
--rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.min.js
--rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/gwosc.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/index.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/docs/source/libraries_images/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/docs/source/libraries_images/.ipynb_checkpoints/
--rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
--rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_1.png
--rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_2.png
--rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_3.png
--rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_4.png
--rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_5.png
--rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_6.png
--rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_7.png
--rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/libraries_images/part_8.png
--rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/library-index-labelling.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/library-indices.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/library-setup.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/monitor-usage.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/reading-the-schema.rst
--rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/docs/source/schema-visualization.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-17 11:18:52.000000 cbcflow-0.1.2a1/docs/source/updating-metadata-from-the-command-line.rst
--rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/updating-metadata-with-the-python-api.rst
--rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/docs/source/what-is-metadata.rst
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/examples/
--rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/examples/initial_example.md
--rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/pyproject.toml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.241124 cbcflow-0.1.2a1/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88914 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     1375 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/setup.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.2a1/setup.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.230291 cbcflow-0.1.2a1/src/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/src/cbcflow/
--rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/__init__.py
--rw-r--r--   0 greg      (1000) greg      (1000)      162 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow/_version.py
--rwxr-xr-x   0 greg      (1000) greg      (1000)     7347 2023-04-18 03:21:14.000000 cbcflow-0.1.2a1/src/cbcflow/cbcflow.py
--rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/configuration.py
--rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/database.py
--rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/gracedb.py
--rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/monitor.py
--rw-r--r--   0 greg      (1000) greg      (1000)     7734 2023-04-18 03:21:14.000000 cbcflow-0.1.2a1/src/cbcflow/parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/process.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/src/cbcflow/schema/
--rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-18 03:29:42.000000 cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)    88914 2023-04-18 03:29:42.000000 cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v2.schema
--rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:29:42.000000 cbcflow-0.1.2a1/src/cbcflow/schema/index-v1.schema
--rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/src/cbcflow/schema.py
--rw-r--r--   0 greg      (1000) greg      (1000)     4189 2023-04-13 21:59:09.000000 cbcflow-0.1.2a1/src/cbcflow/utils.py
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/src/cbcflow.egg-info/
--rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/PKG-INFO
--rw-r--r--   0 greg      (1000) greg      (1000)     3060 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/SOURCES.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/dependency_links.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      355 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/entry_points.txt
--rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/requires.txt
--rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-18 03:29:43.000000 cbcflow-0.1.2a1/src/cbcflow.egg-info/top_level.txt
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/tests/
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/tests/files_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/cbc-meta-data-example.json
--rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/test-file-for-linking-1.txt
--rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/test-file-for-linking-2.txt
--rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_json_1.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_json_2.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_1.yaml
--rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_2.yaml
-drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:29:43.251958 cbcflow-0.1.2a1/tests/library_for_testing/
--rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230227hp-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230331e-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230401h-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230402dv-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230403ae-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230404hb-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/library_for_testing/S230404jc-cbc-metadata.json
--rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/library_for_testing/library.cfg
--rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/library_for_testing/testing-library-index.json
--rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.2a1/tests/test_database.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.2a1/tests/test_metadata.py
--rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.2a1/tests/test_parser.py
--rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.2a1/tests/test_schema.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/
+-rw-r--r--   0 greg      (1000) greg      (1000)       37 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/.gitattributes
+-rw-r--r--   0 greg      (1000) greg      (1000)      217 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/.gitignore
+-rw-r--r--   0 greg      (1000) greg      (1000)     1533 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/.gitlab-ci.yml
+-rw-r--r--   0 greg      (1000) greg      (1000)      873 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/.pre-commit-config.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      405 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/CHANGELOG.md
+-rw-r--r--   0 greg      (1000) greg      (1000)     1084 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/LICENSE.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      123 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/MANIFEST.in
+-rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     2394 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/README.md
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.955842 cbcflow-0.1.2a4/docs/
+-rw-r--r--   0 greg      (1000) greg      (1000)      613 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/Makefile
+-rw-r--r--   0 greg      (1000) greg      (1000)       53 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/requirements.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/_templates/
+-rw-r--r--   0 greg      (1000) greg      (1000)      662 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/_templates/custom-class-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1408 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/_templates/custom-module-template.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1158 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/actionitems.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      690 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/adding-to-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)       39 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/asimov.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2616 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/conf.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1770 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/configuration.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1444 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/development-setup.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/example_mini_schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)     2924 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/example.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     6391 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.css
+-rw-r--r--   0 greg      (1000) greg      (1000)    27212 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.html
+-rw-r--r--   0 greg      (1000) greg      (1000)      984 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.min.js
+-rw-r--r--   0 greg      (1000) greg      (1000)      458 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/gwosc.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1191 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/index.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     2799 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/libraries_images/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/docs/source/libraries_images/.ipynb_checkpoints/
+-rw-r--r--   0 greg      (1000) greg      (1000)    72683 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
+-rw-r--r--   0 greg      (1000) greg      (1000)     8993 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_1.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    15966 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_2.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    38016 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_3.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    51488 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_4.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    41435 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_5.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    54941 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_6.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    67345 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_7.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    72180 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/libraries_images/part_8.png
+-rw-r--r--   0 greg      (1000) greg      (1000)    10255 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/library-index-labelling.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1358 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/library-indices.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1960 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/library-setup.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     1782 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/monitor-usage.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4809 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/reading-the-schema.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)      106 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/docs/source/schema-visualization.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    15476 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/updating-metadata-from-the-command-line.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)    12152 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/updating-metadata-with-the-python-api.rst
+-rw-r--r--   0 greg      (1000) greg      (1000)     4916 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/docs/source/what-is-metadata.rst
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/examples/
+-rw-r--r--   0 greg      (1000) greg      (1000)     7368 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/examples/initial_example.md
+-rw-r--r--   0 greg      (1000) greg      (1000)      860 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/pyproject.toml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88880 2023-04-18 03:35:57.000000 cbcflow-0.1.2a4/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     1503 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/setup.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)      567 2023-04-13 22:38:42.000000 cbcflow-0.1.2a4/setup.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.955842 cbcflow-0.1.2a4/src/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.966676 cbcflow-0.1.2a4/src/cbcflow/
+-rw-r--r--   0 greg      (1000) greg      (1000)     1426 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/__init__.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      162 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/_version.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    12180 2023-04-18 03:35:57.000000 cbcflow-0.1.2a4/src/cbcflow/asimov.py
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     7347 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/src/cbcflow/cbcflow.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     1325 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/configuration.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    29553 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     9226 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/src/cbcflow/gracedb.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    13615 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     4757 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/monitor.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     7734 2023-04-18 03:41:18.000000 cbcflow-0.1.2a4/src/cbcflow/parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    20427 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/process.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/src/cbcflow/schema/
+-rw-r--r--   0 greg      (1000) greg      (1000)    40294 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)    88880 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v2.schema
+-rwxr-xr-x   0 greg      (1000) greg      (1000)     1768 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow/schema/index-v1.schema
+-rw-r--r--   0 greg      (1000) greg      (1000)     2750 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/src/cbcflow/schema.py
+-rw-r--r--   0 greg      (1000) greg      (1000)     5044 2023-04-18 03:35:57.000000 cbcflow-0.1.2a4/src/cbcflow/utils.py
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/src/cbcflow.egg-info/
+-rw-r--r--   0 greg      (1000) greg      (1000)     3039 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/PKG-INFO
+-rw-r--r--   0 greg      (1000) greg      (1000)     3082 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/SOURCES.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        1 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/dependency_links.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      481 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/entry_points.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)      115 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/requires.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)        8 2023-04-18 03:42:04.000000 cbcflow-0.1.2a4/src/cbcflow.egg-info/top_level.txt
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/tests/
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/tests/files_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)    26759 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/cbc-meta-data-example.json
+-rw-r--r--   0 greg      (1000) greg      (1000)       56 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/test-file-for-linking-1.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)       86 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/test-file-for-linking-2.txt
+-rw-r--r--   0 greg      (1000) greg      (1000)     3091 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_json_1.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1221 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_json_2.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1626 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_1.yaml
+-rw-r--r--   0 greg      (1000) greg      (1000)      571 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_2.yaml
+drwxr-xr-x   0 greg      (1000) greg      (1000)        0 2023-04-18 03:42:04.977509 cbcflow-0.1.2a4/tests/library_for_testing/
+-rw-r--r--   0 greg      (1000) greg      (1000)     5338 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230227hp-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4289 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230331e-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     4275 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230401h-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     2416 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230402dv-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3353 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230403ae-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     5238 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230404hb-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     3256 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/library_for_testing/S230404jc-cbc-metadata.json
+-rw-r--r--   0 greg      (1000) greg      (1000)      193 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/library_for_testing/library.cfg
+-rw-r--r--   0 greg      (1000) greg      (1000)       90 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/library_for_testing/testing-library-index.json
+-rw-r--r--   0 greg      (1000) greg      (1000)     1840 2023-04-13 21:35:01.000000 cbcflow-0.1.2a4/tests/test_database.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-04 20:38:56.000000 cbcflow-0.1.2a4/tests/test_metadata.py
+-rw-r--r--   0 greg      (1000) greg      (1000)    23461 2023-04-13 22:03:31.000000 cbcflow-0.1.2a4/tests/test_parser.py
+-rw-r--r--   0 greg      (1000) greg      (1000)      755 2023-04-04 15:21:01.000000 cbcflow-0.1.2a4/tests/test_schema.py
```

### Comparing `cbcflow-0.1.2a1/.gitlab-ci.yml` & `cbcflow-0.1.2a4/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/.pre-commit-config.yaml` & `cbcflow-0.1.2a4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/LICENSE.md` & `cbcflow-0.1.2a4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/PKG-INFO` & `cbcflow-0.1.2a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.2a1
+Version: 0.1.2a4
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/meta-data
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.1.2a1/README.md` & `cbcflow-0.1.2a4/README.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/Makefile` & `cbcflow-0.1.2a4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/_templates/custom-class-template.rst` & `cbcflow-0.1.2a4/docs/source/_templates/custom-class-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/_templates/custom-module-template.rst` & `cbcflow-0.1.2a4/docs/source/_templates/custom-module-template.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/actionitems.rst` & `cbcflow-0.1.2a4/docs/source/actionitems.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/adding-to-the-schema.rst` & `cbcflow-0.1.2a4/docs/source/adding-to-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/conf.py` & `cbcflow-0.1.2a4/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/configuration.rst` & `cbcflow-0.1.2a4/docs/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/development-setup.rst` & `cbcflow-0.1.2a4/docs/source/development-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/example_mini_schema/example.schema` & `cbcflow-0.1.2a4/docs/source/example_mini_schema/example.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.css` & `cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.css`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.html` & `cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.html`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/example_mini_schema/schema_doc.min.js` & `cbcflow-0.1.2a4/docs/source/example_mini_schema/schema_doc.min.js`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/index.rst` & `cbcflow-0.1.2a4/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries.rst` & `cbcflow-0.1.2a4/docs/source/libraries.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_1.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_1.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_2.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_2.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_3.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_3.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_4.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_4.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_5.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_5.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_6.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_6.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_7.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_7.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/libraries_images/part_8.png` & `cbcflow-0.1.2a4/docs/source/libraries_images/part_8.png`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/library-index-labelling.rst` & `cbcflow-0.1.2a4/docs/source/library-index-labelling.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/library-indices.rst` & `cbcflow-0.1.2a4/docs/source/library-indices.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/library-setup.rst` & `cbcflow-0.1.2a4/docs/source/library-setup.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/monitor-usage.rst` & `cbcflow-0.1.2a4/docs/source/monitor-usage.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/reading-the-schema.rst` & `cbcflow-0.1.2a4/docs/source/reading-the-schema.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/updating-metadata-from-the-command-line.rst` & `cbcflow-0.1.2a4/docs/source/updating-metadata-from-the-command-line.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/updating-metadata-with-the-python-api.rst` & `cbcflow-0.1.2a4/docs/source/updating-metadata-with-the-python-api.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/docs/source/what-is-metadata.rst` & `cbcflow-0.1.2a4/docs/source/what-is-metadata.rst`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/examples/initial_example.md` & `cbcflow-0.1.2a4/examples/initial_example.md`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/pyproject.toml` & `cbcflow-0.1.2a4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/schema/cbc-meta-data-v1.schema` & `cbcflow-0.1.2a4/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/schema/cbc-meta-data-v2.schema` & `cbcflow-0.1.2a4/schema/cbc-meta-data-v2.schema`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999596504479317%*

 * *Differences: {"'$defs'": "{'DetcharDetector': {'properties': {'RecommendedMinimumFrequency': {'description': "*

 * *            "'The recommended minimum frequency for analysis - this may be empty if defaults "*

 * *            "should be used', delete: ['default']}, 'RecommendedMaximumFrequency': {'description': "*

 * *            "'The recommended maximum frequency for the analysis - this may be empty if defaults "*

 * *            "should be used'}, 'RecommendedChannel': {'description': 'The channels to use in the "*

 * *            "analysi […]*

```diff
@@ -262,18 +262,17 @@
                 "UID"
             ],
             "type": "object"
         },
         "DetcharDetector": {
             "additionalProperties": false,
             "properties": {
-                "FrameLocation": {
-                    "$ref": "#/$defs/LinkedFile",
-                    "description": "The location of the frames on a cluster - CIT preferred by default. If no mitigation is required this will be the default given the time.",
-                    "type": "object"
+                "FrameType": {
+                    "description": "The type of frame to use - this may be empty if defaults should be used.",
+                    "type": "string"
                 },
                 "GlitchMitigationStatus": {
                     "default": "not yet reviewed",
                     "enum": [
                         "not yet reviewed",
                         "required",
                         "not required",
@@ -285,29 +284,28 @@
                     "description": "An array containing strings with notes, comments, or other miscellaneous data (e.g. string format of a dictionary for some excess data)",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "RecommendedChannel": {
-                    "description": "The channels to use in the analysis for this detector",
+                    "description": "The channels to use in the analysis for this detector - this may be empty if defaults should be used",
                     "pattern": "^(H|L|V|K|G)1:*",
                     "type": "string"
                 },
                 "RecommendedEndTime": {
                     "description": "The validated safe end time to set for downstream analyses to avoid data quality issues",
                     "type": "number"
                 },
                 "RecommendedMaximumFrequency": {
-                    "description": "The recommended maximum frequency for the analysis - this may be set by the PE configurator rather than detchar",
+                    "description": "The recommended maximum frequency for the analysis - this may be empty if defaults should be used",
                     "type": "number"
                 },
                 "RecommendedMinimumFrequency": {
-                    "default": 20.0,
-                    "description": "The recommended minimum frequency for analysis",
+                    "description": "The recommended minimum frequency for analysis - this may be empty if defaults should be used",
                     "type": "number"
                 },
                 "RecommendedStartTime": {
                     "description": "The  validated safe start time to set for downstream analyses to avoid data quality issues",
                     "type": "number"
                 },
                 "UID": {
@@ -2441,16 +2439,15 @@
                     "description": "The list of all detectors that should be analysed in downstream analyses",
                     "items": {
                         "$ref": "#/$defs/DetcharDetector"
                     },
                     "type": "array"
                 },
                 "RecommendedDuration": {
-                    "default": 4.0,
-                    "description": "The  validated safe maximum time duration to set for downstream analyses to avoid data quality issues",
+                    "description": "The  validated safe maximum time duration to set for downstream analyses to avoid data quality issues - this may be empty if defaults should be used",
                     "type": "number"
                 },
                 "Reviewers": {
                     "description": "The names of all reviewers involved",
                     "items": {
                         "type": "string"
                     },
```

### Comparing `cbcflow-0.1.2a1/schema/index-v1.schema` & `cbcflow-0.1.2a4/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/setup.cfg` & `cbcflow-0.1.2a4/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -32,14 +32,18 @@
 	PyYAML
 	gwpy
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
+asimov.hooks.postmonitor = 
+	cbcflow = cbcflow.asimov:Collector
+asimov.hooks.applicator = 
+	cbcflow = cbcflow.asimov:Applicator
 console_scripts = 
 	cbcflow_print = cbcflow:cbcflow.print_metadata
 	cbcflow_pull = cbcflow:cbcflow.pull
 	cbcflow_update_from_flags = cbcflow:cbcflow.update
 	cbcflow_update_from_file = cbcflow:cbcflow.from_file
 	cbcflow_monitor_make = cbcflow:generate_crondor
 	cbcflow_monitor_run = cbcflow:run_monitor
```

### Comparing `cbcflow-0.1.2a1/setup.py` & `cbcflow-0.1.2a4/setup.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/__init__.py` & `cbcflow-0.1.2a4/src/cbcflow/__init__.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/cbcflow.py` & `cbcflow-0.1.2a4/src/cbcflow/cbcflow.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/configuration.py` & `cbcflow-0.1.2a4/src/cbcflow/configuration.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/database.py` & `cbcflow-0.1.2a4/src/cbcflow/database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/gracedb.py` & `cbcflow-0.1.2a4/src/cbcflow/gracedb.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/metadata.py` & `cbcflow-0.1.2a4/src/cbcflow/metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/monitor.py` & `cbcflow-0.1.2a4/src/cbcflow/monitor.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/parser.py` & `cbcflow-0.1.2a4/src/cbcflow/parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/process.py` & `cbcflow-0.1.2a4/src/cbcflow/process.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v1.schema` & `cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/schema/cbc-meta-data-v2.schema` & `cbcflow-0.1.2a4/src/cbcflow/schema/cbc-meta-data-v2.schema`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999596504479317%*

 * *Differences: {"'$defs'": "{'DetcharDetector': {'properties': {'RecommendedMinimumFrequency': {'description': "*

 * *            "'The recommended minimum frequency for analysis - this may be empty if defaults "*

 * *            "should be used', delete: ['default']}, 'RecommendedMaximumFrequency': {'description': "*

 * *            "'The recommended maximum frequency for the analysis - this may be empty if defaults "*

 * *            "should be used'}, 'RecommendedChannel': {'description': 'The channels to use in the "*

 * *            "analysi […]*

```diff
@@ -262,18 +262,17 @@
                 "UID"
             ],
             "type": "object"
         },
         "DetcharDetector": {
             "additionalProperties": false,
             "properties": {
-                "FrameLocation": {
-                    "$ref": "#/$defs/LinkedFile",
-                    "description": "The location of the frames on a cluster - CIT preferred by default. If no mitigation is required this will be the default given the time.",
-                    "type": "object"
+                "FrameType": {
+                    "description": "The type of frame to use - this may be empty if defaults should be used.",
+                    "type": "string"
                 },
                 "GlitchMitigationStatus": {
                     "default": "not yet reviewed",
                     "enum": [
                         "not yet reviewed",
                         "required",
                         "not required",
@@ -285,29 +284,28 @@
                     "description": "An array containing strings with notes, comments, or other miscellaneous data (e.g. string format of a dictionary for some excess data)",
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "RecommendedChannel": {
-                    "description": "The channels to use in the analysis for this detector",
+                    "description": "The channels to use in the analysis for this detector - this may be empty if defaults should be used",
                     "pattern": "^(H|L|V|K|G)1:*",
                     "type": "string"
                 },
                 "RecommendedEndTime": {
                     "description": "The validated safe end time to set for downstream analyses to avoid data quality issues",
                     "type": "number"
                 },
                 "RecommendedMaximumFrequency": {
-                    "description": "The recommended maximum frequency for the analysis - this may be set by the PE configurator rather than detchar",
+                    "description": "The recommended maximum frequency for the analysis - this may be empty if defaults should be used",
                     "type": "number"
                 },
                 "RecommendedMinimumFrequency": {
-                    "default": 20.0,
-                    "description": "The recommended minimum frequency for analysis",
+                    "description": "The recommended minimum frequency for analysis - this may be empty if defaults should be used",
                     "type": "number"
                 },
                 "RecommendedStartTime": {
                     "description": "The  validated safe start time to set for downstream analyses to avoid data quality issues",
                     "type": "number"
                 },
                 "UID": {
@@ -2441,16 +2439,15 @@
                     "description": "The list of all detectors that should be analysed in downstream analyses",
                     "items": {
                         "$ref": "#/$defs/DetcharDetector"
                     },
                     "type": "array"
                 },
                 "RecommendedDuration": {
-                    "default": 4.0,
-                    "description": "The  validated safe maximum time duration to set for downstream analyses to avoid data quality issues",
+                    "description": "The  validated safe maximum time duration to set for downstream analyses to avoid data quality issues - this may be empty if defaults should be used",
                     "type": "number"
                 },
                 "Reviewers": {
                     "description": "The names of all reviewers involved",
                     "items": {
                         "type": "string"
                     },
```

### Comparing `cbcflow-0.1.2a1/src/cbcflow/schema/index-v1.schema` & `cbcflow-0.1.2a4/src/cbcflow/schema/index-v1.schema`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/schema.py` & `cbcflow-0.1.2a4/src/cbcflow/schema.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/src/cbcflow/utils.py` & `cbcflow-0.1.2a4/src/cbcflow/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 """Miscellaneous functions, especially relating to OS I/O"""
 import hashlib
 import os
 import subprocess
 from datetime import datetime
 from jsondiff import Symbol
+import logging
+
+logger = logging.getLogger(__name__)
 
 
 def standardize_list(inlist: list) -> list:
     """Creates a list sorted in a standard way
 
     Parameters
     ==========
@@ -149,7 +152,26 @@
         else:
             val_to_write = val
         if isinstance(key, Symbol):
             string_rep_diff[key.label] = val_to_write
         else:
             string_rep_diff[key] = val_to_write
     return string_rep_diff
+
+
+def get_url_from_public_html_dir(dirpath):
+    """Given a path to a directory in public_html, get the corresponding URL (on CIT)"""
+    if dirpath.split("/")[2] == "public_html":
+        # This is the case where files are being written directly into public html
+        # First get the stuff that comes after public_html - this structure will stay the same
+        url_extension = "/".join(dirpath.split("/")[3:])
+        # next get the user in ldas form
+        url_user = f"~{dirpath.split('/')}"
+        # Combine them
+        dir_url = f"https://ldas-jobs.ligo.caltech.edu/\
+            {url_user}/{url_extension}"
+        return dir_url
+    else:
+        logger.info(
+            "Given directory path was not in public HTML, so URL cannot be extrapolated from it"
+        )
+        return None
```

### Comparing `cbcflow-0.1.2a1/src/cbcflow.egg-info/PKG-INFO` & `cbcflow-0.1.2a4/src/cbcflow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cbcflow
-Version: 0.1.2a1
+Version: 0.1.2a4
 Summary: A package for enabling CBC analyses
 Home-page: https://git.ligo.org/cbc/meta-data
 Author: Gregory Ashton
 Author-email: Gregory Ashton <gregory.ashton@ligo.org>, Rhiannon Udall <rhiannon.udall@ligo.org>
 Project-URL: Homepage, https://git.ligo.org/cbc/projects/meta-data
 Project-URL: Bug Tracker, https://git.ligo.org/cbc/projects/meta-data/-/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cbcflow-0.1.2a1/src/cbcflow.egg-info/SOURCES.txt` & `cbcflow-0.1.2a4/src/cbcflow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -46,14 +46,15 @@
 docs/source/libraries_images/.ipynb_checkpoints/part_8-checkpoint.png
 examples/initial_example.md
 schema/cbc-meta-data-v1.schema
 schema/cbc-meta-data-v2.schema
 schema/index-v1.schema
 src/cbcflow/__init__.py
 src/cbcflow/_version.py
+src/cbcflow/asimov.py
 src/cbcflow/cbcflow.py
 src/cbcflow/configuration.py
 src/cbcflow/database.py
 src/cbcflow/gracedb.py
 src/cbcflow/metadata.py
 src/cbcflow/monitor.py
 src/cbcflow/parser.py
```

### Comparing `cbcflow-0.1.2a1/tests/files_for_testing/cbc-meta-data-example.json` & `cbcflow-0.1.2a4/tests/files_for_testing/cbc-meta-data-example.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/files_for_testing/update_json_1.json` & `cbcflow-0.1.2a4/tests/files_for_testing/update_json_1.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/files_for_testing/update_json_2.json` & `cbcflow-0.1.2a4/tests/files_for_testing/update_json_2.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_1.yaml` & `cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_1.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/files_for_testing/update_yaml_2.yaml` & `cbcflow-0.1.2a4/tests/files_for_testing/update_yaml_2.yaml`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230227hp-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230227hp-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230331e-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230331e-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230401h-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230401h-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230402dv-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230402dv-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230403ae-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230403ae-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230404hb-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230404hb-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/library_for_testing/S230404jc-cbc-metadata.json` & `cbcflow-0.1.2a4/tests/library_for_testing/S230404jc-cbc-metadata.json`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/test_database.py` & `cbcflow-0.1.2a4/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/test_metadata.py` & `cbcflow-0.1.2a4/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/test_parser.py` & `cbcflow-0.1.2a4/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `cbcflow-0.1.2a1/tests/test_schema.py` & `cbcflow-0.1.2a4/tests/test_schema.py`

 * *Files identical despite different names*

