# Comparing `tmp/turing-sdk-0.8.0rc1.tar.gz` & `tmp/turing-sdk-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/turing-sdk-0.8.0rc1.tar", last modified: Tue Jan 31 10:27:46 2023, max compression
+gzip compressed data, was "dist/turing-sdk-0.9.0rc1.tar", last modified: Tue Apr 18 05:46:35 2023, max compression
```

## Comparing `turing-sdk-0.8.0rc1.tar` & `turing-sdk-0.9.0rc1.tar`

### file list

```diff
@@ -1,143 +1,143 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/tests/fixtures/gcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/tests/fixtures/mlflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/_base_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/batch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/batch/config/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/batch/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/batch/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/batch/config/sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/batch/config/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/batch/job.py
--rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/ensembler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/generated/
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/generated/api/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/api/ensembler_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/api/ensembling_job_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/api/project_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    65466 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/api/router_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    36846 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/generated/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      656 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/generated/model/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/autoscaling_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_dataset_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_dataset_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_sink_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/big_query_sink_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/default_traffic_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_config_kind.py
--rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_docker_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_infra_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_job_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_pyfunc_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_standard_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_standard_config_experiment_mappings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembler_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensemblers_paginated_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensemblers_paginated_results_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensemblers_paginated_results_all_of1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_ensembler_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_ensembler_spec_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_paginated_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_paginated_results_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_prediction_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_prediction_source_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_result_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/ensembling_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/field_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/generic_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/generic_ensembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/generic_sink.py
--rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/id_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/job_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/kafka_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/label.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/log_level.py
--rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/pagination_paging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/py_func_ensembler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/py_func_ensembler_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/result_logger_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_details.py
--rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_details_all_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_ensembler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_id_and_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_id_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_version_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_version_config_log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_version_log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/router_version_status.py
--rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/save_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/traffic_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model/traffic_rule_condition.py
--rw-r--r--   0 runner    (1001) docker     (123)    74809 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/generated/models/
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/generated/rest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/router/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/router/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/autoscaling_policy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing/router/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/common/env_var.py
--rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/enricher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8296 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/log_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/resource_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/route.py
--rw-r--r--   0 runner    (1001) docker     (123)    16105 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/router_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    23502 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/router_ensembler_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/router_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/config/traffic_rule.py
--rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/router/router.py
--rw-r--r--   0 runner    (1001) docker     (123)    12009 2023-01-31 10:27:06.000000 turing-sdk-0.8.0rc1/turing/session.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-01-31 10:27:45.000000 turing-sdk-0.8.0rc1/turing/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-31 10:27:46.000000 turing-sdk-0.8.0rc1/turing_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/tests/fixtures/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2253 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/tests/fixtures/mlflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2923 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/_base_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/batch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/batch/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/batch/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/batch/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/batch/config/sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/batch/config/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4517 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/batch/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16147 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/ensembler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/generated/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/generated/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20675 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/api/ensembler_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20603 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/api/ensembling_job_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/api/project_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65466 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/api/router_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36846 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/generated/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      656 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16178 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5116 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/generated/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6952 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/autoscaling_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9300 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7055 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_dataset_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7188 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_dataset_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9734 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7065 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_sink_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/big_query_sink_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9269 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6630 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/default_traffic_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10593 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6837 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_config_kind.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_docker_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7645 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_infra_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7453 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_job_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8052 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_pyfunc_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_standard_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_standard_config_experiment_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6741 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembler_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9405 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensemblers_paginated_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensemblers_paginated_results_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensemblers_paginated_results_all_of1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8831 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7059 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_ensembler_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_ensembler_spec_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_paginated_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6751 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_paginated_results_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9370 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_prediction_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_prediction_source_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7151 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_result_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7890 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/ensembling_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6787 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/field_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6685 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/generic_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/generic_ensembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7107 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/generic_sink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6498 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/id_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6759 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/job_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7512 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/kafka_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6629 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/log_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6892 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/pagination_paging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8014 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10604 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/py_func_ensembler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7242 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/py_func_ensembler_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7347 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/result_logger_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7578 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_details.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6711 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_details_all_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8259 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_ensembler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_id_and_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_id_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6926 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11468 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10067 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_version_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7397 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_version_config_log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8220 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_version_log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/router_version_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7069 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/save_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7152 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/traffic_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7867 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model/traffic_rule_condition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74809 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/generated/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/generated/rest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/router/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/router/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/autoscaling_policy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing/router/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/common/env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5236 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/enricher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8659 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/log_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/resource_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/route.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17334 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/router_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23561 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/router_ensembler_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/router_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7392 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/config/traffic_rule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8880 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/router/router.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11963 2023-04-18 05:45:53.000000 turing-sdk-0.9.0rc1/turing/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-18 05:46:34.000000 turing-sdk-0.9.0rc1/turing/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4981 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 05:46:35.000000 turing-sdk-0.9.0rc1/turing_sdk.egg-info/top_level.txt
```

### Comparing `turing-sdk-0.8.0rc1/PKG-INFO` & `turing-sdk-0.9.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turing-sdk
-Version: 0.8.0rc1
+Version: 0.9.0rc1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Introduction
         The Turing SDK is a Python tool for interacting with the Turing API, and complements the existing Turing UI available 
         for managing router creation, deployment, versioning, etc.
