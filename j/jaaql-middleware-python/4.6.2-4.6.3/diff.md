# Comparing `tmp/jaaql-middleware-python-4.6.2.tar.gz` & `tmp/jaaql-middleware-python-4.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaaql-middleware-python-4.6.2.tar", last modified: Tue Apr  4 18:06:14 2023, max compression
+gzip compressed data, was "jaaql-middleware-python-4.6.3.tar", last modified: Mon Apr 17 22:20:49 2023, max compression
```

## Comparing `jaaql-middleware-python-4.6.2.tar` & `jaaql-middleware-python-4.6.3.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.271120 jaaql-middleware-python-4.6.2/
--rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0      946 2023-04-04 18:06:14.271120 jaaql-middleware-python-4.6.2/PKG-INFO
--rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.194119 jaaql-middleware-python-4.6.2/jaaql/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.199118 jaaql-middleware-python-4.6.2/jaaql/config/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/config/__init__.py
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/config/config-docker.ini
--rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/config/config-test.ini
--rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/config/config.ini
--rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/config_constants.py
--rw-rw-rw-   0        0        0     4835 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.204118 jaaql-middleware-python-4.6.2/jaaql/db/
--rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.2/jaaql/db/__init__.py
--rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/db/db_interface.py
--rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/db/db_pg_interface.py
--rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/db/db_utils.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.209118 jaaql-middleware-python-4.6.2/jaaql/documentation/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/documentation/__init__.py
--rw-rw-rw-   0        0        0     6018 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/documentation/documentation_internal.py
--rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/documentation/documentation_public.py
--rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.2/jaaql/documentation/documentation_shared.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.214119 jaaql-middleware-python-4.6.2/jaaql/email/
--rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.2/jaaql/email/__init__.py
--rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/email/email_manager.py
--rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/email/email_manager_service.py
--rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/email/patch_ems.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.219118 jaaql-middleware-python-4.6.2/jaaql/exceptions/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/exceptions/__init__.py
--rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.2/jaaql/exceptions/custom_http_status.py
--rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.2/jaaql/exceptions/http_status_exception.py
--rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/exceptions/not_yet_implement_exception.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.222118 jaaql-middleware-python-4.6.2/jaaql/interpreter/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/interpreter/__init__.py
--rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/interpreter/interpret_jaaql.py
--rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/jaaql.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.226117 jaaql-middleware-python-4.6.2/jaaql/migrations/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/migrations/__init__.py
--rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.2/jaaql/migrations/migration_history.sql
--rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/migrations/migrations.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.241119 jaaql-middleware-python-4.6.2/jaaql/mvc/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/__init__.py
--rw-rw-rw-   0        0        0    30735 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/base_controller.py
--rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/base_model.py
--rw-rw-rw-   0        0        0     3392 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/controller.py
--rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/controller_interface.py
--rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/exception_queries.py
--rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/generated_queries.py
--rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/handmade_queries.py
--rw-rw-rw-   0        0        0    35749 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/model.py
--rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/model_interface.py
--rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/mvc/response.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.243119 jaaql-middleware-python-4.6.2/jaaql/openapi/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/openapi/__init__.py
--rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/openapi/swagger_documentation.py
--rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.2/jaaql/patch.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.251123 jaaql-middleware-python-4.6.2/jaaql/scripts/
--rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/01.install_domains.generated.sql
--rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/02.install_super_user.exceptions.sql
--rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/03.install_super_user.handwritten.sql
--rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
--rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/05.install_jaaql.exceptions.sql
--rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/06.install_jaaql.handwritten.sql
--rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.2/jaaql/scripts/swagger_template.html
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.255132 jaaql-middleware-python-4.6.2/jaaql/services/
--rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.2/jaaql/services/__init__.py
--rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/services/cached_canned_query_service.py
--rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.2/jaaql/services/patch_script_install.py
--rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/services/script_install.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.263119 jaaql-middleware-python-4.6.2/jaaql/utilities/
--rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/jaaql/utilities/__init__.py
--rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/utilities/crypt_utils.py
--rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/utilities/options.py
--rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/utilities/utils.py
--rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.2/jaaql/utilities/utils_no_project_imports.py
--rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.2/jaaql/utilities/vault.py
-drwxrwxrwx   0        0        0        0 2023-04-04 18:06:14.269118 jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/
--rw-rw-rw-   0        0        0      946 2023-04-04 18:06:14.000000 jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2023-04-04 18:06:14.000000 jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-04 18:06:14.000000 jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      315 2023-04-04 18:06:14.000000 jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-04 18:06:14.000000 jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-04 18:06:14.271120 jaaql-middleware-python-4.6.2/setup.cfg
--rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.633696 jaaql-middleware-python-4.6.3/
+-rw-rw-rw-   0        0        0    18134 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      946 2023-04-17 22:20:49.633696 jaaql-middleware-python-4.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0      453 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.569696 jaaql-middleware-python-4.6.3/jaaql/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.573695 jaaql-middleware-python-4.6.3/jaaql/config/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/config/__init__.py
+-rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config/config-docker.ini
+-rw-rw-rw-   0        0        0      253 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config/config-test.ini
+-rw-rw-rw-   0        0        0      291 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config/config.ini
+-rw-rw-rw-   0        0        0      470 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/config_constants.py
+-rw-rw-rw-   0        0        0     4835 2023-04-17 22:14:35.000000 jaaql-middleware-python-4.6.3/jaaql/constants.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.577696 jaaql-middleware-python-4.6.3/jaaql/db/
+-rw-rw-rw-   0        0        0        0 2022-05-19 20:40:08.000000 jaaql-middleware-python-4.6.3/jaaql/db/__init__.py
+-rw-rw-rw-   0        0        0     7043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/db/db_interface.py
+-rw-rw-rw-   0        0        0    11198 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/db/db_pg_interface.py
+-rw-rw-rw-   0        0        0     6545 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/db/db_utils.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.581695 jaaql-middleware-python-4.6.3/jaaql/documentation/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/__init__.py
+-rw-rw-rw-   0        0        0     6320 2023-04-06 12:25:17.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_internal.py
+-rw-rw-rw-   0        0        0     8192 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_public.py
+-rw-rw-rw-   0        0        0     3456 2023-04-04 18:02:26.000000 jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_shared.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.586696 jaaql-middleware-python-4.6.3/jaaql/email/
+-rw-rw-rw-   0        0        0        0 2022-05-05 10:44:50.000000 jaaql-middleware-python-4.6.3/jaaql/email/__init__.py
+-rw-rw-rw-   0        0        0     3687 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/email/email_manager.py
+-rw-rw-rw-   0        0        0    19242 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/email/email_manager_service.py
+-rw-rw-rw-   0        0        0      234 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/email/patch_ems.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.590696 jaaql-middleware-python-4.6.3/jaaql/exceptions/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      401 2022-04-17 07:42:21.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/custom_http_status.py
+-rw-rw-rw-   0        0        0      985 2022-05-20 15:36:28.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/http_status_exception.py
+-rw-rw-rw-   0        0        0      321 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/exceptions/not_yet_implement_exception.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.592695 jaaql-middleware-python-4.6.3/jaaql/interpreter/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/interpreter/__init__.py
+-rw-rw-rw-   0        0        0    23250 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/interpreter/interpret_jaaql.py
+-rw-rw-rw-   0        0        0     6003 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/jaaql.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.596696 jaaql-middleware-python-4.6.3/jaaql/migrations/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/migrations/__init__.py
+-rw-rw-rw-   0        0        0      683 2022-09-19 00:09:13.000000 jaaql-middleware-python-4.6.3/jaaql/migrations/migration_history.sql
+-rw-rw-rw-   0        0        0    10802 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/migrations/migrations.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.607695 jaaql-middleware-python-4.6.3/jaaql/mvc/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/__init__.py
+-rw-rw-rw-   0        0        0    31004 2023-04-17 22:16:44.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/base_controller.py
+-rw-rw-rw-   0        0        0    25344 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/base_model.py
+-rw-rw-rw-   0        0        0     3727 2023-04-17 22:18:42.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/controller.py
+-rw-rw-rw-   0        0        0      274 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/controller_interface.py
+-rw-rw-rw-   0        0        0     7494 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/exception_queries.py
+-rw-rw-rw-   0        0        0    43043 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/generated_queries.py
+-rw-rw-rw-   0        0        0      232 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/handmade_queries.py
+-rw-rw-rw-   0        0        0    41782 2023-04-17 22:17:20.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/model.py
+-rw-rw-rw-   0        0        0      257 2022-05-07 20:33:26.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/model_interface.py
+-rw-rw-rw-   0        0        0      209 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/mvc/response.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.608696 jaaql-middleware-python-4.6.3/jaaql/openapi/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/openapi/__init__.py
+-rw-rw-rw-   0        0        0    28797 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/openapi/swagger_documentation.py
+-rw-rw-rw-   0        0        0      149 2022-06-11 20:45:39.000000 jaaql-middleware-python-4.6.3/jaaql/patch.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.616695 jaaql-middleware-python-4.6.3/jaaql/scripts/
+-rw-rw-rw-   0        0        0     1379 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/01.install_domains.generated.sql
+-rw-rw-rw-   0        0        0      939 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/02.install_super_user.exceptions.sql
+-rw-rw-rw-   0        0        0     1859 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/03.install_super_user.handwritten.sql
+-rw-rw-rw-   0        0        0     7492 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql
+-rw-rw-rw-   0        0        0      324 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/05.install_jaaql.exceptions.sql
+-rw-rw-rw-   0        0        0      990 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/06.install_jaaql.handwritten.sql
+-rw-rw-rw-   0        0        0     4105 2023-02-12 10:12:32.000000 jaaql-middleware-python-4.6.3/jaaql/scripts/swagger_template.html
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.620695 jaaql-middleware-python-4.6.3/jaaql/services/
+-rw-rw-rw-   0        0        0        0 2022-07-10 13:56:37.000000 jaaql-middleware-python-4.6.3/jaaql/services/__init__.py
+-rw-rw-rw-   0        0        0     2688 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/services/cached_canned_query_service.py
+-rw-rw-rw-   0        0        0      293 2022-07-14 16:23:21.000000 jaaql-middleware-python-4.6.3/jaaql/services/patch_script_install.py
+-rw-rw-rw-   0        0        0     3247 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/services/script_install.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.627696 jaaql-middleware-python-4.6.3/jaaql/utilities/
+-rw-rw-rw-   0        0        0        0 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6698 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/crypt_utils.py
+-rw-rw-rw-   0        0        0     5603 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/options.py
+-rw-rw-rw-   0        0        0     4725 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/utils.py
+-rw-rw-rw-   0        0        0     2428 2023-03-30 14:44:38.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/utils_no_project_imports.py
+-rw-rw-rw-   0        0        0     2160 2022-05-22 11:21:40.000000 jaaql-middleware-python-4.6.3/jaaql/utilities/vault.py
+drwxrwxrwx   0        0        0        0 2023-04-17 22:20:49.632696 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/
+-rw-rw-rw-   0        0        0      946 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      315 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-04-17 22:20:49.000000 jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 22:20:49.633696 jaaql-middleware-python-4.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      893 2022-03-12 16:03:36.000000 jaaql-middleware-python-4.6.3/setup.py
```

### Comparing `jaaql-middleware-python-4.6.2/LICENSE.txt` & `jaaql-middleware-python-4.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/PKG-INFO` & `jaaql-middleware-python-4.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.2
+Version: 4.6.3
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql/constants.py` & `jaaql-middleware-python-4.6.3/jaaql/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,9 +143,9 @@
 USERNAME__anonymous = "anonymous"
 PASSWORD__anonymous = "jaaql_public_password"
 ROLE__jaaql = "jaaql"
 ROLE__postgres = "postgres"
 
 PROTOCOL__postgres = "postgresql://"
 
