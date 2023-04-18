# Comparing `tmp/dm-cli-1.0.5.tar.gz` & `tmp/dm-cli-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dm-cli-1.0.5.tar", last modified: Tue Mar 28 13:06:31 2023, max compression
+gzip compressed data, was "dm-cli-1.0.6.tar", last modified: Tue Apr 18 12:27:02 2023, max compression
```

## Comparing `dm-cli-1.0.5.tar` & `dm-cli-1.0.6.tar`

### file list

```diff
@@ -1,78 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.590977 dm-cli-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-28 13:06:20.000000 dm-cli-1.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-03-28 13:06:31.590977 dm-cli-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-03-28 13:06:20.000000 dm-cli-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.582977 dm-cli-1.0.5/dm_cli/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.582977 dm-cli-1.0.5/dm_cli/bin/
--rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/bin/dm
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.582977 dm-cli-1.0.5/dm_cli/command_group/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/command_group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/command_group/data_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/command_group/entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.582977 dm-cli-1.0.5/dm_cli/dmss_api/
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.586977 dm-cli-1.0.5/dm_cli/dmss_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/access_control_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/blob_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/blueprint_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/datasource_api.py
--rw-r--r--   0 runner    (1001) docker     (123)   150478 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/document_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/entity_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/export_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/health_check_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/lookup_table_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/personal_access_token_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/reference_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/search_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api/whoami_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36779 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.586977 dm-cli-1.0.5/dm_cli/dmss_api/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/access_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/acl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/basic_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/data_source_information.py
--rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/data_source_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/error_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/get_blueprint_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/pat_data.py
--rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/recipe_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/repository.py
--rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/repository_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/storage_attribute.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/storage_data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model/storage_recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.586977 dm-cli-1.0.5/dm_cli/dmss_api/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/dmss_api/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4843 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/import_entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/import_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/package_tree_from_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.586977 dm-cli-1.0.5/dm_cli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/utils/file_structure.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/utils/reference.py
--rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-03-28 13:06:20.000000 dm-cli-1.0.5/dm_cli/utils/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 13:06:31.582977 dm-cli-1.0.5/dm_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-03-28 13:06:31.000000 dm-cli-1.0.5/dm_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-03-28 13:06:31.000000 dm-cli-1.0.5/dm_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 13:06:31.000000 dm-cli-1.0.5/dm_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-03-28 13:06:31.000000 dm-cli-1.0.5/dm_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-28 13:06:31.000000 dm-cli-1.0.5/dm_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 13:06:31.590977 dm-cli-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-03-28 13:06:20.000000 dm-cli-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.090595 dm-cli-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 12:26:54.000000 dm-cli-1.0.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-18 12:27:02.086595 dm-cli-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-04-18 12:26:54.000000 dm-cli-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.082594 dm-cli-1.0.6/dm_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.082594 dm-cli-1.0.6/dm_cli/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)     5086 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/bin/dm
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.082594 dm-cli-1.0.6/dm_cli/command_group/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/command_group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/command_group/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/command_group/entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.082594 dm-cli-1.0.6/dm_cli/dmss_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.086595 dm-cli-1.0.6/dm_cli/dmss_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11210 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/access_control_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10848 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/blob_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/blueprint_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/datasource_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)   150478 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41424 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/document_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10572 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/entity_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10327 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/export_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4791 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/health_check_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/lookup_table_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13725 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/personal_access_token_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/reference_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/search_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api/whoami_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36779 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17227 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5045 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.086595 dm-cli-1.0.6/dm_cli/dmss_api/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11914 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/access_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12095 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/acl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11231 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/basic_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/data_source_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11565 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/data_source_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11233 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12717 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/error_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12306 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/get_blueprint_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12255 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/pat_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13739 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13153 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/recipe_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11793 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13509 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12073 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/repository_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12604 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/storage_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/storage_data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12553 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model/storage_recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80128 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.086595 dm-cli-1.0.6/dm_cli/dmss_api/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12650 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/dmss_api/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4970 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3681 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/import_entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/import_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/package_tree_from_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.086595 dm-cli-1.0.6/dm_cli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/utils/file_structure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/utils/reference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2781 2023-04-18 12:26:54.000000 dm-cli-1.0.6/dm_cli/utils/zip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 12:27:02.082594 dm-cli-1.0.6/dm_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10525 2023-04-18 12:27:01.000000 dm-cli-1.0.6/dm_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-18 12:27:02.000000 dm-cli-1.0.6/dm_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 12:27:01.000000 dm-cli-1.0.6/dm_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-18 12:27:01.000000 dm-cli-1.0.6/dm_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-04-18 12:27:01.000000 dm-cli-1.0.6/dm_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      145 2023-04-18 12:26:54.000000 dm-cli-1.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 12:27:02.090595 dm-cli-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-04-18 12:26:54.000000 dm-cli-1.0.6/setup.py
```

### Comparing `dm-cli-1.0.5/PKG-INFO` & `dm-cli-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/equinor/dm-cli
 Author: 
 Author-email: 
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/dm-cli)](https://pypi.org/project/dm-cli)
         [![PyPi downloads](https://img.shields.io/pypi/dm/dm-cli)](https://pypi.org/project/dm-cli)
```

### Comparing `dm-cli-1.0.5/README.md` & `dm-cli-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/bin/dm` & `dm-cli-1.0.6/dm_cli/bin/dm`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/command_group/data_source.py` & `dm-cli-1.0.6/dm_cli/command_group/data_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         raise FileNotFoundError(f"The path '{path}' is not a file.")
 
     print(f"IMPORTING DATA SOURCE '{data_source_path.name}'")
 
     # Read the data source definition
     with open(data_source_path) as file:
         document = json.load(file)
+        existing_data_sources = dmss_exception_wrapper(dmss_api.data_source_get_all)
+        if any(existing_document["name"] == document["name"] for existing_document in existing_data_sources):
+            print(f"WARNING: data source {document['name']} already exists. Updating existing data source.")
 
         dmss_exception_wrapper(dmss_api.data_source_save, document["name"], document)
         print(f"\tImported data source '{document['name']}' ✓")
 
 
 @data_source_app.command("import-all", help="Import all datasources found in the directory given by 'path'")
 def import_all_data_sources(path: Path):
```

### Comparing `dm-cli-1.0.5/dm_cli/command_group/entities.py` & `dm-cli-1.0.6/dm_cli/command_group/entities.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
             for file in source_path.iterdir():
                 if file.is_file():
                     dmss_exception_wrapper(import_single_entity, file, destination)
                     continue
                 dmss_exception_wrapper(import_folder_entity, file, destination)
             return True
         print(f"Importing PACKAGE '{source}' --> '{destination}'")
-        dmss_exception_wrapper(import_folder_entity, source, destination)
+        dmss_exception_wrapper(import_folder_entity, source_path, destination)
         return True
     else:
         dmss_exception_wrapper(import_single_entity, source_path, destination)
         return True
 
 
 @entities_app.command("delete")
```

### Comparing `dm-cli-1.0.5/dm_cli/dmss.py` & `dm-cli-1.0.6/dm_cli/dmss.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/__init__.py` & `dm-cli-1.0.6/dm_cli/dmss_api/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/access_control_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/access_control_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/blob_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/blob_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/blueprint_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/blueprint_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/datasource_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/datasource_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/default_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/default_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/document_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/document_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/entity_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/entity_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/export_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/export_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/health_check_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/health_check_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/lookup_table_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/lookup_table_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/personal_access_token_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/personal_access_token_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/reference_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/reference_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/search_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/search_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api/whoami_api.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api/whoami_api.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/api_client.py` & `dm-cli-1.0.6/dm_cli/dmss_api/api_client.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/configuration.py` & `dm-cli-1.0.6/dm_cli/dmss_api/configuration.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/exceptions.py` & `dm-cli-1.0.6/dm_cli/dmss_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/access_level.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/access_level.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/acl.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/acl.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/basic_entity.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/basic_entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/data_source_information.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/data_source_information.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/data_source_request.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/data_source_request.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/entity.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/error_response.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/error_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/get_blueprint_response.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/get_blueprint_response.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/lookup.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/lookup.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/pat_data.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/pat_data.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/recipe.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/recipe.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/recipe_attribute.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/recipe_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/reference.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/reference.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/repository.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/repository.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/repository_type.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/repository_type.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/storage_attribute.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/storage_attribute.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/storage_data_types.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/storage_data_types.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model/storage_recipe.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model/storage_recipe.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/model_utils.py` & `dm-cli-1.0.6/dm_cli/dmss_api/model_utils.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/models/__init__.py` & `dm-cli-1.0.6/dm_cli/dmss_api/models/__init__.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/dmss_api/rest.py` & `dm-cli-1.0.6/dm_cli/dmss_api/rest.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/domain.py` & `dm-cli-1.0.6/dm_cli/domain.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,33 +88,35 @@
 
     def _content_to_ref_dict(self):
         result = []
         for child in self.content:
             if isinstance(child, Package):
                 result.append(
                     {
-                        "_id": str(child.uid),
-                        "name": child.name,
-                        "type": SIMOS.PACKAGE.value,
-                        "contained": True,
+                        "ref": str(child.uid),
+                        "targetName": child.name,
+                        "targetType": SIMOS.PACKAGE.value,
+                        "type": "dmss://system/SIMOS/Link",
                     }
                 )
             else:  # Assume the child is a dict
                 if "name" in child:
                     result.append(
                         {
-                            "_id": child["_id"],
-                            "name": child["name"],
-                            "type": child["type"],
-                            "contained": True,
+                            "ref": child["_id"],
+                            "targetName": child["name"],
+                            "targetType": child["type"],
+                            "type": "dmss://system/SIMOS/Link",
                         }
                     )
 
                 else:
-                    result.append({"_id": child["_id"], "type": child["type"], "contained": True})
+                    result.append(
+                        {"ref": child["_id"], "targetType": child["type"], "type": "dmss://system/SIMOS/Link"}
+                    )
         return result
 
 
 TDependencyProtocol = NewType("TDependencyProtocol", Literal["dmss", "http"])
 
 
 @dataclass(frozen=True)
```

### Comparing `dm-cli-1.0.5/dm_cli/enums.py` & `dm-cli-1.0.6/dm_cli/enums.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/import_entity.py` & `dm-cli-1.0.6/dm_cli/import_entity.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/import_package.py` & `dm-cli-1.0.6/dm_cli/import_package.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/package_tree_from_zip.py` & `dm-cli-1.0.6/dm_cli/package_tree_from_zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/utils/file_structure.py` & `dm-cli-1.0.6/dm_cli/utils/file_structure.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/utils/reference.py` & `dm-cli-1.0.6/dm_cli/utils/reference.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli/utils/utils.py` & `dm-cli-1.0.6/dm_cli/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import io
 import json
+import pprint
 from pathlib import Path
 from typing import Dict, List
 from uuid import uuid4
 
+import typer
 from rich import print
 from rich.console import Console
 
 from dm_cli.dmss import ApplicationException, dmss_api
 from dm_cli.dmss_api.exceptions import ApiException, NotFoundException
 
 from ..domain import Dependency, Package
@@ -116,18 +118,18 @@
 
 
 def ensure_package_structure(path: Path):
     """Create any missing packages in the provided path (mkdir -R)"""
     try:
         dmss_api.document_get_by_path(f"dmss://{path}")
     except NotFoundException as e:
-        # error = json.loads(e.body)
-        # if str(f"'{path}'") not in error["message"]:
-        #     print(f"Target package '{path}' is likely corrupt!")
-        #     print(f"\n\t{pprint.pprint(error)}")
-        #     raise typer.Exit(code=1)
+        error = json.loads(e.body)
+        if str(f"{path}") not in error["message"]:
+            print(f"Target package '{path}' is likely corrupt!")
+            pprint.pformat(error)
+            raise typer.Exit(code=1)
 
         if len(path.parts) > 2:  # We're at root package level. Do not check for datasource.
             ensure_package_structure(path.parent)
 
         add_package_to_path(path.name, path)
         print(f"Target folder '{path.name}' was missing in '{path.parent}'. Created: ✓")
```

### Comparing `dm-cli-1.0.5/dm_cli/utils/zip.py` & `dm-cli-1.0.6/dm_cli/utils/zip.py`

 * *Files identical despite different names*

### Comparing `dm-cli-1.0.5/dm_cli.egg-info/PKG-INFO` & `dm-cli-1.0.6/dm_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dm-cli
-Version: 1.0.5
+Version: 1.0.6
 Summary: UNKNOWN
 Home-page: https://github.com/equinor/dm-cli
 Author: 
 Author-email: 
 License: MIT
 Description: [![PyPi version](https://img.shields.io/pypi/v/dm-cli)](https://pypi.org/project/dm-cli)
         [![PyPi downloads](https://img.shields.io/pypi/dm/dm-cli)](https://pypi.org/project/dm-cli)
```

### Comparing `dm-cli-1.0.5/dm_cli.egg-info/SOURCES.txt` & `dm-cli-1.0.6/dm_cli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.md
+requirements.txt
 setup.py
 dm_cli/__init__.py
 dm_cli/dmss.py
 dm_cli/domain.py
 dm_cli/enums.py
 dm_cli/import_entity.py
 dm_cli/import_package.py
```

### Comparing `dm-cli-1.0.5/setup.py` & `dm-cli-1.0.6/setup.py`

 * *Files identical despite different names*