```

### Comparing `turing-sdk-0.8.0rc1/README.md` & `turing-sdk-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/setup.py` & `turing-sdk-0.9.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/tests/fixtures/gcs.py` & `turing-sdk-0.9.0rc1/tests/fixtures/gcs.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/tests/fixtures/mlflow.py` & `turing-sdk-0.9.0rc1/tests/fixtures/mlflow.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/__init__.py` & `turing-sdk-0.9.0rc1/turing/__init__.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/_base_types.py` & `turing-sdk-0.9.0rc1/turing/_base_types.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/batch/config/config.py` & `turing-sdk-0.9.0rc1/turing/batch/config/config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/batch/config/sink.py` & `turing-sdk-0.9.0rc1/turing/batch/config/sink.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/batch/config/source.py` & `turing-sdk-0.9.0rc1/turing/batch/config/source.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/batch/job.py` & `turing-sdk-0.9.0rc1/turing/batch/job.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/ensembler.py` & `turing-sdk-0.9.0rc1/turing/ensembler.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/__init__.py` & `turing-sdk-0.9.0rc1/turing/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/api/ensembler_api.py` & `turing-sdk-0.9.0rc1/turing/generated/api/ensembler_api.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/api/ensembling_job_api.py` & `turing-sdk-0.9.0rc1/turing/generated/api/ensembling_job_api.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/api/project_api.py` & `turing-sdk-0.9.0rc1/turing/generated/api/project_api.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/api/router_api.py` & `turing-sdk-0.9.0rc1/turing/generated/api/router_api.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/api_client.py` & `turing-sdk-0.9.0rc1/turing/generated/api_client.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/apis/__init__.py` & `turing-sdk-0.9.0rc1/turing/generated/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/configuration.py` & `turing-sdk-0.9.0rc1/turing/generated/configuration.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/exceptions.py` & `turing-sdk-0.9.0rc1/turing/generated/exceptions.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/autoscaling_policy.py` & `turing-sdk-0.9.0rc1/turing/generated/model/autoscaling_policy.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_dataset.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_dataset.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_dataset_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_dataset_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_dataset_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_dataset_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_sink.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_sink.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_sink_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_sink_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/big_query_sink_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/big_query_sink_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/dataset.py` & `turing-sdk-0.9.0rc1/turing/generated/model/dataset.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/default_traffic_rule.py` & `turing-sdk-0.9.0rc1/turing/generated/model/default_traffic_rule.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/enricher.py` & `turing-sdk-0.9.0rc1/turing/generated/model/enricher.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_config_kind.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_config_kind.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_docker_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_docker_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_infra_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_infra_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_job_status.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_job_status.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_pyfunc_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_pyfunc_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_standard_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_standard_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_standard_config_experiment_mappings.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_standard_config_experiment_mappings.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembler_type.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembler_type.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensemblers_paginated_results.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensemblers_paginated_results.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensemblers_paginated_results_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensemblers_paginated_results_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensemblers_paginated_results_all_of1.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensemblers_paginated_results_all_of1.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_ensembler_spec.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_ensembler_spec.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_ensembler_spec_result.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_ensembler_spec_result.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_meta.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_meta.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_paginated_results.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_paginated_results.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_paginated_results_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_paginated_results_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_prediction_source.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_prediction_source.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_prediction_source_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_prediction_source_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_result_type.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_result_type.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_sink.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_sink.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_source.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_source.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_job_spec.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_job_spec.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/ensembling_resources.py` & `turing-sdk-0.9.0rc1/turing/generated/model/ensembling_resources.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/env_var.py` & `turing-sdk-0.9.0rc1/turing/generated/model/env_var.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/event.py` & `turing-sdk-0.9.0rc1/turing/generated/model/event.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/experiment_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/experiment_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/field_source.py` & `turing-sdk-0.9.0rc1/turing/generated/model/field_source.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/generic_dataset.py` & `turing-sdk-0.9.0rc1/turing/generated/model/generic_dataset.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/generic_ensembler.py` & `turing-sdk-0.9.0rc1/turing/generated/model/generic_ensembler.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/generic_sink.py` & `turing-sdk-0.9.0rc1/turing/generated/model/generic_sink.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/id_object.py` & `turing-sdk-0.9.0rc1/turing/generated/model/id_object.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/job_id.py` & `turing-sdk-0.9.0rc1/turing/generated/model/job_id.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/kafka_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/kafka_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/label.py` & `turing-sdk-0.9.0rc1/turing/generated/model/label.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/log_level.py` & `turing-sdk-0.9.0rc1/turing/generated/model/log_level.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/pagination_paging.py` & `turing-sdk-0.9.0rc1/turing/generated/model/pagination_paging.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/project.py` & `turing-sdk-0.9.0rc1/turing/generated/model/project.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/protocol.py` & `turing-sdk-0.9.0rc1/turing/generated/model/protocol.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/py_func_ensembler.py` & `turing-sdk-0.9.0rc1/turing/generated/model/py_func_ensembler.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/py_func_ensembler_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/py_func_ensembler_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/resource_request.py` & `turing-sdk-0.9.0rc1/turing/generated/model/resource_request.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/result_logger_type.py` & `turing-sdk-0.9.0rc1/turing/generated/model/result_logger_type.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
             'NOP': "nop",