-VERSION = "4.6.2"
+VERSION = "4.6.3"
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql/db/db_interface.py` & `jaaql-middleware-python-4.6.3/jaaql/db/db_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/db/db_pg_interface.py` & `jaaql-middleware-python-4.6.3/jaaql/db/db_pg_interface.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/db/db_utils.py` & `jaaql-middleware-python-4.6.3/jaaql/db/db_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/documentation/documentation_internal.py` & `jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_internal.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,7 +151,18 @@
                 description="The password with which the dispatcher will authenticate",
                 arg_type=str,
                 example="pa55word"
             )
         ]
     )
 )
+
+DOCUMENTATION__prepare = SwaggerDocumentation(
+    tags="Prepare",
+    methods=SwaggerMethod(
+        name="Prepares queries",
+        description="Prepares a set of queries for an application",
+        method=REST__POST,
+        arguments=ARG_RESP__allow_all,
+        response=RES__allow_all
+    )
+)
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql/documentation/documentation_public.py` & `jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_public.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/documentation/documentation_shared.py` & `jaaql-middleware-python-4.6.3/jaaql/documentation/documentation_shared.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/email/email_manager.py` & `jaaql-middleware-python-4.6.3/jaaql/email/email_manager.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/email/email_manager_service.py` & `jaaql-middleware-python-4.6.3/jaaql/email/email_manager_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/exceptions/http_status_exception.py` & `jaaql-middleware-python-4.6.3/jaaql/exceptions/http_status_exception.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/interpreter/interpret_jaaql.py` & `jaaql-middleware-python-4.6.3/jaaql/interpreter/interpret_jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/jaaql.py` & `jaaql-middleware-python-4.6.3/jaaql/jaaql.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/migrations/migration_history.sql` & `jaaql-middleware-python-4.6.3/jaaql/migrations/migration_history.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/migrations/migrations.py` & `jaaql-middleware-python-4.6.3/jaaql/migrations/migrations.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/mvc/base_controller.py` & `jaaql-middleware-python-4.6.3/jaaql/mvc/base_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ARG__http_inputs = "http_inputs"
 ARG__account_id = "account_id"
 ARG__ip_address = "ip_address"
 ARG__response = "response"
 ARG__username = "username"
 ARG__profiler = "profiler"
 ARG__auth_token = "auth_token"
