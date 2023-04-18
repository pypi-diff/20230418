# Comparing `tmp/oarepo-oai-pmh-harvester-4.0.4.tar.gz` & `tmp/oarepo-oai-pmh-harvester-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-oai-pmh-harvester-4.0.4.tar", last modified: Mon Mar 27 05:58:45 2023, max compression
+gzip compressed data, was "oarepo-oai-pmh-harvester-4.0.5.tar", last modified: Tue Apr 18 08:51:55 2023, max compression
```

## Comparing `oarepo-oai-pmh-harvester-4.0.4.tar` & `oarepo-oai-pmh-harvester-4.0.5.tar`

### file list

```diff
@@ -1,212 +1,212 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.997628 oarepo-oai-pmh-harvester-4.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-27 05:58:44.997628 oarepo-oai-pmh-harvester-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.977627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-03-27 05:58:44.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-03-27 05:58:44.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-27 05:58:44.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-03-27 05:58:44.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-03-27 05:58:44.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-27 05:58:44.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/alembic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/alembic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/alembic/cecc281d2938_create_oarepo_oaipmh_harvester_branch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/harvester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.981627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.985627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.989627 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/ext.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29797 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/models/model.json
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.993628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/facets.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/views.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/proxies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.997628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/readers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/readers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/readers/oai_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/readers/sickle.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.997628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/marcxml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1991 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/uow.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-27 05:58:44.997628 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/writers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/writers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/writers/oai.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/writers/oai_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-03-27 05:58:44.997628 oarepo-oai-pmh-harvester-4.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-27 05:57:34.000000 oarepo-oai-pmh-harvester-4.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.607518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8882 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 08:51:55.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.607518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.607518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14686 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/cecc281d2938_create_oarepo_oaipmh_harvester_branch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5037 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3339 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/harvester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21210 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.611518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17053 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1609 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.615518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20531 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/ext.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29797 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/model.json
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.619518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/facets.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/proxies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/oai_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/sickle.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/marcxml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/uow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10153 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-18 08:51:55.623518 oarepo-oai-pmh-harvester-4.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:50:42.000000 oarepo-oai-pmh-harvester-4.0.5/setup.py
```

### Comparing `oarepo-oai-pmh-harvester-4.0.4/PKG-INFO` & `oarepo-oai-pmh-harvester-4.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-oai-pmh-harvester
-Version: 4.0.4
+Version: 4.0.5
 Summary: OAIPMH harvester
 Description-Content-Type: text/markdown
 
 # OARepo OAI-PMH harvester
 
 An OAI-PMH harvesing library for Invenio 3.5+. The library provides initial transformation 
 of OAI-PMH payload to an intermediary json representation which is later on transformed by
```

### Comparing `oarepo-oai-pmh-harvester-4.0.4/README.md` & `oarepo-oai-pmh-harvester-4.0.5/README.md`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/PKG-INFO` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-oai-pmh-harvester
-Version: 4.0.4
+Version: 4.0.5
 Summary: OAIPMH harvester
 Description-Content-Type: text/markdown
 
 # OARepo OAI-PMH harvester
 
 An OAI-PMH harvesing library for Invenio 3.5+. The library provides initial transformation 
 of OAI-PMH payload to an intermediary json representation which is later on transformed by