-            'CONSOLE': "console",
+            'UPI': "upi",
             'BIGQUERY': "bigquery",
             'KAFKA': "kafka",
         },
     }
 
     validations = {
     }
@@ -98,18 +98,18 @@
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
         """ResultLoggerType - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str): if omitted defaults to "nop", must be one of ["nop", "console", "bigquery", "kafka", ]  # noqa: E501
+            args[0] (str): if omitted defaults to "nop", must be one of ["nop", "upi", "bigquery", "kafka", ]  # noqa: E501
 
         Keyword Args:
-            value (str): if omitted defaults to "nop", must be one of ["nop", "console", "bigquery", "kafka", ]  # noqa: E501
+            value (str): if omitted defaults to "nop", must be one of ["nop", "upi", "bigquery", "kafka", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/route.py` & `turing-sdk-0.9.0rc1/turing/generated/model/route.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_details.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_details.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_details_all_of.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_details_all_of.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_ensembler_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_ensembler_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_events.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_events.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_id.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_id.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_id_and_version.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_id_and_version.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_id_object.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_id_object.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_status.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_status.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_version.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_version.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_version_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_version_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_version_config_log_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_version_config_log_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_version_log_config.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_version_log_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/router_version_status.py` & `turing-sdk-0.9.0rc1/turing/generated/model/router_version_status.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/save_mode.py` & `turing-sdk-0.9.0rc1/turing/generated/model/save_mode.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/traffic_rule.py` & `turing-sdk-0.9.0rc1/turing/generated/model/traffic_rule.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model/traffic_rule_condition.py` & `turing-sdk-0.9.0rc1/turing/generated/model/traffic_rule_condition.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/model_utils.py` & `turing-sdk-0.9.0rc1/turing/generated/model_utils.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/models/__init__.py` & `turing-sdk-0.9.0rc1/turing/generated/models/__init__.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/generated/rest.py` & `turing-sdk-0.9.0rc1/turing/generated/rest.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/project.py` & `turing-sdk-0.9.0rc1/turing/project.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/autoscaling_policy.py` & `turing-sdk-0.9.0rc1/turing/router/config/autoscaling_policy.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/common/env_var.py` & `turing-sdk-0.9.0rc1/turing/router/config/common/env_var.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/enricher.py` & `turing-sdk-0.9.0rc1/turing/router/config/enricher.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/experiment_config.py` & `turing-sdk-0.9.0rc1/turing/router/config/experiment_config.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/log_config.py` & `turing-sdk-0.9.0rc1/turing/router/config/log_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from dataclasses import dataclass
 from typing import Optional, Dict, Union
 from turing.generated.model_utils import OpenApiModel
 
 
 class ResultLoggerType(Enum):
     NOP = "nop"
-    CONSOLE = "console"
+    UPI = "upi"
     BIGQUERY = "bigquery"
     KAFKA = "kafka"
 
     def to_open_api(self) -> OpenApiModel:
         return turing.generated.models.ResultLoggerType(self.value)
 
 
@@ -109,14 +109,22 @@
         if (
             self.result_logger_type == ResultLoggerType.KAFKA
             and self.bigquery_config is not None
         ):
             raise InvalidResultLoggerTypeAndConfigCombination(
                 f"bigquery_config must be set to None when result_logger_type is: {self.result_logger_type}"
             )
+        if (
+            self.result_logger_type == ResultLoggerType.UPI
+            and self.kafka_config is not None
+            and self.bigquery_config is not None
+        ):
+            raise InvalidResultLoggerTypeAndConfigCombination(
+                f"kafka/bigquery config must be set to None when result_logger_type is: {self.result_logger_type}"
+            )
 
 
 class InvalidResultLoggerTypeAndConfigCombination(Exception):
     pass
 
 
 @dataclass
```

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/resource_request.py` & `turing-sdk-0.9.0rc1/turing/router/config/resource_request.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/route.py` & `turing-sdk-0.9.0rc1/turing/router/config/route.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/router_config.py` & `turing-sdk-0.9.0rc1/turing/router/config/router_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,17 @@
     ):
         if isinstance(log_config, LogConfig):
             self._log_config = log_config
         elif isinstance(log_config, dict):
             self._log_config = LogConfig(**log_config)
         else:
             self._log_config = log_config
+        # Verify that only nop or UPI logger is configured for UPI router
+        if self._protocol == Protocol.UPI:
+            self._verify_upi_router_logger()
 
     @property
     def enricher(self) -> Enricher:
         return self._enricher
 
     @enricher.setter
     def enricher(self, enricher: Union[Enricher, Dict]):
@@ -336,14 +339,17 @@
                 )
             elif self._ensembler.type == "pyfunc" and not isinstance(
                 self._ensembler, PyfuncRouterEnsemblerConfig
             ):
                 self._ensembler = PyfuncRouterEnsemblerConfig.from_config(
                     self._ensembler.pyfunc_config
                 )
+        # Verify that only nop or standard ensembler is configured for UPI router
+        if self._protocol == Protocol.UPI:
+            self._verify_upi_router_ensembler()
 
     def to_open_api(self) -> OpenApiModel:
         kwargs = {}
         self._verify_no_duplicate_routes()
 
         # Get default route id if exists
         default_route_id = self._get_default_route_id()
@@ -402,14 +408,34 @@
         route_id_counter = Counter(route.id for route in self.routes)
         most_common_route_id, max_frequency = route_id_counter.most_common(n=1)[0]
         if max_frequency > 1:
             raise turing.router.config.route.DuplicateRouteException(
                 f"Routes with duplicate ids are specified for this traffic rule. Duplicate id: {most_common_route_id}"
             )
 
+    def _verify_upi_router_ensembler(self):
+        # only nop and standard ensembler is allowed
+        if not (
+            isinstance(self.ensembler, NopRouterEnsemblerConfig)
+            or isinstance(self.ensembler, StandardRouterEnsemblerConfig)
+        ):
+            raise turing.router.config.router_ensembler_config.InvalidEnsemblerTypeException(
+                f"UPI router only supports no ensembler or standard ensembler."
+            )
+
+    def _verify_upi_router_logger(self):
+        # only nop or upi logger type is allowed
+        if not (
+            self.log_config.result_logger_type == ResultLoggerType.NOP
+            or self.log_config.result_logger_type == ResultLoggerType.UPI
+        ):
+            raise turing.router.config.log_config.InvalidResultLoggerTypeAndConfigCombination(
+                f"UPI router only supports no logging or UPI logger"
+            )
+
     def to_dict(self):
         att_dict = {}
         for m in inspect.getmembers(self):
             if not inspect.ismethod(m[VALUE_INDEX]) and not m[NAME_INDEX].startswith(
                 "_"
             ):
                 att_dict[m[NAME_INDEX]] = m[VALUE_INDEX]
```

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/router_ensembler_config.py` & `turing-sdk-0.9.0rc1/turing/router/config/router_ensembler_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,7 +658,11 @@
         # Nop config is not passed down to the API. The final_response_route_id property
         # will be parsed in the router config and copied over as appropriate.
         return None
 
 
 class InvalidExperimentMappingException(Exception):
     pass
+
+
+class InvalidEnsemblerTypeException(Exception):
+    pass
```

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/router_version.py` & `turing-sdk-0.9.0rc1/turing/router/config/router_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,17 @@
         self.version = version
         self.created_at = created_at
         self.updated_at = updated_at
         self.environment_name = environment_name
         self.status = RouterStatus(status)
         self.name = name
         self.monitoring_url = monitoring_url
-        self.log_config = RouterVersionLogConfig(**kwargs.get("log_config"))
+        # RouterConfig has to be init first as RouterVersionLogConfig will check fields that exist in RouterConfig
         super().__init__(environment_name=environment_name, name=name, **kwargs)
+        self.log_config = RouterVersionLogConfig(**kwargs.get("log_config"))
 
     def get_config(self) -> RouterConfig:
         """
         Generates a RouterConfig instance from the attributes contained in this object; NOTE that the name and
         environment_name of this version gets passed to the generated RouterConfig. This means that if you were to use
         the generated RouterConfig for another instance, you would have to change its name, and also maybe its
         environment_name