+ARG__auth_token_for_refresh = "auth_token_for_refresh"
 ARG__connection = "connection"
 ARG__is_the_anonymous_user = "is_the_anonymous_user"
 ARG__verification_hook = "verification_hook"
 ARG_START__connection = "connection__"
 ARG_START__jaaql_connection = "jaaql_" + ARG_START__connection
 
 CONTENT__encoding = "charset=utf-8"
@@ -480,14 +481,17 @@
                             supply_dict[ARG__response] = jaaql_resp
 
                         if ARG__auth_token in inspect.getfullargspec(view_func_local).args:
                             if not swagger_documentation.security:
                                 raise Exception(ERR__method_required_token)
                             supply_dict[ARG__auth_token] = request.headers.get(HEADER__security)
 
+                        if ARG__auth_token_for_refresh in inspect.getfullargspec(view_func_local).args:
+                            supply_dict[ARG__auth_token_for_refresh] = request.headers.get(HEADER__security)
+
                         if ARG__connection in inspect.getfullargspec(view_func_local).args:
                             if not swagger_documentation.security:
                                 raise Exception(ERR__method_required_connection)
                             supply_dict[ARG__connection] = self.model.create_interface_for_db(account_id, DB__jaaql)
 
                         if ARG__is_the_anonymous_user in inspect.getfullargspec(view_func_local).args:
                             if not swagger_documentation.security:
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql/mvc/base_model.py` & `jaaql-middleware-python-4.6.3/jaaql/mvc/base_model.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/mvc/controller.py` & `jaaql-middleware-python-4.6.3/jaaql/mvc/controller.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,16 +16,16 @@
     def create_app(self):
 
         @self.cors_route('/oauth/token', DOCUMENTATION__oauth_token)
         def fetch_oauth_token(http_inputs: dict, ip_address: str, response: JAAQLResponse):
             return self.model.get_auth_token(**http_inputs, ip_address=ip_address, response=response)
 
         @self.cors_route(ENDPOINT__refresh, DOCUMENTATION__oauth_refresh)
