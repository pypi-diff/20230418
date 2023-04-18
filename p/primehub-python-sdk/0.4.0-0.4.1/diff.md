# Comparing `tmp/primehub-python-sdk-0.4.0.tar.gz` & `tmp/primehub-python-sdk-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "primehub-python-sdk-0.4.0.tar", last modified: Thu Mar  2 02:08:56 2023, max compression
+gzip compressed data, was "primehub-python-sdk-0.4.1.tar", last modified: Tue Apr 18 08:56:10 2023, max compression
```

## Comparing `primehub-python-sdk-0.4.0.tar` & `primehub-python-sdk-0.4.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.365917 primehub-python-sdk-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-03-02 02:08:56.365917 primehub-python-sdk-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.361916 primehub-python-sdk-0.4.0/primehub/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-02 02:08:46.000000 primehub-python-sdk-0.4.0/primehub/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32134 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_images.py
--rw-r--r--   0 runner    (1001) docker     (123)    16427 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_instancetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_reports.py
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11635 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_users.py
--rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/admin_volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/apptemplates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/deployments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.361916 primehub-python-sdk-0.4.0/primehub/extras/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/extras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/extras/devlab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/extras/doc_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/extras/e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/files.py
--rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/images.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/instancetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/me.py
--rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/notebooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/recurring_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/resource_operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.361916 primehub-python-sdk-0.4.0/primehub/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.365917 primehub-python-sdk-0.4.0/primehub/utils/argparser/
--rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/argparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/completion.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/optionals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/permission.py
--rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/utils/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/primehub/volumes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.365917 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-03-02 02:08:56.000000 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-03-02 02:08:56.000000 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 02:08:56.000000 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-02 02:08:56.000000 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-03-02 02:08:56.000000 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-03-02 02:08:56.000000 primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-02 02:08:56.365917 primehub-python-sdk-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 02:08:56.365917 primehub-python-sdk-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/graphql_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_admin_groups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_admin_images.py
--rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_admin_instancetypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_admin_users.py
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_cli_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_cmd_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_cmd_me.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_graphql_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_group_resource_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_http_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_implementation_in_source_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_output_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_print.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_recurring_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_sdk_to_admin_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_sdk_to_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_sdk_to_cli_module_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_validator_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-03-02 02:08:15.000000 primehub-python-sdk-0.4.0/tests/test_volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.754494 primehub-python-sdk-0.4.1/primehub/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-18 08:55:58.000000 primehub-python-sdk-0.4.1/primehub/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33979 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12069 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16381 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_instancetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_reports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11680 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15105 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/admin_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15498 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/apptemplates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12015 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8124 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13692 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/deployments.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.754494 primehub-python-sdk-0.4.1/primehub/extras/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3058 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/devlab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3777 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/doc_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/extras/e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14569 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10009 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/instancetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13874 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/me.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12715 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11516 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/recurring_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/resource_operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/primehub/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/primehub/utils/argparser/
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/argparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/completion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/optionals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/permission.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12638 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/utils/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/primehub/volumes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3791 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 08:56:10.000000 primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:56:10.758494 primehub-python-sdk-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/graphql_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9162 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_groups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3599 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_images.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8336 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_instancetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_admin_users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_cli_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_cmd_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_cmd_me.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13062 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3591 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_graphql_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_group_resource_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_http_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3361 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_implementation_in_source_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2585 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_output_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_print.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_recurring_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_sdk_to_admin_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8601 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_sdk_to_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_sdk_to_cli_module_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_validator_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-04-18 08:55:23.000000 primehub-python-sdk-0.4.1/tests/test_volumes.py
```

### Comparing `primehub-python-sdk-0.4.0/LICENSE` & `primehub-python-sdk-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/PKG-INFO` & `primehub-python-sdk-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primehub-python-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: PrimeHub Python SDK
 Home-page: https://github.com/InfuseAI/primehub-python-sdk
 Author: qrtt1
 Author-email: qrtt1@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/primehub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `primehub-python-sdk-0.4.0/README.md` & `primehub-python-sdk-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/__init__.py` & `primehub-python-sdk-0.4.1/primehub/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_groups.py` & `primehub-python-sdk-0.4.1/primehub/admin_groups.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,30 @@
 from typing import Dict, Iterator, List, Union, Any
 
 from primehub import HTTPSupport, Helpful, Module, cmd, primehub_load_config
 from primehub.utils import PrimeHubException
 from primehub.utils.optionals import file_flag, toggle_flag
 from primehub.utils.validator import validate_connection
 
+group_basic_info = """
+fragment GroupBasicInfo on Group {
+  id
+  displayName
+  name
+  admins
+  quotaCpu
+  quotaGpu
+  quotaMemory
+  projectQuotaCpu
+  projectQuotaGpu
+  projectQuotaMemory
+  sharedVolumeCapacity
+}
+"""
+
 
 def invalid_config(message: str):
     example = """
     {"name": "group_name", "displayName": "", "enabledDeployment": false, "enabledSharedVolume": false,
     "quotaCpu": 0.5, "quotaGpu": 0, "quotaMemory": null, "projectQuotaCpu": null, "projectQuotaGpu": null,
     "projectQuotaMemory": null, "admins": "", "users": {"connect": [{"id": "user1_id"}, {"id": "user2_id"}]}}
     """.strip()
@@ -207,15 +223,15 @@
         :return The volume
         """
 
         # assign the connected group
         config['global'] = False
         config['groups'] = dict(connect=[dict(id=group_id, writable=writable)])
 
-        return self.primehub.admin_volumes.create(config)
+        return self.primehub.admin.admin_volumes.create(config)
 
     @cmd(name='disconnect-volume', description='Make the volume leave the group')
     def disconnect_volume(self, group_id: str, volume_id: str) -> Dict:
         """
         Make the volume leave the group
 
         :type group_id: str
@@ -293,15 +309,15 @@
 
         :type group_id: str
         :param group_id: The group id
 
         :rtype list
         :return volumes list
         """
-        results = self.primehub.admin_groups.get(group_id)
+        results = self.primehub.admin.admin_groups.get(group_id)
         if 'id' not in results or 'volumes' not in results:
             return results
         return results['volumes']
 
 
 class AdminGroupsInstanceTypes(HTTPSupport):
 
@@ -342,15 +358,15 @@
         :return The instanceType
         """
 
         # assign the connected group
         config['global'] = False
         config['groups'] = dict(connect=[dict(id=group_id)])
 
-        return self.primehub.admin_instancetypes.create(config)
+        return self.primehub.admin.admin_instancetypes.create(config)
 
     @cmd(name='disconnect-instancetype', description='Make the instanceType leave the group')
     def disconnect_instancetype(self, group_id: str, instancetype_id: str) -> Dict:
         """
         Make the instanceType leave the group
 
         :type group_id: str
@@ -435,15 +451,15 @@
 
         :type group_id: str
         :param group_id: The group id
 
         :rtype list
         :return instance-type list
         """
-        results = self.primehub.admin_groups.get(group_id)
+        results = self.primehub.admin.admin_groups.get(group_id)
         if 'id' not in results or 'instanceTypes' not in results:
             return results
         return results['instanceTypes']
 
 
 class AdminGroupsImages(HTTPSupport):
 
@@ -483,15 +499,15 @@
         :return The image
         """
 
         # assign the connected group
         config['global'] = False
         config['groups'] = dict(connect=[dict(id=group_id)])
 
-        return self.primehub.admin_images.create(config)
+        return self.primehub.admin.admin_images.create(config)
 
     @cmd(name='disconnect-image', description='Make the image leave the group')
     def disconnect_image(self, group_id: str, image_id: str) -> Dict:
         """
         Make the image leave the group
 
         :type group_id: str
@@ -598,15 +614,15 @@
 
         :type group_id: str
         :param group_id: The group id
 
         :rtype list
         :return image list
         """
-        results = self.primehub.admin_groups.get(group_id)
+        results = self.primehub.admin.admin_groups.get(group_id)
         if 'id' not in results or 'images' not in results:
             return results
         return results['images']
 
 
 class AdminGroupsUsers(HTTPSupport):
 
@@ -762,15 +778,15 @@
                 u['group_admin'] = True
             else:
                 u['group_admin'] = False
 
         return users
 
     def _make_group_admins(self, group_id: str, user_id: str, added: bool):
-        user_dict = self.primehub.admin_users.get(user_id)
+        user_dict = self.primehub.admin.admin_users.get(user_id)
         username = None
         if 'id' in user_dict and 'username' in user_dict:
             username = user_dict['username']
 
         if username is None:
             # it is not possible to make a new list
             return None
@@ -840,26 +856,30 @@
             ...GroupBasicInfo
           }
         }
         fragment GroupBasicInfo on Group {
           id
           displayName
           name
-          admins
           quotaCpu
           quotaGpu
           quotaMemory
           projectQuotaCpu
           projectQuotaGpu
           projectQuotaMemory
           sharedVolumeCapacity
         }
-        """
+        """ + group_basic_info
 
         apply_auto_fill(config)
+
+        # cannot specify admins when creating
+        if config.get('admins'):
+            config['admins'] = ''
+
         results = self.request({'data': validate(config)}, query)
 
         if 'data' not in results:
             return results
         return results['data']['createGroup']
 
     @cmd(name='list', description='List groups', return_required=True, optionals=[('page', int)])
@@ -889,28 +909,15 @@
             }
             pageInfo {
               currentPage
               totalPage
             }
           }
         }
-        fragment GroupBasicInfo on Group {
-          id
-          displayName
-          name
-          admins
-          quotaCpu
-          quotaGpu
-          quotaMemory
-          projectQuotaCpu
-          projectQuotaGpu
-          projectQuotaMemory
-          sharedVolumeCapacity
-        }
-        """
+        """ + group_basic_info
 
         variables: dict = {'orderBy': {}, 'where': {}}
         page = kwargs.get('page', 0)
         if page > 0:
             variables['page'] = page
             results = self.request(variables, query)
             for e in results['data']['group']['edges']:
@@ -1008,18 +1015,21 @@
 
         variables = {'where': {'id': id}, 'everyoneGroupWhere': {
             'id': self._everyone_group_id()}}
         results = self.request(variables, query)
 
         if 'data' not in results:
             return results
-
-        results['data']['group']['volumes'] = results['data']['group'].pop('datasets', '[]')
-
-        return results['data']['group']
+        group = results['data']['group']
+        if not group:
+            return group
+
+        group['volumes'] = group.pop('datasets', '[]')
+        self._output_format_admins(id, group)
+        return group
 
     def _everyone_group_id(self) -> dict:
         query = """
         query {
           me {
             groups {
               id
@@ -1066,39 +1076,48 @@
         :param config: the configurations for the updated group
 
         :rtype: dict
         :return: the group
         """
 
         query = """
-        mutation UpdateGroup($data: GroupUpdateInput!, $where: GroupWhereUniqueInput!) {
+        mutation UpdateGroup(
+          $data: GroupUpdateInput!,
+          $where: GroupWhereUniqueInput!
+        ) {
           updateGroup(data: $data, where: $where) {
             ...GroupBasicInfo
           }
         }
-        fragment GroupBasicInfo on Group {
-          id
-          displayName
-          name
-          admins
-          quotaCpu
-          quotaGpu
-          quotaMemory
-          projectQuotaCpu
-          projectQuotaGpu
-          projectQuotaMemory
-          sharedVolumeCapacity
-        }
-        """
+        """ + group_basic_info
+
+        if config.get('admins'):
+            config['admins'] = self._transform_admins(id, config.get('admins', []))
+
         variables = {'where': {'id': id}, 'data': validate(config, True)}
         results = self.request(variables, query)
 
         if 'data' not in results:
             return results
-        return results['data']['updateGroup']
+
+        updated_query = """
+        query Group(
+          $where: GroupWhereUniqueInput!
+        ) {
+          group(where: $where) {
+            ...GroupBasicInfo
+          }
+        }
+        """ + group_basic_info
+        updated_results = self.request({'where': {'id': id}}, updated_query)
+        if 'data' not in updated_results:
+            return updated_results
+        updated_group = updated_results['data']['group']
+        self._output_format_admins(id, updated_group)
+        return updated_group
 
     @cmd(name='delete', description='Delete the group by id', return_required=True)
     def delete(self, id: str) -> dict:
         """
         Delete the group by id
 
         :type id: str
@@ -1117,9 +1136,46 @@
         """
 
         results = self.request({'where': {'id': id}}, query)
         if 'data' not in results:
             return results
         return results['data']['deleteGroup']
 
+    def _transform_admins(self, id: str, user_ids: List[str]):
+        if len(user_ids) == 0:
+            return ''
+
+        member_dict = {}
+        users = self.primehub.admin.admin_groups.list_users(id)
+        for user in users:
+            user_id = user['id']
+            username = user['username']
+            member_dict[user_id] = username
+
+        admin_usernames = []
+        invalid_user_ids = []
+        for user_id in user_ids:
+            if user_id in member_dict:
+                admin_usernames.append(member_dict[user_id])
+            else:
+                invalid_user_ids.append(user_id)
+
+        if len(invalid_user_ids) > 0:
+            _invalid_ids = ', '.join(invalid_user_ids)
+            msg = f'admins contain invalid user ids: {_invalid_ids}'
+            raise PrimeHubException(msg)
+        return ','.join(admin_usernames)
+
+    def _output_format_admins(self, id: str, group: dict):
+        admin_users = []
+        admin_usernames = group.get('admins', '').split(',')
+        users = self.primehub.admin.admin_groups.list_users(id)
+        for user in users:
+            if user['username'] in admin_usernames:
+                admin_users.append(dict(
+                    id=user['id'],
+                    username=user['username']
+                ))
+        group['admins'] = admin_users
+
     def help_description(self):
         return "Manage groups"
```

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_images.py` & `primehub-python-sdk-0.4.1/primehub/admin_images.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Iterator
 
 from primehub import Helpful, Module, cmd, primehub_load_config
 from primehub.utils import PrimeHubException, resource_not_found
 from primehub.utils.optionals import file_flag