```

### Comparing `turing-sdk-0.8.0rc1/turing/router/config/traffic_rule.py` & `turing-sdk-0.9.0rc1/turing/router/config/traffic_rule.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/router/router.py` & `turing-sdk-0.9.0rc1/turing/router/router.py`

 * *Files identical despite different names*

### Comparing `turing-sdk-0.8.0rc1/turing/session.py` & `turing-sdk-0.9.0rc1/turing/session.py`

 * *Files 3% similar despite different names*

```diff
@@ -35,36 +35,33 @@
 
 
 class TuringSession:
     """
     Session object for interacting with Turing back-end
     """
 
-    OAUTH_SCOPES = ["https://www.googleapis.com/auth/userinfo.email"]
-
     def __init__(
         self, host: str, project_name: str = None, use_google_oauth: bool = True
     ):
         """
         Create new session
 
         :param host: URL of Turing API
         :param project_name: name of the project, this session should stick to
         :param use_google_oauth: should be True if Turing API is protected with Google OAuth
         """
         config = Configuration(host=os.path.join(host, "v1"))
         self._api_client = ApiClient(config)
 
         if use_google_oauth:
-            import google.auth
+            from caraml_auth.id_token_credentials import get_default_id_token_credentials
             from google.auth.transport.requests import Request
             from google.auth.transport.urllib3 import urllib3, AuthorizedHttp
 
-            # Load default credentials
-            credentials, _ = google.auth.default(scopes=TuringSession.OAUTH_SCOPES)
+            credentials = get_default_id_token_credentials(target_audience="sdk.caraml")
             # Refresh credentials, in case it's coming from Compute Engine.
             # See: https://github.com/googleapis/google-auth-library-python/issues/1211
             credentials.refresh(Request())
 
             authorized_http = AuthorizedHttp(credentials, urllib3.PoolManager())
             self._api_client.rest_client.pool_manager = authorized_http
```

### Comparing `turing-sdk-0.8.0rc1/turing_sdk.egg-info/PKG-INFO` & `turing-sdk-0.9.0rc1/turing_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turing-sdk
-Version: 0.8.0rc1
+Version: 0.9.0rc1
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Introduction
         The Turing SDK is a Python tool for interacting with the Turing API, and complements the existing Turing UI available 
         for managing router creation, deployment, versioning, etc.
```

### Comparing `turing-sdk-0.8.0rc1/turing_sdk.egg-info/SOURCES.txt` & `turing-sdk-0.9.0rc1/turing_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