-        def refresh_oauth_token(auth_token: str, ip_address: str):
-            return self.model.refresh_auth_token(auth_token, ip_address)
+        def refresh_oauth_token(auth_token_for_refresh: str, ip_address: str):
+            return self.model.refresh_auth_token(auth_token_for_refresh, ip_address)
 
         @self.cors_route(ENDPOINT__install, DOCUMENTATION__install)
         def install(http_inputs: dict):
             return self.model.install(**http_inputs)
 
         @self.cors_route('/internal/is_installed', DOCUMENTATION__is_installed)
         def is_installed(response: JAAQLResponse):
@@ -35,14 +35,19 @@
         def is_alive():
             self.model.is_alive()
 
         @self.cors_route('/accounts', DOCUMENTATION__create_account)
         def accounts(connection: DBInterface, http_inputs: dict):
             self.model.create_account_with_potential_password(connection, **http_inputs)
 
+        @self.cors_route('/prepare', DOCUMENTATION__prepare)
+        def prepare(connection: DBInterface, account_id: str, http_inputs: dict):
+            raise HttpStatusException("Not yet implemented", HTTPStatus.NOT_IMPLEMENTED)
+            # self.model.prepare_queries(connection, account_id, http_inputs)
+
         @self.cors_route('/account/password', DOCUMENTATION__password)
         def password(account_id: str, username: str, ip_address: str, http_inputs: dict):
             return self.model.add_my_account_password(account_id, username, ip_address, **http_inputs)
 
         @self.cors_route('/submit', DOCUMENTATION__submit)
         def submit(http_inputs: dict, account_id: str, verification_hook: queue.Queue):
             return self.model.submit(http_inputs, account_id, verification_hook=verification_hook)
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql/mvc/exception_queries.py` & `jaaql-middleware-python-4.6.3/jaaql/mvc/exception_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/mvc/generated_queries.py` & `jaaql-middleware-python-4.6.3/jaaql/mvc/generated_queries.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/mvc/model.py` & `jaaql-middleware-python-4.6.3/jaaql/mvc/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,14 +105,131 @@
                                     is_the_anonymous_user)
 
         if password:
             self.add_account_password(account_id, password)
 
         return account_id
 