-from primehub.utils.validator import validate_name, validate_groups, validate_group_exists
+from primehub.utils.validator import validate_name, validate_group_exists
 
 
 def _error_handler(response):
     import re
 
     if 'errors' in response:
         message = [x for x in response['errors'] if 'message' in x]
@@ -386,15 +386,14 @@
 
 def validate(payload: dict, for_update=False):
     if not for_update:
         validate_name(payload)
 
     validate_image_type(payload)
     validate_image_spec(payload)
-    validate_groups(payload)
 
     return payload
 
 
 def validate_image_spec(payload):
     image_spec: dict = payload.get('imageSpec', None)
     if image_spec is None:
```

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_instancetypes.py` & `primehub-python-sdk-0.4.1/primehub/admin_instancetypes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 from typing import Iterator, Dict, Any
 
 from primehub import Helpful, Module, cmd, primehub_load_config
 from primehub.utils import PrimeHubException, resource_not_found
 from primehub.utils.optionals import file_flag
-from primehub.utils.validator import validate_name, validate_groups, validate_group_exists
+from primehub.utils.validator import validate_name, validate_group_exists
 
 NODE_SELECTOR_KEY_LEN_ERROR = 'nodeSelector: len(key) should be less or equal to 63'
 NODE_SELECTOR_KV_TYPE_ERROR = 'nodeSelector: key and value must be a string'
 
 TOLERATION_EFFECT_ERROR = 'toleration: effect should be one of the ' \
                           '{NoSchedule, PreferNoSchedule and NoExecute}'
 
@@ -405,15 +405,14 @@
 def required_str_lengths_3_63(field):
     return f'{field} value must a string and len(value) between 3 and 63'
 
 
 def validate(payload: dict, for_update=False):
     if not for_update:
         validate_name(payload)
-    validate_groups(payload)
 
     validate_cpu_fields(payload)
     validate_memory_fields(payload)
     validate_gpu_field(payload)
     validate_tolerations_field(payload)
     validate_node_selector_field(payload)
```

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_reports.py` & `primehub-python-sdk-0.4.1/primehub/admin_reports.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_secrets.py` & `primehub-python-sdk-0.4.1/primehub/admin_secrets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_users.py` & `primehub-python-sdk-0.4.1/primehub/admin_users.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,14 +348,16 @@
         }
         """
 
         results = self.request({'where': {'id': id}}, query)
         if 'data' not in results:
             return results
         user = results['data']['user']
+        if not user:
+            return user
 
         # hide the everyone group
         groups = user['groups']
         user['groups'] = [x for x in groups if x['name'] != 'everyone']
         return user
 
     @cmd(name='delete', description='Delete an user by id', return_required=True)
```

### Comparing `primehub-python-sdk-0.4.0/primehub/admin_volumes.py` & `primehub-python-sdk-0.4.1/primehub/admin_volumes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/apps.py` & `primehub-python-sdk-0.4.1/primehub/apps.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/apptemplates.py` & `primehub-python-sdk-0.4.1/primehub/apptemplates.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/cli.py` & `primehub-python-sdk-0.4.1/primehub/cli.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/config.py` & `primehub-python-sdk-0.4.1/primehub/config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/datasets.py` & `primehub-python-sdk-0.4.1/primehub/datasets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/deployments.py` & `primehub-python-sdk-0.4.1/primehub/deployments.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/extras/devlab.py` & `primehub-python-sdk-0.4.1/primehub/extras/devlab.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/extras/doc_generator.py` & `primehub-python-sdk-0.4.1/primehub/extras/doc_generator.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/extras/e2e.py` & `primehub-python-sdk-0.4.1/primehub/extras/e2e.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/files.py` & `primehub-python-sdk-0.4.1/primehub/files.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/groups.py` & `primehub-python-sdk-0.4.1/primehub/groups.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/images.py` & `primehub-python-sdk-0.4.1/primehub/images.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/info.py` & `primehub-python-sdk-0.4.1/primehub/info.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/instancetypes.py` & `primehub-python-sdk-0.4.1/primehub/instancetypes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/jobs.py` & `primehub-python-sdk-0.4.1/primehub/jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/me.py` & `primehub-python-sdk-0.4.1/primehub/me.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/models.py` & `primehub-python-sdk-0.4.1/primehub/models.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/notebooks.py` & `primehub-python-sdk-0.4.1/primehub/notebooks.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/recurring_jobs.py` & `primehub-python-sdk-0.4.1/primehub/recurring_jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/resource_operations.py` & `primehub-python-sdk-0.4.1/primehub/resource_operations.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/secrets.py` & `primehub-python-sdk-0.4.1/primehub/secrets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/__init__.py` & `primehub-python-sdk-0.4.1/primehub/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/argparser/__init__.py` & `primehub-python-sdk-0.4.1/primehub/utils/argparser/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/completion.py` & `primehub-python-sdk-0.4.1/primehub/utils/completion.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/core.py` & `primehub-python-sdk-0.4.1/primehub/utils/core.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/decorators.py` & `primehub-python-sdk-0.4.1/primehub/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/display.py` & `primehub-python-sdk-0.4.1/primehub/utils/display.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/http_client.py` & `primehub-python-sdk-0.4.1/primehub/utils/http_client.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/permission.py` & `primehub-python-sdk-0.4.1/primehub/utils/permission.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/utils/validator.py` & `primehub-python-sdk-0.4.1/primehub/utils/validator.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub/volumes.py` & `primehub-python-sdk-0.4.1/primehub/volumes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/PKG-INFO` & `primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: primehub-python-sdk
-Version: 0.4.0
+Version: 0.4.1
 Summary: PrimeHub Python SDK
 Home-page: https://github.com/InfuseAI/primehub-python-sdk
 Author: qrtt1
 Author-email: qrtt1@infuseai.io
 Project-URL: Bug Tracker, https://github.com/InfuseAI/primehub/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `primehub-python-sdk-0.4.0/primehub_python_sdk.egg-info/SOURCES.txt` & `primehub-python-sdk-0.4.1/primehub_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/setup.py` & `primehub-python-sdk-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/__init__.py` & `primehub-python-sdk-0.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/graphql_formatter.py` & `primehub-python-sdk-0.4.1/tests/graphql_formatter.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_admin_groups.py` & `primehub-python-sdk-0.4.1/tests/test_admin_groups.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_admin_images.py` & `primehub-python-sdk-0.4.1/tests/test_admin_images.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_admin_instancetypes.py` & `primehub-python-sdk-0.4.1/tests/test_admin_instancetypes.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_admin_users.py` & `primehub-python-sdk-0.4.1/tests/test_admin_users.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_cli_config.py` & `primehub-python-sdk-0.4.1/tests/test_cli_config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_cmd_config.py` & `primehub-python-sdk-0.4.1/tests/test_cmd_config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_cmd_me.py` & `primehub-python-sdk-0.4.1/tests/test_cmd_me.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_config.py` & `primehub-python-sdk-0.4.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_datasets.py` & `primehub-python-sdk-0.4.1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_files.py` & `primehub-python-sdk-0.4.1/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_graphql_lint.py` & `primehub-python-sdk-0.4.1/tests/test_graphql_lint.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_group_resource_operation.py` & `primehub-python-sdk-0.4.1/tests/test_group_resource_operation.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_http_utils.py` & `primehub-python-sdk-0.4.1/tests/test_http_utils.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_implementation_in_source_level.py` & `primehub-python-sdk-0.4.1/tests/test_implementation_in_source_level.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_jobs.py` & `primehub-python-sdk-0.4.1/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_print.py` & `primehub-python-sdk-0.4.1/tests/test_print.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_recurring_jobs.py` & `primehub-python-sdk-0.4.1/tests/test_recurring_jobs.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_sdk_to_admin_cli.py` & `primehub-python-sdk-0.4.1/tests/test_sdk_to_admin_cli.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_sdk_to_cli.py` & `primehub-python-sdk-0.4.1/tests/test_sdk_to_cli.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_sdk_to_cli_module_alias.py` & `primehub-python-sdk-0.4.1/tests/test_sdk_to_cli_module_alias.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_test_utils.py` & `primehub-python-sdk-0.4.1/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_validator_tools.py` & `primehub-python-sdk-0.4.1/tests/test_validator_tools.py`

 * *Files identical despite different names*

### Comparing `primehub-python-sdk-0.4.0/tests/test_volumes.py` & `primehub-python-sdk-0.4.1/tests/test_volumes.py`

 * *Files identical despite different names*

