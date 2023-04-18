# Comparing `tmp/adapta-2.1.1.tar.gz` & `tmp/adapta-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adapta-2.1.1.tar", max compression
+gzip compressed data, was "adapta-2.2.0.tar", max compression
```

## Comparing `adapta-2.1.1.tar` & `adapta-2.2.0.tar`

### file list

```diff
@@ -1,73 +1,74 @@
--rw-r--r--   0        0        0    10693 2023-04-12 11:49:34.504297 adapta-2.1.1/LICENSE
--rw-r--r--   0        0        0      666 2023-04-12 11:49:34.504297 adapta-2.1.1/README.md
--rw-r--r--   0        0        0      663 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/__init__.py
--rw-r--r--   0        0        0       22 2023-04-12 11:49:54.497748 adapta-2.1.1/adapta/_version.py
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/connectors/__init__.py
--rw-r--r--   0        0        0      694 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/connectors/service_bus/__init__.py
--rw-r--r--   0        0        0     1914 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/connectors/service_bus/_connector.py
--rw-r--r--   0        0        0     4111 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/README.md
--rw-r--r--   0        0        0      667 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/__init__.py
--rw-r--r--   0        0        0    12390 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/_base.py
--rw-r--r--   0        0        0     2950 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/_internal.py
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/handlers/__init__.py
--rw-r--r--   0        0        0     9168 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/handlers/datadog_api_handler.py
--rw-r--r--   0        0        0     2211 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/handlers/safe_stream_handler.py
--rw-r--r--   0        0        0      741 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/models/__init__.py
--rw-r--r--   0        0        0      794 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/models/_log_level.py
--rw-r--r--   0        0        0      963 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/logs/models/_logs_metadata.py
--rw-r--r--   0        0        0      672 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/__init__.py
--rw-r--r--   0        0        0     3215 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/_base.py
--rw-r--r--   0        0        0     1930 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/providers/README.md
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/providers/__init__.py
--rw-r--r--   0        0        0     4466 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/metrics/providers/datadog_provider.py
--rw-r--r--   0        0        0      653 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/__init__.py
--rw-r--r--   0        0        0     1223 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/_model.py
--rw-r--r--   0        0        0      699 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/mlflow/__init__.py
--rw-r--r--   0        0        0     5319 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/mlflow/_client.py
--rw-r--r--   0        0        0     3820 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/ml/mlflow/_functions.py
--rw-r--r--   0        0        0      674 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/process_communication/__init__.py
--rw-r--r--   0        0        0     3362 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/process_communication/_models.py
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/__init__.py
--rw-r--r--   0        0        0     1303 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/__init__.py
--rw-r--r--   0        0        0     7396 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/_azure_client.py
--rw-r--r--   0        0        0     2396 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/_base.py
--rw-r--r--   0        0        0     1787 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/_local_client.py
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.504297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/__init__.py
--rw-r--r--   0        0        0     2695 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
--rw-r--r--   0        0        0     2601 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py
--rw-r--r--   0        0        0     3454 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/security/clients/hashicorp_vault/oidc_client.py
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/__init__.py
--rw-r--r--   0        0        0     1208 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/README.md
--rw-r--r--   0        0        0      622 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/__init__.py
--rw-r--r--   0        0        0     9605 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/azure_storage_client.py
--rw-r--r--   0        0        0     4791 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/blob/base.py
--rw-r--r--   0        0        0      665 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/cache/__init__.py
--rw-r--r--   0        0        0     3451 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/cache/_base.py
--rw-r--r--   0        0        0     3365 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/cache/redis_cache.py
--rw-r--r--   0        0        0     2451 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/README.md
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/__init__.py
--rw-r--r--   0        0        0     4691 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/azure_sql.py
--rw-r--r--   0        0        0      675 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/models/__init__.py
--rw-r--r--   0        0        0     1447 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/models/_models.py
--rw-r--r--   0        0        0     7711 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/odbc.py
--rw-r--r--   0        0        0     4523 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/database/trino_sql.py
--rw-r--r--   0        0        0     2386 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/README.md
--rw-r--r--   0        0        0      721 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/__init__.py
--rw-r--r--   0        0        0    11493 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/_functions.py
--rw-r--r--   0        0        0     2247 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/delta_lake/_models.py
--rw-r--r--   0        0        0      598 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/__init__.py
--rw-r--r--   0        0        0     5302 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/azure.py
--rw-r--r--   0        0        0     2063 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/base.py
--rw-r--r--   0        0        0     5711 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/format.py
--rw-r--r--   0        0        0     6627 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/hive.py
--rw-r--r--   0        0        0     1519 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/models/local.py
--rw-r--r--   0        0        0      529 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/README.md
--rw-r--r--   0        0        0      666 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/__init__.py
--rw-r--r--   0        0        0     2216 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/_base.py
--rw-r--r--   0        0        0     2358 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/azure_secret_client.py
--rw-r--r--   0        0        0     2887 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
--rw-r--r--   0        0        0      668 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/utils/__init__.py
--rw-r--r--   0        0        0     3578 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/utils/_common.py
--rw-r--r--   0        0        0     3815 2023-04-12 11:49:34.508297 adapta-2.1.1/adapta/utils/concurrent_task_runner.py
--rw-r--r--   0        0        0     2185 2023-04-12 11:49:54.497748 adapta-2.1.1/pyproject.toml
--rw-r--r--   0        0        0     2763 1970-01-01 00:00:00.000000 adapta-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0    10693 2023-04-18 07:40:29.766467 adapta-2.2.0/LICENSE
+-rw-r--r--   0        0        0      666 2023-04-18 07:40:29.766467 adapta-2.2.0/README.md
+-rw-r--r--   0        0        0      663 2023-04-18 07:40:29.766467 adapta-2.2.0/adapta/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-18 07:40:45.386594 adapta-2.2.0/adapta/_version.py
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/connectors/__init__.py
+-rw-r--r--   0        0        0      694 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/connectors/service_bus/__init__.py
+-rw-r--r--   0        0        0     1914 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/connectors/service_bus/_connector.py
+-rw-r--r--   0        0        0     4111 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/README.md
+-rw-r--r--   0        0        0      667 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/__init__.py
+-rw-r--r--   0        0        0    12390 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/_base.py
+-rw-r--r--   0        0        0     2950 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/_internal.py
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/handlers/__init__.py
+-rw-r--r--   0        0        0     9167 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/handlers/datadog_api_handler.py
+-rw-r--r--   0        0        0     2211 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/handlers/safe_stream_handler.py
+-rw-r--r--   0        0        0      741 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/models/__init__.py
+-rw-r--r--   0        0        0      794 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/models/_log_level.py
+-rw-r--r--   0        0        0      963 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/logs/models/_logs_metadata.py
+-rw-r--r--   0        0        0      672 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/metrics/__init__.py
+-rw-r--r--   0        0        0     3215 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/metrics/_base.py
+-rw-r--r--   0        0        0     1930 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/metrics/providers/README.md
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/metrics/providers/__init__.py
+-rw-r--r--   0        0        0     4466 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/metrics/providers/datadog_provider.py
+-rw-r--r--   0        0        0      653 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/ml/__init__.py
+-rw-r--r--   0        0        0     1223 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/ml/_model.py
+-rw-r--r--   0        0        0      699 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/ml/mlflow/__init__.py
+-rw-r--r--   0        0        0     5319 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/ml/mlflow/_client.py
+-rw-r--r--   0        0        0     3820 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/ml/mlflow/_functions.py
+-rw-r--r--   0        0        0      674 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/process_communication/__init__.py
+-rw-r--r--   0        0        0     3362 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/process_communication/_models.py
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/__init__.py
+-rw-r--r--   0        0        0     1303 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/__init__.py
+-rw-r--r--   0        0        0     7396 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/_azure_client.py
+-rw-r--r--   0        0        0     2396 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/_base.py
+-rw-r--r--   0        0        0     1787 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/_local_client.py
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/hashicorp_vault/__init__.py
+-rw-r--r--   0        0        0     2695 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py
+-rw-r--r--   0        0        0     2601 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py
+-rw-r--r--   0        0        0     3454 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/security/clients/hashicorp_vault/oidc_client.py
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/__init__.py
+-rw-r--r--   0        0        0     1208 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/blob/README.md
+-rw-r--r--   0        0        0      622 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/blob/__init__.py
+-rw-r--r--   0        0        0     9605 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/blob/azure_storage_client.py
+-rw-r--r--   0        0        0     4791 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/blob/base.py
+-rw-r--r--   0        0        0      665 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/cache/__init__.py
+-rw-r--r--   0        0        0     3451 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/cache/_base.py
+-rw-r--r--   0        0        0     3365 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/cache/redis_cache.py
+-rw-r--r--   0        0        0     2451 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/README.md
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/__init__.py
+-rw-r--r--   0        0        0     4691 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/azure_sql.py
+-rw-r--r--   0        0        0      675 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/models/__init__.py
+-rw-r--r--   0        0        0     1447 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/models/_models.py
+-rw-r--r--   0        0        0     7711 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/odbc.py
+-rw-r--r--   0        0        0     4523 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/database/trino_sql.py
+-rw-r--r--   0        0        0     2386 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/delta_lake/README.md
+-rw-r--r--   0        0        0      721 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/delta_lake/__init__.py
+-rw-r--r--   0        0        0    11493 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/delta_lake/_functions.py
+-rw-r--r--   0        0        0     2247 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/delta_lake/_models.py
+-rw-r--r--   0        0        0      598 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/models/__init__.py
+-rw-r--r--   0        0        0     5302 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/models/azure.py
+-rw-r--r--   0        0        0     2063 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/models/base.py
+-rw-r--r--   0        0        0     5711 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/models/format.py
+-rw-r--r--   0        0        0     6627 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/models/hive.py
+-rw-r--r--   0        0        0     1519 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/models/local.py
+-rw-r--r--   0        0        0      529 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/secrets/README.md
+-rw-r--r--   0        0        0      666 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/secrets/__init__.py
+-rw-r--r--   0        0        0     2216 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/secrets/_base.py
+-rw-r--r--   0        0        0     2358 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/secrets/azure_secret_client.py
+-rw-r--r--   0        0        0     2887 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py
+-rw-r--r--   0        0        0     2761 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/utils/README.md
+-rw-r--r--   0        0        0      668 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/utils/__init__.py
+-rw-r--r--   0        0        0     5161 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/utils/_common.py
+-rw-r--r--   0        0        0     3815 2023-04-18 07:40:29.770467 adapta-2.2.0/adapta/utils/concurrent_task_runner.py
+-rw-r--r--   0        0        0     2168 2023-04-18 07:40:45.386594 adapta-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2815 1970-01-01 00:00:00.000000 adapta-2.2.0/PKG-INFO
```

### Comparing `adapta-2.1.1/LICENSE` & `adapta-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/README.md` & `adapta-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/__init__.py` & `adapta-2.2.0/adapta/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/connectors/__init__.py` & `adapta-2.2.0/adapta/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/connectors/service_bus/__init__.py` & `adapta-2.2.0/adapta/connectors/service_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/connectors/service_bus/_connector.py` & `adapta-2.2.0/adapta/connectors/service_bus/_connector.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/README.md` & `adapta-2.2.0/adapta/logs/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/__init__.py` & `adapta-2.2.0/adapta/logs/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/_base.py` & `adapta-2.2.0/adapta/logs/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/_internal.py` & `adapta-2.2.0/adapta/logs/_internal.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/handlers/__init__.py` & `adapta-2.2.0/adapta/logs/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/handlers/datadog_api_handler.py` & `adapta-2.2.0/adapta/logs/handlers/datadog_api_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     """
     Logging handler for DataDog.
     """
 
     def __init__(
         self,
         *,
-        buffer_size=10,
+        buffer_size=0,
         async_handler=False,
         debug=False,
         max_flush_retry_time=30,
         ignore_flush_failure=True,
         fixed_tags: Optional[Dict[str, str]] = None,
     ):
         """
```

### Comparing `adapta-2.1.1/adapta/logs/handlers/safe_stream_handler.py` & `adapta-2.2.0/adapta/logs/handlers/safe_stream_handler.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/models/__init__.py` & `adapta-2.2.0/adapta/logs/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/models/_log_level.py` & `adapta-2.2.0/adapta/logs/models/_log_level.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/logs/models/_logs_metadata.py` & `adapta-2.2.0/adapta/logs/models/_logs_metadata.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/metrics/__init__.py` & `adapta-2.2.0/adapta/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/metrics/_base.py` & `adapta-2.2.0/adapta/metrics/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/metrics/providers/README.md` & `adapta-2.2.0/adapta/metrics/providers/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/metrics/providers/__init__.py` & `adapta-2.2.0/adapta/metrics/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/metrics/providers/datadog_provider.py` & `adapta-2.2.0/adapta/metrics/providers/datadog_provider.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/ml/__init__.py` & `adapta-2.2.0/adapta/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/ml/_model.py` & `adapta-2.2.0/adapta/ml/_model.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/ml/mlflow/__init__.py` & `adapta-2.2.0/adapta/ml/mlflow/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/ml/mlflow/_client.py` & `adapta-2.2.0/adapta/ml/mlflow/_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/ml/mlflow/_functions.py` & `adapta-2.2.0/adapta/ml/mlflow/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/process_communication/__init__.py` & `adapta-2.2.0/adapta/process_communication/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/process_communication/_models.py` & `adapta-2.2.0/adapta/process_communication/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/__init__.py` & `adapta-2.2.0/adapta/security/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/__init__.py` & `adapta-2.2.0/adapta/security/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/_azure_client.py` & `adapta-2.2.0/adapta/security/clients/_azure_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/_base.py` & `adapta-2.2.0/adapta/security/clients/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/_local_client.py` & `adapta-2.2.0/adapta/security/clients/_local_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/hashicorp_vault/__init__.py` & `adapta-2.2.0/adapta/security/clients/hashicorp_vault/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py` & `adapta-2.2.0/adapta/security/clients/hashicorp_vault/hashicorp_vault_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/hashicorp_vault/kubernetes_client.py` & `adapta-2.2.0/adapta/security/clients/hashicorp_vault/kubernetes_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/security/clients/hashicorp_vault/oidc_client.py` & `adapta-2.2.0/adapta/security/clients/hashicorp_vault/oidc_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/__init__.py` & `adapta-2.2.0/adapta/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/blob/README.md` & `adapta-2.2.0/adapta/storage/blob/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/blob/__init__.py` & `adapta-2.2.0/adapta/storage/blob/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/blob/azure_storage_client.py` & `adapta-2.2.0/adapta/storage/blob/azure_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/blob/base.py` & `adapta-2.2.0/adapta/storage/blob/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/cache/__init__.py` & `adapta-2.2.0/adapta/storage/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/cache/_base.py` & `adapta-2.2.0/adapta/storage/cache/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/cache/redis_cache.py` & `adapta-2.2.0/adapta/storage/cache/redis_cache.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/README.md` & `adapta-2.2.0/adapta/storage/database/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/__init__.py` & `adapta-2.2.0/adapta/storage/database/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/azure_sql.py` & `adapta-2.2.0/adapta/storage/database/azure_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/models/__init__.py` & `adapta-2.2.0/adapta/storage/database/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/models/_models.py` & `adapta-2.2.0/adapta/storage/database/models/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/odbc.py` & `adapta-2.2.0/adapta/storage/database/odbc.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/database/trino_sql.py` & `adapta-2.2.0/adapta/storage/database/trino_sql.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/delta_lake/README.md` & `adapta-2.2.0/adapta/storage/delta_lake/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/delta_lake/__init__.py` & `adapta-2.2.0/adapta/storage/delta_lake/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/delta_lake/_functions.py` & `adapta-2.2.0/adapta/storage/delta_lake/_functions.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/delta_lake/_models.py` & `adapta-2.2.0/adapta/storage/delta_lake/_models.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/models/__init__.py` & `adapta-2.2.0/adapta/storage/models/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/models/azure.py` & `adapta-2.2.0/adapta/storage/models/azure.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/models/base.py` & `adapta-2.2.0/adapta/storage/models/base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/models/format.py` & `adapta-2.2.0/adapta/storage/models/format.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/models/hive.py` & `adapta-2.2.0/adapta/storage/models/hive.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/models/local.py` & `adapta-2.2.0/adapta/storage/models/local.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/secrets/README.md` & `adapta-2.2.0/adapta/storage/secrets/README.md`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/secrets/__init__.py` & `adapta-2.2.0/adapta/storage/secrets/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/secrets/_base.py` & `adapta-2.2.0/adapta/storage/secrets/_base.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/secrets/azure_secret_client.py` & `adapta-2.2.0/adapta/storage/secrets/azure_secret_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py` & `adapta-2.2.0/adapta/storage/secrets/hashicorp_vault_secret_storage_client.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/utils/__init__.py` & `adapta-2.2.0/adapta/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `adapta-2.1.1/adapta/utils/_common.py` & `adapta-2.2.0/adapta/utils/concurrent_task_runner.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-"""Common utility functions. All of these are imported into __init__.py"""
+"""
+ Models used by utility methods
+"""
 #  Copyright (c) 2023. ECCO Sneaks & Data
 #
 #  Licensed under the Apache License, Version 2.0 (the "License");
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
@@ -10,104 +12,97 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 
-import contextlib
-import math
-import time
-from collections import namedtuple
-from functools import partial
-from typing import List, Optional, Dict, Any, Tuple
-
-import requests
-from requests.adapters import HTTPAdapter
-from urllib3 import Retry
-
-
-def doze(seconds: int, doze_period_ms: int = 100) -> int:
-    """Sleeps for time given in seconds.
-
-    Note for Windows users: doze_period_ms less than 15 doesn't work correctly.
-
-    Args:
-        seconds: Seconds to doze for
-        doze_period_ms: Milliseconds per doze cycle
-
-    Returns: Time elapsed in nanoseconds
-
-    """
-    loops = int(seconds * 1000 / doze_period_ms)
-    start = time.monotonic_ns()
-    for _ in range(loops):
-        time.sleep(doze_period_ms / 1000)
-
-    return time.monotonic_ns() - start
-
-
-def session_with_retries(
-    method_list: Tuple[str, ...] = ("HEAD", "GET", "OPTIONS", "TRACE"),
-    request_timeout: Optional[float] = 300,
-    status_list: Tuple[int, ...] = (400, 429, 500, 502, 503, 504),
-    retry_count: int = 4,
-):
-    """
-     Provisions http session manager with retries.
-    :return:
-    """
-    retry_strategy = Retry(
-        total=retry_count,
-        status_forcelist=status_list,
-        allowed_methods=method_list,
-        backoff_factor=1,
-    )
-    adapter = HTTPAdapter(max_retries=retry_strategy)
-    http = requests.Session()
-    http.mount("https://", adapter)
-    http.mount("http://", adapter)
-    http.request = partial(http.request, timeout=request_timeout)
-    http.send = partial(http.send, timeout=request_timeout)
-
-    return http
-
-
-def convert_datadog_tags(tag_dict: Optional[Dict[str, str]]) -> Optional[List[str]]:
-    """
-     Converts tags dictionary to Datadog tag format.
-
-    :param tag_dict: Dictionary of tags.
-    :return: A list of tag_key:tag_value
-    """
-    if not tag_dict:
-        return None
-    return [f"{k}:{v}" for k, v in tag_dict.items()]
-
-
-@contextlib.contextmanager
-def operation_time():
-    """
-      Returns execution time for the context block.
-
-    :param operation: A method to measure execution time for.
-    :return: A tuple of (method_execution_time_ns, method_result)
-    """
-    result = namedtuple("OperationDuration", ["start", "end", "elapsed"])
-    result.start = time.monotonic_ns()
-    result.end = 0
-    result.elapsed = 0
-    yield result
-    result.end = time.monotonic_ns()
-    result.elapsed = result.end - result.start
-
-
-def chunk_list(value: List[Any], num_chunks: int) -> List[List[Any]]:
-    """
-     Chunks the provided list into a specified number of chunks. This method is thread-safe.
-
-    :param value: A list to chunk.
-    :param num_chunks: Number of chunks to generate.
-    :return: A list that has num_chunks lists in it. Total length equals length of the original list.
-    """
-    chunk_size = math.ceil(len(value) / num_chunks)
-    return [value[el_pos : el_pos + chunk_size] for el_pos in range(0, len(value), chunk_size)]
+import concurrent
+import os
+import sys
+from concurrent.futures import ThreadPoolExecutor, ProcessPoolExecutor
+from dataclasses import dataclass
+from typing import Callable, Any, List, TypeVar, Generic, Optional, Dict
+
+T = TypeVar("T")
+
+
+@dataclass
+class Executable(Generic[T]):
+    """
+    A single executable function with arguments, ready to run if invoked.
+    """
+
+    func: Callable[[...], T]
+    args: List[Any]
+    alias: str
+
+
+class ConcurrentTaskRunner(Generic[T]):
+    """
+     Provides parallel execution capability for a list of given functions.
+
+      my_funcs = [Executable(func=my_func1, args=[arg1, .., argN], alias='task1'),..]
+      threads = len(os.sched_getaffinity(0))
+      runner = ConcurrentTaskRunner(my_funcs, threads, True)
+
+      # get results lazily
+      tasks = runner.run()['taskN'].result()
+
+      # get results as they come
+      task_results = runner.run(lazy=False)
+
+     NB: For CPU bound work, set use_processes to True, otherwise overall run time will not improve due to GIL.
+
+    :param func_list: A list of (function, arguments) tuples to parallelise.
+    :param num_threads: Maximum number of threads to use. On Linux platforms use len(os.sched_getaffinity(0))
+          to get number of threads available to current process
+    :param use_processes: Use processes instead of thread for parallelisation. Preferrable for work that depends on GIL release.
+    """
+
+    def __init__(
+        self,
+        func_list: List[Executable[T]],
+        num_threads: Optional[int] = None,
+        use_processes: bool = False,
+    ):
+        self._func_list = func_list
+        self._num_threads = num_threads
+        self._use_processes = use_processes
+
+    def _run_tasks(self) -> Dict[str, concurrent.futures.Future]:
+        """
+         Executes a list of functions in parallel using threads or processes.
+
+        :param lazy: Whether to collect results right away or leave this to the caller.
+        :return: A dictionary of (callable_name, callable_future)
+        """
+        worker_count = self._num_threads or (
+            len(os.sched_getaffinity(0)) if sys.platform != "win32" else os.cpu_count()
+        )
+        runner_pool = (
+            ProcessPoolExecutor(max_workers=worker_count)
+            if self._use_processes
+            else ThreadPoolExecutor(max_workers=worker_count)
+        )
+        with runner_pool:
+            return {
+                executable.alias: runner_pool.submit(executable.func, *executable.args)
+                for executable in self._func_list
+            }
+
+    def lazy(self) -> Dict[str, concurrent.futures.Future]:
+        """
+         Executes the function list without explicitly collecting the results, allowing them to be retrieved by the client
+         when needed.
+
+        :return: A dictionary of (task_alias, task_future)
+        """
+        return self._run_tasks()
+
+    def eager(self) -> Dict[str, T]:
+        """
+         Executes the function list and wait for all threads to complete execution before returning
+
+        :return: A dictionary of (task_alias, task_result)
+        """
+        return {task_name: task.result() for task_name, task in self._run_tasks().items()}
```

### Comparing `adapta-2.1.1/pyproject.toml` & `adapta-2.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "adapta"
-version = "2.1.1"
+version = "2.2.0"
 description = "Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier."
 authors = ["ECCO Sneaks & Data <esdsupport@ecco.com>"]
 maintainers = ['GZU <gzu@ecco.com>', 'JRB <ext-jrb@ecco.com>']
 license = 'Apache 2.0'
 readme = "README.md"
 repository = 'https://github.com/SneaksAndData/adapta'
 
 [tool.poetry.dependencies]
-python = ">=3.9, <3.11"
+python = ">=3.9, <3.12"
 requests = "^2.26"
 backoff = "^2.2"
 cryptography = "~36.0"
-pandas = ">1.3,<1.5"
+pandas = ">=1.5,<2.0"
 pyarrow = ">=7.0"
 dataclasses-json = "~0.5.7"
 
 deltalake = { version = "~0.8.1", optional = true }
 
 azure-identity = { version = "~1.7", optional = true }
 azure-storage-blob = { version = ">12.7.0,<=12.10.0", optional = true }
@@ -80,15 +80,14 @@
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1"
 pytest-mock = "~3.6.1"
 pytest-cov = "~2.12"
 pylint = "^2.12"
 cryptography = "~36.0"
-pandas = "~1.4.1"
 black = "^22"
 
 [tool.black]
 line-length = 120
 
 [build-system]
 requires = ["poetry-core>=1.2.0"]
```

### Comparing `adapta-2.1.1/PKG-INFO` & `adapta-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: adapta
-Version: 2.1.1
+Version: 2.2.0
 Summary: Logging, data connectors, monitoring, secret handling and general lifehacks to make data people lives easier.
 Home-page: https://github.com/SneaksAndData/adapta
 License: Apache 2.0
 Author: ECCO Sneaks & Data
 Author-email: esdsupport@ecco.com
 Maintainer: GZU
 Maintainer-email: gzu@ecco.com
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: azure
 Provides-Extra: caching
 Provides-Extra: databases
 Provides-Extra: datadog
 Provides-Extra: hashicorp
 Provides-Extra: ml
 Provides-Extra: storage
@@ -33,15 +34,15 @@
 Requires-Dist: dataclasses-json (>=0.5.7,<0.6.0)
 Requires-Dist: datadog (>=0.44.0,<0.45.0) ; extra == "datadog"
 Requires-Dist: datadog-api-client (>=1.12.0,<1.13.0) ; extra == "datadog"
 Requires-Dist: deltalake (>=0.8.1,<0.9.0) ; extra == "storage"
 Requires-Dist: fsspec (==2022.8.2)
 Requires-Dist: hvac (==0.11.2) ; extra == "hashicorp"
 Requires-Dist: mlflow-skinny (>=1.28,<1.29) ; extra == "ml"
-Requires-Dist: pandas (>1.3,<1.5)
+Requires-Dist: pandas (>=1.5,<2.0)
 Requires-Dist: pyarrow (>=7.0)
 Requires-Dist: pyodbc (>=4.0,<4.1) ; extra == "databases"
 Requires-Dist: redis[hiredis] (>=4.4.0,<4.5.0) ; extra == "caching"
 Requires-Dist: requests (>=2.26,<3.0)
 Requires-Dist: trino[sqlalchemy] (==0.319.0) ; extra == "trino"
 Project-URL: Repository, https://github.com/SneaksAndData/adapta
 Description-Content-Type: text/markdown
```