+    def validate_query(self, queries: list, query, allow_list=True):
+        if isinstance(query, list) and allow_list:
+            for sub_query in query:
+                self.validate_query(queries, sub_query, allow_list=False)
+            return
+
+        if not isinstance(query, dict):
+            raise HttpStatusException("Expected query to be dict")
+
+        if "line_number" not in query:
+            raise HttpStatusException("Expected line number in query")
+        if not isinstance(query["line_number"], int):
+            raise HttpStatusException("Expected integer as line number for query")
+
+        if "position" not in query:
+            raise HttpStatusException("Expected position in query")
+        if not isinstance(query["position"], int):
+            raise HttpStatusException("Expected integer as position for query")
+
+        if "name" not in query:
+            raise HttpStatusException("Expected name in query")
+        if not isinstance(query["name"], str):
+            raise HttpStatusException("Expected string as name for query")
+
+        not_allowed = [key for key in query.keys() if key not in ["name", "position", "line_number"]]
+        if len(not_allowed):
+            raise HttpStatusException("Unexpected keys in query: " + ", ".join(not_allowed))
+
+        queries.append(query)
+
+    def prepare_queries(self, connection: DBInterface, account_id: str, inputs: dict):
+        # Important! Permission check by checking that the user can in insert into the application table. This is equivalent of checking if the user
+        # owns the application. We currently have no concept of application ownership
+        res = execute_supplied_statement_singleton(connection, """SELECT
+    *
+FROM information_schema.role_table_grants
+WHERE
+    table_schema = quote_ident('public')
+    AND table_catalog = 'jaaql'
+    AND table_name = quote_ident('application')
+    AND grantee = :grantee
+    AND privilege_type = 'INSERT'
+        """, parameters={"grantee": account_id}, as_objects=True, singleton_message="You do not have permissions to prepare queries!")
+
+        if KEY__application not in inputs:
+            raise HttpStatusException("Missing application from request")
+
+        if not isinstance(inputs[KEY__application], str):
+            raise HttpStatusException("Application must be a string")
+
+        application = application__select(connection, inputs[KEY__application])
+
+        for frame, requests in inputs.items():
+            if frame == KEY__application:
+                continue  # This is not a frame but the application name
+
+            if not isinstance(requests, list):
+                raise HttpStatusException("Requests must be a list type")
+
+            found_singletons = []
+            found_queries = []
+
+            for found_request in requests:
+                if not isinstance(found_request, dict):
+                    raise HttpStatusException("Request must be a dictionary type")
+
+                if "singletons" not in found_request and "queries" not in found_request:
+                    raise HttpStatusException("Request must have either singletons or queries")
+
+                if "parameters" in found_request:
+                    parameters = found_request["parameters"]
+                    if not isinstance(parameters, list):
+                        raise HttpStatusException("Expected parameters to be list type")
+                    for parameter in parameters:
+                        if not isinstance(parameter, dict):
+                            raise HttpStatusException("Parameter must be of dict type")
+
+                        if "line_number" not in parameter:
+                            raise HttpStatusException("Parameter must have line number")
+                        if "position" not in parameter:
+                            raise HttpStatusException("Parameter must have position")
+                        if "name" not in parameter:
+                            raise HttpStatusException("Parameter must have name")
+                        line_number = parameter["line_number"]
+                        position = parameter["position"]
+                        name = parameter["name"]
+                        if not isinstance(line_number, int):
+                            raise HttpStatusException("Parameter line number must be an integer")
+                        if not isinstance(position, int):
+                            raise HttpStatusException("Parameter position must be an integer")
+                        if not isinstance(name, str):
+                            raise HttpStatusException("Parameter name must be a string")
+
+                        disallowed_keys = [key for key in parameter.keys() if key not in ["line_number", "position", "name"]]
+                        if len(disallowed_keys) != 0:
+                            raise HttpStatusException("Unrecognised keys found in parameter: " + ", ".join(disallowed_keys))
+
+                if "singletons" in found_request:
+                    singletons = found_request["singletons"]
+                    if not isinstance(singletons, dict):
+                        raise HttpStatusException("Expected singletons to be dictionary type")
+                    for query in singletons:
+                        self.validate_query(found_singletons, query)
+
+                if "queries" in found_request:
+                    queries = found_request["queries"]
+                    if not isinstance(queries, dict):
+                        raise HttpStatusException("Expected queries to be dictionary type")
+                    for query in queries:
+                        if isinstance(query, dict):
+                            if "line_number" in query:
+                                self.validate_query(found_singletons, query)
+                            else:
+                                pass  # We are dealing with a store type query
+                        if isinstance(query, list):
+                            self.validate_query(found_singletons, query)
+
     def is_super_admin(self, connection: DBInterface):
         res = execute_supplied_statement_singleton(connection, "select usesuper from pg_user where usename = CURRENT_USER",
                                                    as_objects=True)["usesuper"]
         if not res:
             raise HttpStatusException("You do not have super user privileges")
 
     def clean(self, connection: DBInterface):
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql/openapi/swagger_documentation.py` & `jaaql-middleware-python-4.6.3/jaaql/openapi/swagger_documentation.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/scripts/01.install_domains.generated.sql` & `jaaql-middleware-python-4.6.3/jaaql/scripts/01.install_domains.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/scripts/02.install_super_user.exceptions.sql` & `jaaql-middleware-python-4.6.3/jaaql/scripts/02.install_super_user.exceptions.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/scripts/03.install_super_user.handwritten.sql` & `jaaql-middleware-python-4.6.3/jaaql/scripts/03.install_super_user.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/scripts/04.install_jaaql_data_structures.generated.sql` & `jaaql-middleware-python-4.6.3/jaaql/scripts/04.install_jaaql_data_structures.generated.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/scripts/06.install_jaaql.handwritten.sql` & `jaaql-middleware-python-4.6.3/jaaql/scripts/06.install_jaaql.handwritten.sql`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/scripts/swagger_template.html` & `jaaql-middleware-python-4.6.3/jaaql/scripts/swagger_template.html`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/services/cached_canned_query_service.py` & `jaaql-middleware-python-4.6.3/jaaql/services/cached_canned_query_service.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/services/script_install.py` & `jaaql-middleware-python-4.6.3/jaaql/services/script_install.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/utilities/crypt_utils.py` & `jaaql-middleware-python-4.6.3/jaaql/utilities/crypt_utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/utilities/options.py` & `jaaql-middleware-python-4.6.3/jaaql/utilities/options.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/utilities/utils.py` & `jaaql-middleware-python-4.6.3/jaaql/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/utilities/utils_no_project_imports.py` & `jaaql-middleware-python-4.6.3/jaaql/utilities/utils_no_project_imports.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql/utilities/vault.py` & `jaaql-middleware-python-4.6.3/jaaql/utilities/vault.py`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/PKG-INFO` & `jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaaql-middleware-python
-Version: 4.6.2
+Version: 4.6.3
 Summary: The jaaql package, allowing for rapid development and deployment of RESTful HTTP applications
 Home-page: https://github.com/JAAQL/JAAQL-middleware-python
 Author: Software Quality Measurement and Improvement bv
 Author-email: aaron.tasker@sqmi.nl
 License: Mozilla Public License Version 2.0 with Commons Clause
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `jaaql-middleware-python-4.6.2/jaaql_middleware_python.egg-info/SOURCES.txt` & `jaaql-middleware-python-4.6.3/jaaql_middleware_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaaql-middleware-python-4.6.2/setup.py` & `jaaql-middleware-python-4.6.3/setup.py`

 * *Files identical despite different names*

