# Comparing `tmp/python_dlt-0.2.0a9.tar.gz` & `tmp/python-dlt-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_dlt-0.2.0a9.tar", max compression
+gzip compressed data, was "python-dlt-0.2.1.tar", last modified: Tue Apr 18 13:51:46 2023, max compression
```

## Comparing `python_dlt-0.2.0a9.tar` & `python-dlt-0.2.1.tar`

### file list

```diff
@@ -1,195 +1,11 @@
--rw-r--r--   0        0        0    11343 2022-06-03 15:05:59.024600 python_dlt-0.2.0a9/LICENSE.txt
--rw-r--r--   0        0        0     4222 2022-09-15 12:13:36.104313 python_dlt-0.2.0a9/QUICKSTART.md
--rw-r--r--   0        0        0     1555 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/__init__.py
--rw-r--r--   0        0        0       21 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/__version__.py
--rw-r--r--   0        0        0       31 2022-11-27 12:55:51.874732 python_dlt-0.2.0a9/dlt/cli/__init__.py
--rw-r--r--   0        0        0     7512 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/cli/_dlt.py
--rw-r--r--   0        0        0     1961 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/cli/config_toml_writer.py
--rw-r--r--   0        0        0    15801 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/cli/deploy_command.py
--rw-r--r--   0        0        0      162 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/cli/echo.py
--rw-r--r--   0        0        0      259 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/cli/exceptions.py
--rw-r--r--   0        0        0    14921 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/cli/init_command.py
--rw-r--r--   0        0        0      106 2022-11-27 12:56:10.734732 python_dlt-0.2.0a9/dlt/cli/typing.py
--rw-r--r--   0        0        0     2497 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/cli/utils.py
--rw-r--r--   0        0        0      245 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/__init__.py
--rw-r--r--   0        0        0     1265 2022-08-24 09:42:09.472789 python_dlt-0.2.0a9/dlt/common/arithmetics.py
--rw-r--r--   0        0        0      451 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/__init__.py
--rw-r--r--   0        0        0     4489 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/accessors.py
--rw-r--r--   0        0        0     2630 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/container.py
--rw-r--r--   0        0        0     5694 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/exceptions.py
--rw-r--r--   0        0        0     5816 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/inject.py
--rw-r--r--   0        0        0      252 2022-12-02 14:59:55.574492 python_dlt-0.2.0a9/dlt/common/configuration/providers/__init__.py
--rw-r--r--   0        0        0     1095 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/context.py
--rw-r--r--   0        0        0     1199 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/dictionary.py
--rw-r--r--   0        0        0     2068 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/environ.py
--rw-r--r--   0        0        0      762 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/provider.py
--rw-r--r--   0        0        0     3170 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/providers/toml.py
--rw-r--r--   0        0        0    16225 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/resolve.py
--rw-r--r--   0        0        0      837 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/__init__.py
--rw-r--r--   0        0        0     8648 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/base_configuration.py
--rw-r--r--   0        0        0      503 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/config_namespace_context.py
--rw-r--r--   0        0        0     1683 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/config_providers_context.py
--rw-r--r--   0        0        0     1196 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/exceptions.py
--rw-r--r--   0        0        0     2918 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/gcp_client_credentials.py
--rw-r--r--   0        0        0      556 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/load_volume_configuration.py
--rw-r--r--   0        0        0      417 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/normalize_volume_configuration.py
--rw-r--r--   0        0        0     1062 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/pool_runner_configuration.py
--rw-r--r--   0        0        0     2313 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/postgres_credentials.py
--rw-r--r--   0        0        0     1812 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/run_configuration.py
--rw-r--r--   0        0        0      944 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/specs/schema_volume_configuration.py
--rw-r--r--   0        0        0     4926 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/configuration/utils.py
--rw-r--r--   0        0        0      260 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/__init__.py
--rw-r--r--   0        0        0     5149 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/buffered.py
--rw-r--r--   0        0        0     1696 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/escape.py
--rw-r--r--   0        0        0      962 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/exceptions.py
--rw-r--r--   0        0        0     5235 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/data_writers/writers.py
--rw-r--r--   0        0        0     6567 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/destination.py
--rw-r--r--   0        0        0     4545 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/exceptions.py
--rw-r--r--   0        0        0     2220 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/git.py
--rw-r--r--   0        0        0     4184 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/json.py
--rw-r--r--   0        0        0     8725 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/logger.py
--rw-r--r--   0        0        0        0 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/normalizers/__init__.py
--rw-r--r--   0        0        0      472 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/normalizers/exceptions.py
--rw-r--r--   0        0        0      691 2022-12-02 14:59:55.584492 python_dlt-0.2.0a9/dlt/common/normalizers/json/__init__.py
--rw-r--r--   0        0        0    10510 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/normalizers/json/relational.py
--rw-r--r--   0        0        0      300 2022-06-27 16:30:05.091379 python_dlt-0.2.0a9/dlt/common/normalizers/names/__init__.py
--rw-r--r--   0        0        0     2600 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/normalizers/names/snake_case.py
--rw-r--r--   0        0        0      406 2022-06-03 17:49:47.664600 python_dlt-0.2.0a9/dlt/common/pendulum.py
--rw-r--r--   0        0        0     6055 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/pipeline.py
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/reflection/__init__.py
--rw-r--r--   0        0        0      374 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/reflection/function_visitor.py
--rw-r--r--   0        0        0     4644 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/reflection/spec.py
--rw-r--r--   0        0        0     2517 2022-12-05 21:04:23.672896 python_dlt-0.2.0a9/dlt/common/reflection/utils.py
--rw-r--r--   0        0        0      154 2022-08-26 15:28:07.203730 python_dlt-0.2.0a9/dlt/common/runners/__init__.py
--rw-r--r--   0        0        0      768 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/runners/init.py
--rw-r--r--   0        0        0     7529 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/runners/pool_runner.py
--rw-r--r--   0        0        0     4041 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/runners/runnable.py
--rw-r--r--   0        0        0      728 2022-06-28 10:52:24.103559 python_dlt-0.2.0a9/dlt/common/runners/stdout.py
--rw-r--r--   0        0        0     3629 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/runners/venv.py
--rw-r--r--   0        0        0      369 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/__init__.py
--rw-r--r--   0        0        0      772 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/configuration.py
--rw-r--r--   0        0        0     1939 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/detections.py
--rw-r--r--   0        0        0     2977 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/exceptions.py
--rw-r--r--   0        0        0    24247 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/schema/schema.py
--rw-r--r--   0        0        0     3010 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/schema/typing.py
--rw-r--r--   0        0        0    24569 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/schema/utils.py
--rw-r--r--   0        0        0     1277 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/signals.py
--rw-r--r--   0        0        0      410 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/__init__.py
--rw-r--r--   0        0        0     1713 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/data_item_storage.py
--rw-r--r--   0        0        0     2582 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/exceptions.py
--rw-r--r--   0        0        0     7767 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/file_storage.py
--rw-r--r--   0        0        0     2527 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/storages/live_schema_storage.py
--rw-r--r--   0        0        0    12318 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/load_storage.py
--rw-r--r--   0        0        0     2387 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/normalize_storage.py
--rw-r--r--   0        0        0     8505 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/common/storages/schema_storage.py
--rw-r--r--   0        0        0     2465 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/storages/versioned_storage.py
--rw-r--r--   0        0        0     2054 2022-06-28 10:52:24.103559 python_dlt-0.2.0a9/dlt/common/telemetry.py
--rw-r--r--   0        0        0     1108 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/time.py
--rw-r--r--   0        0        0     3816 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/typing.py
--rw-r--r--   0        0        0     6708 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/common/utils.py
--rw-r--r--   0        0        0     3686 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/validation.py
--rw-r--r--   0        0        0     1185 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/common/wei.py
--rw-r--r--   0        0        0      876 2022-06-03 13:18:25.174600 python_dlt-0.2.0a9/dlt/dbt_runner/README.md
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/dbt_runner/__init__.py
--rw-r--r--   0        0        0     2748 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/dbt_runner/configuration.py
--rw-r--r--   0        0        0      159 2022-06-03 13:18:25.174600 python_dlt-0.2.0a9/dlt/dbt_runner/exceptions.py
--rw-r--r--   0        0        0     8129 2022-12-02 14:59:55.594492 python_dlt-0.2.0a9/dlt/dbt_runner/runner.py
--rw-r--r--   0        0        0     3197 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/dbt_runner/utils.py
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/__init__.py
--rw-r--r--   0        0        0      437 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/bigquery/README.md
--rw-r--r--   0        0        0     1725 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/bigquery/__init__.py
--rw-r--r--   0        0        0    11216 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/bigquery/bigquery.py
--rw-r--r--   0        0        0      382 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/bigquery/configuration.py
--rw-r--r--   0        0        0     6283 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/bigquery/sql_client.py
--rw-r--r--   0        0        0     1587 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/dummy/__init__.py
--rw-r--r--   0        0        0      625 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/dummy/configuration.py
--rw-r--r--   0        0        0     4667 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/dummy/dummy.py
--rw-r--r--   0        0        0     3604 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/exceptions.py
--rw-r--r--   0        0        0     7151 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/job_client_impl.py
--rw-r--r--   0        0        0      251 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/postgres/README.md
--rw-r--r--   0        0        0     1847 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/postgres/__init__.py
--rw-r--r--   0        0        0      400 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/postgres/configuration.py
--rw-r--r--   0        0        0    10352 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/destinations/postgres/postgres.py
--rw-r--r--   0        0        0     4830 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/postgres/sql_client.py
--rw-r--r--   0        0        0     1191 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/README.md
--rw-r--r--   0        0        0     1778 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/__init__.py
--rw-r--r--   0        0        0      306 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/configuration.py
--rw-r--r--   0        0        0     3651 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/redshift/redshift.py
--rw-r--r--   0        0        0     3863 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/destinations/sql_client.py
--rw-r--r--   0        0        0      564 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/destinations/typing.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 python_dlt-0.2.0a9/dlt/extract/__init__.py
--rw-r--r--   0        0        0    10674 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/extract/decorators.py
--rw-r--r--   0        0        0    10604 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/exceptions.py
--rw-r--r--   0        0        0     5430 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/extract/extract.py
--rw-r--r--   0        0        0    24256 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/pipe.py
--rw-r--r--   0        0        0    22304 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/source.py
--rw-r--r--   0        0        0     1500 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/extract/typing.py
--rw-r--r--   0        0        0        0 2022-08-14 16:06:42.572263 python_dlt-0.2.0a9/dlt/helpers/__init__.py
--rw-r--r--   0        0        0     2373 2022-12-02 14:59:55.604492 python_dlt-0.2.0a9/dlt/helpers/pandas.py
--rw-r--r--   0        0        0     7360 2022-12-05 22:14:32.612895 python_dlt-0.2.0a9/dlt/helpers/streamlit.py
--rw-r--r--   0        0        0       31 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/__init__.py
--rw-r--r--   0        0        0      905 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/configuration.py
--rw-r--r--   0        0        0     1109 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/exceptions.py
--rw-r--r--   0        0        0    13834 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/load/load.py
--rw-r--r--   0        0        0       32 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/normalize/__init__.py
--rw-r--r--   0        0        0     1138 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/normalize/configuration.py
--rw-r--r--   0        0        0        0 2022-08-09 19:58:51.837922 python_dlt-0.2.0a9/dlt/normalize/exceptions.py
--rw-r--r--   0        0        0    14328 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/normalize/normalize.py
--rw-r--r--   0        0        0     1880 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/README.md
--rw-r--r--   0        0        0     3800 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/__init__.py
--rw-r--r--   0        0        0     1235 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/pipeline/configuration.py
--rw-r--r--   0        0        0     3291 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/pipeline/exceptions.py
--rw-r--r--   0        0        0    44978 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/pipeline/pipeline.py
--rw-r--r--   0        0        0     5917 2022-12-04 21:46:36.159175 python_dlt-0.2.0a9/dlt/pipeline/state.py
--rw-r--r--   0        0        0     2803 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/trace.py
--rw-r--r--   0        0        0       92 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/pipeline/typing.py
--rw-r--r--   0        0        0        0 2022-06-03 13:18:25.174600 python_dlt-0.2.0a9/dlt/py.typed
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/reflection/__init__.py
--rw-r--r--   0        0        0      563 2022-12-02 14:59:55.614492 python_dlt-0.2.0a9/dlt/reflection/names.py
--rw-r--r--   0        0        0     2141 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/dlt/reflection/script_inspector.py
--rw-r--r--   0        0        0     6186 2022-12-05 22:53:45.442896 python_dlt-0.2.0a9/dlt/reflection/script_visitor.py
--rw-r--r--   0        0        0      745 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/.dlt/example.secrets.toml
--rw-r--r--   0        0        0     3777 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/README.md
--rw-r--r--   0        0        0        0 2022-05-20 13:04:18.202424 python_dlt-0.2.0a9/examples/__init__.py
--rw-r--r--   0        0        0     2859 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/_helpers.py
--rw-r--r--   0        0        0       91 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/chess/.dlt/config.toml
--rw-r--r--   0        0        0       75 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/chess/.dlt/secrets.toml
--rw-r--r--   0        0        0        0 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/chess/__init__.py
--rw-r--r--   0        0        0     1971 2022-12-02 15:00:00.154492 python_dlt-0.2.0a9/examples/chess/chess.py
--rw-r--r--   0        0        0    23882 2022-05-20 13:04:18.272424 python_dlt-0.2.0a9/examples/data/channels.json
--rw-r--r--   0        0        0      530 2022-05-31 08:33:39.199428 python_dlt-0.2.0a9/examples/data/demo_example.json
--rw-r--r--   0        0        0    71730 2022-05-20 13:04:18.602424 python_dlt-0.2.0a9/examples/data/messages.json
--rw-r--r--   0        0        0   386829 2022-06-26 22:03:48.615163 python_dlt-0.2.0a9/examples/data/rasa_trackers/2888158124550630_tracker.jsonl
--rw-r--r--   0        0        0   213456 2022-06-26 22:03:45.545163 python_dlt-0.2.0a9/examples/data/rasa_trackers/8629c904-0c26-4f0b-927b-14d48db43c28_tracker.jsonl
--rw-r--r--   0        0        0     2669 2022-06-23 14:46:53.157751 python_dlt-0.2.0a9/examples/data/singer_taps/csv_catalog.json
--rw-r--r--   0        0        0      210 2022-06-23 14:46:53.157751 python_dlt-0.2.0a9/examples/data/singer_taps/model_annotations.csv
--rw-r--r--   0        0        0     8010 2022-06-23 14:46:53.157751 python_dlt-0.2.0a9/examples/data/singer_taps/tap_google_sheet.jsonl
--rw-r--r--   0        0        0  4458258 2022-06-23 14:46:53.167751 python_dlt-0.2.0a9/examples/data/singer_taps/tap_hubspot.jsonl
--rw-r--r--   0        0        0     6429 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/demo_example.py
--rw-r--r--   0        0        0     3748 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/discord_iterator.py
--rw-r--r--   0        0        0     3371 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/google_drive_csv.py
--rw-r--r--   0        0        0      311 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/google_sheets.py
--rw-r--r--   0        0        0     6832 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/quickstart.py
--rw-r--r--   0        0        0     1358 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/rasa_example.py
--rw-r--r--   0        0        0     1467 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/read_table.py
--rw-r--r--   0        0        0     1068 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/restore_pipeline.py
--rw-r--r--   0        0        0        0 2022-06-09 15:05:08.450657 python_dlt-0.2.0a9/examples/schemas/__init__.py
--rw-r--r--   0        0        0    12510 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/discord.schema.yml
--rw-r--r--   0        0        0     1933 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/dlt_quickstart.schema.yaml
--rw-r--r--   0        0        0     1208 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/hubspot.schema.yaml
--rw-r--r--   0        0        0     4492 2022-12-02 14:59:55.624492 python_dlt-0.2.0a9/examples/schemas/inferred_demo.schema.yml
--rw-r--r--   0        0        0     1346 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/singer_tap_example.py
--rw-r--r--   0        0        0      731 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/singer_tap_jsonl_example.py
--rw-r--r--   0        0        0        0 2022-06-09 15:05:08.450657 python_dlt-0.2.0a9/examples/sources/__init__.py
--rw-r--r--   0        0        0     1969 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/google_sheets.py
--rw-r--r--   0        0        0     1029 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/jsonl.py
--rw-r--r--   0        0        0       22 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/rasa/__init__.py
--rw-r--r--   0        0        0     3287 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/rasa/rasa.py
--rw-r--r--   0        0        0     1959 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/rasa/rasa.schema.yaml
--rw-r--r--   0        0        0     3702 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/singer_tap.py
--rw-r--r--   0        0        0     2461 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/sql_query.py
--rw-r--r--   0        0        0      869 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sources/stdout.py
--rw-r--r--   0        0        0      807 2022-12-02 14:59:55.634492 python_dlt-0.2.0a9/examples/sync_schema_example.py
--rw-r--r--   0        0        0     3493 2022-12-05 22:54:08.432896 python_dlt-0.2.0a9/pyproject.toml
--rw-r--r--   0        0        0     7812 1970-01-01 00:00:00.000000 python_dlt-0.2.0a9/setup.py
--rw-r--r--   0        0        0     7444 1970-01-01 00:00:00.000000 python_dlt-0.2.0a9/PKG-INFO
+drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-18 13:51:46.578830 python-dlt-0.2.1/
+-rw-r--r--   0 burnash    (501) staff       (20)      337 2023-04-18 13:51:46.578598 python-dlt-0.2.1/PKG-INFO
+-rw-r--r--   0 burnash    (501) staff       (20)      139 2023-04-18 10:25:13.000000 python-dlt-0.2.1/README.md
+drwxr-xr-x   0 burnash    (501) staff       (20)        0 2023-04-18 13:51:46.578317 python-dlt-0.2.1/python_dlt.egg-info/
+-rw-r--r--   0 burnash    (501) staff       (20)      337 2023-04-18 13:51:46.000000 python-dlt-0.2.1/python_dlt.egg-info/PKG-INFO
+-rw-r--r--   0 burnash    (501) staff       (20)      187 2023-04-18 13:51:46.000000 python-dlt-0.2.1/python_dlt.egg-info/SOURCES.txt
+-rw-r--r--   0 burnash    (501) staff       (20)        1 2023-04-18 13:51:46.000000 python-dlt-0.2.1/python_dlt.egg-info/dependency_links.txt
+-rw-r--r--   0 burnash    (501) staff       (20)       11 2023-04-18 13:51:46.000000 python-dlt-0.2.1/python_dlt.egg-info/requires.txt
+-rw-r--r--   0 burnash    (501) staff       (20)        1 2023-04-18 13:51:46.000000 python-dlt-0.2.1/python_dlt.egg-info/top_level.txt
+-rw-r--r--   0 burnash    (501) staff       (20)       38 2023-04-18 13:51:46.578905 python-dlt-0.2.1/setup.cfg
+-rw-r--r--   0 burnash    (501) staff       (20)      555 2023-04-18 13:49:34.000000 python-dlt-0.2.1/setup.py
```