```

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oai_pmh_harvester.egg-info/entry_points.txt` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oai_pmh_harvester.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/alembic/b2a45c3a744e_initial_revision.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/cli.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/cli.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/ext.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/harvester.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/harvester.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/ext.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/models/model.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/models/model.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/api.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/jsonschemas/oai_batch-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/records/mappings/os-v2/oai_batch/oai_batch-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/services/records/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_batch/views.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_batch/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/ext.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/models/model.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/models/model.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/api.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/jsonschemas/oai_harvester-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/records/mappings/os-v2/oai_harvester/oai_harvester-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/facets.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/services/records/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_harvester/views.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_harvester/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/ext.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/models/model.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/models/model.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/api.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/jsonschemas/oai_record-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/records/mappings/os-v2/oai_record/oai_record-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/facets.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/services/records/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_record/views.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_record/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/ext.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/ext.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/models/model.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/models/model.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/api.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/api.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/jsonschemas/oai_run-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/records/mappings/os-v2/oai_run/oai_run-1.0.0.json`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/resources/records/ui.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/config.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/config.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/facets.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/facets.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/search.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/search.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/services/records/ui_schema.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/oai_run/views.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/oai_run/views.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/permissions.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/permissions.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/readers/oai_dir.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/oai_dir.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/readers/sickle.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/readers/sickle.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/batch.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/batch.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/marcxml.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/marcxml.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/transformers/rule.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/transformers/rule.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/uow.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/uow.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from flask import current_app
 from invenio_records_resources.services.uow import RecordCommitOp, UnitOfWork
 from opensearchpy.helpers import bulk
 from opensearchpy.helpers import expand_action as default_expand_action
 
+from oarepo_runtime.relations.uow import CachingUnitOfWork
+
 
 class BulkRecordCommitOp(RecordCommitOp):
     def __init__(self, rc: RecordCommitOp):
         super().__init__(rc._record, rc._indexer, rc._index_refresh)
         self._previous = rc
 
     def on_register(self, uow):
@@ -29,15 +31,15 @@
             "_version_type": self._indexer._version_type,
             "_source": body,
         }
         action.update(arguments)
         return action
 
 
-class BulkUnitOfWork(UnitOfWork):
+class BulkUnitOfWork(CachingUnitOfWork):
     def register(self, op):
         if isinstance(op, RecordCommitOp):
             op = BulkRecordCommitOp(op)
         return super().register(op)
 
     def commit(self):
         super().commit()
```

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/utils.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/utils.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/writers/oai.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,17 +113,19 @@
     def read_oai_records(self, batch):
         oai_records = {
             x["oai_identifier"]: x
             for x in list(
                 record_service.scan(
                     self._identity,
                     params={
-                        "oai_identifier": [
-                            e.context["oai"]["identifier"] for e in batch.entries
-                        ]
+                        "facets": {
+                            "oai_identifier": [
+                                e.context["oai"]["identifier"] for e in batch.entries
+                            ]
+                        }
                     },
                 )
             )
         }
         for e in batch.entries:
             oai_rec = oai_records.get(e.context["oai"]["identifier"])
             if oai_rec and oai_rec.get("local_identifier"):
@@ -135,17 +137,19 @@
     def create_oai_records(self, batch, uow):
         oai_records = {
             x["oai_identifier"]: x
             for x in list(
                 record_service.scan(
                     self._identity,
                     params={
-                        "oai_identifier": [
-                            e.context["oai"]["identifier"] for e in batch.entries
-                        ]
+                        "facets": {
+                            "oai_identifier": [
+                                e.context["oai"]["identifier"] for e in batch.entries
+                            ]
+                        }
                     },
                 )
             )
         }
         for e in batch.entries:
             oai_rec = oai_records.get(e.context["oai"]["identifier"])
             if oai_rec:
@@ -231,13 +235,13 @@
                         )
         return batch
 
     def delete_entry(self, entry, uow):
         oai_record = list(
             record_service.scan(
                 self._identity,
-                params={"oai_identifier": [entry.context["oai"]["identifier"]]},
+                params={"facets": {"oai_identifier": [entry.context["oai"]["identifier"]]}},
             )
         )
         if oai_record and "local_identifier" in oai_record[0]:
             entry.entry["id"] = oai_record[0]["local_identifier"]
             self.writer.delete(entry, uow=uow)
```

### Comparing `oarepo-oai-pmh-harvester-4.0.4/oarepo_oaipmh_harvester/writers/oai_dir.py` & `oarepo-oai-pmh-harvester-4.0.5/oarepo_oaipmh_harvester/writers/oai_dir.py`

 * *Files identical despite different names*

### Comparing `oarepo-oai-pmh-harvester-4.0.4/setup.cfg` & `oarepo-oai-pmh-harvester-4.0.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = oarepo-oai-pmh-harvester
-version = 4.0.4
+version = 4.0.5
 description = OAIPMH harvester
 authors = ["Alzbeta Pokorna <alzbeta.pokorna@cesnet.cz>", "Miroslav Simek <miroslav.simek@cesnet.cz>"]
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
```

