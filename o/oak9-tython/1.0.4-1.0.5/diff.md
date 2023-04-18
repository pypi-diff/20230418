# Comparing `tmp/oak9_tython-1.0.4.tar.gz` & `tmp/oak9_tython-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oak9_tython-1.0.4.tar", last modified: Mon Apr 17 20:43:26 2023, max compression
+gzip compressed data, was "oak9_tython-1.0.5.tar", last modified: Tue Apr 18 15:43:39 2023, max compression
```

## Comparing `oak9_tython-1.0.4.tar` & `oak9_tython-1.0.5.tar`

### file list

```diff
@@ -1,1167 +1,1167 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.433546 oak9_tython-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-17 20:43:26.433546 oak9_tython-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.209544 oak9_tython-1.0.4/oak9/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.209544 oak9_tython-1.0.4/oak9/tython/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.209544 oak9_tython-1.0.4/oak9/tython/core/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/blueprint_meta_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_repo_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/empty_implements_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/no_implements_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.213544 oak9_tython-1.0.4/oak9/tython/core/cf_types/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/cf_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/cf_types/capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.217544 oak9_tython-1.0.4/oak9/tython/core/sdk/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/sdk/graph_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/sdk/helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/sdk/resource_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.217544 oak9_tython-1.0.4/oak9/tython/core/services/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/services/runner_input_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    31762 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/types_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5887 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/core/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.217544 oak9_tython-1.0.4/oak9/tython/models/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.293545 oak9_tython-1.0.4/oak9/tython/models/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_accessanalyzer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_accessanalyzer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_acmpca_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_acmpca_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_acmpca_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_alexa_ask_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_alexa_ask_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_amazonmq_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_amazonmq_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_amazonmq_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_amplify_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_amplify_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_amplify_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31462 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigateway_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    85923 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigateway_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigateway_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigatewayv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigatewayv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appconfig_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appconfig_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appconfig_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    88173 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationautoscaling_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationinsights_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationinsights_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    39964 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appmesh_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   115709 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appmesh_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appmesh_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appsync_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41375 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appsync_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_appsync_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_athena_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_athena_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_athena_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscaling_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscaling_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscaling_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscalingplans_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscalingplans_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_batch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_batch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_batch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_budgets_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_budgets_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_budgets_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cassandra_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cassandra_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cassandra_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_certificatemanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_certificatemanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_chatbot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_chatbot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_chatbot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloud9_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloud9_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloud9_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudformation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudformation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudformation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudfront_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    68732 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudfront_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudfront_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudtrail_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudtrail_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudwatch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudwatch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codebuild_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38727 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codebuild_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codebuild_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codecommit_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codecommit_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codecommit_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codedeploy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codedeploy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codedeploy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codeguruprofiler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codegurureviewer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codegurureviewer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codepipeline_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codepipeline_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codepipeline_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarconnections_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarconnections_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarnotifications_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarnotifications_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cognito_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    87415 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cognito_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_cognito_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_config_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    46100 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_config_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_config_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_datapipeline_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_datapipeline_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_datapipeline_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_detective_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_detective_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_detective_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_directoryservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_directoryservice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_directoryservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dlm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dlm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dlm_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    32336 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_docdb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_docdb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_docdb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_table_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_table_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    64868 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_instance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_networkacl_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    70103 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   219118 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_securitygroup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_subnet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_subnet_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecr_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28648 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    86946 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_efs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_efs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_efs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_eks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_eks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_eks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticbeanstalk_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    60919 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticsearch_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticsearch_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_emr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    85681 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_emr_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_emr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_events_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_events_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_events_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_eventschemas_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_eventschemas_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_eventschemas_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_fms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_fms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_fms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_fsx_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_fsx_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_fsx_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_gamelift_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_gamelift_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_gamelift_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_globalaccelerator_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_globalaccelerator_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    35328 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_glue_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   104308 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_glue_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_glue_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    36639 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_greengrass_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   102539 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_greengrass_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_greengrass_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_groundstation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_groundstation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_groundstation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_guardduty_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_guardduty_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_guardduty_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iam_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_imagebuilder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33357 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_imagebuilder_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_inspector_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_inspector_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_inspector_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot1click_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot1click_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot1click_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57057 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotanalytics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    56169 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotanalytics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotevents_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39864 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotevents_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotevents_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalytics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20301 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    56745 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    60879 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisfirehose_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_kms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_lakeformation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_lakeformation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_lakeformation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_lambda_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38931 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_lambda_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_lambda_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_logs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_logs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_logs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_macie_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_macie_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_macie_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_managedblockchain_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_managedblockchain_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_mediaconvert_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_mediaconvert_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_msk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_msk_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_msk_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_neptune_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_neptune_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_neptune_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_networkmanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_networkmanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_networkmanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    56713 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworkscm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworkscm_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_qldb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_qldb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_qldb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ram_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ram_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ram_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38105 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbcluster_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbinstance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_redshift_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_redshift_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_redshift_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_resourcegroups_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_resourcegroups_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_robomaker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_robomaker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_robomaker_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53resolver_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53resolver_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53resolver_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25507 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_s3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    78676 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_s3_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_s3_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22303 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sagemaker_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    66680 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sagemaker_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sagemaker_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sdb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sdb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sdb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_secretsmanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_secretsmanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_securityhub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_securityhub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_securityhub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicecatalog_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicecatalog_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicediscovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicediscovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sns_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sns_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sns_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sqs_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sqs_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sqs_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ssm_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ssm_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_ssm_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sso_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sso_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_sso_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_stepfunctions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_stepfunctions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_synthetics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_synthetics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_synthetics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_transfer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_transfer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_transfer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_waf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_waf_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_waf_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafregional_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafregional_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafregional_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafv2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   117299 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafv2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafv2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_workspaces_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_workspaces_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/aws/aws_workspaces_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.321545 oak9_tython-1.0.4/oak9/tython/models/azure/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_aad_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_aad_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    49201 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   143537 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    71546 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30626 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cache_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cache_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    71498 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cdn_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    34710 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    67043 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    47220 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   120178 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45682 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30190 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    84581 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_devices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39037 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_devices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    62661 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   158843 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_documentdb_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_elastic_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30105 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    47435 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40962 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_keyvault_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23604 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    63082 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    59960 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23525 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)   101699 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   301469 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18672 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    45382 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    45963 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   131181 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31831 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40696 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    44588 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_servicebus_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    63020 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    68845 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    31681 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_storage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    91315 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_storage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    75724 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_web_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   231864 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_web_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.405546 oak9_tython-1.0.4/oak9/tython/models/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45414 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_access_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   115626 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_access_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_access_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_active_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_active_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_active_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apigee_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apigee_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apigee_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apikeys_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apikeys_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    30961 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_app_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    80283 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_app_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_app_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_artifact_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_artifact_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_artifact_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_assured_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_assured_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_assured_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigquery_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   107299 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigquery_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigtable_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigtable_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_billing_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_billing_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_billing_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_binary_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_binary_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_binary_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_certificate_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_certificate_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_certificate_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    37530 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloud_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    96409 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloud_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloud_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudbuild_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_clouddeploy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudfunctions_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudiot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudiot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_composer_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_composer_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_composer_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_attached_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_attached_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_backend_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    39586 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_backend_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_disk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_disk_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_external_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_external_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_firewall_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_forwarding_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_global_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_global_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ha_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ha_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_health_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_health_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_http_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_http_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_https_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_https_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_image_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_image_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    42340 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_instance_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   110570 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_instance_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_interconnect_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_managed_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_managed_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_node_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_node_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_packet_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_packet_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_per_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_per_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_project_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    63992 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_region_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   170051 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_region_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_reservation_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_route_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_route_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_router_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_router_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_security_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_security_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_shared_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_shared_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_snapshot_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ssl_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_target_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_target_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    44049 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_url_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   112435 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_url_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_vpn_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    64469 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_container_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   166581 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_container_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_container_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    63657 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   146148 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_data_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataplex_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataplex_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    96272 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataproc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   222604 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataproc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_datastore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_datastore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_datastore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_deployment_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_deployment_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_deployment_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27903 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dialogflow_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    76337 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dialogflow_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dns_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dns_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dns_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_document_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_document_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_document_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_endpoints_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_endpoints_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_essential_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_essential_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_essential_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_eventarc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_eventarc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_filestore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_filestore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_filestore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firebaserules_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firebaserules_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firestore_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firestore_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firestore_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_folder_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_folder_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_folder_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_game_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_game_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_game_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_gke_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_gke_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_gke_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_container_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_healthcare_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_healthcare_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iam_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iam_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iam_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iap_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    55725 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iap_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iap_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_identity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27338 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_identity_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_identity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_kms_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25293 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_kms_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_kms_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_logging_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_logging_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_logging_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_memcache_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_memcache_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_memcache_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_ml_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_ml_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_ml_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_monitoring_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    81993 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_monitoring_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_network_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    62722 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_network_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_network_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_notebooks_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57020 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_notebooks_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_org_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_org_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_org_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_organization_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_organization_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_organization_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    39464 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_os_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    95395 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_os_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_os_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_privateca_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   110520 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_privateca_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_privateca_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_project_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_project_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_project_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_pubsub_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    41253 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_pubsub_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_recaptcha_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_recaptcha_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_redis_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_redis_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_redis_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_resource_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_scc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_scc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_scc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_secret_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_secret_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_secret_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sourcerepo_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_spanner_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_spanner_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_spanner_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sql_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sql_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sql_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_storage_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    66063 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_storage_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_storage_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tags_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tags_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tags_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tpu_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tpu_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tpu_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vertex_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vertex_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vertex_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vpc_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vpc_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vpc_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_workflows_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_workflows_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_workflows_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.413545 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    50422 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.417546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.417546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.417546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33586 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.417546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.417546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.417546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.421546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   105265 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)   323853 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.421546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.421546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.421546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.425546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    33982 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.425546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.425546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.425546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.425546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25542 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.425546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    30642 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38980 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    35874 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.429546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.433546 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apiserverinternal.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apps.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authorization.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.batch.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.certificates.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.coordination.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.core.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.discovery.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.events.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta2_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta3_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.node.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.policy.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.rbac.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.resource.v1alpha1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.scheduling.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1beta1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.apiextensionsapiserver.pkg.apis.apiextensions.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.api.resource_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.apis.meta.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.runtime_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.util.intstr_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.version_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io.k8s.kubeaggregator.pkg.apis.apiregistration.v1_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.433546 oak9_tython-1.0.4/oak9/tython/models/shared/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/shared/shared_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/shared/shared_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/oak9/tython/models/shared/shared_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-04-17 20:43:24.000000 oak9_tython-1.0.4/oak9/tython/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 20:43:26.433546 oak9_tython-1.0.4/oak9_tython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-17 20:43:26.000000 oak9_tython-1.0.4/oak9_tython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    60432 2023-04-17 20:43:26.000000 oak9_tython-1.0.4/oak9_tython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 20:43:26.000000 oak9_tython-1.0.4/oak9_tython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-17 20:43:26.000000 oak9_tython-1.0.4/oak9_tython.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 20:43:26.433546 oak9_tython-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-17 20:43:25.000000 oak9_tython-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    11303 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.197701 oak9_tython-1.0.5/oak9/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.197701 oak9_tython-1.0.5/oak9/tython/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1740 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/blueprint_meta_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5112 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_repo_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/empty_implements_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/no_implements_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/cf_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/cf_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/cf_types/capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.201701 oak9_tython-1.0.5/oak9/tython/core/sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/sdk/graph_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/sdk/helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29304 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/sdk/resource_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.205701 oak9_tython-1.0.5/oak9/tython/core/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/services/runner_input_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31762 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4553 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/types_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/core/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.205701 oak9_tython-1.0.5/oak9/tython/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.237701 oak9_tython-1.0.5/oak9/tython/models/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_accessanalyzer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_accessanalyzer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5141 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_acmpca_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13347 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_acmpca_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_acmpca_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_alexa_ask_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6812 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_alexa_ask_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_amazonmq_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25041 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_amazonmq_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_amazonmq_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6920 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_amplify_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_amplify_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_amplify_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31462 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigateway_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85923 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigateway_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigateway_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigatewayv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50555 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigatewayv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appconfig_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19678 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appconfig_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appconfig_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30951 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88173 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7076 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19467 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationautoscaling_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationinsights_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21374 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationinsights_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39964 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appmesh_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115709 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appmesh_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appmesh_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appsync_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41375 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appsync_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_appsync_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_athena_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18274 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_athena_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_athena_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13531 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscaling_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42606 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscaling_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscaling_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscalingplans_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18071 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscalingplans_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18382 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12345 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_batch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36233 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_batch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_batch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5367 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_budgets_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13698 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_budgets_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_budgets_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cassandra_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cassandra_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cassandra_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_certificatemanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_certificatemanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1661 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_chatbot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_chatbot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_chatbot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloud9_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4907 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloud9_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloud9_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7022 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudformation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20260 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudformation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudformation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22318 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudfront_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68732 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudfront_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudfront_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudtrail_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7057 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudtrail_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudwatch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21664 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudwatch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12808 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codebuild_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38727 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codebuild_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codebuild_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codecommit_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6979 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codecommit_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codecommit_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10304 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codedeploy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29770 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codedeploy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codedeploy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codeguruprofiler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codegurureviewer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codegurureviewer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10233 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codepipeline_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28478 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codepipeline_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codepipeline_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarconnections_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarconnections_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarnotifications_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4642 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarnotifications_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29385 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cognito_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87415 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cognito_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_cognito_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_config_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46100 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_config_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_config_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3716 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_datapipeline_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9518 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_datapipeline_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_datapipeline_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_detective_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_detective_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_detective_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_directoryservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7012 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_directoryservice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_directoryservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6454 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dlm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16200 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dlm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dlm_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10837 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32336 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5677 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_docdb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14512 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_docdb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_docdb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5269 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6223 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_table_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17149 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_table_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21091 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64868 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_instance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6707 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_networkacl_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70103 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   219118 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5351 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9142 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_securitygroup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_subnet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_subnet_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8411 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5960 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecr_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28648 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86946 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_efs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_efs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_efs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_eks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21226 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_eks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_eks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4115 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10982 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14970 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7602 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20565 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticbeanstalk_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6553 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17776 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21617 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60919 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticsearch_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21808 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticsearch_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_emr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85681 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_emr_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_emr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_events_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26337 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_events_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_events_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_eventschemas_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_eventschemas_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_eventschemas_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3513 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_fms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9096 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_fms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_fms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_fsx_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12187 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_fsx_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_fsx_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13358 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_gamelift_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41568 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_gamelift_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_gamelift_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3951 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_globalaccelerator_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9898 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_globalaccelerator_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35328 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_glue_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104308 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_glue_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_glue_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36639 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_greengrass_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   102539 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_greengrass_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_greengrass_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_groundstation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14785 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_groundstation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_groundstation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5644 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_guardduty_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_guardduty_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_guardduty_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21526 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iam_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_imagebuilder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33357 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_imagebuilder_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_inspector_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6824 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_inspector_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_inspector_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5276 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot1click_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10860 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot1click_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot1click_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19142 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57057 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19224 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotanalytics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56169 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotanalytics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13872 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotevents_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39864 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotevents_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotevents_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13201 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36688 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalytics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20301 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56745 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21240 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60879 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisfirehose_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9216 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_lakeformation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17321 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_lakeformation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_lakeformation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12835 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_lambda_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38931 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_lambda_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_lambda_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3515 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_logs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_logs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_logs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_macie_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_macie_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_macie_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_managedblockchain_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_managedblockchain_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_mediaconvert_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11898 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_mediaconvert_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8586 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_msk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25415 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_msk_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_msk_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7763 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_neptune_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20243 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_neptune_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_neptune_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_networkmanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18000 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_networkmanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_networkmanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19887 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56713 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworkscm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworkscm_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2973 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_qldb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_qldb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_qldb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ram_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ram_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ram_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12749 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38105 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbcluster_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41488 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbinstance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17496 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_redshift_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18711 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_redshift_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_redshift_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_resourcegroups_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_resourcegroups_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_robomaker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20021 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_robomaker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_robomaker_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22633 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53resolver_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12428 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53resolver_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53resolver_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25507 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_s3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78676 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_s3_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_s3_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22303 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sagemaker_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66680 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sagemaker_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sagemaker_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sdb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1749 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sdb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sdb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_secretsmanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13368 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_secretsmanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_securityhub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_securityhub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_securityhub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12610 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicecatalog_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36406 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicecatalog_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicediscovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16141 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicediscovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4287 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sns_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9867 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sns_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sns_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sqs_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sqs_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sqs_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20022 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ssm_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58274 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ssm_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_ssm_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2475 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sso_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sso_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_sso_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_stepfunctions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13061 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_stepfunctions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3605 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_synthetics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9251 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_synthetics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_synthetics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_transfer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12237 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_transfer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_transfer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8016 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_waf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24035 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_waf_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_waf_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafregional_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31254 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafregional_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafregional_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42450 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafv2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   117299 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafv2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafv2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_workspaces_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_workspaces_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/aws/aws_workspaces_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.253701 oak9_tython-1.0.5/oak9/tython/models/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_aad_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12672 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_aad_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49201 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   143537 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25696 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71546 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11299 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30626 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cache_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20103 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cache_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24555 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71498 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cdn_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13303 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34710 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24988 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    67043 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47220 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120178 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17128 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45682 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30190 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84581 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14370 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_devices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39037 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_devices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62661 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158843 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_documentdb_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12551 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_elastic_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11170 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30105 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18584 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47435 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14542 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40962 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_keyvault_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4216 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27988 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    74977 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22861 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59960 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7569 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17773 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4062 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13919 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39073 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8504 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23525 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101699 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   301469 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18672 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45382 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4836 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11094 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10959 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45963 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   131181 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8631 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23980 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31831 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14385 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40696 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44588 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_servicebus_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21076 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63020 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18795 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52816 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11732 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23111 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68845 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31681 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_storage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    91315 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_storage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9815 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26168 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75724 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_web_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   231864 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_web_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.289700 oak9_tython-1.0.5/oak9/tython/models/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45414 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_access_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115626 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_access_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_access_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_active_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7619 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_active_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_active_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8937 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apigee_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25139 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apigee_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apigee_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apikeys_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apikeys_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30961 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_app_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80283 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_app_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_app_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5128 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_artifact_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12241 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_artifact_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_artifact_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_assured_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7184 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_assured_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_assured_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37001 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigquery_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   107299 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigquery_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9900 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigtable_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27966 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigtable_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_billing_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20649 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_billing_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_billing_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7668 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_binary_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19474 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_binary_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_binary_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8570 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_certificate_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18218 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_certificate_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_certificate_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37530 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloud_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96409 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloud_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloud_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15790 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40556 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudbuild_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7100 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15497 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_clouddeploy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8924 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21782 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudfunctions_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10349 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudiot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24504 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudiot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11922 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_composer_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26830 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_composer_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_composer_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_attached_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_attached_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11618 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_backend_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39586 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_backend_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_disk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18576 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_disk_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_external_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_external_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6890 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_firewall_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3546 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_forwarding_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6270 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_global_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15306 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_global_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ha_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3978 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ha_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_health_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13681 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_health_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_http_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_http_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_https_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_https_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5123 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_image_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12943 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_image_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42340 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_instance_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110570 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_instance_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6921 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_interconnect_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_managed_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4463 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_managed_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15279 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_node_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11015 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_node_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_packet_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8366 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_packet_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3236 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_per_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6175 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_per_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63992 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_region_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   170051 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_region_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4600 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9971 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_reservation_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16511 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_route_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_route_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_router_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21517 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_router_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_security_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15857 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_security_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6463 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_shared_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4190 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_shared_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_snapshot_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6795 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ssl_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_target_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22344 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_target_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44049 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_url_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112435 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_url_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_vpn_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64469 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_container_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166581 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_container_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_container_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63657 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146148 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_data_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7537 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6851 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataplex_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16028 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataplex_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96272 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataproc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   222604 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataproc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_datastore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_datastore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_datastore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3279 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_deployment_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_deployment_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_deployment_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27903 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dialogflow_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76337 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dialogflow_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8058 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dns_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21255 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dns_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dns_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_document_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_document_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_document_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_endpoints_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17507 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_endpoints_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_essential_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_essential_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_essential_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4398 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_eventarc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9933 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_eventarc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_filestore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8236 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_filestore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_filestore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firebaserules_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firebaserules_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firestore_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firestore_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firestore_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8264 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_folder_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22601 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_folder_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_folder_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_game_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25773 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_game_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_game_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_gke_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_gke_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_gke_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4257 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_container_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2147 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5311 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2143 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2099 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20029 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_healthcare_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54960 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_healthcare_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iam_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9133 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iam_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iam_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18718 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iap_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55725 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iap_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iap_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11359 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_identity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27338 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_identity_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_identity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9327 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_kms_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25293 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_kms_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_kms_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14681 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_logging_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41658 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_logging_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_logging_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5977 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_memcache_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12666 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_memcache_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_memcache_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_ml_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_ml_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_ml_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32793 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_monitoring_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81993 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_monitoring_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25569 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_network_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62722 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_network_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_network_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21893 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_notebooks_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57020 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_notebooks_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3065 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_org_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_org_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_org_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_organization_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22030 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_organization_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_organization_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39464 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_os_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95395 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_os_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_os_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42045 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_privateca_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110520 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_privateca_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_privateca_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12149 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_project_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33462 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_project_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_project_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_pubsub_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41253 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_pubsub_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3867 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_recaptcha_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_recaptcha_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6108 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_redis_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14339 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_redis_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_redis_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_resource_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_scc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_scc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_scc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7245 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_secret_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_secret_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_secret_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17204 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10257 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sourcerepo_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_spanner_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20855 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_spanner_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_spanner_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sql_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37529 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sql_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sql_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23694 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_storage_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66063 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_storage_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_storage_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6904 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tags_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19373 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tags_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tags_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tpu_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tpu_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tpu_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vertex_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vertex_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vertex_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vpc_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vpc_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vpc_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_workflows_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_workflows_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_workflows_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6438 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17234 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6603 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16974 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17232 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50422 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11838 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7683 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20317 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12861 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33586 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.293700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8782 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24958 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9615 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   105265 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)   323853 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10238 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10235 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12278 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33982 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3778 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7157 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4793 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10116 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18427 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9473 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25542 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.297700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11266 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30642 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38980 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1001 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35874 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2204 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4138 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.admissionregistration.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apiserverinternal.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.apps.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authentication.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.authorization.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.autoscaling.v2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.batch.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.certificates.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.coordination.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.core.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.discovery.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.events.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta2_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.flowcontrol.v1beta3_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.networking.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.node.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.policy.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.rbac.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.resource.v1alpha1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.scheduling.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.api.storage.v1beta1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.apiextensionsapiserver.pkg.apis.apiextensions.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.api.resource_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.apis.meta.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.runtime_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.util.intstr_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.apimachinery.pkg.version_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io.k8s.kubeaggregator.pkg.apis.apiregistration.v1_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9/tython/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14203 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/shared/shared_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49220 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/shared/shared_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2501 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/models/shared/shared_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4736 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/oak9/tython/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/oak9_tython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-18 15:43:39.000000 oak9_tython-1.0.5/oak9_tython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    60432 2023-04-18 15:43:39.000000 oak9_tython-1.0.5/oak9_tython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 15:43:39.000000 oak9_tython-1.0.5/oak9_tython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 15:43:39.000000 oak9_tython-1.0.5/oak9_tython.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 15:43:39.301700 oak9_tython-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-04-18 15:43:36.000000 oak9_tython-1.0.5/setup.py
```

### Comparing `oak9_tython-1.0.4/LICENSE` & `oak9_tython-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/PKG-INFO` & `oak9_tython-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oak9_tython
-Version: 1.0.4
+Version: 1.0.5
 Author: ['Claudio Balbin <cbalbin@oak9.io>', 'Brandon Nicoll <bnicoll@oak9.io>']
 Project-URL: Homepage, https://github.com/oak9io/tython
 Project-URL: Bug Tracker, https://github.com/oak9io/tython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `oak9_tython-1.0.4/README.md` & `oak9_tython-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/blueprint_docstring.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/customer_blueprint_repo_test.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/git_utils.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/git_utils.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/multiple_policies_per_file_repo.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_implementation_docstring_test.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_repo.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_repo.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/policy_repo_test.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/policy_repo_test.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/python_source_file_utils.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/docstring_at_the_function_level.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/no_docstring_for_module.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/docstring/well_formed_single_docstring_for_module_and_function.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/aws/well_formed_aws_config_implementation.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/azure/well_formed_implements_field_multiple_values.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/sparce_implementation_class.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_aws_config_implementation.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_multiple_values.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_field_single_value_with_a_space_after_implements.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py` & `oak9_tython-1.0.5/oak9/tython/core/bp_metadata_utils/testdata/oak9/well_formed_implements_single_func.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/exception.py` & `oak9_tython-1.0.5/oak9/tython/core/exception.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/logger.py` & `oak9_tython-1.0.5/oak9/tython/core/logger.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/sdk/graph_helper.py` & `oak9_tython-1.0.5/oak9/tython/core/sdk/graph_helper.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/sdk/helper.py` & `oak9_tython-1.0.5/oak9/tython/core/sdk/helper.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/sdk/resource_map.py` & `oak9_tython-1.0.5/oak9/tython/core/sdk/resource_map.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/services/runner_input_service.py` & `oak9_tython-1.0.5/oak9/tython/core/services/runner_input_service.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,28 +5,26 @@
 from core.types import Finding
 
 class RunnerInputService:
     '''
     Provides access to the runner input data
     '''
 
-    def fetch_runner_input(argsObj):
+    def fetch_runner_input(args_obj):
         # TODO: WARNING - MUST REPLACE WITH PROD URL ONLY BEFORE RELEASE!!!!
         endpoint = "https://devapi.oak9.cloud/console/"
 
-        # TODO: Safety check the values in the argsObj. No reason to call the API
-        # if any of these values are missing/invalid
-        if argsObj["data_endpoint"] != None and argsObj["data_endpoint"] != "":
-            endpoint = argsObj['data_endpoint']
+        if "data_endpoint" in args_obj and args_obj["data_endpoint"] != "":
+            endpoint = args_obj['data_endpoint']
 
-        url = f"{endpoint}{argsObj['org_id']}/sac/{argsObj['project_id']}/runnerinput/"
-        response = requests.get(url, auth=(argsObj['org_id'], argsObj['api_key']))
+        url = f"{endpoint}{args_obj['org_id']}/sac/{args_obj['project_id']}/runnerinput/"
+        response = requests.get(url, auth=(args_obj['org_id'], args_obj['api_key']))
 
         if response.status_code == 401:
-            print(f"WARNING: Unable to fetch {argsObj['project_id']} data, please verify your credentials.")
+            print(f"WARNING: Unable to fetch {args_obj['project_id']} data, please verify your credentials.")
             return []
 
         runner_inputs = []
 
         raw_snake_case_input = Helper.snake_case_json(response.json())
 
         for raw_item in raw_snake_case_input:
@@ -35,18 +33,23 @@
                 root_node['node']['resource']['data']['value'] = bytes(root_node['node']['resource']['data']['value'])
             Helper.remove_attributes(item, "has_")
             runner_inputs.append(RunnerInput(**item))
 
         return runner_inputs
 
 
-    def apply_findings(findings: list[Finding]):
+    def apply_findings(args_obj, findings: list[Finding]):
         '''
         Apply a findings list to the oak9 project
         '''
+        endpoint = "https://devapi.oak9.cloud/console/"
+
+        if "data_endpoint" in args_obj and args_obj["data_endpoint"] != "":
+            endpoint = args_obj['data_endpoint']
+
         violations = []
 
         for finding in findings:
             violations.append(finding.to_violation().__json__())
 
         payload = {
             "runtime": "Python",
@@ -64,25 +67,19 @@
                     "violations": violations,
                     "oak9Guidance": "",
                     "mappedIndustryFrameworks": []
                 }
             ]
         }
 
-        json_config = None
-        config_path = "D:\\git\\oak9.sac.fw\\cli\\config.json" # fetch from env vars?
-        with open(config_path, 'r') as file:
-            json_config = json.load(file)
-
-        url = f"{json_config['dataEndpoint']}{json_config['orgId']}/sac/{json_config['projectId']}/validation/apply/"
-        headers = {"Authorization": f"Bearer {json_config['apiKey']}"}
-        response = requests.post(url, headers=headers, json=payload)
+        url = f"{endpoint}{args_obj['org_id']}/sac/{args_obj['project_id']}/validation/apply/"
+        response = requests.post(url, auth=(args_obj['org_id'], args_obj['api_key']), json=payload)
 
         if response.status_code != 200:
-            print(f"WARNING: Unable to apply {json_config['projectId']} findings, please verify your credentials.")
+            print(f"WARNING: Unable to apply {args_obj['api_key']} findings, please verify your credentials.")
             return None
         
         return response.text
     
 
     def fetch_runner_input_local(request_id: str):
```

### Comparing `oak9_tython-1.0.4/oak9/tython/core/tools.py` & `oak9_tython-1.0.5/oak9/tython/core/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Module providingFunction utilities for the runner."""
 import importlib.util
 from typing import List, Tuple, Optional
 from core.types import Resource
 from core.logger import _logger
 from core.exception import GrpcPopulationException
-from oak9.sacprotobuf.internal.design_gap_pb2 import DesignGap, Violation
-from oak9.sacprotobuf.internal.runner_exceptions_pb2 import RunnerException
+from oak9.tython.models.shared.shared_pb2 import DesignGap, Violation, RunnerException
 from google.protobuf.message import Message
 
 log = _logger()
 
 def module_from_file(module_name, file_path):
     spec = importlib.util.spec_from_file_location(module_name, file_path)
     module = importlib.util.module_from_spec(spec)
```

### Comparing `oak9_tython-1.0.4/oak9/tython/core/types.py` & `oak9_tython-1.0.5/oak9/tython/core/types.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/types_tests.py` & `oak9_tython-1.0.5/oak9/tython/core/types_tests.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/core/utilities.py` & `oak9_tython-1.0.5/oak9/tython/core/utilities.py`

 * *Files 8% similar despite different names*

```diff
@@ -189,7 +189,26 @@
         obj_list.append([keyvault.vaults])
         config_list.append(get_config_id(keyvault, 'access_policies', keyvault.vaults))
         is_defined = True
     if not (len(keyvault.vaults_access_policies) > 0 or len(keyvault.vaults.access_policies) > 0):
         config_list.append(get_config_id(keyvault, 'vaults_access_policies', keyvault))
 
     return (is_defined, config_list, obj_list)
+
+
+def verify_config_arguments(args_obj):
+    """
+    Verifies if the obligatory attributes are available
+    """
+    
+    if "org_id" not in args_obj or args_obj["org_id"] == "":
+        raise Exception("Missing org_id configuration")
+    
+    if "project_id" not in args_obj or args_obj["project_id"] == "":
+        raise Exception("Missing project_id configuration")
+    
+    if "api_key" not in args_obj or args_obj["api_key"] == "":
+        raise Exception("Missing api_key configuration")
+    
+    if "blueprint_package_path" not in args_obj or args_obj["blueprint_package_path"] == "":
+        raise Exception("Missing blueprint_package_path configuration")
+
```

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_accessanalyzer_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_accessanalyzer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_accessanalyzer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_acmpca_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_acmpca_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_acmpca_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_acmpca_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_alexa_ask_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_alexa_ask_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_alexa_ask_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_amazonmq_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_amazonmq_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_amazonmq_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_amazonmq_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_amplify_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_amplify_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_amplify_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_amplify_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigateway_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigateway_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigateway_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigateway_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigatewayv2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigatewayv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_apigatewayv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appconfig_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appconfig_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appconfig_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appconfig_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appflow_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appflow_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appflow_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationautoscaling_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationautoscaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationinsights_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationinsights_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_applicationinsights_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appmesh_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appmesh_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appmesh_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appmesh_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appsync_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appsync_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_appsync_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_appsync_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_athena_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_athena_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_athena_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_athena_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscaling_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscaling_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscaling_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscaling_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscalingplans_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscalingplans_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_autoscalingplans_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_backup_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_backup_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_batch_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_batch_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_batch_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_batch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_budgets_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_budgets_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_budgets_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_budgets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cassandra_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cassandra_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cassandra_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cassandra_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_certificatemanager_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_certificatemanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_certificatemanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_chatbot_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_chatbot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_chatbot_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_chatbot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloud9_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloud9_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloud9_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloud9_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudformation_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudformation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudformation_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudformation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudfront_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudfront_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudfront_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudfront_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudtrail_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudtrail_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudtrail_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudwatch_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudwatch_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cloudwatch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codebuild_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codebuild_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codebuild_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codebuild_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codecommit_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codecommit_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codecommit_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codecommit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codedeploy_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codedeploy_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codedeploy_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codedeploy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codeguruprofiler_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codeguruprofiler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codegurureviewer_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codegurureviewer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codegurureviewer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codepipeline_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codepipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codepipeline_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codepipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestar_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestar_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestar_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarconnections_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarconnections_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarconnections_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarnotifications_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarnotifications_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_codestarnotifications_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cognito_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cognito_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_cognito_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_cognito_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_config_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_config_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_config_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_config_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_datapipeline_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_datapipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_datapipeline_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_datapipeline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_detective_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_detective_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_detective_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_detective_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_directoryservice_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_directoryservice_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_directoryservice_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_directoryservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dlm_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dlm_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dlm_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dlm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dms_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dms_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_docdb_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_docdb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_docdb_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_docdb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_table_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_table_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_dynamodb_table_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_dhcpoptions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_instance_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_networkacl_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_networkacl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_route_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_route_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_route_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_securitygroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_subnet_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_subnet_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_subnet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpc_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ec2_vpcendpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecr_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecr_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecr_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecs_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ecs_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ecs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_efs_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_efs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_efs_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_efs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_eks_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_eks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_eks_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_eks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_cachecluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticache_replicationgroup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticbeanstalk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticloadbalancingv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticsearch_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticsearch_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_elasticsearch_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_emr_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_emr_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_emr_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_emr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_events_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_events_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_events_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_eventschemas_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_eventschemas_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_eventschemas_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_eventschemas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_fms_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_fms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_fms_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_fms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_fsx_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_fsx_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_fsx_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_fsx_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_gamelift_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_gamelift_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_gamelift_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_gamelift_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_globalaccelerator_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_globalaccelerator_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_globalaccelerator_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_glue_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_glue_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_glue_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_glue_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_greengrass_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_greengrass_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_greengrass_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_greengrass_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_groundstation_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_groundstation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_groundstation_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_groundstation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_guardduty_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_guardduty_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_guardduty_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_guardduty_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iam_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iam_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iam_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_imagebuilder_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_imagebuilder_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_imagebuilder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_inspector_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_inspector_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_inspector_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_inspector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot1click_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot1click_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot1click_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot1click_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iot_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotanalytics_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotanalytics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotanalytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotevents_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotevents_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_iotevents_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_iotevents_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesis_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesis_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesis_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalytics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisanalyticsv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisfirehose_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kinesisfirehose_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kms_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_kms_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_kms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_lakeformation_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_lakeformation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_lakeformation_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_lakeformation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_lambda_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_lambda_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_lambda_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_lambda_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_logs_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_logs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_logs_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_logs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_macie_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_macie_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_macie_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_macie_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_managedblockchain_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_managedblockchain_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_managedblockchain_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_mediaconvert_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_mediaconvert_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_mediaconvert_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_msk_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_msk_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_msk_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_msk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_neptune_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_neptune_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_neptune_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_neptune_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_networkmanager_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_networkmanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_networkmanager_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_networkmanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworks_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworks_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworkscm_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworkscm_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_opsworkscm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_qldb_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_qldb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_qldb_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_qldb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ram_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ram_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ram_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ram_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbcluster_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbcluster_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbinstance_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_dbinstance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_rds_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_rds_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_redshift_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_redshift_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_redshift_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_redshift_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_resourcegroups_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_resourcegroups_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_resourcegroups_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_robomaker_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_robomaker_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_robomaker_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_robomaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53resolver_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53resolver_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_route53resolver_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_route53resolver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_s3_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_s3_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_s3_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_s3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sagemaker_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sagemaker_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sagemaker_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sagemaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sdb_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sdb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sdb_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sdb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_secretsmanager_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_secretsmanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_secretsmanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_securityhub_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_securityhub_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_securityhub_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_securityhub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicecatalog_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicecatalog_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicecatalog_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicediscovery_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicediscovery_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_servicediscovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sns_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sns_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sns_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sns_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sqs_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sqs_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sqs_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sqs_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ssm_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ssm_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_ssm_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_ssm_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sso_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_sso_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_sso_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_stepfunctions_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_stepfunctions_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_stepfunctions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_synthetics_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_synthetics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_synthetics_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_synthetics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_transfer_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_transfer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_transfer_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_transfer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_waf_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_waf_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_waf_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_waf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafregional_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafregional_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafregional_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafregional_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafv2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafv2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_wafv2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_wafv2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_workspaces_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_workspaces_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/aws/aws_workspaces_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/aws/aws_workspaces_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_aad_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_aad_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_aad_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_apimanagement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_containerapps_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cache_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cache_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cache_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cdn_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_cdn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachines_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_compute_virtualmachinescalesets_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerregistry_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_containerservice_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_devices_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_devices_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_devices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_documentdb_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_elastic_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_elastic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_eventgrid_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_healthcareapis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotcentral_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_iotsecurity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_keyvault_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_kubernetes_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,117 +10,141 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from oak9.tython.models.shared import shared_pb2 as shared_dot_shared__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7azure/azure_microsoft_network_applicationgateways.proto\x12\x37oak9.tython.azure.microsoft_network_applicationgateways\x1a\x13shared/shared.proto\"\x93\x01\n%Microsoft_Network_applicationGateways\x12j\n\x14\x61pplication_gateways\x18\x01 \x01(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGateways\"\x1a\n\x0cHttpListener\x12\n\n\x02id\x18\x01 \x01(\t\"!\n\x13\x42\x61\x63kendHttpSettings\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x12\x42\x61\x63kendAddressPool\x12\n\n\x02id\x18\x01 \x01(\t\"\x1a\n\x0c\x46rontendPort\x12\n\n\x02id\x18\x01 \x01(\t\"%\n\x17\x46rontendIPConfiguration\x12\n\n\x02id\x18\x01 \x01(\t\"\x14\n\x06Subnet\x12\n\n\x02id\x18\x01 \x01(\t\"\x1d\n\x0fPublicIpAddress\x12\n\n\x02id\x18\x01 \x01(\t\"\x82\x02\n-ApplicationGatewaysPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x89\x01\n%private_link_service_connection_state\x18\x03 \x01(\x0b\x32Z.oak9.tython.azure.microsoft_network_applicationgateways.PrivateLinkServiceConnectionState\"b\n!PrivateLinkServiceConnectionState\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x18\n\x10\x61\x63tions_required\x18\x03 \x01(\t\"\xb6\x1a\n\x13\x41pplicationGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x64\n\x04tags\x18\x04 \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGateways.TagsEntry\x12[\n\x03sku\x18\x05 \x01(\x0b\x32N.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySku\x12h\n\nssl_policy\x18\x06 \x01(\x0b\x32T.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslPolicy\x12}\n\x19gateway_ip_configurations\x18\x07 \x03(\x0b\x32Z.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayIPConfiguration\x12\x89\x01\n\x1b\x61uthentication_certificates\x18\x08 \x03(\x0b\x32\x64.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayAuthenticationCertificate\x12\x84\x01\n\x19trusted_root_certificates\x18\t \x03(\x0b\x32\x61.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayTrustedRootCertificate\x12\x88\x01\n\x1btrusted_client_certificates\x18\n \x03(\x0b\x32\x63.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayTrustedClientCertificate\x12s\n\x10ssl_certificates\x18\x0b \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslCertificate\x12\x86\x01\n\x1a\x66rontend_ip_configurations\x18\x0c \x03(\x0b\x32\x62.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFrontendIPConfiguration\x12o\n\x0e\x66rontend_ports\x18\r \x03(\x0b\x32W.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFrontendPort\x12`\n\x06probes\x18\x0e \x03(\x0b\x32P.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayProbe\x12|\n\x15\x62\x61\x63kend_address_pools\x18\x0f \x03(\x0b\x32].oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayBackendAddressPool\x12\x88\x01\n backend_http_settings_collection\x18\x10 \x03(\x0b\x32^.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayBackendHttpSettings\x12o\n\x0ehttp_listeners\x18\x11 \x03(\x0b\x32W.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayHttpListener\x12k\n\x0cssl_profiles\x18\x12 \x03(\x0b\x32U.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslProfile\x12l\n\rurl_path_maps\x18\x13 \x03(\x0b\x32U.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayUrlPathMap\x12|\n\x15request_routing_rules\x18\x14 \x03(\x0b\x32].oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRequestRoutingRule\x12t\n\x11rewrite_rule_sets\x18\x15 \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRuleSet\x12\x81\x01\n\x17redirect_configurations\x18\x16 \x03(\x0b\x32`.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRedirectConfiguration\x12\x9e\x01\n&web_application_firewall_configuration\x18\x17 \x01(\x0b\x32n.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayWebApplicationFirewallConfiguration\x12\x17\n\x0f\x66irewall_policy\x18\x18 \x01(\t\x12\x14\n\x0c\x65nable_http2\x18\x19 \x01(\x08\x12\x13\n\x0b\x65nable_fips\x18\x1a \x01(\x08\x12\x82\x01\n\x17\x61utoscale_configuration\x18\x1b \x01(\x0b\x32\x61.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayAutoscaleConfiguration\x12\x88\x01\n\x1bprivate_link_configurations\x18\x1c \x03(\x0b\x32\x63.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayPrivateLinkConfiguration\x12{\n\x1b\x63ustom_error_configurations\x18\x1d \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayCustomError\x12)\n!force_firewall_policy_association\x18\x1e \x01(\x08\x12\r\n\x05zones\x18\x1f \x03(\t\x12\x61\n\x08identity\x18  \x01(\x0b\x32O.oak9.tython.azure.microsoft_network_applicationgateways.ManagedServiceIdentity\x12\xa1\x01\n1application_gateways_private_endpoint_connections\x18! \x03(\x0b\x32\x66.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaysPrivateEndpointConnections\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf5\x01\n\x16ManagedServiceIdentity\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x8d\x01\n\x18user_assigned_identities\x18\x02 \x03(\x0b\x32k.oak9.tython.azure.microsoft_network_applicationgateways.ManagedServiceIdentity.UserAssignedIdentitiesEntry\x1a=\n\x1bUserAssignedIdentitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xbd\x01\n*ApplicationGatewayPrivateLinkConfiguration\x12\x80\x01\n\x11ip_configurations\x18\x01 \x03(\x0b\x32\x65.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayPrivateLinkIpConfiguration\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xe0\x01\n,ApplicationGatewayPrivateLinkIpConfiguration\x12\x1a\n\x12private_ip_address\x18\x01 \x01(\t\x12$\n\x1cprivate_ip_allocation_method\x18\x02 \x01(\t\x12O\n\x06subnet\x18\x03 \x01(\x0b\x32?.oak9.tython.azure.microsoft_network_applicationgateways.Subnet\x12\x0f\n\x07primary\x18\x04 \x01(\x08\x12\x0c\n\x04name\x18\x05 \x01(\t\"V\n(ApplicationGatewayAutoscaleConfiguration\x12\x14\n\x0cmin_capacity\x18\x01 \x01(\x05\x12\x14\n\x0cmax_capacity\x18\x02 \x01(\x05\"\x88\x04\n5ApplicationGatewayWebApplicationFirewallConfiguration\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rfirewall_mode\x18\x02 \x01(\t\x12\x15\n\rrule_set_type\x18\x03 \x01(\t\x12\x18\n\x10rule_set_version\x18\x04 \x01(\t\x12\x82\x01\n\x14\x64isabled_rule_groups\x18\x05 \x03(\x0b\x32\x64.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFirewallDisabledRuleGroup\x12\x1a\n\x12request_body_check\x18\x06 \x01(\x08\x12\x1d\n\x15max_request_body_size\x18\x07 \x01(\x05\x12#\n\x1bmax_request_body_size_in_kb\x18\x08 \x01(\x05\x12\x1f\n\x17\x66ile_upload_limit_in_mb\x18\t \x01(\x05\x12p\n\nexclusions\x18\n \x03(\x0b\x32\\.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFirewallExclusion\"p\n#ApplicationGatewayFirewallExclusion\x12\x16\n\x0ematch_variable\x18\x01 \x01(\t\x12\x1f\n\x17selector_match_operator\x18\x02 \x01(\t\x12\x10\n\x08selector\x18\x03 \x01(\t\"U\n+ApplicationGatewayFirewallDisabledRuleGroup\x12\x17\n\x0frule_group_name\x18\x01 \x01(\t\x12\r\n\x05rules\x18\x02 \x03(\x05\"\xf9\x01\n\'ApplicationGatewayRedirectConfiguration\x12\x15\n\rredirect_type\x18\x01 \x01(\t\x12\x17\n\x0ftarget_listener\x18\x02 \x01(\t\x12\x12\n\ntarget_url\x18\x03 \x01(\t\x12\x14\n\x0cinclude_path\x18\x04 \x01(\x08\x12\x1c\n\x14include_query_string\x18\x05 \x01(\x08\x12\x1d\n\x15request_routing_rules\x18\x06 \x03(\t\x12\x15\n\rurl_path_maps\x18\x07 \x03(\t\x12\x12\n\npath_rules\x18\x08 \x03(\t\x12\x0c\n\x04name\x18\t \x01(\t\"\x9f\x01\n ApplicationGatewayRewriteRuleSet\x12m\n\rrewrite_rules\x18\x01 \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRule\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xae\x02\n\x1d\x41pplicationGatewayRewriteRule\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rrule_sequence\x18\x02 \x01(\x05\x12s\n\nconditions\x18\x03 \x03(\x0b\x32_.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRuleCondition\x12s\n\naction_set\x18\x04 \x01(\x0b\x32_.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRuleActionSet\"\xb1\x03\n&ApplicationGatewayRewriteRuleActionSet\x12\x85\x01\n\x1drequest_header_configurations\x18\x01 \x03(\x0b\x32^.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayHeaderConfiguration\x12\x86\x01\n\x1eresponse_header_configurations\x18\x02 \x03(\x0b\x32^.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayHeaderConfiguration\x12v\n\x11url_configuration\x18\x03 \x01(\x0b\x32[.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayUrlConfiguration\"k\n\"ApplicationGatewayUrlConfiguration\x12\x15\n\rmodified_path\x18\x01 \x01(\t\x12\x1d\n\x15modified_query_string\x18\x02 \x01(\t\x12\x0f\n\x07reroute\x18\x03 \x01(\x08\"R\n%ApplicationGatewayHeaderConfiguration\x12\x13\n\x0bheader_name\x18\x01 \x01(\t\x12\x14\n\x0cheader_value\x18\x02 \x01(\t\"p\n&ApplicationGatewayRewriteRuleCondition\x12\x10\n\x08variable\x18\x01 \x01(\t\x12\x0f\n\x07pattern\x18\x02 \x01(\t\x12\x13\n\x0bignore_case\x18\x03 \x01(\x08\x12\x0e\n\x06negate\x18\x04 \x01(\x08\"\xdf\x03\n$ApplicationGatewayRequestRoutingRule\x12\x11\n\trule_type\x18\x01 \x01(\t\x12\x10\n\x08priority\x18\x02 \x01(\x05\x12i\n\x14\x62\x61\x63kend_address_pool\x18\x03 \x01(\x0b\x32K.oak9.tython.azure.microsoft_network_applicationgateways.BackendAddressPool\x12k\n\x15\x62\x61\x63kend_http_settings\x18\x04 \x01(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.BackendHttpSettings\x12\\\n\rhttp_listener\x18\x05 \x01(\x0b\x32\x45.oak9.tython.azure.microsoft_network_applicationgateways.HttpListener\x12\x14\n\x0curl_path_map\x18\x06 \x01(\t\x12\x18\n\x10rewrite_rule_set\x18\x07 \x01(\t\x12\x1e\n\x16redirect_configuration\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\"\xac\x02\n\x1c\x41pplicationGatewayUrlPathMap\x12$\n\x1c\x64\x65\x66\x61ult_backend_address_pool\x18\x01 \x01(\t\x12%\n\x1d\x64\x65\x66\x61ult_backend_http_settings\x18\x02 \x01(\t\x12 \n\x18\x64\x65\x66\x61ult_rewrite_rule_set\x18\x03 \x01(\t\x12&\n\x1e\x64\x65\x66\x61ult_redirect_configuration\x18\x04 \x01(\t\x12g\n\npath_rules\x18\x05 \x03(\x0b\x32S.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayPathRule\x12\x0c\n\x04name\x18\x06 \x01(\t\"\xe4\x02\n\x1a\x41pplicationGatewayPathRule\x12\r\n\x05paths\x18\x01 \x03(\t\x12i\n\x14\x62\x61\x63kend_address_pool\x18\x02 \x01(\x0b\x32K.oak9.tython.azure.microsoft_network_applicationgateways.BackendAddressPool\x12k\n\x15\x62\x61\x63kend_http_settings\x18\x03 \x01(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.BackendHttpSettings\x12\x1e\n\x16redirect_configuration\x18\x04 \x01(\t\x12\x18\n\x10rewrite_rule_set\x18\x05 \x01(\t\x12\x17\n\x0f\x66irewall_policy\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\"\xc3\x02\n\x1c\x41pplicationGatewaySslProfile\x12#\n\x1btrusted_client_certificates\x18\x01 \x03(\t\x12h\n\nssl_policy\x18\x02 \x01(\x0b\x32T.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslPolicy\x12\x85\x01\n\x19\x63lient_auth_configuration\x18\x03 \x01(\x0b\x32\x62.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayClientAuthConfiguration\x12\x0c\n\x04name\x18\x04 \x01(\t\"R\n)ApplicationGatewayClientAuthConfiguration\x12%\n\x1dverify_client_cert_issuer_d_n\x18\x01 \x01(\x08\"\xa6\x04\n\x1e\x41pplicationGatewayHttpListener\x12s\n\x19\x66rontend_ip_configuration\x18\x01 \x01(\x0b\x32P.oak9.tython.azure.microsoft_network_applicationgateways.FrontendIPConfiguration\x12\\\n\rfrontend_port\x18\x02 \x01(\x0b\x32\x45.oak9.tython.azure.microsoft_network_applicationgateways.FrontendPort\x12\x10\n\x08protocol\x18\x03 \x01(\t\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x17\n\x0fssl_certificate\x18\x05 \x01(\t\x12\x13\n\x0bssl_profile\x18\x06 \x01(\t\x12&\n\x1erequire_server_name_indication\x18\x07 \x01(\x08\x12{\n\x1b\x63ustom_error_configurations\x18\x08 \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayCustomError\x12\x17\n\x0f\x66irewall_policy\x18\t \x01(\t\x12\x12\n\nhost_names\x18\n \x03(\t\x12\x0c\n\x04name\x18\x0b \x01(\t\"S\n\x1d\x41pplicationGatewayCustomError\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x1d\n\x15\x63ustom_error_page_url\x18\x02 \x01(\t\"\xe3\x03\n%ApplicationGatewayBackendHttpSettings\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08protocol\x18\x02 \x01(\t\x12\x1d\n\x15\x63ookie_based_affinity\x18\x03 \x01(\t\x12\x17\n\x0frequest_timeout\x18\x04 \x01(\x05\x12\r\n\x05probe\x18\x05 \x01(\t\x12#\n\x1b\x61uthentication_certificates\x18\x06 \x03(\t\x12!\n\x19trusted_root_certificates\x18\x07 \x03(\t\x12z\n\x13\x63onnection_draining\x18\x08 \x01(\x0b\x32].oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayConnectionDraining\x12\x11\n\thost_name\x18\t \x01(\t\x12+\n#pick_host_name_from_backend_address\x18\n \x01(\x08\x12\x1c\n\x14\x61\x66\x66inity_cookie_name\x18\x0b \x01(\t\x12\x15\n\rprobe_enabled\x18\x0c \x01(\x08\x12\x0c\n\x04path\x18\r \x01(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\"U\n$ApplicationGatewayConnectionDraining\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1c\n\x14\x64rain_timeout_in_sec\x18\x02 \x01(\x05\"\xaa\x01\n$ApplicationGatewayBackendAddressPool\x12t\n\x11\x62\x61\x63kend_addresses\x18\x01 \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayBackendAddress\x12\x0c\n\x04name\x18\x02 \x01(\t\"D\n ApplicationGatewayBackendAddress\x12\x0c\n\x04\x66qdn\x18\x01 \x01(\t\x12\x12\n\nip_address\x18\x02 \x01(\t\"\xdf\x02\n\x17\x41pplicationGatewayProbe\x12\x10\n\x08protocol\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0f\n\x07timeout\x18\x05 \x01(\x05\x12\x1b\n\x13unhealthy_threshold\x18\x06 \x01(\x05\x12\x31\n)pick_host_name_from_backend_http_settings\x18\x07 \x01(\x08\x12\x13\n\x0bmin_servers\x18\x08 \x01(\x05\x12r\n\x05match\x18\t \x01(\x0b\x32\x63.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayProbeHealthResponseMatch\x12\x0c\n\x04port\x18\n \x01(\x05\x12\x0c\n\x04name\x18\x0b \x01(\t\"P\n*ApplicationGatewayProbeHealthResponseMatch\x12\x0c\n\x04\x62ody\x18\x01 \x01(\t\x12\x14\n\x0cstatus_codes\x18\x02 \x03(\t\"<\n\x1e\x41pplicationGatewayFrontendPort\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd5\x02\n)ApplicationGatewayFrontendIPConfiguration\x12\x1a\n\x12private_ip_address\x18\x01 \x01(\t\x12$\n\x1cprivate_ip_allocation_method\x18\x02 \x01(\t\x12O\n\x06subnet\x18\x03 \x01(\x0b\x32?.oak9.tython.azure.microsoft_network_applicationgateways.Subnet\x12\"\n\x1aprivate_link_configuration\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x63\n\x11public_ip_address\x18\x06 \x01(\x0b\x32H.oak9.tython.azure.microsoft_network_applicationgateways.PublicIpAddress\"m\n ApplicationGatewaySslCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x1b\n\x13key_vault_secret_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\"H\n*ApplicationGatewayTrustedClientCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"c\n(ApplicationGatewayTrustedRootCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x1b\n\x13key_vault_secret_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"I\n+ApplicationGatewayAuthenticationCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x82\x01\n!ApplicationGatewayIPConfiguration\x12O\n\x06subnet\x18\x01 \x01(\x0b\x32?.oak9.tython.azure.microsoft_network_applicationgateways.Subnet\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x9c\x01\n\x1b\x41pplicationGatewaySslPolicy\x12\x1e\n\x16\x64isabled_ssl_protocols\x18\x01 \x03(\t\x12\x13\n\x0bpolicy_type\x18\x02 \x01(\t\x12\x13\n\x0bpolicy_name\x18\x03 \x01(\t\x12\x15\n\rcipher_suites\x18\x04 \x03(\t\x12\x1c\n\x14min_protocol_version\x18\x05 \x01(\t\"E\n\x15\x41pplicationGatewaySku\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04tier\x18\x02 \x01(\t\x12\x10\n\x08\x63\x61pacity\x18\x03 \x01(\x05\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n7azure/azure_microsoft_network_applicationgateways.proto\x12\x37oak9.tython.azure.microsoft_network_applicationgateways\x1a\x13shared/shared.proto\"\xbe\x02\n%Microsoft_Network_applicationGateways\x12j\n\x14\x61pplication_gateways\x18\x01 \x01(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGateways\x12\xa8\x01\n5application_gateway_web_application_firewall_policies\x18\x02 \x01(\x0b\x32i.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayWebApplicationFirewallPolicies\"\x1a\n\x0cHttpListener\x12\n\n\x02id\x18\x01 \x01(\t\"!\n\x13\x42\x61\x63kendHttpSettings\x12\n\n\x02id\x18\x01 \x01(\t\" \n\x12\x42\x61\x63kendAddressPool\x12\n\n\x02id\x18\x01 \x01(\t\"\x1a\n\x0c\x46rontendPort\x12\n\n\x02id\x18\x01 \x01(\t\"%\n\x17\x46rontendIPConfiguration\x12\n\n\x02id\x18\x01 \x01(\t\"\x14\n\x06Subnet\x12\n\n\x02id\x18\x01 \x01(\t\"\x1d\n\x0fPublicIpAddress\x12\n\n\x02id\x18\x01 \x01(\t\"\x82\x02\n-ApplicationGatewaysPrivateEndpointConnections\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x89\x01\n%private_link_service_connection_state\x18\x03 \x01(\x0b\x32Z.oak9.tython.azure.microsoft_network_applicationgateways.PrivateLinkServiceConnectionState\"b\n!PrivateLinkServiceConnectionState\x12\x0e\n\x06status\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x18\n\x10\x61\x63tions_required\x18\x03 \x01(\t\"\xb6\x1a\n\x13\x41pplicationGateways\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x64\n\x04tags\x18\x04 \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGateways.TagsEntry\x12[\n\x03sku\x18\x05 \x01(\x0b\x32N.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySku\x12h\n\nssl_policy\x18\x06 \x01(\x0b\x32T.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslPolicy\x12}\n\x19gateway_ip_configurations\x18\x07 \x03(\x0b\x32Z.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayIPConfiguration\x12\x89\x01\n\x1b\x61uthentication_certificates\x18\x08 \x03(\x0b\x32\x64.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayAuthenticationCertificate\x12\x84\x01\n\x19trusted_root_certificates\x18\t \x03(\x0b\x32\x61.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayTrustedRootCertificate\x12\x88\x01\n\x1btrusted_client_certificates\x18\n \x03(\x0b\x32\x63.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayTrustedClientCertificate\x12s\n\x10ssl_certificates\x18\x0b \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslCertificate\x12\x86\x01\n\x1a\x66rontend_ip_configurations\x18\x0c \x03(\x0b\x32\x62.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFrontendIPConfiguration\x12o\n\x0e\x66rontend_ports\x18\r \x03(\x0b\x32W.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFrontendPort\x12`\n\x06probes\x18\x0e \x03(\x0b\x32P.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayProbe\x12|\n\x15\x62\x61\x63kend_address_pools\x18\x0f \x03(\x0b\x32].oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayBackendAddressPool\x12\x88\x01\n backend_http_settings_collection\x18\x10 \x03(\x0b\x32^.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayBackendHttpSettings\x12o\n\x0ehttp_listeners\x18\x11 \x03(\x0b\x32W.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayHttpListener\x12k\n\x0cssl_profiles\x18\x12 \x03(\x0b\x32U.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslProfile\x12l\n\rurl_path_maps\x18\x13 \x03(\x0b\x32U.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayUrlPathMap\x12|\n\x15request_routing_rules\x18\x14 \x03(\x0b\x32].oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRequestRoutingRule\x12t\n\x11rewrite_rule_sets\x18\x15 \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRuleSet\x12\x81\x01\n\x17redirect_configurations\x18\x16 \x03(\x0b\x32`.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRedirectConfiguration\x12\x9e\x01\n&web_application_firewall_configuration\x18\x17 \x01(\x0b\x32n.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayWebApplicationFirewallConfiguration\x12\x17\n\x0f\x66irewall_policy\x18\x18 \x01(\t\x12\x14\n\x0c\x65nable_http2\x18\x19 \x01(\x08\x12\x13\n\x0b\x65nable_fips\x18\x1a \x01(\x08\x12\x82\x01\n\x17\x61utoscale_configuration\x18\x1b \x01(\x0b\x32\x61.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayAutoscaleConfiguration\x12\x88\x01\n\x1bprivate_link_configurations\x18\x1c \x03(\x0b\x32\x63.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayPrivateLinkConfiguration\x12{\n\x1b\x63ustom_error_configurations\x18\x1d \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayCustomError\x12)\n!force_firewall_policy_association\x18\x1e \x01(\x08\x12\r\n\x05zones\x18\x1f \x03(\t\x12\x61\n\x08identity\x18  \x01(\x0b\x32O.oak9.tython.azure.microsoft_network_applicationgateways.ManagedServiceIdentity\x12\xa1\x01\n1application_gateways_private_endpoint_connections\x18! \x03(\x0b\x32\x66.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaysPrivateEndpointConnections\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xf5\x01\n\x16ManagedServiceIdentity\x12\x0c\n\x04type\x18\x01 \x01(\t\x12\x8d\x01\n\x18user_assigned_identities\x18\x02 \x03(\x0b\x32k.oak9.tython.azure.microsoft_network_applicationgateways.ManagedServiceIdentity.UserAssignedIdentitiesEntry\x1a=\n\x1bUserAssignedIdentitiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xbd\x01\n*ApplicationGatewayPrivateLinkConfiguration\x12\x80\x01\n\x11ip_configurations\x18\x01 \x03(\x0b\x32\x65.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayPrivateLinkIpConfiguration\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xe0\x01\n,ApplicationGatewayPrivateLinkIpConfiguration\x12\x1a\n\x12private_ip_address\x18\x01 \x01(\t\x12$\n\x1cprivate_ip_allocation_method\x18\x02 \x01(\t\x12O\n\x06subnet\x18\x03 \x01(\x0b\x32?.oak9.tython.azure.microsoft_network_applicationgateways.Subnet\x12\x0f\n\x07primary\x18\x04 \x01(\x08\x12\x0c\n\x04name\x18\x05 \x01(\t\"V\n(ApplicationGatewayAutoscaleConfiguration\x12\x14\n\x0cmin_capacity\x18\x01 \x01(\x05\x12\x14\n\x0cmax_capacity\x18\x02 \x01(\x05\"\x88\x04\n5ApplicationGatewayWebApplicationFirewallConfiguration\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x15\n\rfirewall_mode\x18\x02 \x01(\t\x12\x15\n\rrule_set_type\x18\x03 \x01(\t\x12\x18\n\x10rule_set_version\x18\x04 \x01(\t\x12\x82\x01\n\x14\x64isabled_rule_groups\x18\x05 \x03(\x0b\x32\x64.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFirewallDisabledRuleGroup\x12\x1a\n\x12request_body_check\x18\x06 \x01(\x08\x12\x1d\n\x15max_request_body_size\x18\x07 \x01(\x05\x12#\n\x1bmax_request_body_size_in_kb\x18\x08 \x01(\x05\x12\x1f\n\x17\x66ile_upload_limit_in_mb\x18\t \x01(\x05\x12p\n\nexclusions\x18\n \x03(\x0b\x32\\.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayFirewallExclusion\"p\n#ApplicationGatewayFirewallExclusion\x12\x16\n\x0ematch_variable\x18\x01 \x01(\t\x12\x1f\n\x17selector_match_operator\x18\x02 \x01(\t\x12\x10\n\x08selector\x18\x03 \x01(\t\"U\n+ApplicationGatewayFirewallDisabledRuleGroup\x12\x17\n\x0frule_group_name\x18\x01 \x01(\t\x12\r\n\x05rules\x18\x02 \x03(\x05\"\xf9\x01\n\'ApplicationGatewayRedirectConfiguration\x12\x15\n\rredirect_type\x18\x01 \x01(\t\x12\x17\n\x0ftarget_listener\x18\x02 \x01(\t\x12\x12\n\ntarget_url\x18\x03 \x01(\t\x12\x14\n\x0cinclude_path\x18\x04 \x01(\x08\x12\x1c\n\x14include_query_string\x18\x05 \x01(\x08\x12\x1d\n\x15request_routing_rules\x18\x06 \x03(\t\x12\x15\n\rurl_path_maps\x18\x07 \x03(\t\x12\x12\n\npath_rules\x18\x08 \x03(\t\x12\x0c\n\x04name\x18\t \x01(\t\"\x9f\x01\n ApplicationGatewayRewriteRuleSet\x12m\n\rrewrite_rules\x18\x01 \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRule\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xae\x02\n\x1d\x41pplicationGatewayRewriteRule\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rrule_sequence\x18\x02 \x01(\x05\x12s\n\nconditions\x18\x03 \x03(\x0b\x32_.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRuleCondition\x12s\n\naction_set\x18\x04 \x01(\x0b\x32_.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayRewriteRuleActionSet\"\xb1\x03\n&ApplicationGatewayRewriteRuleActionSet\x12\x85\x01\n\x1drequest_header_configurations\x18\x01 \x03(\x0b\x32^.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayHeaderConfiguration\x12\x86\x01\n\x1eresponse_header_configurations\x18\x02 \x03(\x0b\x32^.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayHeaderConfiguration\x12v\n\x11url_configuration\x18\x03 \x01(\x0b\x32[.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayUrlConfiguration\"k\n\"ApplicationGatewayUrlConfiguration\x12\x15\n\rmodified_path\x18\x01 \x01(\t\x12\x1d\n\x15modified_query_string\x18\x02 \x01(\t\x12\x0f\n\x07reroute\x18\x03 \x01(\x08\"R\n%ApplicationGatewayHeaderConfiguration\x12\x13\n\x0bheader_name\x18\x01 \x01(\t\x12\x14\n\x0cheader_value\x18\x02 \x01(\t\"p\n&ApplicationGatewayRewriteRuleCondition\x12\x10\n\x08variable\x18\x01 \x01(\t\x12\x0f\n\x07pattern\x18\x02 \x01(\t\x12\x13\n\x0bignore_case\x18\x03 \x01(\x08\x12\x0e\n\x06negate\x18\x04 \x01(\x08\"\xdf\x03\n$ApplicationGatewayRequestRoutingRule\x12\x11\n\trule_type\x18\x01 \x01(\t\x12\x10\n\x08priority\x18\x02 \x01(\x05\x12i\n\x14\x62\x61\x63kend_address_pool\x18\x03 \x01(\x0b\x32K.oak9.tython.azure.microsoft_network_applicationgateways.BackendAddressPool\x12k\n\x15\x62\x61\x63kend_http_settings\x18\x04 \x01(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.BackendHttpSettings\x12\\\n\rhttp_listener\x18\x05 \x01(\x0b\x32\x45.oak9.tython.azure.microsoft_network_applicationgateways.HttpListener\x12\x14\n\x0curl_path_map\x18\x06 \x01(\t\x12\x18\n\x10rewrite_rule_set\x18\x07 \x01(\t\x12\x1e\n\x16redirect_configuration\x18\x08 \x01(\t\x12\x0c\n\x04name\x18\t \x01(\t\"\xac\x02\n\x1c\x41pplicationGatewayUrlPathMap\x12$\n\x1c\x64\x65\x66\x61ult_backend_address_pool\x18\x01 \x01(\t\x12%\n\x1d\x64\x65\x66\x61ult_backend_http_settings\x18\x02 \x01(\t\x12 \n\x18\x64\x65\x66\x61ult_rewrite_rule_set\x18\x03 \x01(\t\x12&\n\x1e\x64\x65\x66\x61ult_redirect_configuration\x18\x04 \x01(\t\x12g\n\npath_rules\x18\x05 \x03(\x0b\x32S.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayPathRule\x12\x0c\n\x04name\x18\x06 \x01(\t\"\xe4\x02\n\x1a\x41pplicationGatewayPathRule\x12\r\n\x05paths\x18\x01 \x03(\t\x12i\n\x14\x62\x61\x63kend_address_pool\x18\x02 \x01(\x0b\x32K.oak9.tython.azure.microsoft_network_applicationgateways.BackendAddressPool\x12k\n\x15\x62\x61\x63kend_http_settings\x18\x03 \x01(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.BackendHttpSettings\x12\x1e\n\x16redirect_configuration\x18\x04 \x01(\t\x12\x18\n\x10rewrite_rule_set\x18\x05 \x01(\t\x12\x17\n\x0f\x66irewall_policy\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\"\xc3\x02\n\x1c\x41pplicationGatewaySslProfile\x12#\n\x1btrusted_client_certificates\x18\x01 \x03(\t\x12h\n\nssl_policy\x18\x02 \x01(\x0b\x32T.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewaySslPolicy\x12\x85\x01\n\x19\x63lient_auth_configuration\x18\x03 \x01(\x0b\x32\x62.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayClientAuthConfiguration\x12\x0c\n\x04name\x18\x04 \x01(\t\"R\n)ApplicationGatewayClientAuthConfiguration\x12%\n\x1dverify_client_cert_issuer_d_n\x18\x01 \x01(\x08\"\xa6\x04\n\x1e\x41pplicationGatewayHttpListener\x12s\n\x19\x66rontend_ip_configuration\x18\x01 \x01(\x0b\x32P.oak9.tython.azure.microsoft_network_applicationgateways.FrontendIPConfiguration\x12\\\n\rfrontend_port\x18\x02 \x01(\x0b\x32\x45.oak9.tython.azure.microsoft_network_applicationgateways.FrontendPort\x12\x10\n\x08protocol\x18\x03 \x01(\t\x12\x11\n\thost_name\x18\x04 \x01(\t\x12\x17\n\x0fssl_certificate\x18\x05 \x01(\t\x12\x13\n\x0bssl_profile\x18\x06 \x01(\t\x12&\n\x1erequire_server_name_indication\x18\x07 \x01(\x08\x12{\n\x1b\x63ustom_error_configurations\x18\x08 \x03(\x0b\x32V.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayCustomError\x12\x17\n\x0f\x66irewall_policy\x18\t \x01(\t\x12\x12\n\nhost_names\x18\n \x03(\t\x12\x0c\n\x04name\x18\x0b \x01(\t\"S\n\x1d\x41pplicationGatewayCustomError\x12\x13\n\x0bstatus_code\x18\x01 \x01(\t\x12\x1d\n\x15\x63ustom_error_page_url\x18\x02 \x01(\t\"\xe3\x03\n%ApplicationGatewayBackendHttpSettings\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x10\n\x08protocol\x18\x02 \x01(\t\x12\x1d\n\x15\x63ookie_based_affinity\x18\x03 \x01(\t\x12\x17\n\x0frequest_timeout\x18\x04 \x01(\x05\x12\r\n\x05probe\x18\x05 \x01(\t\x12#\n\x1b\x61uthentication_certificates\x18\x06 \x03(\t\x12!\n\x19trusted_root_certificates\x18\x07 \x03(\t\x12z\n\x13\x63onnection_draining\x18\x08 \x01(\x0b\x32].oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayConnectionDraining\x12\x11\n\thost_name\x18\t \x01(\t\x12+\n#pick_host_name_from_backend_address\x18\n \x01(\x08\x12\x1c\n\x14\x61\x66\x66inity_cookie_name\x18\x0b \x01(\t\x12\x15\n\rprobe_enabled\x18\x0c \x01(\x08\x12\x0c\n\x04path\x18\r \x01(\t\x12\x0c\n\x04name\x18\x0e \x01(\t\"U\n$ApplicationGatewayConnectionDraining\x12\x0f\n\x07\x65nabled\x18\x01 \x01(\x08\x12\x1c\n\x14\x64rain_timeout_in_sec\x18\x02 \x01(\x05\"\xaa\x01\n$ApplicationGatewayBackendAddressPool\x12t\n\x11\x62\x61\x63kend_addresses\x18\x01 \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayBackendAddress\x12\x0c\n\x04name\x18\x02 \x01(\t\"D\n ApplicationGatewayBackendAddress\x12\x0c\n\x04\x66qdn\x18\x01 \x01(\t\x12\x12\n\nip_address\x18\x02 \x01(\t\"\xdf\x02\n\x17\x41pplicationGatewayProbe\x12\x10\n\x08protocol\x18\x01 \x01(\t\x12\x0c\n\x04host\x18\x02 \x01(\t\x12\x0c\n\x04path\x18\x03 \x01(\t\x12\x10\n\x08interval\x18\x04 \x01(\x05\x12\x0f\n\x07timeout\x18\x05 \x01(\x05\x12\x1b\n\x13unhealthy_threshold\x18\x06 \x01(\x05\x12\x31\n)pick_host_name_from_backend_http_settings\x18\x07 \x01(\x08\x12\x13\n\x0bmin_servers\x18\x08 \x01(\x05\x12r\n\x05match\x18\t \x01(\x0b\x32\x63.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayProbeHealthResponseMatch\x12\x0c\n\x04port\x18\n \x01(\x05\x12\x0c\n\x04name\x18\x0b \x01(\t\"P\n*ApplicationGatewayProbeHealthResponseMatch\x12\x0c\n\x04\x62ody\x18\x01 \x01(\t\x12\x14\n\x0cstatus_codes\x18\x02 \x03(\t\"<\n\x1e\x41pplicationGatewayFrontendPort\x12\x0c\n\x04port\x18\x01 \x01(\x05\x12\x0c\n\x04name\x18\x02 \x01(\t\"\xd5\x02\n)ApplicationGatewayFrontendIPConfiguration\x12\x1a\n\x12private_ip_address\x18\x01 \x01(\t\x12$\n\x1cprivate_ip_allocation_method\x18\x02 \x01(\t\x12O\n\x06subnet\x18\x03 \x01(\x0b\x32?.oak9.tython.azure.microsoft_network_applicationgateways.Subnet\x12\"\n\x1aprivate_link_configuration\x18\x04 \x01(\t\x12\x0c\n\x04name\x18\x05 \x01(\t\x12\x63\n\x11public_ip_address\x18\x06 \x01(\x0b\x32H.oak9.tython.azure.microsoft_network_applicationgateways.PublicIpAddress\"m\n ApplicationGatewaySslCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x1b\n\x13key_vault_secret_id\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t\"H\n*ApplicationGatewayTrustedClientCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"c\n(ApplicationGatewayTrustedRootCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x1b\n\x13key_vault_secret_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\"I\n+ApplicationGatewayAuthenticationCertificate\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x82\x01\n!ApplicationGatewayIPConfiguration\x12O\n\x06subnet\x18\x01 \x01(\x0b\x32?.oak9.tython.azure.microsoft_network_applicationgateways.Subnet\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x9c\x01\n\x1b\x41pplicationGatewaySslPolicy\x12\x1e\n\x16\x64isabled_ssl_protocols\x18\x01 \x03(\t\x12\x13\n\x0bpolicy_type\x18\x02 \x01(\t\x12\x13\n\x0bpolicy_name\x18\x03 \x01(\t\x12\x15\n\rcipher_suites\x18\x04 \x03(\t\x12\x1c\n\x14min_protocol_version\x18\x05 \x01(\t\"E\n\x15\x41pplicationGatewaySku\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04tier\x18\x02 \x01(\t\x12\x10\n\x08\x63\x61pacity\x18\x03 \x01(\x05\"\xf7\x04\n0ApplicationGatewayWebApplicationFirewallPolicies\x12\x37\n\rresource_info\x18\x01 \x01(\x0b\x32 .oak9.tython.shared.ResourceInfo\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x10\n\x08location\x18\x03 \x01(\t\x12\x81\x01\n\x04tags\x18\x04 \x03(\x0b\x32s.oak9.tython.azure.microsoft_network_applicationgateways.ApplicationGatewayWebApplicationFirewallPolicies.TagsEntry\x12`\n\x0fpolicy_settings\x18\x05 \x01(\x0b\x32G.oak9.tython.azure.microsoft_network_applicationgateways.PolicySettings\x12o\n\x0c\x63ustom_rules\x18\x06 \x03(\x0b\x32Y.oak9.tython.azure.microsoft_network_applicationgateways.WebApplicationFirewallCustomRule\x12\x66\n\rmanaged_rules\x18\x07 \x01(\x0b\x32O.oak9.tython.azure.microsoft_network_applicationgateways.ManagedRulesDefinition\x1a+\n\tTagsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xe1\x01\n\x16ManagedRulesDefinition\x12\x63\n\nexclusions\x18\x01 \x03(\x0b\x32O.oak9.tython.azure.microsoft_network_applicationgateways.OwaspCrsExclusionEntry\x12\x62\n\x11managed_rule_sets\x18\x02 \x03(\x0b\x32G.oak9.tython.azure.microsoft_network_applicationgateways.ManagedRuleSet\"\xb2\x01\n\x0eManagedRuleSet\x12\x15\n\rrule_set_type\x18\x01 \x01(\t\x12\x18\n\x10rule_set_version\x18\x02 \x01(\t\x12o\n\x14rule_group_overrides\x18\x03 \x03(\x0b\x32Q.oak9.tython.azure.microsoft_network_applicationgateways.ManagedRuleGroupOverride\"\x90\x01\n\x18ManagedRuleGroupOverride\x12\x17\n\x0frule_group_name\x18\x01 \x01(\t\x12[\n\x05rules\x18\x02 \x03(\x0b\x32L.oak9.tython.azure.microsoft_network_applicationgateways.ManagedRuleOverride\"5\n\x13ManagedRuleOverride\x12\x0f\n\x07rule_id\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\"c\n\x16OwaspCrsExclusionEntry\x12\x16\n\x0ematch_variable\x18\x01 \x01(\t\x12\x1f\n\x17selector_match_operator\x18\x02 \x01(\t\x12\x10\n\x08selector\x18\x03 \x01(\t\"\xc8\x01\n WebApplicationFirewallCustomRule\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x10\n\x08priority\x18\x02 \x01(\x05\x12\x11\n\trule_type\x18\x03 \x01(\t\x12\x61\n\x10match_conditions\x18\x04 \x03(\x0b\x32G.oak9.tython.azure.microsoft_network_applicationgateways.MatchCondition\x12\x0e\n\x06\x61\x63tion\x18\x05 \x01(\t\"\xc8\x01\n\x0eMatchCondition\x12_\n\x0fmatch_variables\x18\x01 \x03(\x0b\x32\x46.oak9.tython.azure.microsoft_network_applicationgateways.MatchVariable\x12\x10\n\x08operator\x18\x02 \x01(\t\x12\x19\n\x11negation_conditon\x18\x03 \x01(\x08\x12\x14\n\x0cmatch_values\x18\x04 \x03(\t\x12\x12\n\ntransforms\x18\x05 \x03(\t\"8\n\rMatchVariable\x12\x15\n\rvariable_name\x18\x01 \x01(\t\x12\x10\n\x08selector\x18\x02 \x01(\t\"\x8f\x01\n\x0ePolicySettings\x12\r\n\x05state\x18\x01 \x01(\t\x12\x0c\n\x04mode\x18\x02 \x01(\t\x12\x1a\n\x12request_body_check\x18\x03 \x01(\x08\x12#\n\x1bmax_request_body_size_in_kb\x18\x04 \x01(\x05\x12\x1f\n\x17\x66ile_upload_limit_in_mb\x18\x05 \x01(\x05\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'azure.azure_microsoft_network_applicationgateways_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _APPLICATIONGATEWAYS_TAGSENTRY._options = None
   _APPLICATIONGATEWAYS_TAGSENTRY._serialized_options = b'8\001'
   _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._options = None
   _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_options = b'8\001'
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLPOLICIES_TAGSENTRY._options = None
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLPOLICIES_TAGSENTRY._serialized_options = b'8\001'
   _MICROSOFT_NETWORK_APPLICATIONGATEWAYS._serialized_start=138
-  _MICROSOFT_NETWORK_APPLICATIONGATEWAYS._serialized_end=285
-  _HTTPLISTENER._serialized_start=287
-  _HTTPLISTENER._serialized_end=313
-  _BACKENDHTTPSETTINGS._serialized_start=315
-  _BACKENDHTTPSETTINGS._serialized_end=348
-  _BACKENDADDRESSPOOL._serialized_start=350
-  _BACKENDADDRESSPOOL._serialized_end=382
-  _FRONTENDPORT._serialized_start=384
-  _FRONTENDPORT._serialized_end=410
-  _FRONTENDIPCONFIGURATION._serialized_start=412
-  _FRONTENDIPCONFIGURATION._serialized_end=449
-  _SUBNET._serialized_start=451
-  _SUBNET._serialized_end=471
-  _PUBLICIPADDRESS._serialized_start=473
-  _PUBLICIPADDRESS._serialized_end=502
-  _APPLICATIONGATEWAYSPRIVATEENDPOINTCONNECTIONS._serialized_start=505
-  _APPLICATIONGATEWAYSPRIVATEENDPOINTCONNECTIONS._serialized_end=763
-  _PRIVATELINKSERVICECONNECTIONSTATE._serialized_start=765
-  _PRIVATELINKSERVICECONNECTIONSTATE._serialized_end=863
-  _APPLICATIONGATEWAYS._serialized_start=866
-  _APPLICATIONGATEWAYS._serialized_end=4248
-  _APPLICATIONGATEWAYS_TAGSENTRY._serialized_start=4205
-  _APPLICATIONGATEWAYS_TAGSENTRY._serialized_end=4248
-  _MANAGEDSERVICEIDENTITY._serialized_start=4251
-  _MANAGEDSERVICEIDENTITY._serialized_end=4496
-  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_start=4435
-  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_end=4496
-  _APPLICATIONGATEWAYPRIVATELINKCONFIGURATION._serialized_start=4499
-  _APPLICATIONGATEWAYPRIVATELINKCONFIGURATION._serialized_end=4688
-  _APPLICATIONGATEWAYPRIVATELINKIPCONFIGURATION._serialized_start=4691
-  _APPLICATIONGATEWAYPRIVATELINKIPCONFIGURATION._serialized_end=4915
-  _APPLICATIONGATEWAYAUTOSCALECONFIGURATION._serialized_start=4917
-  _APPLICATIONGATEWAYAUTOSCALECONFIGURATION._serialized_end=5003
-  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLCONFIGURATION._serialized_start=5006
-  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLCONFIGURATION._serialized_end=5526
-  _APPLICATIONGATEWAYFIREWALLEXCLUSION._serialized_start=5528
-  _APPLICATIONGATEWAYFIREWALLEXCLUSION._serialized_end=5640
-  _APPLICATIONGATEWAYFIREWALLDISABLEDRULEGROUP._serialized_start=5642
-  _APPLICATIONGATEWAYFIREWALLDISABLEDRULEGROUP._serialized_end=5727
-  _APPLICATIONGATEWAYREDIRECTCONFIGURATION._serialized_start=5730
-  _APPLICATIONGATEWAYREDIRECTCONFIGURATION._serialized_end=5979
-  _APPLICATIONGATEWAYREWRITERULESET._serialized_start=5982
-  _APPLICATIONGATEWAYREWRITERULESET._serialized_end=6141
-  _APPLICATIONGATEWAYREWRITERULE._serialized_start=6144
-  _APPLICATIONGATEWAYREWRITERULE._serialized_end=6446
-  _APPLICATIONGATEWAYREWRITERULEACTIONSET._serialized_start=6449
-  _APPLICATIONGATEWAYREWRITERULEACTIONSET._serialized_end=6882
-  _APPLICATIONGATEWAYURLCONFIGURATION._serialized_start=6884
-  _APPLICATIONGATEWAYURLCONFIGURATION._serialized_end=6991
-  _APPLICATIONGATEWAYHEADERCONFIGURATION._serialized_start=6993
-  _APPLICATIONGATEWAYHEADERCONFIGURATION._serialized_end=7075
-  _APPLICATIONGATEWAYREWRITERULECONDITION._serialized_start=7077
-  _APPLICATIONGATEWAYREWRITERULECONDITION._serialized_end=7189
-  _APPLICATIONGATEWAYREQUESTROUTINGRULE._serialized_start=7192
-  _APPLICATIONGATEWAYREQUESTROUTINGRULE._serialized_end=7671
-  _APPLICATIONGATEWAYURLPATHMAP._serialized_start=7674
-  _APPLICATIONGATEWAYURLPATHMAP._serialized_end=7974
-  _APPLICATIONGATEWAYPATHRULE._serialized_start=7977
-  _APPLICATIONGATEWAYPATHRULE._serialized_end=8333
-  _APPLICATIONGATEWAYSSLPROFILE._serialized_start=8336
-  _APPLICATIONGATEWAYSSLPROFILE._serialized_end=8659
-  _APPLICATIONGATEWAYCLIENTAUTHCONFIGURATION._serialized_start=8661
-  _APPLICATIONGATEWAYCLIENTAUTHCONFIGURATION._serialized_end=8743
-  _APPLICATIONGATEWAYHTTPLISTENER._serialized_start=8746
-  _APPLICATIONGATEWAYHTTPLISTENER._serialized_end=9296
-  _APPLICATIONGATEWAYCUSTOMERROR._serialized_start=9298
-  _APPLICATIONGATEWAYCUSTOMERROR._serialized_end=9381
-  _APPLICATIONGATEWAYBACKENDHTTPSETTINGS._serialized_start=9384
-  _APPLICATIONGATEWAYBACKENDHTTPSETTINGS._serialized_end=9867
-  _APPLICATIONGATEWAYCONNECTIONDRAINING._serialized_start=9869
-  _APPLICATIONGATEWAYCONNECTIONDRAINING._serialized_end=9954
-  _APPLICATIONGATEWAYBACKENDADDRESSPOOL._serialized_start=9957
-  _APPLICATIONGATEWAYBACKENDADDRESSPOOL._serialized_end=10127
-  _APPLICATIONGATEWAYBACKENDADDRESS._serialized_start=10129
-  _APPLICATIONGATEWAYBACKENDADDRESS._serialized_end=10197
-  _APPLICATIONGATEWAYPROBE._serialized_start=10200
-  _APPLICATIONGATEWAYPROBE._serialized_end=10551
-  _APPLICATIONGATEWAYPROBEHEALTHRESPONSEMATCH._serialized_start=10553
-  _APPLICATIONGATEWAYPROBEHEALTHRESPONSEMATCH._serialized_end=10633
-  _APPLICATIONGATEWAYFRONTENDPORT._serialized_start=10635
-  _APPLICATIONGATEWAYFRONTENDPORT._serialized_end=10695
-  _APPLICATIONGATEWAYFRONTENDIPCONFIGURATION._serialized_start=10698
-  _APPLICATIONGATEWAYFRONTENDIPCONFIGURATION._serialized_end=11039
-  _APPLICATIONGATEWAYSSLCERTIFICATE._serialized_start=11041
-  _APPLICATIONGATEWAYSSLCERTIFICATE._serialized_end=11150
-  _APPLICATIONGATEWAYTRUSTEDCLIENTCERTIFICATE._serialized_start=11152
-  _APPLICATIONGATEWAYTRUSTEDCLIENTCERTIFICATE._serialized_end=11224
-  _APPLICATIONGATEWAYTRUSTEDROOTCERTIFICATE._serialized_start=11226
-  _APPLICATIONGATEWAYTRUSTEDROOTCERTIFICATE._serialized_end=11325
-  _APPLICATIONGATEWAYAUTHENTICATIONCERTIFICATE._serialized_start=11327
-  _APPLICATIONGATEWAYAUTHENTICATIONCERTIFICATE._serialized_end=11400
-  _APPLICATIONGATEWAYIPCONFIGURATION._serialized_start=11403
-  _APPLICATIONGATEWAYIPCONFIGURATION._serialized_end=11533
-  _APPLICATIONGATEWAYSSLPOLICY._serialized_start=11536
-  _APPLICATIONGATEWAYSSLPOLICY._serialized_end=11692
-  _APPLICATIONGATEWAYSKU._serialized_start=11694
-  _APPLICATIONGATEWAYSKU._serialized_end=11763
+  _MICROSOFT_NETWORK_APPLICATIONGATEWAYS._serialized_end=456
+  _HTTPLISTENER._serialized_start=458
+  _HTTPLISTENER._serialized_end=484
+  _BACKENDHTTPSETTINGS._serialized_start=486
+  _BACKENDHTTPSETTINGS._serialized_end=519
+  _BACKENDADDRESSPOOL._serialized_start=521
+  _BACKENDADDRESSPOOL._serialized_end=553
+  _FRONTENDPORT._serialized_start=555
+  _FRONTENDPORT._serialized_end=581
+  _FRONTENDIPCONFIGURATION._serialized_start=583
+  _FRONTENDIPCONFIGURATION._serialized_end=620
+  _SUBNET._serialized_start=622
+  _SUBNET._serialized_end=642
+  _PUBLICIPADDRESS._serialized_start=644
+  _PUBLICIPADDRESS._serialized_end=673
+  _APPLICATIONGATEWAYSPRIVATEENDPOINTCONNECTIONS._serialized_start=676
+  _APPLICATIONGATEWAYSPRIVATEENDPOINTCONNECTIONS._serialized_end=934
+  _PRIVATELINKSERVICECONNECTIONSTATE._serialized_start=936
+  _PRIVATELINKSERVICECONNECTIONSTATE._serialized_end=1034
+  _APPLICATIONGATEWAYS._serialized_start=1037
+  _APPLICATIONGATEWAYS._serialized_end=4419
+  _APPLICATIONGATEWAYS_TAGSENTRY._serialized_start=4376
+  _APPLICATIONGATEWAYS_TAGSENTRY._serialized_end=4419
+  _MANAGEDSERVICEIDENTITY._serialized_start=4422
+  _MANAGEDSERVICEIDENTITY._serialized_end=4667
+  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_start=4606
+  _MANAGEDSERVICEIDENTITY_USERASSIGNEDIDENTITIESENTRY._serialized_end=4667
+  _APPLICATIONGATEWAYPRIVATELINKCONFIGURATION._serialized_start=4670
+  _APPLICATIONGATEWAYPRIVATELINKCONFIGURATION._serialized_end=4859
+  _APPLICATIONGATEWAYPRIVATELINKIPCONFIGURATION._serialized_start=4862
+  _APPLICATIONGATEWAYPRIVATELINKIPCONFIGURATION._serialized_end=5086
+  _APPLICATIONGATEWAYAUTOSCALECONFIGURATION._serialized_start=5088
+  _APPLICATIONGATEWAYAUTOSCALECONFIGURATION._serialized_end=5174
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLCONFIGURATION._serialized_start=5177
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLCONFIGURATION._serialized_end=5697
+  _APPLICATIONGATEWAYFIREWALLEXCLUSION._serialized_start=5699
+  _APPLICATIONGATEWAYFIREWALLEXCLUSION._serialized_end=5811
+  _APPLICATIONGATEWAYFIREWALLDISABLEDRULEGROUP._serialized_start=5813
+  _APPLICATIONGATEWAYFIREWALLDISABLEDRULEGROUP._serialized_end=5898
+  _APPLICATIONGATEWAYREDIRECTCONFIGURATION._serialized_start=5901
+  _APPLICATIONGATEWAYREDIRECTCONFIGURATION._serialized_end=6150
+  _APPLICATIONGATEWAYREWRITERULESET._serialized_start=6153
+  _APPLICATIONGATEWAYREWRITERULESET._serialized_end=6312
+  _APPLICATIONGATEWAYREWRITERULE._serialized_start=6315
+  _APPLICATIONGATEWAYREWRITERULE._serialized_end=6617
+  _APPLICATIONGATEWAYREWRITERULEACTIONSET._serialized_start=6620
+  _APPLICATIONGATEWAYREWRITERULEACTIONSET._serialized_end=7053
+  _APPLICATIONGATEWAYURLCONFIGURATION._serialized_start=7055
+  _APPLICATIONGATEWAYURLCONFIGURATION._serialized_end=7162
+  _APPLICATIONGATEWAYHEADERCONFIGURATION._serialized_start=7164
+  _APPLICATIONGATEWAYHEADERCONFIGURATION._serialized_end=7246
+  _APPLICATIONGATEWAYREWRITERULECONDITION._serialized_start=7248
+  _APPLICATIONGATEWAYREWRITERULECONDITION._serialized_end=7360
+  _APPLICATIONGATEWAYREQUESTROUTINGRULE._serialized_start=7363
+  _APPLICATIONGATEWAYREQUESTROUTINGRULE._serialized_end=7842
+  _APPLICATIONGATEWAYURLPATHMAP._serialized_start=7845
+  _APPLICATIONGATEWAYURLPATHMAP._serialized_end=8145
+  _APPLICATIONGATEWAYPATHRULE._serialized_start=8148
+  _APPLICATIONGATEWAYPATHRULE._serialized_end=8504
+  _APPLICATIONGATEWAYSSLPROFILE._serialized_start=8507
+  _APPLICATIONGATEWAYSSLPROFILE._serialized_end=8830
+  _APPLICATIONGATEWAYCLIENTAUTHCONFIGURATION._serialized_start=8832
+  _APPLICATIONGATEWAYCLIENTAUTHCONFIGURATION._serialized_end=8914
+  _APPLICATIONGATEWAYHTTPLISTENER._serialized_start=8917
+  _APPLICATIONGATEWAYHTTPLISTENER._serialized_end=9467
+  _APPLICATIONGATEWAYCUSTOMERROR._serialized_start=9469
+  _APPLICATIONGATEWAYCUSTOMERROR._serialized_end=9552
+  _APPLICATIONGATEWAYBACKENDHTTPSETTINGS._serialized_start=9555
+  _APPLICATIONGATEWAYBACKENDHTTPSETTINGS._serialized_end=10038
+  _APPLICATIONGATEWAYCONNECTIONDRAINING._serialized_start=10040
+  _APPLICATIONGATEWAYCONNECTIONDRAINING._serialized_end=10125
+  _APPLICATIONGATEWAYBACKENDADDRESSPOOL._serialized_start=10128
+  _APPLICATIONGATEWAYBACKENDADDRESSPOOL._serialized_end=10298
+  _APPLICATIONGATEWAYBACKENDADDRESS._serialized_start=10300
+  _APPLICATIONGATEWAYBACKENDADDRESS._serialized_end=10368
+  _APPLICATIONGATEWAYPROBE._serialized_start=10371
+  _APPLICATIONGATEWAYPROBE._serialized_end=10722
+  _APPLICATIONGATEWAYPROBEHEALTHRESPONSEMATCH._serialized_start=10724
+  _APPLICATIONGATEWAYPROBEHEALTHRESPONSEMATCH._serialized_end=10804
+  _APPLICATIONGATEWAYFRONTENDPORT._serialized_start=10806
+  _APPLICATIONGATEWAYFRONTENDPORT._serialized_end=10866
+  _APPLICATIONGATEWAYFRONTENDIPCONFIGURATION._serialized_start=10869
+  _APPLICATIONGATEWAYFRONTENDIPCONFIGURATION._serialized_end=11210
+  _APPLICATIONGATEWAYSSLCERTIFICATE._serialized_start=11212
+  _APPLICATIONGATEWAYSSLCERTIFICATE._serialized_end=11321
+  _APPLICATIONGATEWAYTRUSTEDCLIENTCERTIFICATE._serialized_start=11323
+  _APPLICATIONGATEWAYTRUSTEDCLIENTCERTIFICATE._serialized_end=11395
+  _APPLICATIONGATEWAYTRUSTEDROOTCERTIFICATE._serialized_start=11397
+  _APPLICATIONGATEWAYTRUSTEDROOTCERTIFICATE._serialized_end=11496
+  _APPLICATIONGATEWAYAUTHENTICATIONCERTIFICATE._serialized_start=11498
+  _APPLICATIONGATEWAYAUTHENTICATIONCERTIFICATE._serialized_end=11571
+  _APPLICATIONGATEWAYIPCONFIGURATION._serialized_start=11574
+  _APPLICATIONGATEWAYIPCONFIGURATION._serialized_end=11704
+  _APPLICATIONGATEWAYSSLPOLICY._serialized_start=11707
+  _APPLICATIONGATEWAYSSLPOLICY._serialized_end=11863
+  _APPLICATIONGATEWAYSKU._serialized_start=11865
+  _APPLICATIONGATEWAYSKU._serialized_end=11934
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLPOLICIES._serialized_start=11937
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLPOLICIES._serialized_end=12568
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLPOLICIES_TAGSENTRY._serialized_start=4376
+  _APPLICATIONGATEWAYWEBAPPLICATIONFIREWALLPOLICIES_TAGSENTRY._serialized_end=4419
+  _MANAGEDRULESDEFINITION._serialized_start=12571
+  _MANAGEDRULESDEFINITION._serialized_end=12796
+  _MANAGEDRULESET._serialized_start=12799
+  _MANAGEDRULESET._serialized_end=12977
+  _MANAGEDRULEGROUPOVERRIDE._serialized_start=12980
+  _MANAGEDRULEGROUPOVERRIDE._serialized_end=13124
+  _MANAGEDRULEOVERRIDE._serialized_start=13126
+  _MANAGEDRULEOVERRIDE._serialized_end=13179
+  _OWASPCRSEXCLUSIONENTRY._serialized_start=13181
+  _OWASPCRSEXCLUSIONENTRY._serialized_end=13280
+  _WEBAPPLICATIONFIREWALLCUSTOMRULE._serialized_start=13283
+  _WEBAPPLICATIONFIREWALLCUSTOMRULE._serialized_end=13483
+  _MATCHCONDITION._serialized_start=13486
+  _MATCHCONDITION._serialized_end=13686
+  _MATCHVARIABLE._serialized_start=13688
+  _MATCHVARIABLE._serialized_end=13744
+  _POLICYSETTINGS._serialized_start=13747
+  _POLICYSETTINGS._serialized_end=13890
 # @@protoc_insertion_point(module_scope)
```

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_applicationgateways_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -14,1291 +14,1268 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class Microsoft_Network_applicationGateways(google.protobuf.message.Message):
+class NotebooksEnvironmentXContainerImage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    APPLICATION_GATEWAYS_FIELD_NUMBER: builtins.int
-    @property
-    def application_gateways(self) -> global___ApplicationGateways: ...
+    REPOSITORY_FIELD_NUMBER: builtins.int
+    TAG_FIELD_NUMBER: builtins.int
+    repository: builtins.str
+    tag: builtins.str
     def __init__(
         self,
         *,
-        application_gateways: global___ApplicationGateways | None = ...,
+        repository: builtins.str = ...,
+        tag: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["application_gateways", b"application_gateways"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application_gateways", b"application_gateways"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
 
-global___Microsoft_Network_applicationGateways = Microsoft_Network_applicationGateways
+global___NotebooksEnvironmentXContainerImage = NotebooksEnvironmentXContainerImage
 
 @typing_extensions.final
-class HttpListener(google.protobuf.message.Message):
+class NotebooksEnvironmentXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    id: builtins.str
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___HttpListener = HttpListener
+global___NotebooksEnvironmentXTimeouts = NotebooksEnvironmentXTimeouts
 
 @typing_extensions.final
-class BackendHttpSettings(google.protobuf.message.Message):
+class NotebooksEnvironmentXVmImage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    id: builtins.str
+    IMAGE_FAMILY_FIELD_NUMBER: builtins.int
+    IMAGE_NAME_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    image_family: builtins.str
+    image_name: builtins.str
+    project: builtins.str
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
+        image_family: builtins.str = ...,
+        image_name: builtins.str = ...,
+        project: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["image_family", b"image_family", "image_name", b"image_name", "project", b"project"]) -> None: ...
 
-global___BackendHttpSettings = BackendHttpSettings
+global___NotebooksEnvironmentXVmImage = NotebooksEnvironmentXVmImage
 
 @typing_extensions.final
-class BackendAddressPool(google.protobuf.message.Message):
+class NotebooksEnvironment(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    CREATE_TIME_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    DISPLAY_NAME_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
+    POST_STARTUP_SCRIPT_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    CONTAINER_IMAGE_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    VM_IMAGE_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    create_time: builtins.str
+    description: builtins.str
+    display_name: builtins.str
     id: builtins.str
+    location: builtins.str
+    name: builtins.str
+    post_startup_script: builtins.str
+    project: builtins.str
+    @property
+    def container_image(self) -> global___NotebooksEnvironmentXContainerImage: ...
+    @property
+    def timeouts(self) -> global___NotebooksEnvironmentXTimeouts: ...
+    @property
+    def vm_image(self) -> global___NotebooksEnvironmentXVmImage: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
+        create_time: builtins.str = ...,
+        description: builtins.str = ...,
+        display_name: builtins.str = ...,
         id: builtins.str = ...,
+        location: builtins.str = ...,
+        name: builtins.str = ...,
+        post_startup_script: builtins.str = ...,
+        project: builtins.str = ...,
+        container_image: global___NotebooksEnvironmentXContainerImage | None = ...,
+        timeouts: global___NotebooksEnvironmentXTimeouts | None = ...,
+        vm_image: global___NotebooksEnvironmentXVmImage | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["container_image", b"container_image", "resource_info", b"resource_info", "timeouts", b"timeouts", "vm_image", b"vm_image"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["container_image", b"container_image", "create_time", b"create_time", "description", b"description", "display_name", b"display_name", "id", b"id", "location", b"location", "name", b"name", "post_startup_script", b"post_startup_script", "project", b"project", "resource_info", b"resource_info", "timeouts", b"timeouts", "vm_image", b"vm_image"]) -> None: ...
 
-global___BackendAddressPool = BackendAddressPool
+global___NotebooksEnvironment = NotebooksEnvironment
 
 @typing_extensions.final
-class FrontendPort(google.protobuf.message.Message):
+class NotebooksInstanceXAcceleratorConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    id: builtins.str
+    CORE_COUNT_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    core_count: builtins.float
+    type: builtins.str
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
+        core_count: builtins.float = ...,
+        type: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["core_count", b"core_count", "type", b"type"]) -> None: ...
 
-global___FrontendPort = FrontendPort
+global___NotebooksInstanceXAcceleratorConfig = NotebooksInstanceXAcceleratorConfig
 
 @typing_extensions.final
-class FrontendIPConfiguration(google.protobuf.message.Message):
+class NotebooksInstanceXContainerImage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    id: builtins.str
+    REPOSITORY_FIELD_NUMBER: builtins.int
+    TAG_FIELD_NUMBER: builtins.int
+    repository: builtins.str
+    tag: builtins.str
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
+        repository: builtins.str = ...,
+        tag: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
 
-global___FrontendIPConfiguration = FrontendIPConfiguration
+global___NotebooksInstanceXContainerImage = NotebooksInstanceXContainerImage
 
 @typing_extensions.final
-class Subnet(google.protobuf.message.Message):
+class NotebooksInstanceXReservationAffinity(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    id: builtins.str
+    CONSUME_RESERVATION_TYPE_FIELD_NUMBER: builtins.int
+    KEY_FIELD_NUMBER: builtins.int
+    VALUES_FIELD_NUMBER: builtins.int
+    consume_reservation_type: builtins.str
+    key: builtins.str
+    @property
+    def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
+        consume_reservation_type: builtins.str = ...,
+        key: builtins.str = ...,
+        values: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["consume_reservation_type", b"consume_reservation_type", "key", b"key", "values", b"values"]) -> None: ...
 
-global___Subnet = Subnet
+global___NotebooksInstanceXReservationAffinity = NotebooksInstanceXReservationAffinity
 
 @typing_extensions.final
-class PublicIpAddress(google.protobuf.message.Message):
+class NotebooksInstanceXShieldedInstanceConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ID_FIELD_NUMBER: builtins.int
-    id: builtins.str
+    ENABLE_INTEGRITY_MONITORING_FIELD_NUMBER: builtins.int
+    ENABLE_SECURE_BOOT_FIELD_NUMBER: builtins.int
+    ENABLE_VTPM_FIELD_NUMBER: builtins.int
+    enable_integrity_monitoring: builtins.bool
+    enable_secure_boot: builtins.bool
+    enable_vtpm: builtins.bool
     def __init__(
         self,
         *,
-        id: builtins.str = ...,
+        enable_integrity_monitoring: builtins.bool = ...,
+        enable_secure_boot: builtins.bool = ...,
+        enable_vtpm: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["enable_integrity_monitoring", b"enable_integrity_monitoring", "enable_secure_boot", b"enable_secure_boot", "enable_vtpm", b"enable_vtpm"]) -> None: ...
 
-global___PublicIpAddress = PublicIpAddress
+global___NotebooksInstanceXShieldedInstanceConfig = NotebooksInstanceXShieldedInstanceConfig
 
 @typing_extensions.final
-class ApplicationGatewaysPrivateEndpointConnections(google.protobuf.message.Message):
+class NotebooksInstanceXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    PRIVATE_LINK_SERVICE_CONNECTION_STATE_FIELD_NUMBER: builtins.int
-    @property
-    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
-    name: builtins.str
-    @property
-    def private_link_service_connection_state(self) -> global___PrivateLinkServiceConnectionState: ...
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
     def __init__(
         self,
         *,
-        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
-        name: builtins.str = ...,
-        private_link_service_connection_state: global___PrivateLinkServiceConnectionState | None = ...,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["private_link_service_connection_state", b"private_link_service_connection_state", "resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "private_link_service_connection_state", b"private_link_service_connection_state", "resource_info", b"resource_info"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___ApplicationGatewaysPrivateEndpointConnections = ApplicationGatewaysPrivateEndpointConnections
+global___NotebooksInstanceXTimeouts = NotebooksInstanceXTimeouts
 
 @typing_extensions.final
-class PrivateLinkServiceConnectionState(google.protobuf.message.Message):
+class NotebooksInstanceXVmImage(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    STATUS_FIELD_NUMBER: builtins.int
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    ACTIONS_REQUIRED_FIELD_NUMBER: builtins.int
-    status: builtins.str
-    description: builtins.str
-    actions_required: builtins.str
+    IMAGE_FAMILY_FIELD_NUMBER: builtins.int
+    IMAGE_NAME_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    image_family: builtins.str
+    image_name: builtins.str
+    project: builtins.str
     def __init__(
         self,
         *,
-        status: builtins.str = ...,
-        description: builtins.str = ...,
-        actions_required: builtins.str = ...,
+        image_family: builtins.str = ...,
+        image_name: builtins.str = ...,
+        project: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["actions_required", b"actions_required", "description", b"description", "status", b"status"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["image_family", b"image_family", "image_name", b"image_name", "project", b"project"]) -> None: ...
 
-global___PrivateLinkServiceConnectionState = PrivateLinkServiceConnectionState
+global___NotebooksInstanceXVmImage = NotebooksInstanceXVmImage
 
 @typing_extensions.final
-class ApplicationGateways(google.protobuf.message.Message):
+class NotebooksInstance(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class TagsEntry(google.protobuf.message.Message):
+    class LabelsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
-    TAGS_FIELD_NUMBER: builtins.int
-    SKU_FIELD_NUMBER: builtins.int
-    SSL_POLICY_FIELD_NUMBER: builtins.int
-    GATEWAY_IP_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    AUTHENTICATION_CERTIFICATES_FIELD_NUMBER: builtins.int
-    TRUSTED_ROOT_CERTIFICATES_FIELD_NUMBER: builtins.int
-    TRUSTED_CLIENT_CERTIFICATES_FIELD_NUMBER: builtins.int
-    SSL_CERTIFICATES_FIELD_NUMBER: builtins.int
-    FRONTEND_IP_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    FRONTEND_PORTS_FIELD_NUMBER: builtins.int
-    PROBES_FIELD_NUMBER: builtins.int
-    BACKEND_ADDRESS_POOLS_FIELD_NUMBER: builtins.int
-    BACKEND_HTTP_SETTINGS_COLLECTION_FIELD_NUMBER: builtins.int
-    HTTP_LISTENERS_FIELD_NUMBER: builtins.int
-    SSL_PROFILES_FIELD_NUMBER: builtins.int
-    URL_PATH_MAPS_FIELD_NUMBER: builtins.int
-    REQUEST_ROUTING_RULES_FIELD_NUMBER: builtins.int
-    REWRITE_RULE_SETS_FIELD_NUMBER: builtins.int
-    REDIRECT_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    WEB_APPLICATION_FIREWALL_CONFIGURATION_FIELD_NUMBER: builtins.int
-    FIREWALL_POLICY_FIELD_NUMBER: builtins.int
-    ENABLE_HTTP2_FIELD_NUMBER: builtins.int
-    ENABLE_FIPS_FIELD_NUMBER: builtins.int
-    AUTOSCALE_CONFIGURATION_FIELD_NUMBER: builtins.int
-    PRIVATE_LINK_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    CUSTOM_ERROR_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    FORCE_FIREWALL_POLICY_ASSOCIATION_FIELD_NUMBER: builtins.int
-    ZONES_FIELD_NUMBER: builtins.int
-    IDENTITY_FIELD_NUMBER: builtins.int
-    APPLICATION_GATEWAYS_PRIVATE_ENDPOINT_CONNECTIONS_FIELD_NUMBER: builtins.int
-    @property
-    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
-    name: builtins.str
-    location: builtins.str
-    @property
-    def tags(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    @property
-    def sku(self) -> global___ApplicationGatewaySku: ...
-    @property
-    def ssl_policy(self) -> global___ApplicationGatewaySslPolicy: ...
-    @property
-    def gateway_ip_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayIPConfiguration]: ...
-    @property
-    def authentication_certificates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayAuthenticationCertificate]: ...
-    @property
-    def trusted_root_certificates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayTrustedRootCertificate]: ...
-    @property
-    def trusted_client_certificates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayTrustedClientCertificate]: ...
-    @property
-    def ssl_certificates(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewaySslCertificate]: ...
-    @property
-    def frontend_ip_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayFrontendIPConfiguration]: ...
-    @property
-    def frontend_ports(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayFrontendPort]: ...
-    @property
-    def probes(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayProbe]: ...
-    @property
-    def backend_address_pools(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayBackendAddressPool]: ...
-    @property
-    def backend_http_settings_collection(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayBackendHttpSettings]: ...
-    @property
-    def http_listeners(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayHttpListener]: ...
-    @property
-    def ssl_profiles(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewaySslProfile]: ...
-    @property
-    def url_path_maps(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayUrlPathMap]: ...
-    @property
-    def request_routing_rules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayRequestRoutingRule]: ...
-    @property
-    def rewrite_rule_sets(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayRewriteRuleSet]: ...
-    @property
-    def redirect_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayRedirectConfiguration]: ...
-    @property
-    def web_application_firewall_configuration(self) -> global___ApplicationGatewayWebApplicationFirewallConfiguration: ...
-    firewall_policy: builtins.str
-    enable_http2: builtins.bool
-    enable_fips: builtins.bool
-    @property
-    def autoscale_configuration(self) -> global___ApplicationGatewayAutoscaleConfiguration: ...
-    @property
-    def private_link_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayPrivateLinkConfiguration]: ...
-    @property
-    def custom_error_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayCustomError]: ...
-    force_firewall_policy_association: builtins.bool
-    @property
-    def zones(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    @property
-    def identity(self) -> global___ManagedServiceIdentity: ...
-    @property
-    def application_gateways_private_endpoint_connections(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewaysPrivateEndpointConnections]: ...
-    def __init__(
-        self,
-        *,
-        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
-        name: builtins.str = ...,
-        location: builtins.str = ...,
-        tags: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-        sku: global___ApplicationGatewaySku | None = ...,
-        ssl_policy: global___ApplicationGatewaySslPolicy | None = ...,
-        gateway_ip_configurations: collections.abc.Iterable[global___ApplicationGatewayIPConfiguration] | None = ...,
-        authentication_certificates: collections.abc.Iterable[global___ApplicationGatewayAuthenticationCertificate] | None = ...,
-        trusted_root_certificates: collections.abc.Iterable[global___ApplicationGatewayTrustedRootCertificate] | None = ...,
-        trusted_client_certificates: collections.abc.Iterable[global___ApplicationGatewayTrustedClientCertificate] | None = ...,
-        ssl_certificates: collections.abc.Iterable[global___ApplicationGatewaySslCertificate] | None = ...,
-        frontend_ip_configurations: collections.abc.Iterable[global___ApplicationGatewayFrontendIPConfiguration] | None = ...,
-        frontend_ports: collections.abc.Iterable[global___ApplicationGatewayFrontendPort] | None = ...,
-        probes: collections.abc.Iterable[global___ApplicationGatewayProbe] | None = ...,
-        backend_address_pools: collections.abc.Iterable[global___ApplicationGatewayBackendAddressPool] | None = ...,
-        backend_http_settings_collection: collections.abc.Iterable[global___ApplicationGatewayBackendHttpSettings] | None = ...,
-        http_listeners: collections.abc.Iterable[global___ApplicationGatewayHttpListener] | None = ...,
-        ssl_profiles: collections.abc.Iterable[global___ApplicationGatewaySslProfile] | None = ...,
-        url_path_maps: collections.abc.Iterable[global___ApplicationGatewayUrlPathMap] | None = ...,
-        request_routing_rules: collections.abc.Iterable[global___ApplicationGatewayRequestRoutingRule] | None = ...,
-        rewrite_rule_sets: collections.abc.Iterable[global___ApplicationGatewayRewriteRuleSet] | None = ...,
-        redirect_configurations: collections.abc.Iterable[global___ApplicationGatewayRedirectConfiguration] | None = ...,
-        web_application_firewall_configuration: global___ApplicationGatewayWebApplicationFirewallConfiguration | None = ...,
-        firewall_policy: builtins.str = ...,
-        enable_http2: builtins.bool = ...,
-        enable_fips: builtins.bool = ...,
-        autoscale_configuration: global___ApplicationGatewayAutoscaleConfiguration | None = ...,
-        private_link_configurations: collections.abc.Iterable[global___ApplicationGatewayPrivateLinkConfiguration] | None = ...,
-        custom_error_configurations: collections.abc.Iterable[global___ApplicationGatewayCustomError] | None = ...,
-        force_firewall_policy_association: builtins.bool = ...,
-        zones: collections.abc.Iterable[builtins.str] | None = ...,
-        identity: global___ManagedServiceIdentity | None = ...,
-        application_gateways_private_endpoint_connections: collections.abc.Iterable[global___ApplicationGatewaysPrivateEndpointConnections] | None = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["autoscale_configuration", b"autoscale_configuration", "identity", b"identity", "resource_info", b"resource_info", "sku", b"sku", "ssl_policy", b"ssl_policy", "web_application_firewall_configuration", b"web_application_firewall_configuration"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["application_gateways_private_endpoint_connections", b"application_gateways_private_endpoint_connections", "authentication_certificates", b"authentication_certificates", "autoscale_configuration", b"autoscale_configuration", "backend_address_pools", b"backend_address_pools", "backend_http_settings_collection", b"backend_http_settings_collection", "custom_error_configurations", b"custom_error_configurations", "enable_fips", b"enable_fips", "enable_http2", b"enable_http2", "firewall_policy", b"firewall_policy", "force_firewall_policy_association", b"force_firewall_policy_association", "frontend_ip_configurations", b"frontend_ip_configurations", "frontend_ports", b"frontend_ports", "gateway_ip_configurations", b"gateway_ip_configurations", "http_listeners", b"http_listeners", "identity", b"identity", "location", b"location", "name", b"name", "private_link_configurations", b"private_link_configurations", "probes", b"probes", "redirect_configurations", b"redirect_configurations", "request_routing_rules", b"request_routing_rules", "resource_info", b"resource_info", "rewrite_rule_sets", b"rewrite_rule_sets", "sku", b"sku", "ssl_certificates", b"ssl_certificates", "ssl_policy", b"ssl_policy", "ssl_profiles", b"ssl_profiles", "tags", b"tags", "trusted_client_certificates", b"trusted_client_certificates", "trusted_root_certificates", b"trusted_root_certificates", "url_path_maps", b"url_path_maps", "web_application_firewall_configuration", b"web_application_firewall_configuration", "zones", b"zones"]) -> None: ...
-
-global___ApplicationGateways = ApplicationGateways
-
-@typing_extensions.final
-class ManagedServiceIdentity(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
     @typing_extensions.final
-    class UserAssignedIdentitiesEntry(google.protobuf.message.Message):
+    class MetadataEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    TYPE_FIELD_NUMBER: builtins.int
-    USER_ASSIGNED_IDENTITIES_FIELD_NUMBER: builtins.int
-    type: builtins.str
-    @property
-    def user_assigned_identities(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    def __init__(
-        self,
-        *,
-        type: builtins.str = ...,
-        user_assigned_identities: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["type", b"type", "user_assigned_identities", b"user_assigned_identities"]) -> None: ...
-
-global___ManagedServiceIdentity = ManagedServiceIdentity
-
-@typing_extensions.final
-class ApplicationGatewayPrivateLinkConfiguration(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    IP_CONFIGURATIONS_FIELD_NUMBER: builtins.int
+    BOOT_DISK_SIZE_GB_FIELD_NUMBER: builtins.int
+    BOOT_DISK_TYPE_FIELD_NUMBER: builtins.int
+    CREATE_TIME_FIELD_NUMBER: builtins.int
+    CUSTOM_GPU_DRIVER_PATH_FIELD_NUMBER: builtins.int
+    DATA_DISK_SIZE_GB_FIELD_NUMBER: builtins.int
+    DATA_DISK_TYPE_FIELD_NUMBER: builtins.int
+    DISK_ENCRYPTION_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    INSTALL_GPU_DRIVER_FIELD_NUMBER: builtins.int
+    INSTANCE_OWNERS_FIELD_NUMBER: builtins.int
+    KMS_KEY_FIELD_NUMBER: builtins.int
+    LABELS_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    MACHINE_TYPE_FIELD_NUMBER: builtins.int
+    METADATA_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    @property
-    def ip_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayPrivateLinkIpConfiguration]: ...
-    name: builtins.str
-    def __init__(
-        self,
-        *,
-        ip_configurations: collections.abc.Iterable[global___ApplicationGatewayPrivateLinkIpConfiguration] | None = ...,
-        name: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ip_configurations", b"ip_configurations", "name", b"name"]) -> None: ...
-
-global___ApplicationGatewayPrivateLinkConfiguration = ApplicationGatewayPrivateLinkConfiguration
-
-@typing_extensions.final
-class ApplicationGatewayPrivateLinkIpConfiguration(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    PRIVATE_IP_ADDRESS_FIELD_NUMBER: builtins.int
-    PRIVATE_IP_ALLOCATION_METHOD_FIELD_NUMBER: builtins.int
+    NETWORK_FIELD_NUMBER: builtins.int
+    NIC_TYPE_FIELD_NUMBER: builtins.int
+    NO_PROXY_ACCESS_FIELD_NUMBER: builtins.int
+    NO_PUBLIC_IP_FIELD_NUMBER: builtins.int
+    NO_REMOVE_DATA_DISK_FIELD_NUMBER: builtins.int
+    POST_STARTUP_SCRIPT_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    PROXY_URI_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_SCOPES_FIELD_NUMBER: builtins.int
+    STATE_FIELD_NUMBER: builtins.int
     SUBNET_FIELD_NUMBER: builtins.int
-    PRIMARY_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    private_ip_address: builtins.str
-    private_ip_allocation_method: builtins.str
+    TAGS_FIELD_NUMBER: builtins.int
+    UPDATE_TIME_FIELD_NUMBER: builtins.int
+    ACCELERATOR_CONFIG_FIELD_NUMBER: builtins.int
+    CONTAINER_IMAGE_FIELD_NUMBER: builtins.int
+    RESERVATION_AFFINITY_FIELD_NUMBER: builtins.int
+    SHIELDED_INSTANCE_CONFIG_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    VM_IMAGE_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    boot_disk_size_gb: builtins.float
+    boot_disk_type: builtins.str
+    create_time: builtins.str
+    custom_gpu_driver_path: builtins.str
+    data_disk_size_gb: builtins.float
+    data_disk_type: builtins.str
+    disk_encryption: builtins.str
+    id: builtins.str
+    install_gpu_driver: builtins.bool
+    @property
+    def instance_owners(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    kms_key: builtins.str
     @property
-    def subnet(self) -> global___Subnet: ...
-    primary: builtins.bool
+    def labels(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    location: builtins.str
+    machine_type: builtins.str
+    @property
+    def metadata(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     name: builtins.str
-    def __init__(
-        self,
-        *,
-        private_ip_address: builtins.str = ...,
-        private_ip_allocation_method: builtins.str = ...,
-        subnet: global___Subnet | None = ...,
-        primary: builtins.bool = ...,
-        name: builtins.str = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["subnet", b"subnet"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "primary", b"primary", "private_ip_address", b"private_ip_address", "private_ip_allocation_method", b"private_ip_allocation_method", "subnet", b"subnet"]) -> None: ...
-
-global___ApplicationGatewayPrivateLinkIpConfiguration = ApplicationGatewayPrivateLinkIpConfiguration
-
-@typing_extensions.final
-class ApplicationGatewayAutoscaleConfiguration(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    MIN_CAPACITY_FIELD_NUMBER: builtins.int
-    MAX_CAPACITY_FIELD_NUMBER: builtins.int
-    min_capacity: builtins.int
-    max_capacity: builtins.int
-    def __init__(
-        self,
-        *,
-        min_capacity: builtins.int = ...,
-        max_capacity: builtins.int = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["max_capacity", b"max_capacity", "min_capacity", b"min_capacity"]) -> None: ...
-
-global___ApplicationGatewayAutoscaleConfiguration = ApplicationGatewayAutoscaleConfiguration
-
-@typing_extensions.final
-class ApplicationGatewayWebApplicationFirewallConfiguration(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    ENABLED_FIELD_NUMBER: builtins.int
-    FIREWALL_MODE_FIELD_NUMBER: builtins.int
-    RULE_SET_TYPE_FIELD_NUMBER: builtins.int
-    RULE_SET_VERSION_FIELD_NUMBER: builtins.int
-    DISABLED_RULE_GROUPS_FIELD_NUMBER: builtins.int
-    REQUEST_BODY_CHECK_FIELD_NUMBER: builtins.int
-    MAX_REQUEST_BODY_SIZE_FIELD_NUMBER: builtins.int
-    MAX_REQUEST_BODY_SIZE_IN_KB_FIELD_NUMBER: builtins.int
-    FILE_UPLOAD_LIMIT_IN_MB_FIELD_NUMBER: builtins.int
-    EXCLUSIONS_FIELD_NUMBER: builtins.int
-    enabled: builtins.bool
-    firewall_mode: builtins.str
-    rule_set_type: builtins.str
-    rule_set_version: builtins.str
+    network: builtins.str
+    nic_type: builtins.str
+    no_proxy_access: builtins.bool
+    no_public_ip: builtins.bool
+    no_remove_data_disk: builtins.bool
+    post_startup_script: builtins.str
+    project: builtins.str
+    proxy_uri: builtins.str
+    service_account: builtins.str
     @property
-    def disabled_rule_groups(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayFirewallDisabledRuleGroup]: ...
-    request_body_check: builtins.bool
-    max_request_body_size: builtins.int
-    max_request_body_size_in_kb: builtins.int
-    file_upload_limit_in_mb: builtins.int
+    def service_account_scopes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    state: builtins.str
+    subnet: builtins.str
     @property
-    def exclusions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayFirewallExclusion]: ...
-    def __init__(
-        self,
-        *,
-        enabled: builtins.bool = ...,
-        firewall_mode: builtins.str = ...,
-        rule_set_type: builtins.str = ...,
-        rule_set_version: builtins.str = ...,
-        disabled_rule_groups: collections.abc.Iterable[global___ApplicationGatewayFirewallDisabledRuleGroup] | None = ...,
-        request_body_check: builtins.bool = ...,
-        max_request_body_size: builtins.int = ...,
-        max_request_body_size_in_kb: builtins.int = ...,
-        file_upload_limit_in_mb: builtins.int = ...,
-        exclusions: collections.abc.Iterable[global___ApplicationGatewayFirewallExclusion] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["disabled_rule_groups", b"disabled_rule_groups", "enabled", b"enabled", "exclusions", b"exclusions", "file_upload_limit_in_mb", b"file_upload_limit_in_mb", "firewall_mode", b"firewall_mode", "max_request_body_size", b"max_request_body_size", "max_request_body_size_in_kb", b"max_request_body_size_in_kb", "request_body_check", b"request_body_check", "rule_set_type", b"rule_set_type", "rule_set_version", b"rule_set_version"]) -> None: ...
-
-global___ApplicationGatewayWebApplicationFirewallConfiguration = ApplicationGatewayWebApplicationFirewallConfiguration
-
-@typing_extensions.final
-class ApplicationGatewayFirewallExclusion(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    MATCH_VARIABLE_FIELD_NUMBER: builtins.int
-    SELECTOR_MATCH_OPERATOR_FIELD_NUMBER: builtins.int
-    SELECTOR_FIELD_NUMBER: builtins.int
-    match_variable: builtins.str
-    selector_match_operator: builtins.str
-    selector: builtins.str
-    def __init__(
-        self,
-        *,
-        match_variable: builtins.str = ...,
-        selector_match_operator: builtins.str = ...,
-        selector: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["match_variable", b"match_variable", "selector", b"selector", "selector_match_operator", b"selector_match_operator"]) -> None: ...
-
-global___ApplicationGatewayFirewallExclusion = ApplicationGatewayFirewallExclusion
-
-@typing_extensions.final
-class ApplicationGatewayFirewallDisabledRuleGroup(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    RULE_GROUP_NAME_FIELD_NUMBER: builtins.int
-    RULES_FIELD_NUMBER: builtins.int
-    rule_group_name: builtins.str
+    def tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    update_time: builtins.str
     @property
-    def rules(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.int]: ...
-    def __init__(
-        self,
-        *,
-        rule_group_name: builtins.str = ...,
-        rules: collections.abc.Iterable[builtins.int] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["rule_group_name", b"rule_group_name", "rules", b"rules"]) -> None: ...
-
-global___ApplicationGatewayFirewallDisabledRuleGroup = ApplicationGatewayFirewallDisabledRuleGroup
-
-@typing_extensions.final
-class ApplicationGatewayRedirectConfiguration(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-    REDIRECT_TYPE_FIELD_NUMBER: builtins.int
-    TARGET_LISTENER_FIELD_NUMBER: builtins.int
-    TARGET_URL_FIELD_NUMBER: builtins.int
-    INCLUDE_PATH_FIELD_NUMBER: builtins.int
-    INCLUDE_QUERY_STRING_FIELD_NUMBER: builtins.int
-    REQUEST_ROUTING_RULES_FIELD_NUMBER: builtins.int
-    URL_PATH_MAPS_FIELD_NUMBER: builtins.int
-    PATH_RULES_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    redirect_type: builtins.str
-    target_listener: builtins.str
-    target_url: builtins.str
-    include_path: builtins.bool
-    include_query_string: builtins.bool
+    def accelerator_config(self) -> global___NotebooksInstanceXAcceleratorConfig: ...
     @property
-    def request_routing_rules(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    def container_image(self) -> global___NotebooksInstanceXContainerImage: ...
     @property
-    def url_path_maps(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    def reservation_affinity(self) -> global___NotebooksInstanceXReservationAffinity: ...
     @property
-    def path_rules(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    name: builtins.str
+    def shielded_instance_config(self) -> global___NotebooksInstanceXShieldedInstanceConfig: ...
+    @property
+    def timeouts(self) -> global___NotebooksInstanceXTimeouts: ...
+    @property
+    def vm_image(self) -> global___NotebooksInstanceXVmImage: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        redirect_type: builtins.str = ...,
-        target_listener: builtins.str = ...,
-        target_url: builtins.str = ...,
-        include_path: builtins.bool = ...,
-        include_query_string: builtins.bool = ...,
-        request_routing_rules: collections.abc.Iterable[builtins.str] | None = ...,
-        url_path_maps: collections.abc.Iterable[builtins.str] | None = ...,
-        path_rules: collections.abc.Iterable[builtins.str] | None = ...,
+        boot_disk_size_gb: builtins.float = ...,
+        boot_disk_type: builtins.str = ...,
+        create_time: builtins.str = ...,
+        custom_gpu_driver_path: builtins.str = ...,
+        data_disk_size_gb: builtins.float = ...,
+        data_disk_type: builtins.str = ...,
+        disk_encryption: builtins.str = ...,
+        id: builtins.str = ...,
+        install_gpu_driver: builtins.bool = ...,
+        instance_owners: collections.abc.Iterable[builtins.str] | None = ...,
+        kms_key: builtins.str = ...,
+        labels: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        location: builtins.str = ...,
+        machine_type: builtins.str = ...,
+        metadata: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         name: builtins.str = ...,
+        network: builtins.str = ...,
+        nic_type: builtins.str = ...,
+        no_proxy_access: builtins.bool = ...,
+        no_public_ip: builtins.bool = ...,
+        no_remove_data_disk: builtins.bool = ...,
+        post_startup_script: builtins.str = ...,
+        project: builtins.str = ...,
+        proxy_uri: builtins.str = ...,
+        service_account: builtins.str = ...,
+        service_account_scopes: collections.abc.Iterable[builtins.str] | None = ...,
+        state: builtins.str = ...,
+        subnet: builtins.str = ...,
+        tags: collections.abc.Iterable[builtins.str] | None = ...,
+        update_time: builtins.str = ...,
+        accelerator_config: global___NotebooksInstanceXAcceleratorConfig | None = ...,
+        container_image: global___NotebooksInstanceXContainerImage | None = ...,
+        reservation_affinity: global___NotebooksInstanceXReservationAffinity | None = ...,
+        shielded_instance_config: global___NotebooksInstanceXShieldedInstanceConfig | None = ...,
+        timeouts: global___NotebooksInstanceXTimeouts | None = ...,
+        vm_image: global___NotebooksInstanceXVmImage | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["include_path", b"include_path", "include_query_string", b"include_query_string", "name", b"name", "path_rules", b"path_rules", "redirect_type", b"redirect_type", "request_routing_rules", b"request_routing_rules", "target_listener", b"target_listener", "target_url", b"target_url", "url_path_maps", b"url_path_maps"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "container_image", b"container_image", "reservation_affinity", b"reservation_affinity", "resource_info", b"resource_info", "shielded_instance_config", b"shielded_instance_config", "timeouts", b"timeouts", "vm_image", b"vm_image"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "boot_disk_size_gb", b"boot_disk_size_gb", "boot_disk_type", b"boot_disk_type", "container_image", b"container_image", "create_time", b"create_time", "custom_gpu_driver_path", b"custom_gpu_driver_path", "data_disk_size_gb", b"data_disk_size_gb", "data_disk_type", b"data_disk_type", "disk_encryption", b"disk_encryption", "id", b"id", "install_gpu_driver", b"install_gpu_driver", "instance_owners", b"instance_owners", "kms_key", b"kms_key", "labels", b"labels", "location", b"location", "machine_type", b"machine_type", "metadata", b"metadata", "name", b"name", "network", b"network", "nic_type", b"nic_type", "no_proxy_access", b"no_proxy_access", "no_public_ip", b"no_public_ip", "no_remove_data_disk", b"no_remove_data_disk", "post_startup_script", b"post_startup_script", "project", b"project", "proxy_uri", b"proxy_uri", "reservation_affinity", b"reservation_affinity", "resource_info", b"resource_info", "service_account", b"service_account", "service_account_scopes", b"service_account_scopes", "shielded_instance_config", b"shielded_instance_config", "state", b"state", "subnet", b"subnet", "tags", b"tags", "timeouts", b"timeouts", "update_time", b"update_time", "vm_image", b"vm_image"]) -> None: ...
 
-global___ApplicationGatewayRedirectConfiguration = ApplicationGatewayRedirectConfiguration
+global___NotebooksInstance = NotebooksInstance
 
 @typing_extensions.final
-class ApplicationGatewayRewriteRuleSet(google.protobuf.message.Message):
+class NotebooksInstanceIamBindingXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    REWRITE_RULES_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    @property
-    def rewrite_rules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayRewriteRule]: ...
-    name: builtins.str
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    EXPRESSION_FIELD_NUMBER: builtins.int
+    TITLE_FIELD_NUMBER: builtins.int
+    description: builtins.str
+    expression: builtins.str
+    title: builtins.str
     def __init__(
         self,
         *,
-        rewrite_rules: collections.abc.Iterable[global___ApplicationGatewayRewriteRule] | None = ...,
-        name: builtins.str = ...,
+        description: builtins.str = ...,
+        expression: builtins.str = ...,
+        title: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "rewrite_rules", b"rewrite_rules"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
 
-global___ApplicationGatewayRewriteRuleSet = ApplicationGatewayRewriteRuleSet
+global___NotebooksInstanceIamBindingXCondition = NotebooksInstanceIamBindingXCondition
 
 @typing_extensions.final
-class ApplicationGatewayRewriteRule(google.protobuf.message.Message):
+class NotebooksInstanceIamBinding(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    RULE_SEQUENCE_FIELD_NUMBER: builtins.int
-    CONDITIONS_FIELD_NUMBER: builtins.int
-    ACTION_SET_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    rule_sequence: builtins.int
+    ETAG_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    INSTANCE_NAME_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    MEMBERS_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    CONDITION_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    etag: builtins.str
+    id: builtins.str
+    instance_name: builtins.str
+    location: builtins.str
     @property
-    def conditions(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayRewriteRuleCondition]: ...
+    def members(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    project: builtins.str
+    role: builtins.str
     @property
-    def action_set(self) -> global___ApplicationGatewayRewriteRuleActionSet: ...
+    def condition(self) -> global___NotebooksInstanceIamBindingXCondition: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        name: builtins.str = ...,
-        rule_sequence: builtins.int = ...,
-        conditions: collections.abc.Iterable[global___ApplicationGatewayRewriteRuleCondition] | None = ...,
-        action_set: global___ApplicationGatewayRewriteRuleActionSet | None = ...,
+        etag: builtins.str = ...,
+        id: builtins.str = ...,
+        instance_name: builtins.str = ...,
+        location: builtins.str = ...,
+        members: collections.abc.Iterable[builtins.str] | None = ...,
+        project: builtins.str = ...,
+        role: builtins.str = ...,
+        condition: global___NotebooksInstanceIamBindingXCondition | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["action_set", b"action_set"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["action_set", b"action_set", "conditions", b"conditions", "name", b"name", "rule_sequence", b"rule_sequence"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "instance_name", b"instance_name", "location", b"location", "members", b"members", "project", b"project", "resource_info", b"resource_info", "role", b"role"]) -> None: ...
 
-global___ApplicationGatewayRewriteRule = ApplicationGatewayRewriteRule
+global___NotebooksInstanceIamBinding = NotebooksInstanceIamBinding
 
 @typing_extensions.final
-class ApplicationGatewayRewriteRuleActionSet(google.protobuf.message.Message):
+class NotebooksInstanceIamMemberXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    REQUEST_HEADER_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    RESPONSE_HEADER_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    URL_CONFIGURATION_FIELD_NUMBER: builtins.int
-    @property
-    def request_header_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayHeaderConfiguration]: ...
-    @property
-    def response_header_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayHeaderConfiguration]: ...
-    @property
-    def url_configuration(self) -> global___ApplicationGatewayUrlConfiguration: ...
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    EXPRESSION_FIELD_NUMBER: builtins.int
+    TITLE_FIELD_NUMBER: builtins.int
+    description: builtins.str
+    expression: builtins.str
+    title: builtins.str
     def __init__(
         self,
         *,
-        request_header_configurations: collections.abc.Iterable[global___ApplicationGatewayHeaderConfiguration] | None = ...,
-        response_header_configurations: collections.abc.Iterable[global___ApplicationGatewayHeaderConfiguration] | None = ...,
-        url_configuration: global___ApplicationGatewayUrlConfiguration | None = ...,
+        description: builtins.str = ...,
+        expression: builtins.str = ...,
+        title: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["url_configuration", b"url_configuration"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["request_header_configurations", b"request_header_configurations", "response_header_configurations", b"response_header_configurations", "url_configuration", b"url_configuration"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
 
-global___ApplicationGatewayRewriteRuleActionSet = ApplicationGatewayRewriteRuleActionSet
+global___NotebooksInstanceIamMemberXCondition = NotebooksInstanceIamMemberXCondition
 
 @typing_extensions.final
-class ApplicationGatewayUrlConfiguration(google.protobuf.message.Message):
+class NotebooksInstanceIamMember(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    MODIFIED_PATH_FIELD_NUMBER: builtins.int
-    MODIFIED_QUERY_STRING_FIELD_NUMBER: builtins.int
-    REROUTE_FIELD_NUMBER: builtins.int
-    modified_path: builtins.str
-    modified_query_string: builtins.str
-    reroute: builtins.bool
+    ETAG_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    INSTANCE_NAME_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    MEMBER_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    CONDITION_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    etag: builtins.str
+    id: builtins.str
+    instance_name: builtins.str
+    location: builtins.str
+    member: builtins.str
+    project: builtins.str
+    role: builtins.str
+    @property
+    def condition(self) -> global___NotebooksInstanceIamMemberXCondition: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        modified_path: builtins.str = ...,
-        modified_query_string: builtins.str = ...,
-        reroute: builtins.bool = ...,
+        etag: builtins.str = ...,
+        id: builtins.str = ...,
+        instance_name: builtins.str = ...,
+        location: builtins.str = ...,
+        member: builtins.str = ...,
+        project: builtins.str = ...,
+        role: builtins.str = ...,
+        condition: global___NotebooksInstanceIamMemberXCondition | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["modified_path", b"modified_path", "modified_query_string", b"modified_query_string", "reroute", b"reroute"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "instance_name", b"instance_name", "location", b"location", "member", b"member", "project", b"project", "resource_info", b"resource_info", "role", b"role"]) -> None: ...
 
-global___ApplicationGatewayUrlConfiguration = ApplicationGatewayUrlConfiguration
+global___NotebooksInstanceIamMember = NotebooksInstanceIamMember
 
 @typing_extensions.final
-class ApplicationGatewayHeaderConfiguration(google.protobuf.message.Message):
+class NotebooksInstanceIamPolicy(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    HEADER_NAME_FIELD_NUMBER: builtins.int
-    HEADER_VALUE_FIELD_NUMBER: builtins.int
-    header_name: builtins.str
-    header_value: builtins.str
+    ETAG_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    INSTANCE_NAME_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    POLICY_DATA_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    etag: builtins.str
+    id: builtins.str
+    instance_name: builtins.str
+    location: builtins.str
+    policy_data: builtins.str
+    project: builtins.str
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        header_name: builtins.str = ...,
-        header_value: builtins.str = ...,
+        etag: builtins.str = ...,
+        id: builtins.str = ...,
+        instance_name: builtins.str = ...,
+        location: builtins.str = ...,
+        policy_data: builtins.str = ...,
+        project: builtins.str = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["header_name", b"header_name", "header_value", b"header_value"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["etag", b"etag", "id", b"id", "instance_name", b"instance_name", "location", b"location", "policy_data", b"policy_data", "project", b"project", "resource_info", b"resource_info"]) -> None: ...
 
-global___ApplicationGatewayHeaderConfiguration = ApplicationGatewayHeaderConfiguration
+global___NotebooksInstanceIamPolicy = NotebooksInstanceIamPolicy
 
 @typing_extensions.final
-class ApplicationGatewayRewriteRuleCondition(google.protobuf.message.Message):
+class NotebooksLocationXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    VARIABLE_FIELD_NUMBER: builtins.int
-    PATTERN_FIELD_NUMBER: builtins.int
-    IGNORE_CASE_FIELD_NUMBER: builtins.int
-    NEGATE_FIELD_NUMBER: builtins.int
-    variable: builtins.str
-    pattern: builtins.str
-    ignore_case: builtins.bool
-    negate: builtins.bool
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
     def __init__(
         self,
         *,
-        variable: builtins.str = ...,
-        pattern: builtins.str = ...,
-        ignore_case: builtins.bool = ...,
-        negate: builtins.bool = ...,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["ignore_case", b"ignore_case", "negate", b"negate", "pattern", b"pattern", "variable", b"variable"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___ApplicationGatewayRewriteRuleCondition = ApplicationGatewayRewriteRuleCondition
+global___NotebooksLocationXTimeouts = NotebooksLocationXTimeouts
 
 @typing_extensions.final
-class ApplicationGatewayRequestRoutingRule(google.protobuf.message.Message):
+class NotebooksLocation(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    RULE_TYPE_FIELD_NUMBER: builtins.int
-    PRIORITY_FIELD_NUMBER: builtins.int
-    BACKEND_ADDRESS_POOL_FIELD_NUMBER: builtins.int
-    BACKEND_HTTP_SETTINGS_FIELD_NUMBER: builtins.int
-    HTTP_LISTENER_FIELD_NUMBER: builtins.int
-    URL_PATH_MAP_FIELD_NUMBER: builtins.int
-    REWRITE_RULE_SET_FIELD_NUMBER: builtins.int
-    REDIRECT_CONFIGURATION_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    rule_type: builtins.str
-    priority: builtins.int
-    @property
-    def backend_address_pool(self) -> global___BackendAddressPool: ...
+    PROJECT_FIELD_NUMBER: builtins.int
+    SELF_LINK_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    id: builtins.str
+    name: builtins.str
+    project: builtins.str
+    self_link: builtins.str
     @property
-    def backend_http_settings(self) -> global___BackendHttpSettings: ...
+    def timeouts(self) -> global___NotebooksLocationXTimeouts: ...
     @property
-    def http_listener(self) -> global___HttpListener: ...
-    url_path_map: builtins.str
-    rewrite_rule_set: builtins.str
-    redirect_configuration: builtins.str
-    name: builtins.str
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        rule_type: builtins.str = ...,
-        priority: builtins.int = ...,
-        backend_address_pool: global___BackendAddressPool | None = ...,
-        backend_http_settings: global___BackendHttpSettings | None = ...,
-        http_listener: global___HttpListener | None = ...,
-        url_path_map: builtins.str = ...,
-        rewrite_rule_set: builtins.str = ...,
-        redirect_configuration: builtins.str = ...,
+        id: builtins.str = ...,
         name: builtins.str = ...,
+        project: builtins.str = ...,
+        self_link: builtins.str = ...,
+        timeouts: global___NotebooksLocationXTimeouts | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["backend_address_pool", b"backend_address_pool", "backend_http_settings", b"backend_http_settings", "http_listener", b"http_listener"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["backend_address_pool", b"backend_address_pool", "backend_http_settings", b"backend_http_settings", "http_listener", b"http_listener", "name", b"name", "priority", b"priority", "redirect_configuration", b"redirect_configuration", "rewrite_rule_set", b"rewrite_rule_set", "rule_type", b"rule_type", "url_path_map", b"url_path_map"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "name", b"name", "project", b"project", "resource_info", b"resource_info", "self_link", b"self_link", "timeouts", b"timeouts"]) -> None: ...
 
-global___ApplicationGatewayRequestRoutingRule = ApplicationGatewayRequestRoutingRule
+global___NotebooksLocation = NotebooksLocation
 
 @typing_extensions.final
-class ApplicationGatewayUrlPathMap(google.protobuf.message.Message):
+class NotebooksRuntimeXAccessConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DEFAULT_BACKEND_ADDRESS_POOL_FIELD_NUMBER: builtins.int
-    DEFAULT_BACKEND_HTTP_SETTINGS_FIELD_NUMBER: builtins.int
-    DEFAULT_REWRITE_RULE_SET_FIELD_NUMBER: builtins.int
-    DEFAULT_REDIRECT_CONFIGURATION_FIELD_NUMBER: builtins.int
-    PATH_RULES_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    default_backend_address_pool: builtins.str
-    default_backend_http_settings: builtins.str
-    default_rewrite_rule_set: builtins.str
-    default_redirect_configuration: builtins.str
-    @property
-    def path_rules(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayPathRule]: ...
-    name: builtins.str
+    ACCESS_TYPE_FIELD_NUMBER: builtins.int
+    PROXY_URI_FIELD_NUMBER: builtins.int
+    RUNTIME_OWNER_FIELD_NUMBER: builtins.int
+    access_type: builtins.str
+    proxy_uri: builtins.str
+    runtime_owner: builtins.str
     def __init__(
         self,
         *,
-        default_backend_address_pool: builtins.str = ...,
-        default_backend_http_settings: builtins.str = ...,
-        default_rewrite_rule_set: builtins.str = ...,
-        default_redirect_configuration: builtins.str = ...,
-        path_rules: collections.abc.Iterable[global___ApplicationGatewayPathRule] | None = ...,
-        name: builtins.str = ...,
+        access_type: builtins.str = ...,
+        proxy_uri: builtins.str = ...,
+        runtime_owner: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["default_backend_address_pool", b"default_backend_address_pool", "default_backend_http_settings", b"default_backend_http_settings", "default_redirect_configuration", b"default_redirect_configuration", "default_rewrite_rule_set", b"default_rewrite_rule_set", "name", b"name", "path_rules", b"path_rules"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["access_type", b"access_type", "proxy_uri", b"proxy_uri", "runtime_owner", b"runtime_owner"]) -> None: ...
 
-global___ApplicationGatewayUrlPathMap = ApplicationGatewayUrlPathMap
+global___NotebooksRuntimeXAccessConfig = NotebooksRuntimeXAccessConfig
 
 @typing_extensions.final
-class ApplicationGatewayPathRule(google.protobuf.message.Message):
+class NotebooksRuntimeXSoftwareConfigXKernels(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PATHS_FIELD_NUMBER: builtins.int
-    BACKEND_ADDRESS_POOL_FIELD_NUMBER: builtins.int
-    BACKEND_HTTP_SETTINGS_FIELD_NUMBER: builtins.int
-    REDIRECT_CONFIGURATION_FIELD_NUMBER: builtins.int
-    REWRITE_RULE_SET_FIELD_NUMBER: builtins.int
-    FIREWALL_POLICY_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    @property
-    def paths(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    @property
-    def backend_address_pool(self) -> global___BackendAddressPool: ...
-    @property
-    def backend_http_settings(self) -> global___BackendHttpSettings: ...
-    redirect_configuration: builtins.str
-    rewrite_rule_set: builtins.str
-    firewall_policy: builtins.str
-    name: builtins.str
+    REPOSITORY_FIELD_NUMBER: builtins.int
+    TAG_FIELD_NUMBER: builtins.int
+    repository: builtins.str
+    tag: builtins.str
     def __init__(
         self,
         *,
-        paths: collections.abc.Iterable[builtins.str] | None = ...,
-        backend_address_pool: global___BackendAddressPool | None = ...,
-        backend_http_settings: global___BackendHttpSettings | None = ...,
-        redirect_configuration: builtins.str = ...,
-        rewrite_rule_set: builtins.str = ...,
-        firewall_policy: builtins.str = ...,
-        name: builtins.str = ...,
+        repository: builtins.str = ...,
+        tag: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["backend_address_pool", b"backend_address_pool", "backend_http_settings", b"backend_http_settings"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["backend_address_pool", b"backend_address_pool", "backend_http_settings", b"backend_http_settings", "firewall_policy", b"firewall_policy", "name", b"name", "paths", b"paths", "redirect_configuration", b"redirect_configuration", "rewrite_rule_set", b"rewrite_rule_set"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
 
-global___ApplicationGatewayPathRule = ApplicationGatewayPathRule
+global___NotebooksRuntimeXSoftwareConfigXKernels = NotebooksRuntimeXSoftwareConfigXKernels
 
 @typing_extensions.final
-class ApplicationGatewaySslProfile(google.protobuf.message.Message):
+class NotebooksRuntimeXSoftwareConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    TRUSTED_CLIENT_CERTIFICATES_FIELD_NUMBER: builtins.int
-    SSL_POLICY_FIELD_NUMBER: builtins.int
-    CLIENT_AUTH_CONFIGURATION_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    @property
-    def trusted_client_certificates(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    CUSTOM_GPU_DRIVER_PATH_FIELD_NUMBER: builtins.int
+    ENABLE_HEALTH_MONITORING_FIELD_NUMBER: builtins.int
+    IDLE_SHUTDOWN_FIELD_NUMBER: builtins.int
+    IDLE_SHUTDOWN_TIMEOUT_FIELD_NUMBER: builtins.int
+    INSTALL_GPU_DRIVER_FIELD_NUMBER: builtins.int
+    NOTEBOOK_UPGRADE_SCHEDULE_FIELD_NUMBER: builtins.int
+    POST_STARTUP_SCRIPT_FIELD_NUMBER: builtins.int
+    POST_STARTUP_SCRIPT_BEHAVIOR_FIELD_NUMBER: builtins.int
+    UPGRADEABLE_FIELD_NUMBER: builtins.int
+    KERNELS_FIELD_NUMBER: builtins.int
+    custom_gpu_driver_path: builtins.str
+    enable_health_monitoring: builtins.bool
+    idle_shutdown: builtins.bool
+    idle_shutdown_timeout: builtins.float
+    install_gpu_driver: builtins.bool
+    notebook_upgrade_schedule: builtins.str
+    post_startup_script: builtins.str
+    post_startup_script_behavior: builtins.str
+    upgradeable: builtins.bool
     @property
-    def ssl_policy(self) -> global___ApplicationGatewaySslPolicy: ...
-    @property
-    def client_auth_configuration(self) -> global___ApplicationGatewayClientAuthConfiguration: ...
-    name: builtins.str
+    def kernels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NotebooksRuntimeXSoftwareConfigXKernels]: ...
     def __init__(
         self,
         *,
-        trusted_client_certificates: collections.abc.Iterable[builtins.str] | None = ...,
-        ssl_policy: global___ApplicationGatewaySslPolicy | None = ...,
-        client_auth_configuration: global___ApplicationGatewayClientAuthConfiguration | None = ...,
-        name: builtins.str = ...,
+        custom_gpu_driver_path: builtins.str = ...,
+        enable_health_monitoring: builtins.bool = ...,
+        idle_shutdown: builtins.bool = ...,
+        idle_shutdown_timeout: builtins.float = ...,
+        install_gpu_driver: builtins.bool = ...,
+        notebook_upgrade_schedule: builtins.str = ...,
+        post_startup_script: builtins.str = ...,
+        post_startup_script_behavior: builtins.str = ...,
+        upgradeable: builtins.bool = ...,
+        kernels: collections.abc.Iterable[global___NotebooksRuntimeXSoftwareConfigXKernels] | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["client_auth_configuration", b"client_auth_configuration", "ssl_policy", b"ssl_policy"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["client_auth_configuration", b"client_auth_configuration", "name", b"name", "ssl_policy", b"ssl_policy", "trusted_client_certificates", b"trusted_client_certificates"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["custom_gpu_driver_path", b"custom_gpu_driver_path", "enable_health_monitoring", b"enable_health_monitoring", "idle_shutdown", b"idle_shutdown", "idle_shutdown_timeout", b"idle_shutdown_timeout", "install_gpu_driver", b"install_gpu_driver", "kernels", b"kernels", "notebook_upgrade_schedule", b"notebook_upgrade_schedule", "post_startup_script", b"post_startup_script", "post_startup_script_behavior", b"post_startup_script_behavior", "upgradeable", b"upgradeable"]) -> None: ...
 
-global___ApplicationGatewaySslProfile = ApplicationGatewaySslProfile
+global___NotebooksRuntimeXSoftwareConfig = NotebooksRuntimeXSoftwareConfig
 
 @typing_extensions.final
-class ApplicationGatewayClientAuthConfiguration(google.protobuf.message.Message):
+class NotebooksRuntimeXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    VERIFY_CLIENT_CERT_ISSUER_D_N_FIELD_NUMBER: builtins.int
-    verify_client_cert_issuer_d_n: builtins.bool
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
     def __init__(
         self,
         *,
-        verify_client_cert_issuer_d_n: builtins.bool = ...,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["verify_client_cert_issuer_d_n", b"verify_client_cert_issuer_d_n"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___ApplicationGatewayClientAuthConfiguration = ApplicationGatewayClientAuthConfiguration
+global___NotebooksRuntimeXTimeouts = NotebooksRuntimeXTimeouts
 
 @typing_extensions.final
-class ApplicationGatewayHttpListener(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    FRONTEND_IP_CONFIGURATION_FIELD_NUMBER: builtins.int
-    FRONTEND_PORT_FIELD_NUMBER: builtins.int
-    PROTOCOL_FIELD_NUMBER: builtins.int
-    HOST_NAME_FIELD_NUMBER: builtins.int
-    SSL_CERTIFICATE_FIELD_NUMBER: builtins.int
-    SSL_PROFILE_FIELD_NUMBER: builtins.int
-    REQUIRE_SERVER_NAME_INDICATION_FIELD_NUMBER: builtins.int
-    CUSTOM_ERROR_CONFIGURATIONS_FIELD_NUMBER: builtins.int
-    FIREWALL_POLICY_FIELD_NUMBER: builtins.int
-    HOST_NAMES_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    @property
-    def frontend_ip_configuration(self) -> global___FrontendIPConfiguration: ...
-    @property
-    def frontend_port(self) -> global___FrontendPort: ...
-    protocol: builtins.str
-    host_name: builtins.str
-    ssl_certificate: builtins.str
-    ssl_profile: builtins.str
-    require_server_name_indication: builtins.bool
-    @property
-    def custom_error_configurations(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayCustomError]: ...
-    firewall_policy: builtins.str
-    @property
-    def host_names(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    name: builtins.str
+    CORE_COUNT_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    core_count: builtins.float
+    type: builtins.str
     def __init__(
         self,
         *,
-        frontend_ip_configuration: global___FrontendIPConfiguration | None = ...,
-        frontend_port: global___FrontendPort | None = ...,
-        protocol: builtins.str = ...,
-        host_name: builtins.str = ...,
-        ssl_certificate: builtins.str = ...,
-        ssl_profile: builtins.str = ...,
-        require_server_name_indication: builtins.bool = ...,
-        custom_error_configurations: collections.abc.Iterable[global___ApplicationGatewayCustomError] | None = ...,
-        firewall_policy: builtins.str = ...,
-        host_names: collections.abc.Iterable[builtins.str] | None = ...,
-        name: builtins.str = ...,
+        core_count: builtins.float = ...,
+        type: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["frontend_ip_configuration", b"frontend_ip_configuration", "frontend_port", b"frontend_port"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_error_configurations", b"custom_error_configurations", "firewall_policy", b"firewall_policy", "frontend_ip_configuration", b"frontend_ip_configuration", "frontend_port", b"frontend_port", "host_name", b"host_name", "host_names", b"host_names", "name", b"name", "protocol", b"protocol", "require_server_name_indication", b"require_server_name_indication", "ssl_certificate", b"ssl_certificate", "ssl_profile", b"ssl_profile"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["core_count", b"core_count", "type", b"type"]) -> None: ...
 
-global___ApplicationGatewayHttpListener = ApplicationGatewayHttpListener
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig
 
 @typing_extensions.final
-class ApplicationGatewayCustomError(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    STATUS_CODE_FIELD_NUMBER: builtins.int
-    CUSTOM_ERROR_PAGE_URL_FIELD_NUMBER: builtins.int
-    status_code: builtins.str
-    custom_error_page_url: builtins.str
+    REPOSITORY_FIELD_NUMBER: builtins.int
+    TAG_FIELD_NUMBER: builtins.int
+    repository: builtins.str
+    tag: builtins.str
     def __init__(
         self,
         *,
-        status_code: builtins.str = ...,
-        custom_error_page_url: builtins.str = ...,
+        repository: builtins.str = ...,
+        tag: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_error_page_url", b"custom_error_page_url", "status_code", b"status_code"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
 
-global___ApplicationGatewayCustomError = ApplicationGatewayCustomError
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages
 
 @typing_extensions.final
-class ApplicationGatewayBackendHttpSettings(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PORT_FIELD_NUMBER: builtins.int
-    PROTOCOL_FIELD_NUMBER: builtins.int
-    COOKIE_BASED_AFFINITY_FIELD_NUMBER: builtins.int
-    REQUEST_TIMEOUT_FIELD_NUMBER: builtins.int
-    PROBE_FIELD_NUMBER: builtins.int
-    AUTHENTICATION_CERTIFICATES_FIELD_NUMBER: builtins.int
-    TRUSTED_ROOT_CERTIFICATES_FIELD_NUMBER: builtins.int
-    CONNECTION_DRAINING_FIELD_NUMBER: builtins.int
-    HOST_NAME_FIELD_NUMBER: builtins.int
-    PICK_HOST_NAME_FROM_BACKEND_ADDRESS_FIELD_NUMBER: builtins.int
-    AFFINITY_COOKIE_NAME_FIELD_NUMBER: builtins.int
-    PROBE_ENABLED_FIELD_NUMBER: builtins.int
-    PATH_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    port: builtins.int
-    protocol: builtins.str
-    cookie_based_affinity: builtins.str
-    request_timeout: builtins.int
-    probe: builtins.str
-    @property
-    def authentication_certificates(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    @property
-    def trusted_root_certificates(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    @property
-    def connection_draining(self) -> global___ApplicationGatewayConnectionDraining: ...
-    host_name: builtins.str
-    pick_host_name_from_backend_address: builtins.bool
-    affinity_cookie_name: builtins.str
-    probe_enabled: builtins.bool
-    path: builtins.str
-    name: builtins.str
-    def __init__(
-        self,
-        *,
-        port: builtins.int = ...,
-        protocol: builtins.str = ...,
-        cookie_based_affinity: builtins.str = ...,
-        request_timeout: builtins.int = ...,
-        probe: builtins.str = ...,
-        authentication_certificates: collections.abc.Iterable[builtins.str] | None = ...,
-        trusted_root_certificates: collections.abc.Iterable[builtins.str] | None = ...,
-        connection_draining: global___ApplicationGatewayConnectionDraining | None = ...,
-        host_name: builtins.str = ...,
-        pick_host_name_from_backend_address: builtins.bool = ...,
-        affinity_cookie_name: builtins.str = ...,
-        probe_enabled: builtins.bool = ...,
-        path: builtins.str = ...,
-        name: builtins.str = ...,
-    ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["connection_draining", b"connection_draining"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["affinity_cookie_name", b"affinity_cookie_name", "authentication_certificates", b"authentication_certificates", "connection_draining", b"connection_draining", "cookie_based_affinity", b"cookie_based_affinity", "host_name", b"host_name", "name", b"name", "path", b"path", "pick_host_name_from_backend_address", b"pick_host_name_from_backend_address", "port", b"port", "probe", b"probe", "probe_enabled", b"probe_enabled", "protocol", b"protocol", "request_timeout", b"request_timeout", "trusted_root_certificates", b"trusted_root_certificates"]) -> None: ...
-
-global___ApplicationGatewayBackendHttpSettings = ApplicationGatewayBackendHttpSettings
+    @typing_extensions.final
+    class LabelsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-@typing_extensions.final
-class ApplicationGatewayConnectionDraining(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    ENABLED_FIELD_NUMBER: builtins.int
-    DRAIN_TIMEOUT_IN_SEC_FIELD_NUMBER: builtins.int
-    enabled: builtins.bool
-    drain_timeout_in_sec: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    DISK_NAME_FIELD_NUMBER: builtins.int
+    DISK_SIZE_GB_FIELD_NUMBER: builtins.int
+    DISK_TYPE_FIELD_NUMBER: builtins.int
+    LABELS_FIELD_NUMBER: builtins.int
+    description: builtins.str
+    disk_name: builtins.str
+    disk_size_gb: builtins.float
+    disk_type: builtins.str
+    @property
+    def labels(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     def __init__(
         self,
         *,
-        enabled: builtins.bool = ...,
-        drain_timeout_in_sec: builtins.int = ...,
+        description: builtins.str = ...,
+        disk_name: builtins.str = ...,
+        disk_size_gb: builtins.float = ...,
+        disk_type: builtins.str = ...,
+        labels: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["drain_timeout_in_sec", b"drain_timeout_in_sec", "enabled", b"enabled"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "disk_name", b"disk_name", "disk_size_gb", b"disk_size_gb", "disk_type", b"disk_type", "labels", b"labels"]) -> None: ...
 
-global___ApplicationGatewayConnectionDraining = ApplicationGatewayConnectionDraining
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams
 
 @typing_extensions.final
-class ApplicationGatewayBackendAddressPool(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BACKEND_ADDRESSES_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
+    AUTO_DELETE_FIELD_NUMBER: builtins.int
+    BOOT_FIELD_NUMBER: builtins.int
+    DEVICE_NAME_FIELD_NUMBER: builtins.int
+    GUEST_OS_FEATURES_FIELD_NUMBER: builtins.int
+    INDEX_FIELD_NUMBER: builtins.int
+    INTERFACE_FIELD_NUMBER: builtins.int
+    KIND_FIELD_NUMBER: builtins.int
+    LICENSES_FIELD_NUMBER: builtins.int
+    MODE_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    INITIALIZE_PARAMS_FIELD_NUMBER: builtins.int
+    auto_delete: builtins.bool
+    boot: builtins.bool
+    device_name: builtins.str
+    @property
+    def guest_os_features(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    index: builtins.float
+    interface: builtins.str
+    kind: builtins.str
+    @property
+    def licenses(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    mode: builtins.str
+    source: builtins.str
+    type: builtins.str
     @property
-    def backend_addresses(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___ApplicationGatewayBackendAddress]: ...
-    name: builtins.str
+    def initialize_params(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams: ...
     def __init__(
         self,
         *,
-        backend_addresses: collections.abc.Iterable[global___ApplicationGatewayBackendAddress] | None = ...,
-        name: builtins.str = ...,
+        auto_delete: builtins.bool = ...,
+        boot: builtins.bool = ...,
+        device_name: builtins.str = ...,
+        guest_os_features: collections.abc.Iterable[builtins.str] | None = ...,
+        index: builtins.float = ...,
+        interface: builtins.str = ...,
+        kind: builtins.str = ...,
+        licenses: collections.abc.Iterable[builtins.str] | None = ...,
+        mode: builtins.str = ...,
+        source: builtins.str = ...,
+        type: builtins.str = ...,
+        initialize_params: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["backend_addresses", b"backend_addresses", "name", b"name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["initialize_params", b"initialize_params"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["auto_delete", b"auto_delete", "boot", b"boot", "device_name", b"device_name", "guest_os_features", b"guest_os_features", "index", b"index", "initialize_params", b"initialize_params", "interface", b"interface", "kind", b"kind", "licenses", b"licenses", "mode", b"mode", "source", b"source", "type", b"type"]) -> None: ...
 
-global___ApplicationGatewayBackendAddressPool = ApplicationGatewayBackendAddressPool
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk
 
 @typing_extensions.final
-class ApplicationGatewayBackendAddress(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    FQDN_FIELD_NUMBER: builtins.int
-    IP_ADDRESS_FIELD_NUMBER: builtins.int
-    fqdn: builtins.str
-    ip_address: builtins.str
+    KMS_KEY_FIELD_NUMBER: builtins.int
+    kms_key: builtins.str
     def __init__(
         self,
         *,
-        fqdn: builtins.str = ...,
-        ip_address: builtins.str = ...,
+        kms_key: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["fqdn", b"fqdn", "ip_address", b"ip_address"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["kms_key", b"kms_key"]) -> None: ...
 
-global___ApplicationGatewayBackendAddress = ApplicationGatewayBackendAddress
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig
 
 @typing_extensions.final
-class ApplicationGatewayProbe(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PROTOCOL_FIELD_NUMBER: builtins.int
-    HOST_FIELD_NUMBER: builtins.int
-    PATH_FIELD_NUMBER: builtins.int
-    INTERVAL_FIELD_NUMBER: builtins.int
-    TIMEOUT_FIELD_NUMBER: builtins.int
-    UNHEALTHY_THRESHOLD_FIELD_NUMBER: builtins.int
-    PICK_HOST_NAME_FROM_BACKEND_HTTP_SETTINGS_FIELD_NUMBER: builtins.int
-    MIN_SERVERS_FIELD_NUMBER: builtins.int
-    MATCH_FIELD_NUMBER: builtins.int
-    PORT_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    protocol: builtins.str
-    host: builtins.str
-    path: builtins.str
-    interval: builtins.int
-    timeout: builtins.int
-    unhealthy_threshold: builtins.int
-    pick_host_name_from_backend_http_settings: builtins.bool
-    min_servers: builtins.int
-    @property
-    def match(self) -> global___ApplicationGatewayProbeHealthResponseMatch: ...
-    port: builtins.int
-    name: builtins.str
+    ENABLE_INTEGRITY_MONITORING_FIELD_NUMBER: builtins.int
+    ENABLE_SECURE_BOOT_FIELD_NUMBER: builtins.int
+    ENABLE_VTPM_FIELD_NUMBER: builtins.int
+    enable_integrity_monitoring: builtins.bool
+    enable_secure_boot: builtins.bool
+    enable_vtpm: builtins.bool
     def __init__(
         self,
         *,
-        protocol: builtins.str = ...,
-        host: builtins.str = ...,
-        path: builtins.str = ...,
-        interval: builtins.int = ...,
-        timeout: builtins.int = ...,
-        unhealthy_threshold: builtins.int = ...,
-        pick_host_name_from_backend_http_settings: builtins.bool = ...,
-        min_servers: builtins.int = ...,
-        match: global___ApplicationGatewayProbeHealthResponseMatch | None = ...,
-        port: builtins.int = ...,
-        name: builtins.str = ...,
+        enable_integrity_monitoring: builtins.bool = ...,
+        enable_secure_boot: builtins.bool = ...,
+        enable_vtpm: builtins.bool = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["match", b"match"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["host", b"host", "interval", b"interval", "match", b"match", "min_servers", b"min_servers", "name", b"name", "path", b"path", "pick_host_name_from_backend_http_settings", b"pick_host_name_from_backend_http_settings", "port", b"port", "protocol", b"protocol", "timeout", b"timeout", "unhealthy_threshold", b"unhealthy_threshold"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["enable_integrity_monitoring", b"enable_integrity_monitoring", "enable_secure_boot", b"enable_secure_boot", "enable_vtpm", b"enable_vtpm"]) -> None: ...
 
-global___ApplicationGatewayProbe = ApplicationGatewayProbe
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig
 
 @typing_extensions.final
-class ApplicationGatewayProbeHealthResponseMatch(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachineXVirtualMachineConfig(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    BODY_FIELD_NUMBER: builtins.int
-    STATUS_CODES_FIELD_NUMBER: builtins.int
-    body: builtins.str
-    @property
-    def status_codes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    def __init__(
-        self,
-        *,
-        body: builtins.str = ...,
-        status_codes: collections.abc.Iterable[builtins.str] | None = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["body", b"body", "status_codes", b"status_codes"]) -> None: ...
+    @typing_extensions.final
+    class GuestAttributesEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-global___ApplicationGatewayProbeHealthResponseMatch = ApplicationGatewayProbeHealthResponseMatch
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-@typing_extensions.final
-class ApplicationGatewayFrontendPort(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    @typing_extensions.final
+    class LabelsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    PORT_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    port: builtins.int
-    name: builtins.str
-    def __init__(
-        self,
-        *,
-        port: builtins.int = ...,
-        name: builtins.str = ...,
-    ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "port", b"port"]) -> None: ...
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-global___ApplicationGatewayFrontendPort = ApplicationGatewayFrontendPort
+    @typing_extensions.final
+    class MetadataEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-@typing_extensions.final
-class ApplicationGatewayFrontendIPConfiguration(google.protobuf.message.Message):
-    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    PRIVATE_IP_ADDRESS_FIELD_NUMBER: builtins.int
-    PRIVATE_IP_ALLOCATION_METHOD_FIELD_NUMBER: builtins.int
+    GUEST_ATTRIBUTES_FIELD_NUMBER: builtins.int
+    INTERNAL_IP_ONLY_FIELD_NUMBER: builtins.int
+    LABELS_FIELD_NUMBER: builtins.int
+    MACHINE_TYPE_FIELD_NUMBER: builtins.int
+    METADATA_FIELD_NUMBER: builtins.int
+    NETWORK_FIELD_NUMBER: builtins.int
+    NIC_TYPE_FIELD_NUMBER: builtins.int
+    RESERVED_IP_RANGE_FIELD_NUMBER: builtins.int
     SUBNET_FIELD_NUMBER: builtins.int
-    PRIVATE_LINK_CONFIGURATION_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    PUBLIC_IP_ADDRESS_FIELD_NUMBER: builtins.int
-    private_ip_address: builtins.str
-    private_ip_allocation_method: builtins.str
+    TAGS_FIELD_NUMBER: builtins.int
+    ZONE_FIELD_NUMBER: builtins.int
+    ACCELERATOR_CONFIG_FIELD_NUMBER: builtins.int
+    CONTAINER_IMAGES_FIELD_NUMBER: builtins.int
+    DATA_DISK_FIELD_NUMBER: builtins.int
+    ENCRYPTION_CONFIG_FIELD_NUMBER: builtins.int
+    SHIELDED_INSTANCE_CONFIG_FIELD_NUMBER: builtins.int
     @property
-    def subnet(self) -> global___Subnet: ...
-    private_link_configuration: builtins.str
-    name: builtins.str
+    def guest_attributes(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    internal_ip_only: builtins.bool
+    @property
+    def labels(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    machine_type: builtins.str
+    @property
+    def metadata(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    network: builtins.str
+    nic_type: builtins.str
+    reserved_ip_range: builtins.str
+    subnet: builtins.str
     @property
-    def public_ip_address(self) -> global___PublicIpAddress: ...
+    def tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    zone: builtins.str
+    @property
+    def accelerator_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig: ...
+    @property
+    def container_images(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages]: ...
+    @property
+    def data_disk(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk: ...
+    @property
+    def encryption_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig: ...
+    @property
+    def shielded_instance_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig: ...
     def __init__(
         self,
         *,
-        private_ip_address: builtins.str = ...,
-        private_ip_allocation_method: builtins.str = ...,
-        subnet: global___Subnet | None = ...,
-        private_link_configuration: builtins.str = ...,
-        name: builtins.str = ...,
-        public_ip_address: global___PublicIpAddress | None = ...,
+        guest_attributes: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        internal_ip_only: builtins.bool = ...,
+        labels: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        machine_type: builtins.str = ...,
+        metadata: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        network: builtins.str = ...,
+        nic_type: builtins.str = ...,
+        reserved_ip_range: builtins.str = ...,
+        subnet: builtins.str = ...,
+        tags: collections.abc.Iterable[builtins.str] | None = ...,
+        zone: builtins.str = ...,
+        accelerator_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig | None = ...,
+        container_images: collections.abc.Iterable[global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages] | None = ...,
+        data_disk: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk | None = ...,
+        encryption_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig | None = ...,
+        shielded_instance_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["public_ip_address", b"public_ip_address", "subnet", b"subnet"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "private_ip_address", b"private_ip_address", "private_ip_allocation_method", b"private_ip_allocation_method", "private_link_configuration", b"private_link_configuration", "public_ip_address", b"public_ip_address", "subnet", b"subnet"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "data_disk", b"data_disk", "encryption_config", b"encryption_config", "shielded_instance_config", b"shielded_instance_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "container_images", b"container_images", "data_disk", b"data_disk", "encryption_config", b"encryption_config", "guest_attributes", b"guest_attributes", "internal_ip_only", b"internal_ip_only", "labels", b"labels", "machine_type", b"machine_type", "metadata", b"metadata", "network", b"network", "nic_type", b"nic_type", "reserved_ip_range", b"reserved_ip_range", "shielded_instance_config", b"shielded_instance_config", "subnet", b"subnet", "tags", b"tags", "zone", b"zone"]) -> None: ...
 
-global___ApplicationGatewayFrontendIPConfiguration = ApplicationGatewayFrontendIPConfiguration
+global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfig
 
 @typing_extensions.final
-class ApplicationGatewaySslCertificate(google.protobuf.message.Message):
+class NotebooksRuntimeXVirtualMachine(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DATA_FIELD_NUMBER: builtins.int
-    PASSWORD_FIELD_NUMBER: builtins.int
-    KEY_VAULT_SECRET_ID_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    data: builtins.str
-    password: builtins.str
-    key_vault_secret_id: builtins.str
-    name: builtins.str
+    INSTANCE_ID_FIELD_NUMBER: builtins.int
+    INSTANCE_NAME_FIELD_NUMBER: builtins.int
+    VIRTUAL_MACHINE_CONFIG_FIELD_NUMBER: builtins.int
+    instance_id: builtins.str
+    instance_name: builtins.str
+    @property
+    def virtual_machine_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfig: ...
     def __init__(
         self,
         *,
-        data: builtins.str = ...,
-        password: builtins.str = ...,
-        key_vault_secret_id: builtins.str = ...,
-        name: builtins.str = ...,
+        instance_id: builtins.str = ...,
+        instance_name: builtins.str = ...,
+        virtual_machine_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfig | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "key_vault_secret_id", b"key_vault_secret_id", "name", b"name", "password", b"password"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["virtual_machine_config", b"virtual_machine_config"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["instance_id", b"instance_id", "instance_name", b"instance_name", "virtual_machine_config", b"virtual_machine_config"]) -> None: ...
 
-global___ApplicationGatewaySslCertificate = ApplicationGatewaySslCertificate
+global___NotebooksRuntimeXVirtualMachine = NotebooksRuntimeXVirtualMachine
 
 @typing_extensions.final
-class ApplicationGatewayTrustedClientCertificate(google.protobuf.message.Message):
+class NotebooksRuntime(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DATA_FIELD_NUMBER: builtins.int
+    @typing_extensions.final
+    class MetricsEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    HEALTH_STATE_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    METRICS_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    data: builtins.str
+    PROJECT_FIELD_NUMBER: builtins.int
+    STATE_FIELD_NUMBER: builtins.int
+    ACCESS_CONFIG_FIELD_NUMBER: builtins.int
+    SOFTWARE_CONFIG_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    VIRTUAL_MACHINE_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    health_state: builtins.str
+    id: builtins.str
+    location: builtins.str
+    @property
+    def metrics(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     name: builtins.str
+    project: builtins.str
+    state: builtins.str
+    @property
+    def access_config(self) -> global___NotebooksRuntimeXAccessConfig: ...
+    @property
+    def software_config(self) -> global___NotebooksRuntimeXSoftwareConfig: ...
+    @property
+    def timeouts(self) -> global___NotebooksRuntimeXTimeouts: ...
+    @property
+    def virtual_machine(self) -> global___NotebooksRuntimeXVirtualMachine: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        data: builtins.str = ...,
+        health_state: builtins.str = ...,
+        id: builtins.str = ...,
+        location: builtins.str = ...,
+        metrics: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         name: builtins.str = ...,
+        project: builtins.str = ...,
+        state: builtins.str = ...,
+        access_config: global___NotebooksRuntimeXAccessConfig | None = ...,
+        software_config: global___NotebooksRuntimeXSoftwareConfig | None = ...,
+        timeouts: global___NotebooksRuntimeXTimeouts | None = ...,
+        virtual_machine: global___NotebooksRuntimeXVirtualMachine | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "name", b"name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["access_config", b"access_config", "resource_info", b"resource_info", "software_config", b"software_config", "timeouts", b"timeouts", "virtual_machine", b"virtual_machine"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["access_config", b"access_config", "health_state", b"health_state", "id", b"id", "location", b"location", "metrics", b"metrics", "name", b"name", "project", b"project", "resource_info", b"resource_info", "software_config", b"software_config", "state", b"state", "timeouts", b"timeouts", "virtual_machine", b"virtual_machine"]) -> None: ...
 
-global___ApplicationGatewayTrustedClientCertificate = ApplicationGatewayTrustedClientCertificate
+global___NotebooksRuntime = NotebooksRuntime
 
 @typing_extensions.final
-class ApplicationGatewayTrustedRootCertificate(google.protobuf.message.Message):
+class NotebooksRuntimeIamBindingXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DATA_FIELD_NUMBER: builtins.int
-    KEY_VAULT_SECRET_ID_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    data: builtins.str
-    key_vault_secret_id: builtins.str
-    name: builtins.str
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    EXPRESSION_FIELD_NUMBER: builtins.int
+    TITLE_FIELD_NUMBER: builtins.int
+    description: builtins.str
+    expression: builtins.str
+    title: builtins.str
     def __init__(
         self,
         *,
-        data: builtins.str = ...,
-        key_vault_secret_id: builtins.str = ...,
-        name: builtins.str = ...,
+        description: builtins.str = ...,
+        expression: builtins.str = ...,
+        title: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "key_vault_secret_id", b"key_vault_secret_id", "name", b"name"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
 
-global___ApplicationGatewayTrustedRootCertificate = ApplicationGatewayTrustedRootCertificate
+global___NotebooksRuntimeIamBindingXCondition = NotebooksRuntimeIamBindingXCondition
 
 @typing_extensions.final
-class ApplicationGatewayAuthenticationCertificate(google.protobuf.message.Message):
+class NotebooksRuntimeIamBinding(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DATA_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    data: builtins.str
-    name: builtins.str
+    ETAG_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    MEMBERS_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    RUNTIME_NAME_FIELD_NUMBER: builtins.int
+    CONDITION_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    etag: builtins.str
+    id: builtins.str
+    location: builtins.str
+    @property
+    def members(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    project: builtins.str
+    role: builtins.str
+    runtime_name: builtins.str
+    @property
+    def condition(self) -> global___NotebooksRuntimeIamBindingXCondition: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        data: builtins.str = ...,
-        name: builtins.str = ...,
+        etag: builtins.str = ...,
+        id: builtins.str = ...,
+        location: builtins.str = ...,
+        members: collections.abc.Iterable[builtins.str] | None = ...,
+        project: builtins.str = ...,
+        role: builtins.str = ...,
+        runtime_name: builtins.str = ...,
+        condition: global___NotebooksRuntimeIamBindingXCondition | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["data", b"data", "name", b"name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "location", b"location", "members", b"members", "project", b"project", "resource_info", b"resource_info", "role", b"role", "runtime_name", b"runtime_name"]) -> None: ...
 
-global___ApplicationGatewayAuthenticationCertificate = ApplicationGatewayAuthenticationCertificate
+global___NotebooksRuntimeIamBinding = NotebooksRuntimeIamBinding
 
 @typing_extensions.final
-class ApplicationGatewayIPConfiguration(google.protobuf.message.Message):
+class NotebooksRuntimeIamMemberXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    SUBNET_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    @property
-    def subnet(self) -> global___Subnet: ...
-    name: builtins.str
+    DESCRIPTION_FIELD_NUMBER: builtins.int
+    EXPRESSION_FIELD_NUMBER: builtins.int
+    TITLE_FIELD_NUMBER: builtins.int
+    description: builtins.str
+    expression: builtins.str
+    title: builtins.str
     def __init__(
         self,
         *,
-        subnet: global___Subnet | None = ...,
-        name: builtins.str = ...,
+        description: builtins.str = ...,
+        expression: builtins.str = ...,
+        title: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["subnet", b"subnet"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["name", b"name", "subnet", b"subnet"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
 
-global___ApplicationGatewayIPConfiguration = ApplicationGatewayIPConfiguration
+global___NotebooksRuntimeIamMemberXCondition = NotebooksRuntimeIamMemberXCondition
 
 @typing_extensions.final
-class ApplicationGatewaySslPolicy(google.protobuf.message.Message):
+class NotebooksRuntimeIamMember(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DISABLED_SSL_PROTOCOLS_FIELD_NUMBER: builtins.int
-    POLICY_TYPE_FIELD_NUMBER: builtins.int
-    POLICY_NAME_FIELD_NUMBER: builtins.int
-    CIPHER_SUITES_FIELD_NUMBER: builtins.int
-    MIN_PROTOCOL_VERSION_FIELD_NUMBER: builtins.int
+    ETAG_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    MEMBER_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    RUNTIME_NAME_FIELD_NUMBER: builtins.int
+    CONDITION_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    etag: builtins.str
+    id: builtins.str
+    location: builtins.str
+    member: builtins.str
+    project: builtins.str
+    role: builtins.str
+    runtime_name: builtins.str
     @property
-    def disabled_ssl_protocols(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    policy_type: builtins.str
-    policy_name: builtins.str
+    def condition(self) -> global___NotebooksRuntimeIamMemberXCondition: ...
     @property
-    def cipher_suites(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    min_protocol_version: builtins.str
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        disabled_ssl_protocols: collections.abc.Iterable[builtins.str] | None = ...,
-        policy_type: builtins.str = ...,
-        policy_name: builtins.str = ...,
-        cipher_suites: collections.abc.Iterable[builtins.str] | None = ...,
-        min_protocol_version: builtins.str = ...,
+        etag: builtins.str = ...,
+        id: builtins.str = ...,
+        location: builtins.str = ...,
+        member: builtins.str = ...,
+        project: builtins.str = ...,
+        role: builtins.str = ...,
+        runtime_name: builtins.str = ...,
+        condition: global___NotebooksRuntimeIamMemberXCondition | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["cipher_suites", b"cipher_suites", "disabled_ssl_protocols", b"disabled_ssl_protocols", "min_protocol_version", b"min_protocol_version", "policy_name", b"policy_name", "policy_type", b"policy_type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "location", b"location", "member", b"member", "project", b"project", "resource_info", b"resource_info", "role", b"role", "runtime_name", b"runtime_name"]) -> None: ...
 
-global___ApplicationGatewaySslPolicy = ApplicationGatewaySslPolicy
+global___NotebooksRuntimeIamMember = NotebooksRuntimeIamMember
 
 @typing_extensions.final
-class ApplicationGatewaySku(google.protobuf.message.Message):
+class NotebooksRuntimeIamPolicy(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    NAME_FIELD_NUMBER: builtins.int
-    TIER_FIELD_NUMBER: builtins.int
-    CAPACITY_FIELD_NUMBER: builtins.int
-    name: builtins.str
-    tier: builtins.str
-    capacity: builtins.int
+    ETAG_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    LOCATION_FIELD_NUMBER: builtins.int
+    POLICY_DATA_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    RUNTIME_NAME_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    etag: builtins.str
+    id: builtins.str
+    location: builtins.str
+    policy_data: builtins.str
+    project: builtins.str
+    runtime_name: builtins.str
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        name: builtins.str = ...,
-        tier: builtins.str = ...,
-        capacity: builtins.int = ...,
+        etag: builtins.str = ...,
+        id: builtins.str = ...,
+        location: builtins.str = ...,
+        policy_data: builtins.str = ...,
+        project: builtins.str = ...,
+        runtime_name: builtins.str = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["capacity", b"capacity", "name", b"name", "tier", b"tier"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["etag", b"etag", "id", b"id", "location", b"location", "policy_data", b"policy_data", "project", b"project", "resource_info", b"resource_info", "runtime_name", b"runtime_name"]) -> None: ...
 
-global___ApplicationGatewaySku = ApplicationGatewaySku
+global___NotebooksRuntimeIamPolicy = NotebooksRuntimeIamPolicy
```

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_dnszones_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_firewallpolicies_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_networkexperimentprofiles_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_frontdoor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_loadbalancers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_networksecuritygroups_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatednszones_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privateendpoints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_privatelinkservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_routetables_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_trafficmanager_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_network_virtualnetworks_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_backup_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_recoveryservices_siterecovery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_servicebus_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_databases_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_managedinstances_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_sql_servers_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_storage_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_storage_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_storage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_streamanalytics_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_web_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_web_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/azure/azure_microsoft_web_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_access_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_access_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_access_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_access_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_active_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_active_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_active_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_active_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apigee_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apigee_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apigee_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apigee_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apikeys_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apikeys_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_apikeys_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_app_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_app_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_app_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_app_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_artifact_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_artifact_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_artifact_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_artifact_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_assured_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_assured_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_assured_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_assured_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigquery_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigquery_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigquery_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigtable_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigtable_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_bigtable_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_billing_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_billing_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_billing_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_billing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_binary_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_binary_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_binary_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_binary_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_certificate_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_certificate_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_certificate_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_certificate_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloud_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloud_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloud_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloud_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudbuild_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudbuild_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_clouddeploy_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_clouddeploy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudfunctions_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudiot_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudiot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_cloudiot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_composer_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_composer_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_composer_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_composer_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_address_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_address_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_attached_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_attached_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_attached_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_autoscaler_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_backend_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_backend_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_backend_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_disk_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_disk_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_disk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_external_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_external_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_external_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_firewall_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_firewall_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_forwarding_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_global_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_global_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_global_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ha_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ha_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ha_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_health_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_health_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_health_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_http_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_http_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_https_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_https_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_https_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_image_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_image_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_image_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_instance_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_instance_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_instance_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_interconnect_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_managed_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_managed_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_managed_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_network_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_network_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_node_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_node_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_packet_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_packet_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_packet_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_per_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_per_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_per_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_project_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_project_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_region_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_region_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_region_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_reservation_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_reservation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_resource_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_route_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_route_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_route_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_router_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_router_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_router_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_security_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_security_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_security_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_service_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_service_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_shared_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_shared_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_snapshot_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ssl_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_ssl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_subnetwork_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_target_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_target_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_target_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_url_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_url_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_url_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_vpn_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_compute_vpn_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_container_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_container_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_container_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_container_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_data_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_data_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_data_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_data_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataflow_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataflow_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataplex_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataplex_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataplex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataproc_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataproc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dataproc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_datastore_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_datastore_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_datastore_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_datastore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_deployment_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_deployment_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_deployment_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_deployment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dialogflow_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dialogflow_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dialogflow_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dns_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dns_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_dns_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_dns_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_document_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_document_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_document_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_document_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_endpoints_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_endpoints_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_endpoints_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_essential_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_essential_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_essential_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_essential_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_eventarc_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_eventarc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_eventarc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_filestore_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_filestore_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_filestore_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_filestore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firebaserules_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firebaserules_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firebaserules_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firestore_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firestore_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_firestore_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_firestore_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_folder_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_folder_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_folder_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_folder_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_game_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_game_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_game_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_game_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_gke_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_gke_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_gke_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_gke_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_app_engine_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_certificate_manager_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloud_tasks_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudarmor_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_cloudfunctions_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_firewall_policy_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_instance_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_network_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_route_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_compute_subnetwork_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_container_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dataflow_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_dns_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_kms_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_load_balancer_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_memcache_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_pubsub_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_redis_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_secret_manager_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_spanner_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_sql_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_google_storage_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_healthcare_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_healthcare_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_healthcare_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iam_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iam_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iam_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iam_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iap_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iap_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_iap_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_iap_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_identity_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_identity_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_identity_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_identity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_kms_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_kms_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_kms_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_kms_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_logging_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_logging_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_logging_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_memcache_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_memcache_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_memcache_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_memcache_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_ml_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_ml_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_ml_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_ml_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_monitoring_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_monitoring_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_monitoring_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_network_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_network_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_network_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_network_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_notebooks_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_notebooks_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_notebooks_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_storage_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -14,249 +14,234 @@
     import typing as typing_extensions
 else:
     import typing_extensions
 
 DESCRIPTOR: google.protobuf.descriptor.FileDescriptor
 
 @typing_extensions.final
-class NotebooksEnvironmentXContainerImage(google.protobuf.message.Message):
+class StorageBucketXCors(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    REPOSITORY_FIELD_NUMBER: builtins.int
-    TAG_FIELD_NUMBER: builtins.int
-    repository: builtins.str
-    tag: builtins.str
+    MAX_AGE_SECONDS_FIELD_NUMBER: builtins.int
+    METHOD_FIELD_NUMBER: builtins.int
+    ORIGIN_FIELD_NUMBER: builtins.int
+    RESPONSE_HEADER_FIELD_NUMBER: builtins.int
+    max_age_seconds: builtins.float
+    @property
+    def method(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    @property
+    def origin(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    @property
+    def response_header(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     def __init__(
         self,
         *,
-        repository: builtins.str = ...,
-        tag: builtins.str = ...,
+        max_age_seconds: builtins.float = ...,
+        method: collections.abc.Iterable[builtins.str] | None = ...,
+        origin: collections.abc.Iterable[builtins.str] | None = ...,
+        response_header: collections.abc.Iterable[builtins.str] | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["max_age_seconds", b"max_age_seconds", "method", b"method", "origin", b"origin", "response_header", b"response_header"]) -> None: ...
 
-global___NotebooksEnvironmentXContainerImage = NotebooksEnvironmentXContainerImage
+global___StorageBucketXCors = StorageBucketXCors
 
 @typing_extensions.final
-class NotebooksEnvironmentXTimeouts(google.protobuf.message.Message):
+class StorageBucketXEncryption(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CREATE_FIELD_NUMBER: builtins.int
-    DELETE_FIELD_NUMBER: builtins.int
-    UPDATE_FIELD_NUMBER: builtins.int
-    create: builtins.str
-    delete: builtins.str
-    update: builtins.str
+    DEFAULT_KMS_KEY_NAME_FIELD_NUMBER: builtins.int
+    default_kms_key_name: builtins.str
     def __init__(
         self,
         *,
-        create: builtins.str = ...,
-        delete: builtins.str = ...,
-        update: builtins.str = ...,
+        default_kms_key_name: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["default_kms_key_name", b"default_kms_key_name"]) -> None: ...
 
-global___NotebooksEnvironmentXTimeouts = NotebooksEnvironmentXTimeouts
+global___StorageBucketXEncryption = StorageBucketXEncryption
 
 @typing_extensions.final
-class NotebooksEnvironmentXVmImage(google.protobuf.message.Message):
+class StorageBucketXLifecycleRuleXAction(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    IMAGE_FAMILY_FIELD_NUMBER: builtins.int
-    IMAGE_NAME_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
-    image_family: builtins.str
-    image_name: builtins.str
-    project: builtins.str
+    STORAGE_CLASS_FIELD_NUMBER: builtins.int
+    TYPE_FIELD_NUMBER: builtins.int
+    storage_class: builtins.str
+    type: builtins.str
     def __init__(
         self,
         *,
-        image_family: builtins.str = ...,
-        image_name: builtins.str = ...,
-        project: builtins.str = ...,
+        storage_class: builtins.str = ...,
+        type: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["image_family", b"image_family", "image_name", b"image_name", "project", b"project"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["storage_class", b"storage_class", "type", b"type"]) -> None: ...
 
-global___NotebooksEnvironmentXVmImage = NotebooksEnvironmentXVmImage
+global___StorageBucketXLifecycleRuleXAction = StorageBucketXLifecycleRuleXAction
 
 @typing_extensions.final
-class NotebooksEnvironment(google.protobuf.message.Message):
+class StorageBucketXLifecycleRuleXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CREATE_TIME_FIELD_NUMBER: builtins.int
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    DISPLAY_NAME_FIELD_NUMBER: builtins.int
-    ID_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    POST_STARTUP_SCRIPT_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
-    CONTAINER_IMAGE_FIELD_NUMBER: builtins.int
-    TIMEOUTS_FIELD_NUMBER: builtins.int
-    VM_IMAGE_FIELD_NUMBER: builtins.int
-    RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    create_time: builtins.str
-    description: builtins.str
-    display_name: builtins.str
-    id: builtins.str
-    location: builtins.str
-    name: builtins.str
-    post_startup_script: builtins.str
-    project: builtins.str
-    @property
-    def container_image(self) -> global___NotebooksEnvironmentXContainerImage: ...
+    AGE_FIELD_NUMBER: builtins.int
+    CREATED_BEFORE_FIELD_NUMBER: builtins.int
+    CUSTOM_TIME_BEFORE_FIELD_NUMBER: builtins.int
+    DAYS_SINCE_CUSTOM_TIME_FIELD_NUMBER: builtins.int
+    DAYS_SINCE_NONCURRENT_TIME_FIELD_NUMBER: builtins.int
+    MATCHES_PREFIX_FIELD_NUMBER: builtins.int
+    MATCHES_STORAGE_CLASS_FIELD_NUMBER: builtins.int
+    MATCHES_SUFFIX_FIELD_NUMBER: builtins.int
+    NONCURRENT_TIME_BEFORE_FIELD_NUMBER: builtins.int
+    NUM_NEWER_VERSIONS_FIELD_NUMBER: builtins.int
+    WITH_STATE_FIELD_NUMBER: builtins.int
+    age: builtins.float
+    created_before: builtins.str
+    custom_time_before: builtins.str
+    days_since_custom_time: builtins.float
+    days_since_noncurrent_time: builtins.float
     @property
-    def timeouts(self) -> global___NotebooksEnvironmentXTimeouts: ...
+    def matches_prefix(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
-    def vm_image(self) -> global___NotebooksEnvironmentXVmImage: ...
+    def matches_storage_class(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
-    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    def matches_suffix(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    noncurrent_time_before: builtins.str
+    num_newer_versions: builtins.float
+    with_state: builtins.str
     def __init__(
         self,
         *,
-        create_time: builtins.str = ...,
-        description: builtins.str = ...,
-        display_name: builtins.str = ...,
-        id: builtins.str = ...,
-        location: builtins.str = ...,
-        name: builtins.str = ...,
-        post_startup_script: builtins.str = ...,
-        project: builtins.str = ...,
-        container_image: global___NotebooksEnvironmentXContainerImage | None = ...,
-        timeouts: global___NotebooksEnvironmentXTimeouts | None = ...,
-        vm_image: global___NotebooksEnvironmentXVmImage | None = ...,
-        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+        age: builtins.float = ...,
+        created_before: builtins.str = ...,
+        custom_time_before: builtins.str = ...,
+        days_since_custom_time: builtins.float = ...,
+        days_since_noncurrent_time: builtins.float = ...,
+        matches_prefix: collections.abc.Iterable[builtins.str] | None = ...,
+        matches_storage_class: collections.abc.Iterable[builtins.str] | None = ...,
+        matches_suffix: collections.abc.Iterable[builtins.str] | None = ...,
+        noncurrent_time_before: builtins.str = ...,
+        num_newer_versions: builtins.float = ...,
+        with_state: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["container_image", b"container_image", "resource_info", b"resource_info", "timeouts", b"timeouts", "vm_image", b"vm_image"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["container_image", b"container_image", "create_time", b"create_time", "description", b"description", "display_name", b"display_name", "id", b"id", "location", b"location", "name", b"name", "post_startup_script", b"post_startup_script", "project", b"project", "resource_info", b"resource_info", "timeouts", b"timeouts", "vm_image", b"vm_image"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["age", b"age", "created_before", b"created_before", "custom_time_before", b"custom_time_before", "days_since_custom_time", b"days_since_custom_time", "days_since_noncurrent_time", b"days_since_noncurrent_time", "matches_prefix", b"matches_prefix", "matches_storage_class", b"matches_storage_class", "matches_suffix", b"matches_suffix", "noncurrent_time_before", b"noncurrent_time_before", "num_newer_versions", b"num_newer_versions", "with_state", b"with_state"]) -> None: ...
 
-global___NotebooksEnvironment = NotebooksEnvironment
+global___StorageBucketXLifecycleRuleXCondition = StorageBucketXLifecycleRuleXCondition
 
 @typing_extensions.final
-class NotebooksInstanceXAcceleratorConfig(google.protobuf.message.Message):
+class StorageBucketXLifecycleRule(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CORE_COUNT_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
-    core_count: builtins.float
-    type: builtins.str
+    ACTION_FIELD_NUMBER: builtins.int
+    CONDITION_FIELD_NUMBER: builtins.int
+    @property
+    def action(self) -> global___StorageBucketXLifecycleRuleXAction: ...
+    @property
+    def condition(self) -> global___StorageBucketXLifecycleRuleXCondition: ...
     def __init__(
         self,
         *,
-        core_count: builtins.float = ...,
-        type: builtins.str = ...,
+        action: global___StorageBucketXLifecycleRuleXAction | None = ...,
+        condition: global___StorageBucketXLifecycleRuleXCondition | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["core_count", b"core_count", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["action", b"action", "condition", b"condition"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["action", b"action", "condition", b"condition"]) -> None: ...
 
-global___NotebooksInstanceXAcceleratorConfig = NotebooksInstanceXAcceleratorConfig
+global___StorageBucketXLifecycleRule = StorageBucketXLifecycleRule
 
 @typing_extensions.final
-class NotebooksInstanceXContainerImage(google.protobuf.message.Message):
+class StorageBucketXLogging(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    REPOSITORY_FIELD_NUMBER: builtins.int
-    TAG_FIELD_NUMBER: builtins.int
-    repository: builtins.str
-    tag: builtins.str
+    LOG_BUCKET_FIELD_NUMBER: builtins.int
+    LOG_OBJECT_PREFIX_FIELD_NUMBER: builtins.int
+    log_bucket: builtins.str
+    log_object_prefix: builtins.str
     def __init__(
         self,
         *,
-        repository: builtins.str = ...,
-        tag: builtins.str = ...,
+        log_bucket: builtins.str = ...,
+        log_object_prefix: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["log_bucket", b"log_bucket", "log_object_prefix", b"log_object_prefix"]) -> None: ...
 
-global___NotebooksInstanceXContainerImage = NotebooksInstanceXContainerImage
+global___StorageBucketXLogging = StorageBucketXLogging
 
 @typing_extensions.final
-class NotebooksInstanceXReservationAffinity(google.protobuf.message.Message):
+class StorageBucketXRetentionPolicy(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CONSUME_RESERVATION_TYPE_FIELD_NUMBER: builtins.int
-    KEY_FIELD_NUMBER: builtins.int
-    VALUES_FIELD_NUMBER: builtins.int
-    consume_reservation_type: builtins.str
-    key: builtins.str
-    @property
-    def values(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    IS_LOCKED_FIELD_NUMBER: builtins.int
+    RETENTION_PERIOD_FIELD_NUMBER: builtins.int
+    is_locked: builtins.bool
+    retention_period: builtins.float
     def __init__(
         self,
         *,
-        consume_reservation_type: builtins.str = ...,
-        key: builtins.str = ...,
-        values: collections.abc.Iterable[builtins.str] | None = ...,
+        is_locked: builtins.bool = ...,
+        retention_period: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["consume_reservation_type", b"consume_reservation_type", "key", b"key", "values", b"values"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["is_locked", b"is_locked", "retention_period", b"retention_period"]) -> None: ...
 
-global___NotebooksInstanceXReservationAffinity = NotebooksInstanceXReservationAffinity
+global___StorageBucketXRetentionPolicy = StorageBucketXRetentionPolicy
 
 @typing_extensions.final
-class NotebooksInstanceXShieldedInstanceConfig(google.protobuf.message.Message):
+class StorageBucketXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENABLE_INTEGRITY_MONITORING_FIELD_NUMBER: builtins.int
-    ENABLE_SECURE_BOOT_FIELD_NUMBER: builtins.int
-    ENABLE_VTPM_FIELD_NUMBER: builtins.int
-    enable_integrity_monitoring: builtins.bool
-    enable_secure_boot: builtins.bool
-    enable_vtpm: builtins.bool
+    CREATE_FIELD_NUMBER: builtins.int
+    READ_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    read: builtins.str
+    update: builtins.str
     def __init__(
         self,
         *,
-        enable_integrity_monitoring: builtins.bool = ...,
-        enable_secure_boot: builtins.bool = ...,
-        enable_vtpm: builtins.bool = ...,
+        create: builtins.str = ...,
+        read: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enable_integrity_monitoring", b"enable_integrity_monitoring", "enable_secure_boot", b"enable_secure_boot", "enable_vtpm", b"enable_vtpm"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "read", b"read", "update", b"update"]) -> None: ...
 
-global___NotebooksInstanceXShieldedInstanceConfig = NotebooksInstanceXShieldedInstanceConfig
+global___StorageBucketXTimeouts = StorageBucketXTimeouts
 
 @typing_extensions.final
-class NotebooksInstanceXTimeouts(google.protobuf.message.Message):
+class StorageBucketXVersioning(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CREATE_FIELD_NUMBER: builtins.int
-    DELETE_FIELD_NUMBER: builtins.int
-    UPDATE_FIELD_NUMBER: builtins.int
-    create: builtins.str
-    delete: builtins.str
-    update: builtins.str
+    ENABLED_FIELD_NUMBER: builtins.int
+    enabled: builtins.bool
     def __init__(
         self,
         *,
-        create: builtins.str = ...,
-        delete: builtins.str = ...,
-        update: builtins.str = ...,
+        enabled: builtins.bool = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["enabled", b"enabled"]) -> None: ...
 
-global___NotebooksInstanceXTimeouts = NotebooksInstanceXTimeouts
+global___StorageBucketXVersioning = StorageBucketXVersioning
 
 @typing_extensions.final
-class NotebooksInstanceXVmImage(google.protobuf.message.Message):
+class StorageBucketXWebsite(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    IMAGE_FAMILY_FIELD_NUMBER: builtins.int
-    IMAGE_NAME_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
-    image_family: builtins.str
-    image_name: builtins.str
-    project: builtins.str
+    MAIN_PAGE_SUFFIX_FIELD_NUMBER: builtins.int
+    NOT_FOUND_PAGE_FIELD_NUMBER: builtins.int
+    main_page_suffix: builtins.str
+    not_found_page: builtins.str
     def __init__(
         self,
         *,
-        image_family: builtins.str = ...,
-        image_name: builtins.str = ...,
-        project: builtins.str = ...,
+        main_page_suffix: builtins.str = ...,
+        not_found_page: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["image_family", b"image_family", "image_name", b"image_name", "project", b"project"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["main_page_suffix", b"main_page_suffix", "not_found_page", b"not_found_page"]) -> None: ...
 
-global___NotebooksInstanceXVmImage = NotebooksInstanceXVmImage
+global___StorageBucketXWebsite = StorageBucketXWebsite
 
 @typing_extensions.final
-class NotebooksInstance(google.protobuf.message.Message):
+class StorageBucket(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
     class LabelsEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
@@ -267,164 +252,191 @@
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    @typing_extensions.final
-    class MetadataEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
-
-    BOOT_DISK_SIZE_GB_FIELD_NUMBER: builtins.int
-    BOOT_DISK_TYPE_FIELD_NUMBER: builtins.int
-    CREATE_TIME_FIELD_NUMBER: builtins.int
-    CUSTOM_GPU_DRIVER_PATH_FIELD_NUMBER: builtins.int
-    DATA_DISK_SIZE_GB_FIELD_NUMBER: builtins.int
-    DATA_DISK_TYPE_FIELD_NUMBER: builtins.int
-    DISK_ENCRYPTION_FIELD_NUMBER: builtins.int
+    DEFAULT_EVENT_BASED_HOLD_FIELD_NUMBER: builtins.int
+    FORCE_DESTROY_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
-    INSTALL_GPU_DRIVER_FIELD_NUMBER: builtins.int
-    INSTANCE_OWNERS_FIELD_NUMBER: builtins.int
-    KMS_KEY_FIELD_NUMBER: builtins.int
     LABELS_FIELD_NUMBER: builtins.int
     LOCATION_FIELD_NUMBER: builtins.int
-    MACHINE_TYPE_FIELD_NUMBER: builtins.int
-    METADATA_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    NETWORK_FIELD_NUMBER: builtins.int
-    NIC_TYPE_FIELD_NUMBER: builtins.int
-    NO_PROXY_ACCESS_FIELD_NUMBER: builtins.int
-    NO_PUBLIC_IP_FIELD_NUMBER: builtins.int
-    NO_REMOVE_DATA_DISK_FIELD_NUMBER: builtins.int
-    POST_STARTUP_SCRIPT_FIELD_NUMBER: builtins.int
     PROJECT_FIELD_NUMBER: builtins.int
-    PROXY_URI_FIELD_NUMBER: builtins.int
-    SERVICE_ACCOUNT_FIELD_NUMBER: builtins.int
-    SERVICE_ACCOUNT_SCOPES_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    SUBNET_FIELD_NUMBER: builtins.int
-    TAGS_FIELD_NUMBER: builtins.int
-    UPDATE_TIME_FIELD_NUMBER: builtins.int
-    ACCELERATOR_CONFIG_FIELD_NUMBER: builtins.int
-    CONTAINER_IMAGE_FIELD_NUMBER: builtins.int
-    RESERVATION_AFFINITY_FIELD_NUMBER: builtins.int
-    SHIELDED_INSTANCE_CONFIG_FIELD_NUMBER: builtins.int
+    REQUESTER_PAYS_FIELD_NUMBER: builtins.int
+    SELF_LINK_FIELD_NUMBER: builtins.int
+    STORAGE_CLASS_FIELD_NUMBER: builtins.int
+    UNIFORM_BUCKET_LEVEL_ACCESS_FIELD_NUMBER: builtins.int
+    URL_FIELD_NUMBER: builtins.int
+    CORS_FIELD_NUMBER: builtins.int
+    ENCRYPTION_FIELD_NUMBER: builtins.int
+    LIFECYCLE_RULE_FIELD_NUMBER: builtins.int
+    LOGGING_FIELD_NUMBER: builtins.int
+    RETENTION_POLICY_FIELD_NUMBER: builtins.int
     TIMEOUTS_FIELD_NUMBER: builtins.int
-    VM_IMAGE_FIELD_NUMBER: builtins.int
+    VERSIONING_FIELD_NUMBER: builtins.int
+    WEBSITE_FIELD_NUMBER: builtins.int
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    boot_disk_size_gb: builtins.float
-    boot_disk_type: builtins.str
-    create_time: builtins.str
-    custom_gpu_driver_path: builtins.str
-    data_disk_size_gb: builtins.float
-    data_disk_type: builtins.str
-    disk_encryption: builtins.str
+    default_event_based_hold: builtins.bool
+    force_destroy: builtins.bool
     id: builtins.str
-    install_gpu_driver: builtins.bool
-    @property
-    def instance_owners(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    kms_key: builtins.str
     @property
     def labels(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     location: builtins.str
-    machine_type: builtins.str
-    @property
-    def metadata(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     name: builtins.str
-    network: builtins.str
-    nic_type: builtins.str
-    no_proxy_access: builtins.bool
-    no_public_ip: builtins.bool
-    no_remove_data_disk: builtins.bool
-    post_startup_script: builtins.str
     project: builtins.str
-    proxy_uri: builtins.str
-    service_account: builtins.str
+    requester_pays: builtins.bool
+    self_link: builtins.str
+    storage_class: builtins.str
+    uniform_bucket_level_access: builtins.bool
+    url: builtins.str
     @property
-    def service_account_scopes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    state: builtins.str
-    subnet: builtins.str
+    def cors(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StorageBucketXCors]: ...
     @property
-    def tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    update_time: builtins.str
+    def encryption(self) -> global___StorageBucketXEncryption: ...
     @property
-    def accelerator_config(self) -> global___NotebooksInstanceXAcceleratorConfig: ...
+    def lifecycle_rule(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___StorageBucketXLifecycleRule]: ...
     @property
-    def container_image(self) -> global___NotebooksInstanceXContainerImage: ...
+    def logging(self) -> global___StorageBucketXLogging: ...
     @property
-    def reservation_affinity(self) -> global___NotebooksInstanceXReservationAffinity: ...
+    def retention_policy(self) -> global___StorageBucketXRetentionPolicy: ...
     @property
-    def shielded_instance_config(self) -> global___NotebooksInstanceXShieldedInstanceConfig: ...
+    def timeouts(self) -> global___StorageBucketXTimeouts: ...
     @property
-    def timeouts(self) -> global___NotebooksInstanceXTimeouts: ...
+    def versioning(self) -> global___StorageBucketXVersioning: ...
     @property
-    def vm_image(self) -> global___NotebooksInstanceXVmImage: ...
+    def website(self) -> global___StorageBucketXWebsite: ...
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        boot_disk_size_gb: builtins.float = ...,
-        boot_disk_type: builtins.str = ...,
-        create_time: builtins.str = ...,
-        custom_gpu_driver_path: builtins.str = ...,
-        data_disk_size_gb: builtins.float = ...,
-        data_disk_type: builtins.str = ...,
-        disk_encryption: builtins.str = ...,
+        default_event_based_hold: builtins.bool = ...,
+        force_destroy: builtins.bool = ...,
         id: builtins.str = ...,
-        install_gpu_driver: builtins.bool = ...,
-        instance_owners: collections.abc.Iterable[builtins.str] | None = ...,
-        kms_key: builtins.str = ...,
         labels: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         location: builtins.str = ...,
-        machine_type: builtins.str = ...,
-        metadata: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         name: builtins.str = ...,
-        network: builtins.str = ...,
-        nic_type: builtins.str = ...,
-        no_proxy_access: builtins.bool = ...,
-        no_public_ip: builtins.bool = ...,
-        no_remove_data_disk: builtins.bool = ...,
-        post_startup_script: builtins.str = ...,
         project: builtins.str = ...,
-        proxy_uri: builtins.str = ...,
-        service_account: builtins.str = ...,
-        service_account_scopes: collections.abc.Iterable[builtins.str] | None = ...,
-        state: builtins.str = ...,
-        subnet: builtins.str = ...,
-        tags: collections.abc.Iterable[builtins.str] | None = ...,
-        update_time: builtins.str = ...,
-        accelerator_config: global___NotebooksInstanceXAcceleratorConfig | None = ...,
-        container_image: global___NotebooksInstanceXContainerImage | None = ...,
-        reservation_affinity: global___NotebooksInstanceXReservationAffinity | None = ...,
-        shielded_instance_config: global___NotebooksInstanceXShieldedInstanceConfig | None = ...,
-        timeouts: global___NotebooksInstanceXTimeouts | None = ...,
-        vm_image: global___NotebooksInstanceXVmImage | None = ...,
+        requester_pays: builtins.bool = ...,
+        self_link: builtins.str = ...,
+        storage_class: builtins.str = ...,
+        uniform_bucket_level_access: builtins.bool = ...,
+        url: builtins.str = ...,
+        cors: collections.abc.Iterable[global___StorageBucketXCors] | None = ...,
+        encryption: global___StorageBucketXEncryption | None = ...,
+        lifecycle_rule: collections.abc.Iterable[global___StorageBucketXLifecycleRule] | None = ...,
+        logging: global___StorageBucketXLogging | None = ...,
+        retention_policy: global___StorageBucketXRetentionPolicy | None = ...,
+        timeouts: global___StorageBucketXTimeouts | None = ...,
+        versioning: global___StorageBucketXVersioning | None = ...,
+        website: global___StorageBucketXWebsite | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["encryption", b"encryption", "logging", b"logging", "resource_info", b"resource_info", "retention_policy", b"retention_policy", "timeouts", b"timeouts", "versioning", b"versioning", "website", b"website"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["cors", b"cors", "default_event_based_hold", b"default_event_based_hold", "encryption", b"encryption", "force_destroy", b"force_destroy", "id", b"id", "labels", b"labels", "lifecycle_rule", b"lifecycle_rule", "location", b"location", "logging", b"logging", "name", b"name", "project", b"project", "requester_pays", b"requester_pays", "resource_info", b"resource_info", "retention_policy", b"retention_policy", "self_link", b"self_link", "storage_class", b"storage_class", "timeouts", b"timeouts", "uniform_bucket_level_access", b"uniform_bucket_level_access", "url", b"url", "versioning", b"versioning", "website", b"website"]) -> None: ...
+
+global___StorageBucket = StorageBucket
+
+@typing_extensions.final
+class StorageBucketAccessControlXTimeouts(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
+    def __init__(
+        self,
+        *,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
+
+global___StorageBucketAccessControlXTimeouts = StorageBucketAccessControlXTimeouts
+
+@typing_extensions.final
+class StorageBucketAccessControl(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    BUCKET_FIELD_NUMBER: builtins.int
+    DOMAIN_FIELD_NUMBER: builtins.int
+    EMAIL_FIELD_NUMBER: builtins.int
+    ENTITY_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    domain: builtins.str
+    email: builtins.str
+    entity: builtins.str
+    id: builtins.str
+    role: builtins.str
+    @property
+    def timeouts(self) -> global___StorageBucketAccessControlXTimeouts: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    def __init__(
+        self,
+        *,
+        bucket: builtins.str = ...,
+        domain: builtins.str = ...,
+        email: builtins.str = ...,
+        entity: builtins.str = ...,
+        id: builtins.str = ...,
+        role: builtins.str = ...,
+        timeouts: global___StorageBucketAccessControlXTimeouts | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "domain", b"domain", "email", b"email", "entity", b"entity", "id", b"id", "resource_info", b"resource_info", "role", b"role", "timeouts", b"timeouts"]) -> None: ...
+
+global___StorageBucketAccessControl = StorageBucketAccessControl
+
+@typing_extensions.final
+class StorageBucketAcl(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    BUCKET_FIELD_NUMBER: builtins.int
+    DEFAULT_ACL_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    PREDEFINED_ACL_FIELD_NUMBER: builtins.int
+    ROLE_ENTITY_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    default_acl: builtins.str
+    id: builtins.str
+    predefined_acl: builtins.str
+    @property
+    def role_entity(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    def __init__(
+        self,
+        *,
+        bucket: builtins.str = ...,
+        default_acl: builtins.str = ...,
+        id: builtins.str = ...,
+        predefined_acl: builtins.str = ...,
+        role_entity: collections.abc.Iterable[builtins.str] | None = ...,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "container_image", b"container_image", "reservation_affinity", b"reservation_affinity", "resource_info", b"resource_info", "shielded_instance_config", b"shielded_instance_config", "timeouts", b"timeouts", "vm_image", b"vm_image"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "boot_disk_size_gb", b"boot_disk_size_gb", "boot_disk_type", b"boot_disk_type", "container_image", b"container_image", "create_time", b"create_time", "custom_gpu_driver_path", b"custom_gpu_driver_path", "data_disk_size_gb", b"data_disk_size_gb", "data_disk_type", b"data_disk_type", "disk_encryption", b"disk_encryption", "id", b"id", "install_gpu_driver", b"install_gpu_driver", "instance_owners", b"instance_owners", "kms_key", b"kms_key", "labels", b"labels", "location", b"location", "machine_type", b"machine_type", "metadata", b"metadata", "name", b"name", "network", b"network", "nic_type", b"nic_type", "no_proxy_access", b"no_proxy_access", "no_public_ip", b"no_public_ip", "no_remove_data_disk", b"no_remove_data_disk", "post_startup_script", b"post_startup_script", "project", b"project", "proxy_uri", b"proxy_uri", "reservation_affinity", b"reservation_affinity", "resource_info", b"resource_info", "service_account", b"service_account", "service_account_scopes", b"service_account_scopes", "shielded_instance_config", b"shielded_instance_config", "state", b"state", "subnet", b"subnet", "tags", b"tags", "timeouts", b"timeouts", "update_time", b"update_time", "vm_image", b"vm_image"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "default_acl", b"default_acl", "id", b"id", "predefined_acl", b"predefined_acl", "resource_info", b"resource_info", "role_entity", b"role_entity"]) -> None: ...
 
-global___NotebooksInstance = NotebooksInstance
+global___StorageBucketAcl = StorageBucketAcl
 
 @typing_extensions.final
-class NotebooksInstanceIamBindingXCondition(google.protobuf.message.Message):
+class StorageBucketIamBindingXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXPRESSION_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
     description: builtins.str
     expression: builtins.str
@@ -434,61 +446,55 @@
         *,
         description: builtins.str = ...,
         expression: builtins.str = ...,
         title: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
 
-global___NotebooksInstanceIamBindingXCondition = NotebooksInstanceIamBindingXCondition
+global___StorageBucketIamBindingXCondition = StorageBucketIamBindingXCondition
 
 @typing_extensions.final
-class NotebooksInstanceIamBinding(google.protobuf.message.Message):
+class StorageBucketIamBinding(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    BUCKET_FIELD_NUMBER: builtins.int
     ETAG_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
-    INSTANCE_NAME_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
     MEMBERS_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
     ROLE_FIELD_NUMBER: builtins.int
     CONDITION_FIELD_NUMBER: builtins.int
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
     etag: builtins.str
     id: builtins.str
-    instance_name: builtins.str
-    location: builtins.str
     @property
     def members(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    project: builtins.str
     role: builtins.str
     @property
-    def condition(self) -> global___NotebooksInstanceIamBindingXCondition: ...
+    def condition(self) -> global___StorageBucketIamBindingXCondition: ...
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
+        bucket: builtins.str = ...,
         etag: builtins.str = ...,
         id: builtins.str = ...,
-        instance_name: builtins.str = ...,
-        location: builtins.str = ...,
         members: collections.abc.Iterable[builtins.str] | None = ...,
-        project: builtins.str = ...,
         role: builtins.str = ...,
-        condition: global___NotebooksInstanceIamBindingXCondition | None = ...,
+        condition: global___StorageBucketIamBindingXCondition | None = ...,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "instance_name", b"instance_name", "location", b"location", "members", b"members", "project", b"project", "resource_info", b"resource_info", "role", b"role"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "condition", b"condition", "etag", b"etag", "id", b"id", "members", b"members", "resource_info", b"resource_info", "role", b"role"]) -> None: ...
 
-global___NotebooksInstanceIamBinding = NotebooksInstanceIamBinding
+global___StorageBucketIamBinding = StorageBucketIamBinding
 
 @typing_extensions.final
-class NotebooksInstanceIamMemberXCondition(google.protobuf.message.Message):
+class StorageBucketIamMemberXCondition(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     DESCRIPTION_FIELD_NUMBER: builtins.int
     EXPRESSION_FIELD_NUMBER: builtins.int
     TITLE_FIELD_NUMBER: builtins.int
     description: builtins.str
     expression: builtins.str
@@ -498,95 +504,101 @@
         *,
         description: builtins.str = ...,
         expression: builtins.str = ...,
         title: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
 
-global___NotebooksInstanceIamMemberXCondition = NotebooksInstanceIamMemberXCondition
+global___StorageBucketIamMemberXCondition = StorageBucketIamMemberXCondition
 
 @typing_extensions.final
-class NotebooksInstanceIamMember(google.protobuf.message.Message):
+class StorageBucketIamMember(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    BUCKET_FIELD_NUMBER: builtins.int
     ETAG_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
-    INSTANCE_NAME_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
     MEMBER_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
     ROLE_FIELD_NUMBER: builtins.int
     CONDITION_FIELD_NUMBER: builtins.int
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
     etag: builtins.str
     id: builtins.str
-    instance_name: builtins.str
-    location: builtins.str
     member: builtins.str
-    project: builtins.str
     role: builtins.str
     @property
-    def condition(self) -> global___NotebooksInstanceIamMemberXCondition: ...
+    def condition(self) -> global___StorageBucketIamMemberXCondition: ...
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
+        bucket: builtins.str = ...,
         etag: builtins.str = ...,
         id: builtins.str = ...,
-        instance_name: builtins.str = ...,
-        location: builtins.str = ...,
         member: builtins.str = ...,
-        project: builtins.str = ...,
         role: builtins.str = ...,
-        condition: global___NotebooksInstanceIamMemberXCondition | None = ...,
+        condition: global___StorageBucketIamMemberXCondition | None = ...,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "instance_name", b"instance_name", "location", b"location", "member", b"member", "project", b"project", "resource_info", b"resource_info", "role", b"role"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "condition", b"condition", "etag", b"etag", "id", b"id", "member", b"member", "resource_info", b"resource_info", "role", b"role"]) -> None: ...
 
-global___NotebooksInstanceIamMember = NotebooksInstanceIamMember
+global___StorageBucketIamMember = StorageBucketIamMember
 
 @typing_extensions.final
-class NotebooksInstanceIamPolicy(google.protobuf.message.Message):
+class StorageBucketIamPolicy(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    BUCKET_FIELD_NUMBER: builtins.int
     ETAG_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
-    INSTANCE_NAME_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
     POLICY_DATA_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
     etag: builtins.str
     id: builtins.str
-    instance_name: builtins.str
-    location: builtins.str
     policy_data: builtins.str
-    project: builtins.str
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
+        bucket: builtins.str = ...,
         etag: builtins.str = ...,
         id: builtins.str = ...,
-        instance_name: builtins.str = ...,
-        location: builtins.str = ...,
         policy_data: builtins.str = ...,
-        project: builtins.str = ...,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
     def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["etag", b"etag", "id", b"id", "instance_name", b"instance_name", "location", b"location", "policy_data", b"policy_data", "project", b"project", "resource_info", b"resource_info"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "etag", b"etag", "id", b"id", "policy_data", b"policy_data", "resource_info", b"resource_info"]) -> None: ...
+
+global___StorageBucketIamPolicy = StorageBucketIamPolicy
+
+@typing_extensions.final
+class StorageBucketObjectXCustomerEncryption(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    ENCRYPTION_ALGORITHM_FIELD_NUMBER: builtins.int
+    ENCRYPTION_KEY_FIELD_NUMBER: builtins.int
+    encryption_algorithm: builtins.str
+    encryption_key: builtins.str
+    def __init__(
+        self,
+        *,
+        encryption_algorithm: builtins.str = ...,
+        encryption_key: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["encryption_algorithm", b"encryption_algorithm", "encryption_key", b"encryption_key"]) -> None: ...
 
-global___NotebooksInstanceIamPolicy = NotebooksInstanceIamPolicy
+global___StorageBucketObjectXCustomerEncryption = StorageBucketObjectXCustomerEncryption
 
 @typing_extensions.final
-class NotebooksLocationXTimeouts(google.protobuf.message.Message):
+class StorageBucketObjectXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CREATE_FIELD_NUMBER: builtins.int
     DELETE_FIELD_NUMBER: builtins.int
     UPDATE_FIELD_NUMBER: builtins.int
     create: builtins.str
     delete: builtins.str
@@ -596,133 +608,239 @@
         *,
         create: builtins.str = ...,
         delete: builtins.str = ...,
         update: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___NotebooksLocationXTimeouts = NotebooksLocationXTimeouts
+global___StorageBucketObjectXTimeouts = StorageBucketObjectXTimeouts
 
 @typing_extensions.final
-class NotebooksLocation(google.protobuf.message.Message):
+class StorageBucketObject(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
+    @typing_extensions.final
+    class MetadataEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    BUCKET_FIELD_NUMBER: builtins.int
+    CACHE_CONTROL_FIELD_NUMBER: builtins.int
+    CONTENT_FIELD_NUMBER: builtins.int
+    CONTENT_DISPOSITION_FIELD_NUMBER: builtins.int
+    CONTENT_ENCODING_FIELD_NUMBER: builtins.int
+    CONTENT_LANGUAGE_FIELD_NUMBER: builtins.int
+    CONTENT_TYPE_FIELD_NUMBER: builtins.int
+    CRC32C_FIELD_NUMBER: builtins.int
+    DETECT_MD5HASH_FIELD_NUMBER: builtins.int
+    EVENT_BASED_HOLD_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
+    KMS_KEY_NAME_FIELD_NUMBER: builtins.int
+    MD5HASH_FIELD_NUMBER: builtins.int
+    MEDIA_LINK_FIELD_NUMBER: builtins.int
+    METADATA_FIELD_NUMBER: builtins.int
     NAME_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
+    OUTPUT_NAME_FIELD_NUMBER: builtins.int
     SELF_LINK_FIELD_NUMBER: builtins.int
+    SOURCE_FIELD_NUMBER: builtins.int
+    STORAGE_CLASS_FIELD_NUMBER: builtins.int
+    TEMPORARY_HOLD_FIELD_NUMBER: builtins.int
+    CUSTOMER_ENCRYPTION_FIELD_NUMBER: builtins.int
     TIMEOUTS_FIELD_NUMBER: builtins.int
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    cache_control: builtins.str
+    content: builtins.str
+    content_disposition: builtins.str
+    content_encoding: builtins.str
+    content_language: builtins.str
+    content_type: builtins.str
+    crc32c: builtins.str
+    detect_md5hash: builtins.str
+    event_based_hold: builtins.bool
     id: builtins.str
+    kms_key_name: builtins.str
+    md5hash: builtins.str
+    media_link: builtins.str
+    @property
+    def metadata(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
     name: builtins.str
-    project: builtins.str
+    output_name: builtins.str
     self_link: builtins.str
+    source: builtins.str
+    storage_class: builtins.str
+    temporary_hold: builtins.bool
+    @property
+    def customer_encryption(self) -> global___StorageBucketObjectXCustomerEncryption: ...
     @property
-    def timeouts(self) -> global___NotebooksLocationXTimeouts: ...
+    def timeouts(self) -> global___StorageBucketObjectXTimeouts: ...
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
+        bucket: builtins.str = ...,
+        cache_control: builtins.str = ...,
+        content: builtins.str = ...,
+        content_disposition: builtins.str = ...,
+        content_encoding: builtins.str = ...,
+        content_language: builtins.str = ...,
+        content_type: builtins.str = ...,
+        crc32c: builtins.str = ...,
+        detect_md5hash: builtins.str = ...,
+        event_based_hold: builtins.bool = ...,
         id: builtins.str = ...,
+        kms_key_name: builtins.str = ...,
+        md5hash: builtins.str = ...,
+        media_link: builtins.str = ...,
+        metadata: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
         name: builtins.str = ...,
-        project: builtins.str = ...,
+        output_name: builtins.str = ...,
         self_link: builtins.str = ...,
-        timeouts: global___NotebooksLocationXTimeouts | None = ...,
+        source: builtins.str = ...,
+        storage_class: builtins.str = ...,
+        temporary_hold: builtins.bool = ...,
+        customer_encryption: global___StorageBucketObjectXCustomerEncryption | None = ...,
+        timeouts: global___StorageBucketObjectXTimeouts | None = ...,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["id", b"id", "name", b"name", "project", b"project", "resource_info", b"resource_info", "self_link", b"self_link", "timeouts", b"timeouts"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["customer_encryption", b"customer_encryption", "resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "cache_control", b"cache_control", "content", b"content", "content_disposition", b"content_disposition", "content_encoding", b"content_encoding", "content_language", b"content_language", "content_type", b"content_type", "crc32c", b"crc32c", "customer_encryption", b"customer_encryption", "detect_md5hash", b"detect_md5hash", "event_based_hold", b"event_based_hold", "id", b"id", "kms_key_name", b"kms_key_name", "md5hash", b"md5hash", "media_link", b"media_link", "metadata", b"metadata", "name", b"name", "output_name", b"output_name", "resource_info", b"resource_info", "self_link", b"self_link", "source", b"source", "storage_class", b"storage_class", "temporary_hold", b"temporary_hold", "timeouts", b"timeouts"]) -> None: ...
 
-global___NotebooksLocation = NotebooksLocation
+global___StorageBucketObject = StorageBucketObject
 
 @typing_extensions.final
-class NotebooksRuntimeXAccessConfig(google.protobuf.message.Message):
+class StorageDefaultObjectAccessControlXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ACCESS_TYPE_FIELD_NUMBER: builtins.int
-    PROXY_URI_FIELD_NUMBER: builtins.int
-    RUNTIME_OWNER_FIELD_NUMBER: builtins.int
-    access_type: builtins.str
-    proxy_uri: builtins.str
-    runtime_owner: builtins.str
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
     def __init__(
         self,
         *,
-        access_type: builtins.str = ...,
-        proxy_uri: builtins.str = ...,
-        runtime_owner: builtins.str = ...,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["access_type", b"access_type", "proxy_uri", b"proxy_uri", "runtime_owner", b"runtime_owner"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___NotebooksRuntimeXAccessConfig = NotebooksRuntimeXAccessConfig
+global___StorageDefaultObjectAccessControlXTimeouts = StorageDefaultObjectAccessControlXTimeouts
 
 @typing_extensions.final
-class NotebooksRuntimeXSoftwareConfigXKernels(google.protobuf.message.Message):
+class StorageDefaultObjectAccessControl(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    REPOSITORY_FIELD_NUMBER: builtins.int
-    TAG_FIELD_NUMBER: builtins.int
-    repository: builtins.str
-    tag: builtins.str
+    @typing_extensions.final
+    class ProjectTeamEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    BUCKET_FIELD_NUMBER: builtins.int
+    DOMAIN_FIELD_NUMBER: builtins.int
+    EMAIL_FIELD_NUMBER: builtins.int
+    ENTITY_FIELD_NUMBER: builtins.int
+    ENTITY_ID_FIELD_NUMBER: builtins.int
+    GENERATION_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    OBJECT_FIELD_NUMBER: builtins.int
+    PROJECT_TEAM_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    domain: builtins.str
+    email: builtins.str
+    entity: builtins.str
+    entity_id: builtins.str
+    generation: builtins.float
+    id: builtins.str
+    object: builtins.str
+    @property
+    def project_team(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    role: builtins.str
+    @property
+    def timeouts(self) -> global___StorageDefaultObjectAccessControlXTimeouts: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        repository: builtins.str = ...,
-        tag: builtins.str = ...,
+        bucket: builtins.str = ...,
+        domain: builtins.str = ...,
+        email: builtins.str = ...,
+        entity: builtins.str = ...,
+        entity_id: builtins.str = ...,
+        generation: builtins.float = ...,
+        id: builtins.str = ...,
+        object: builtins.str = ...,
+        project_team: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        role: builtins.str = ...,
+        timeouts: global___StorageDefaultObjectAccessControlXTimeouts | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "domain", b"domain", "email", b"email", "entity", b"entity", "entity_id", b"entity_id", "generation", b"generation", "id", b"id", "object", b"object", "project_team", b"project_team", "resource_info", b"resource_info", "role", b"role", "timeouts", b"timeouts"]) -> None: ...
 
-global___NotebooksRuntimeXSoftwareConfigXKernels = NotebooksRuntimeXSoftwareConfigXKernels
+global___StorageDefaultObjectAccessControl = StorageDefaultObjectAccessControl
 
 @typing_extensions.final
-class NotebooksRuntimeXSoftwareConfig(google.protobuf.message.Message):
+class StorageDefaultObjectAcl(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CUSTOM_GPU_DRIVER_PATH_FIELD_NUMBER: builtins.int
-    ENABLE_HEALTH_MONITORING_FIELD_NUMBER: builtins.int
-    IDLE_SHUTDOWN_FIELD_NUMBER: builtins.int
-    IDLE_SHUTDOWN_TIMEOUT_FIELD_NUMBER: builtins.int
-    INSTALL_GPU_DRIVER_FIELD_NUMBER: builtins.int
-    NOTEBOOK_UPGRADE_SCHEDULE_FIELD_NUMBER: builtins.int
-    POST_STARTUP_SCRIPT_FIELD_NUMBER: builtins.int
-    POST_STARTUP_SCRIPT_BEHAVIOR_FIELD_NUMBER: builtins.int
-    UPGRADEABLE_FIELD_NUMBER: builtins.int
-    KERNELS_FIELD_NUMBER: builtins.int
-    custom_gpu_driver_path: builtins.str
-    enable_health_monitoring: builtins.bool
-    idle_shutdown: builtins.bool
-    idle_shutdown_timeout: builtins.float
-    install_gpu_driver: builtins.bool
-    notebook_upgrade_schedule: builtins.str
-    post_startup_script: builtins.str
-    post_startup_script_behavior: builtins.str
-    upgradeable: builtins.bool
+    BUCKET_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    ROLE_ENTITY_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    id: builtins.str
     @property
-    def kernels(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NotebooksRuntimeXSoftwareConfigXKernels]: ...
+    def role_entity(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        custom_gpu_driver_path: builtins.str = ...,
-        enable_health_monitoring: builtins.bool = ...,
-        idle_shutdown: builtins.bool = ...,
-        idle_shutdown_timeout: builtins.float = ...,
-        install_gpu_driver: builtins.bool = ...,
-        notebook_upgrade_schedule: builtins.str = ...,
-        post_startup_script: builtins.str = ...,
-        post_startup_script_behavior: builtins.str = ...,
-        upgradeable: builtins.bool = ...,
-        kernels: collections.abc.Iterable[global___NotebooksRuntimeXSoftwareConfigXKernels] | None = ...,
+        bucket: builtins.str = ...,
+        id: builtins.str = ...,
+        role_entity: collections.abc.Iterable[builtins.str] | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["custom_gpu_driver_path", b"custom_gpu_driver_path", "enable_health_monitoring", b"enable_health_monitoring", "idle_shutdown", b"idle_shutdown", "idle_shutdown_timeout", b"idle_shutdown_timeout", "install_gpu_driver", b"install_gpu_driver", "kernels", b"kernels", "notebook_upgrade_schedule", b"notebook_upgrade_schedule", "post_startup_script", b"post_startup_script", "post_startup_script_behavior", b"post_startup_script_behavior", "upgradeable", b"upgradeable"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "id", b"id", "resource_info", b"resource_info", "role_entity", b"role_entity"]) -> None: ...
 
-global___NotebooksRuntimeXSoftwareConfig = NotebooksRuntimeXSoftwareConfig
+global___StorageDefaultObjectAcl = StorageDefaultObjectAcl
 
 @typing_extensions.final
-class NotebooksRuntimeXTimeouts(google.protobuf.message.Message):
+class StorageHmacKeyXTimeouts(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     CREATE_FIELD_NUMBER: builtins.int
     DELETE_FIELD_NUMBER: builtins.int
     UPDATE_FIELD_NUMBER: builtins.int
     create: builtins.str
     delete: builtins.str
@@ -732,550 +850,639 @@
         *,
         create: builtins.str = ...,
         delete: builtins.str = ...,
         update: builtins.str = ...,
     ) -> None: ...
     def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___NotebooksRuntimeXTimeouts = NotebooksRuntimeXTimeouts
+global___StorageHmacKeyXTimeouts = StorageHmacKeyXTimeouts
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig(google.protobuf.message.Message):
+class StorageHmacKey(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    CORE_COUNT_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
-    core_count: builtins.float
-    type: builtins.str
+    ACCESS_ID_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    PROJECT_FIELD_NUMBER: builtins.int
+    SECRET_FIELD_NUMBER: builtins.int
+    SERVICE_ACCOUNT_EMAIL_FIELD_NUMBER: builtins.int
+    STATE_FIELD_NUMBER: builtins.int
+    TIME_CREATED_FIELD_NUMBER: builtins.int
+    UPDATED_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    access_id: builtins.str
+    id: builtins.str
+    project: builtins.str
+    secret: builtins.str
+    service_account_email: builtins.str
+    state: builtins.str
+    time_created: builtins.str
+    updated: builtins.str
+    @property
+    def timeouts(self) -> global___StorageHmacKeyXTimeouts: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        core_count: builtins.float = ...,
-        type: builtins.str = ...,
+        access_id: builtins.str = ...,
+        id: builtins.str = ...,
+        project: builtins.str = ...,
+        secret: builtins.str = ...,
+        service_account_email: builtins.str = ...,
+        state: builtins.str = ...,
+        time_created: builtins.str = ...,
+        updated: builtins.str = ...,
+        timeouts: global___StorageHmacKeyXTimeouts | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["core_count", b"core_count", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["access_id", b"access_id", "id", b"id", "project", b"project", "resource_info", b"resource_info", "secret", b"secret", "service_account_email", b"service_account_email", "state", b"state", "time_created", b"time_created", "timeouts", b"timeouts", "updated", b"updated"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig
+global___StorageHmacKey = StorageHmacKey
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages(google.protobuf.message.Message):
+class StorageNotification(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    REPOSITORY_FIELD_NUMBER: builtins.int
-    TAG_FIELD_NUMBER: builtins.int
-    repository: builtins.str
-    tag: builtins.str
+    @typing_extensions.final
+    class CustomAttributesEntry(google.protobuf.message.Message):
+        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+        KEY_FIELD_NUMBER: builtins.int
+        VALUE_FIELD_NUMBER: builtins.int
+        key: builtins.str
+        value: builtins.str
+        def __init__(
+            self,
+            *,
+            key: builtins.str = ...,
+            value: builtins.str = ...,
+        ) -> None: ...
+        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+
+    BUCKET_FIELD_NUMBER: builtins.int
+    CUSTOM_ATTRIBUTES_FIELD_NUMBER: builtins.int
+    EVENT_TYPES_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    NOTIFICATION_ID_FIELD_NUMBER: builtins.int
+    OBJECT_NAME_PREFIX_FIELD_NUMBER: builtins.int
+    PAYLOAD_FORMAT_FIELD_NUMBER: builtins.int
+    SELF_LINK_FIELD_NUMBER: builtins.int
+    TOPIC_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    @property
+    def custom_attributes(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    @property
+    def event_types(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    id: builtins.str
+    notification_id: builtins.str
+    object_name_prefix: builtins.str
+    payload_format: builtins.str
+    self_link: builtins.str
+    topic: builtins.str
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        repository: builtins.str = ...,
-        tag: builtins.str = ...,
+        bucket: builtins.str = ...,
+        custom_attributes: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        event_types: collections.abc.Iterable[builtins.str] | None = ...,
+        id: builtins.str = ...,
+        notification_id: builtins.str = ...,
+        object_name_prefix: builtins.str = ...,
+        payload_format: builtins.str = ...,
+        self_link: builtins.str = ...,
+        topic: builtins.str = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+    ) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "custom_attributes", b"custom_attributes", "event_types", b"event_types", "id", b"id", "notification_id", b"notification_id", "object_name_prefix", b"object_name_prefix", "payload_format", b"payload_format", "resource_info", b"resource_info", "self_link", b"self_link", "topic", b"topic"]) -> None: ...
+
+global___StorageNotification = StorageNotification
+
+@typing_extensions.final
+class StorageObjectAccessControlXTimeouts(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CREATE_FIELD_NUMBER: builtins.int
+    DELETE_FIELD_NUMBER: builtins.int
+    UPDATE_FIELD_NUMBER: builtins.int
+    create: builtins.str
+    delete: builtins.str
+    update: builtins.str
+    def __init__(
+        self,
+        *,
+        create: builtins.str = ...,
+        delete: builtins.str = ...,
+        update: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["repository", b"repository", "tag", b"tag"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["create", b"create", "delete", b"delete", "update", b"update"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages
+global___StorageObjectAccessControlXTimeouts = StorageObjectAccessControlXTimeouts
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams(google.protobuf.message.Message):
+class StorageObjectAccessControl(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
     @typing_extensions.final
-    class LabelsEntry(google.protobuf.message.Message):
+    class ProjectTeamEntry(google.protobuf.message.Message):
         DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
         KEY_FIELD_NUMBER: builtins.int
         VALUE_FIELD_NUMBER: builtins.int
         key: builtins.str
         value: builtins.str
         def __init__(
             self,
             *,
             key: builtins.str = ...,
             value: builtins.str = ...,
         ) -> None: ...
         def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
 
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    DISK_NAME_FIELD_NUMBER: builtins.int
-    DISK_SIZE_GB_FIELD_NUMBER: builtins.int
-    DISK_TYPE_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
-    description: builtins.str
-    disk_name: builtins.str
-    disk_size_gb: builtins.float
-    disk_type: builtins.str
+    BUCKET_FIELD_NUMBER: builtins.int
+    DOMAIN_FIELD_NUMBER: builtins.int
+    EMAIL_FIELD_NUMBER: builtins.int
+    ENTITY_FIELD_NUMBER: builtins.int
+    ENTITY_ID_FIELD_NUMBER: builtins.int
+    GENERATION_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    OBJECT_FIELD_NUMBER: builtins.int
+    PROJECT_TEAM_FIELD_NUMBER: builtins.int
+    ROLE_FIELD_NUMBER: builtins.int
+    TIMEOUTS_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    domain: builtins.str
+    email: builtins.str
+    entity: builtins.str
+    entity_id: builtins.str
+    generation: builtins.float
+    id: builtins.str
+    object: builtins.str
     @property
-    def labels(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    def project_team(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
+    role: builtins.str
+    @property
+    def timeouts(self) -> global___StorageObjectAccessControlXTimeouts: ...
+    @property
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        description: builtins.str = ...,
-        disk_name: builtins.str = ...,
-        disk_size_gb: builtins.float = ...,
-        disk_type: builtins.str = ...,
-        labels: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        bucket: builtins.str = ...,
+        domain: builtins.str = ...,
+        email: builtins.str = ...,
+        entity: builtins.str = ...,
+        entity_id: builtins.str = ...,
+        generation: builtins.float = ...,
+        id: builtins.str = ...,
+        object: builtins.str = ...,
+        project_team: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
+        role: builtins.str = ...,
+        timeouts: global___StorageObjectAccessControlXTimeouts | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "disk_name", b"disk_name", "disk_size_gb", b"disk_size_gb", "disk_type", b"disk_type", "labels", b"labels"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "timeouts", b"timeouts"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "domain", b"domain", "email", b"email", "entity", b"entity", "entity_id", b"entity_id", "generation", b"generation", "id", b"id", "object", b"object", "project_team", b"project_team", "resource_info", b"resource_info", "role", b"role", "timeouts", b"timeouts"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams
+global___StorageObjectAccessControl = StorageObjectAccessControl
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk(google.protobuf.message.Message):
+class StorageObjectAcl(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    AUTO_DELETE_FIELD_NUMBER: builtins.int
-    BOOT_FIELD_NUMBER: builtins.int
-    DEVICE_NAME_FIELD_NUMBER: builtins.int
-    GUEST_OS_FEATURES_FIELD_NUMBER: builtins.int
-    INDEX_FIELD_NUMBER: builtins.int
-    INTERFACE_FIELD_NUMBER: builtins.int
-    KIND_FIELD_NUMBER: builtins.int
-    LICENSES_FIELD_NUMBER: builtins.int
-    MODE_FIELD_NUMBER: builtins.int
-    SOURCE_FIELD_NUMBER: builtins.int
-    TYPE_FIELD_NUMBER: builtins.int
-    INITIALIZE_PARAMS_FIELD_NUMBER: builtins.int
-    auto_delete: builtins.bool
-    boot: builtins.bool
-    device_name: builtins.str
-    @property
-    def guest_os_features(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    index: builtins.float
-    interface: builtins.str
-    kind: builtins.str
+    BUCKET_FIELD_NUMBER: builtins.int
+    ID_FIELD_NUMBER: builtins.int
+    OBJECT_FIELD_NUMBER: builtins.int
+    PREDEFINED_ACL_FIELD_NUMBER: builtins.int
+    ROLE_ENTITY_FIELD_NUMBER: builtins.int
+    RESOURCE_INFO_FIELD_NUMBER: builtins.int
+    bucket: builtins.str
+    id: builtins.str
+    object: builtins.str
+    predefined_acl: builtins.str
     @property
-    def licenses(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    mode: builtins.str
-    source: builtins.str
-    type: builtins.str
+    def role_entity(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
-    def initialize_params(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams: ...
+    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        auto_delete: builtins.bool = ...,
-        boot: builtins.bool = ...,
-        device_name: builtins.str = ...,
-        guest_os_features: collections.abc.Iterable[builtins.str] | None = ...,
-        index: builtins.float = ...,
-        interface: builtins.str = ...,
-        kind: builtins.str = ...,
-        licenses: collections.abc.Iterable[builtins.str] | None = ...,
-        mode: builtins.str = ...,
-        source: builtins.str = ...,
-        type: builtins.str = ...,
-        initialize_params: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDiskXInitializeParams | None = ...,
+        bucket: builtins.str = ...,
+        id: builtins.str = ...,
+        object: builtins.str = ...,
+        predefined_acl: builtins.str = ...,
+        role_entity: collections.abc.Iterable[builtins.str] | None = ...,
+        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["initialize_params", b"initialize_params"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["auto_delete", b"auto_delete", "boot", b"boot", "device_name", b"device_name", "guest_os_features", b"guest_os_features", "index", b"index", "initialize_params", b"initialize_params", "interface", b"interface", "kind", b"kind", "licenses", b"licenses", "mode", b"mode", "source", b"source", "type", b"type"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket", b"bucket", "id", b"id", "object", b"object", "predefined_acl", b"predefined_acl", "resource_info", b"resource_info", "role_entity", b"role_entity"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk
+global___StorageObjectAcl = StorageObjectAcl
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig(google.protobuf.message.Message):
+class StorageTransferJobXScheduleXScheduleEndDate(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    KMS_KEY_FIELD_NUMBER: builtins.int
-    kms_key: builtins.str
+    DAY_FIELD_NUMBER: builtins.int
+    MONTH_FIELD_NUMBER: builtins.int
+    YEAR_FIELD_NUMBER: builtins.int
+    day: builtins.float
+    month: builtins.float
+    year: builtins.float
     def __init__(
         self,
         *,
-        kms_key: builtins.str = ...,
+        day: builtins.float = ...,
+        month: builtins.float = ...,
+        year: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["kms_key", b"kms_key"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["day", b"day", "month", b"month", "year", b"year"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig
+global___StorageTransferJobXScheduleXScheduleEndDate = StorageTransferJobXScheduleXScheduleEndDate
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig(google.protobuf.message.Message):
+class StorageTransferJobXScheduleXScheduleStartDate(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ENABLE_INTEGRITY_MONITORING_FIELD_NUMBER: builtins.int
-    ENABLE_SECURE_BOOT_FIELD_NUMBER: builtins.int
-    ENABLE_VTPM_FIELD_NUMBER: builtins.int
-    enable_integrity_monitoring: builtins.bool
-    enable_secure_boot: builtins.bool
-    enable_vtpm: builtins.bool
+    DAY_FIELD_NUMBER: builtins.int
+    MONTH_FIELD_NUMBER: builtins.int
+    YEAR_FIELD_NUMBER: builtins.int
+    day: builtins.float
+    month: builtins.float
+    year: builtins.float
     def __init__(
         self,
         *,
-        enable_integrity_monitoring: builtins.bool = ...,
-        enable_secure_boot: builtins.bool = ...,
-        enable_vtpm: builtins.bool = ...,
+        day: builtins.float = ...,
+        month: builtins.float = ...,
+        year: builtins.float = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["enable_integrity_monitoring", b"enable_integrity_monitoring", "enable_secure_boot", b"enable_secure_boot", "enable_vtpm", b"enable_vtpm"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["day", b"day", "month", b"month", "year", b"year"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig
+global___StorageTransferJobXScheduleXScheduleStartDate = StorageTransferJobXScheduleXScheduleStartDate
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachineXVirtualMachineConfig(google.protobuf.message.Message):
+class StorageTransferJobXScheduleXStartTimeOfDay(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
-    class GuestAttributesEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
-
-    @typing_extensions.final
-    class LabelsEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
-
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+    HOURS_FIELD_NUMBER: builtins.int
+    MINUTES_FIELD_NUMBER: builtins.int
+    NANOS_FIELD_NUMBER: builtins.int
+    SECONDS_FIELD_NUMBER: builtins.int
+    hours: builtins.float
+    minutes: builtins.float
+    nanos: builtins.float
+    seconds: builtins.float
+    def __init__(
+        self,
+        *,
+        hours: builtins.float = ...,
+        minutes: builtins.float = ...,
+        nanos: builtins.float = ...,
+        seconds: builtins.float = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["hours", b"hours", "minutes", b"minutes", "nanos", b"nanos", "seconds", b"seconds"]) -> None: ...
 
-    @typing_extensions.final
-    class MetadataEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+global___StorageTransferJobXScheduleXStartTimeOfDay = StorageTransferJobXScheduleXStartTimeOfDay
 
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+@typing_extensions.final
+class StorageTransferJobXSchedule(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    GUEST_ATTRIBUTES_FIELD_NUMBER: builtins.int
-    INTERNAL_IP_ONLY_FIELD_NUMBER: builtins.int
-    LABELS_FIELD_NUMBER: builtins.int
-    MACHINE_TYPE_FIELD_NUMBER: builtins.int
-    METADATA_FIELD_NUMBER: builtins.int
-    NETWORK_FIELD_NUMBER: builtins.int
-    NIC_TYPE_FIELD_NUMBER: builtins.int
-    RESERVED_IP_RANGE_FIELD_NUMBER: builtins.int
-    SUBNET_FIELD_NUMBER: builtins.int
-    TAGS_FIELD_NUMBER: builtins.int
-    ZONE_FIELD_NUMBER: builtins.int
-    ACCELERATOR_CONFIG_FIELD_NUMBER: builtins.int
-    CONTAINER_IMAGES_FIELD_NUMBER: builtins.int
-    DATA_DISK_FIELD_NUMBER: builtins.int
-    ENCRYPTION_CONFIG_FIELD_NUMBER: builtins.int
-    SHIELDED_INSTANCE_CONFIG_FIELD_NUMBER: builtins.int
-    @property
-    def guest_attributes(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    internal_ip_only: builtins.bool
-    @property
-    def labels(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    machine_type: builtins.str
-    @property
-    def metadata(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    network: builtins.str
-    nic_type: builtins.str
-    reserved_ip_range: builtins.str
-    subnet: builtins.str
-    @property
-    def tags(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    zone: builtins.str
+    REPEAT_INTERVAL_FIELD_NUMBER: builtins.int
+    SCHEDULE_END_DATE_FIELD_NUMBER: builtins.int
+    SCHEDULE_START_DATE_FIELD_NUMBER: builtins.int
+    START_TIME_OF_DAY_FIELD_NUMBER: builtins.int
+    repeat_interval: builtins.str
     @property
-    def accelerator_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig: ...
+    def schedule_end_date(self) -> global___StorageTransferJobXScheduleXScheduleEndDate: ...
     @property
-    def container_images(self) -> google.protobuf.internal.containers.RepeatedCompositeFieldContainer[global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages]: ...
+    def schedule_start_date(self) -> global___StorageTransferJobXScheduleXScheduleStartDate: ...
     @property
-    def data_disk(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk: ...
-    @property
-    def encryption_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig: ...
-    @property
-    def shielded_instance_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig: ...
+    def start_time_of_day(self) -> global___StorageTransferJobXScheduleXStartTimeOfDay: ...
     def __init__(
         self,
         *,
-        guest_attributes: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-        internal_ip_only: builtins.bool = ...,
-        labels: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-        machine_type: builtins.str = ...,
-        metadata: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-        network: builtins.str = ...,
-        nic_type: builtins.str = ...,
-        reserved_ip_range: builtins.str = ...,
-        subnet: builtins.str = ...,
-        tags: collections.abc.Iterable[builtins.str] | None = ...,
-        zone: builtins.str = ...,
-        accelerator_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXAcceleratorConfig | None = ...,
-        container_images: collections.abc.Iterable[global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXContainerImages] | None = ...,
-        data_disk: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXDataDisk | None = ...,
-        encryption_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXEncryptionConfig | None = ...,
-        shielded_instance_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfigXShieldedInstanceConfig | None = ...,
+        repeat_interval: builtins.str = ...,
+        schedule_end_date: global___StorageTransferJobXScheduleXScheduleEndDate | None = ...,
+        schedule_start_date: global___StorageTransferJobXScheduleXScheduleStartDate | None = ...,
+        start_time_of_day: global___StorageTransferJobXScheduleXStartTimeOfDay | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "data_disk", b"data_disk", "encryption_config", b"encryption_config", "shielded_instance_config", b"shielded_instance_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["accelerator_config", b"accelerator_config", "container_images", b"container_images", "data_disk", b"data_disk", "encryption_config", b"encryption_config", "guest_attributes", b"guest_attributes", "internal_ip_only", b"internal_ip_only", "labels", b"labels", "machine_type", b"machine_type", "metadata", b"metadata", "network", b"network", "nic_type", b"nic_type", "reserved_ip_range", b"reserved_ip_range", "shielded_instance_config", b"shielded_instance_config", "subnet", b"subnet", "tags", b"tags", "zone", b"zone"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["schedule_end_date", b"schedule_end_date", "schedule_start_date", b"schedule_start_date", "start_time_of_day", b"start_time_of_day"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["repeat_interval", b"repeat_interval", "schedule_end_date", b"schedule_end_date", "schedule_start_date", b"schedule_start_date", "start_time_of_day", b"start_time_of_day"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfig = NotebooksRuntimeXVirtualMachineXVirtualMachineConfig
+global___StorageTransferJobXSchedule = StorageTransferJobXSchedule
 
 @typing_extensions.final
-class NotebooksRuntimeXVirtualMachine(google.protobuf.message.Message):
+class StorageTransferJobXTransferSpecXAwsS3DataSourceXAwsAccessKey(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    INSTANCE_ID_FIELD_NUMBER: builtins.int
-    INSTANCE_NAME_FIELD_NUMBER: builtins.int
-    VIRTUAL_MACHINE_CONFIG_FIELD_NUMBER: builtins.int
-    instance_id: builtins.str
-    instance_name: builtins.str
+    ACCESS_KEY_ID_FIELD_NUMBER: builtins.int
+    SECRET_ACCESS_KEY_FIELD_NUMBER: builtins.int
+    access_key_id: builtins.str
+    secret_access_key: builtins.str
+    def __init__(
+        self,
+        *,
+        access_key_id: builtins.str = ...,
+        secret_access_key: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["access_key_id", b"access_key_id", "secret_access_key", b"secret_access_key"]) -> None: ...
+
+global___StorageTransferJobXTransferSpecXAwsS3DataSourceXAwsAccessKey = StorageTransferJobXTransferSpecXAwsS3DataSourceXAwsAccessKey
+
+@typing_extensions.final
+class StorageTransferJobXTransferSpecXAwsS3DataSource(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    BUCKET_NAME_FIELD_NUMBER: builtins.int
+    ROLE_ARN_FIELD_NUMBER: builtins.int
+    AWS_ACCESS_KEY_FIELD_NUMBER: builtins.int
+    bucket_name: builtins.str
+    role_arn: builtins.str
     @property
-    def virtual_machine_config(self) -> global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfig: ...
+    def aws_access_key(self) -> global___StorageTransferJobXTransferSpecXAwsS3DataSourceXAwsAccessKey: ...
     def __init__(
         self,
         *,
-        instance_id: builtins.str = ...,
-        instance_name: builtins.str = ...,
-        virtual_machine_config: global___NotebooksRuntimeXVirtualMachineXVirtualMachineConfig | None = ...,
+        bucket_name: builtins.str = ...,
+        role_arn: builtins.str = ...,
+        aws_access_key: global___StorageTransferJobXTransferSpecXAwsS3DataSourceXAwsAccessKey | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["virtual_machine_config", b"virtual_machine_config"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["instance_id", b"instance_id", "instance_name", b"instance_name", "virtual_machine_config", b"virtual_machine_config"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["aws_access_key", b"aws_access_key"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["aws_access_key", b"aws_access_key", "bucket_name", b"bucket_name", "role_arn", b"role_arn"]) -> None: ...
 
-global___NotebooksRuntimeXVirtualMachine = NotebooksRuntimeXVirtualMachine
+global___StorageTransferJobXTransferSpecXAwsS3DataSource = StorageTransferJobXTransferSpecXAwsS3DataSource
 
 @typing_extensions.final
-class NotebooksRuntime(google.protobuf.message.Message):
+class StorageTransferJobXTransferSpecXAzureBlobStorageDataSourceXAzureCredentials(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    @typing_extensions.final
-    class MetricsEntry(google.protobuf.message.Message):
-        DESCRIPTOR: google.protobuf.descriptor.Descriptor
+    SAS_TOKEN_FIELD_NUMBER: builtins.int
+    sas_token: builtins.str
+    def __init__(
+        self,
+        *,
+        sas_token: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["sas_token", b"sas_token"]) -> None: ...
 
-        KEY_FIELD_NUMBER: builtins.int
-        VALUE_FIELD_NUMBER: builtins.int
-        key: builtins.str
-        value: builtins.str
-        def __init__(
-            self,
-            *,
-            key: builtins.str = ...,
-            value: builtins.str = ...,
-        ) -> None: ...
-        def ClearField(self, field_name: typing_extensions.Literal["key", b"key", "value", b"value"]) -> None: ...
+global___StorageTransferJobXTransferSpecXAzureBlobStorageDataSourceXAzureCredentials = StorageTransferJobXTransferSpecXAzureBlobStorageDataSourceXAzureCredentials
 
-    HEALTH_STATE_FIELD_NUMBER: builtins.int
-    ID_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
-    METRICS_FIELD_NUMBER: builtins.int
-    NAME_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
-    STATE_FIELD_NUMBER: builtins.int
-    ACCESS_CONFIG_FIELD_NUMBER: builtins.int
-    SOFTWARE_CONFIG_FIELD_NUMBER: builtins.int
-    TIMEOUTS_FIELD_NUMBER: builtins.int
-    VIRTUAL_MACHINE_FIELD_NUMBER: builtins.int
-    RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    health_state: builtins.str
-    id: builtins.str
-    location: builtins.str
-    @property
-    def metrics(self) -> google.protobuf.internal.containers.ScalarMap[builtins.str, builtins.str]: ...
-    name: builtins.str
-    project: builtins.str
-    state: builtins.str
-    @property
-    def access_config(self) -> global___NotebooksRuntimeXAccessConfig: ...
-    @property
-    def software_config(self) -> global___NotebooksRuntimeXSoftwareConfig: ...
-    @property
-    def timeouts(self) -> global___NotebooksRuntimeXTimeouts: ...
-    @property
-    def virtual_machine(self) -> global___NotebooksRuntimeXVirtualMachine: ...
+@typing_extensions.final
+class StorageTransferJobXTransferSpecXAzureBlobStorageDataSource(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    CONTAINER_FIELD_NUMBER: builtins.int
+    PATH_FIELD_NUMBER: builtins.int
+    STORAGE_ACCOUNT_FIELD_NUMBER: builtins.int
+    AZURE_CREDENTIALS_FIELD_NUMBER: builtins.int
+    container: builtins.str
+    path: builtins.str
+    storage_account: builtins.str
     @property
-    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    def azure_credentials(self) -> global___StorageTransferJobXTransferSpecXAzureBlobStorageDataSourceXAzureCredentials: ...
     def __init__(
         self,
         *,
-        health_state: builtins.str = ...,
-        id: builtins.str = ...,
-        location: builtins.str = ...,
-        metrics: collections.abc.Mapping[builtins.str, builtins.str] | None = ...,
-        name: builtins.str = ...,
-        project: builtins.str = ...,
-        state: builtins.str = ...,
-        access_config: global___NotebooksRuntimeXAccessConfig | None = ...,
-        software_config: global___NotebooksRuntimeXSoftwareConfig | None = ...,
-        timeouts: global___NotebooksRuntimeXTimeouts | None = ...,
-        virtual_machine: global___NotebooksRuntimeXVirtualMachine | None = ...,
-        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+        container: builtins.str = ...,
+        path: builtins.str = ...,
+        storage_account: builtins.str = ...,
+        azure_credentials: global___StorageTransferJobXTransferSpecXAzureBlobStorageDataSourceXAzureCredentials | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["access_config", b"access_config", "resource_info", b"resource_info", "software_config", b"software_config", "timeouts", b"timeouts", "virtual_machine", b"virtual_machine"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["access_config", b"access_config", "health_state", b"health_state", "id", b"id", "location", b"location", "metrics", b"metrics", "name", b"name", "project", b"project", "resource_info", b"resource_info", "software_config", b"software_config", "state", b"state", "timeouts", b"timeouts", "virtual_machine", b"virtual_machine"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["azure_credentials", b"azure_credentials"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["azure_credentials", b"azure_credentials", "container", b"container", "path", b"path", "storage_account", b"storage_account"]) -> None: ...
 
-global___NotebooksRuntime = NotebooksRuntime
+global___StorageTransferJobXTransferSpecXAzureBlobStorageDataSource = StorageTransferJobXTransferSpecXAzureBlobStorageDataSource
 
 @typing_extensions.final
-class NotebooksRuntimeIamBindingXCondition(google.protobuf.message.Message):
+class StorageTransferJobXTransferSpecXGcsDataSink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    EXPRESSION_FIELD_NUMBER: builtins.int
-    TITLE_FIELD_NUMBER: builtins.int
-    description: builtins.str
-    expression: builtins.str
-    title: builtins.str
+    BUCKET_NAME_FIELD_NUMBER: builtins.int
+    PATH_FIELD_NUMBER: builtins.int
+    bucket_name: builtins.str
+    path: builtins.str
     def __init__(
         self,
         *,
-        description: builtins.str = ...,
-        expression: builtins.str = ...,
-        title: builtins.str = ...,
+        bucket_name: builtins.str = ...,
+        path: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket_name", b"bucket_name", "path", b"path"]) -> None: ...
 
-global___NotebooksRuntimeIamBindingXCondition = NotebooksRuntimeIamBindingXCondition
+global___StorageTransferJobXTransferSpecXGcsDataSink = StorageTransferJobXTransferSpecXGcsDataSink
 
 @typing_extensions.final
-class NotebooksRuntimeIamBinding(google.protobuf.message.Message):
+class StorageTransferJobXTransferSpecXGcsDataSource(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ETAG_FIELD_NUMBER: builtins.int
-    ID_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
-    MEMBERS_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
-    ROLE_FIELD_NUMBER: builtins.int
-    RUNTIME_NAME_FIELD_NUMBER: builtins.int
-    CONDITION_FIELD_NUMBER: builtins.int
-    RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    etag: builtins.str
-    id: builtins.str
-    location: builtins.str
-    @property
-    def members(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
-    project: builtins.str
-    role: builtins.str
-    runtime_name: builtins.str
+    BUCKET_NAME_FIELD_NUMBER: builtins.int
+    PATH_FIELD_NUMBER: builtins.int
+    bucket_name: builtins.str
+    path: builtins.str
+    def __init__(
+        self,
+        *,
+        bucket_name: builtins.str = ...,
+        path: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["bucket_name", b"bucket_name", "path", b"path"]) -> None: ...
+
+global___StorageTransferJobXTransferSpecXGcsDataSource = StorageTransferJobXTransferSpecXGcsDataSource
+
+@typing_extensions.final
+class StorageTransferJobXTransferSpecXHttpDataSource(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    LIST_URL_FIELD_NUMBER: builtins.int
+    list_url: builtins.str
+    def __init__(
+        self,
+        *,
+        list_url: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["list_url", b"list_url"]) -> None: ...
+
+global___StorageTransferJobXTransferSpecXHttpDataSource = StorageTransferJobXTransferSpecXHttpDataSource
+
+@typing_extensions.final
+class StorageTransferJobXTransferSpecXObjectConditions(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    EXCLUDE_PREFIXES_FIELD_NUMBER: builtins.int
+    INCLUDE_PREFIXES_FIELD_NUMBER: builtins.int
+    MAX_TIME_ELAPSED_SINCE_LAST_MODIFICATION_FIELD_NUMBER: builtins.int
+    MIN_TIME_ELAPSED_SINCE_LAST_MODIFICATION_FIELD_NUMBER: builtins.int
     @property
-    def condition(self) -> global___NotebooksRuntimeIamBindingXCondition: ...
+    def exclude_prefixes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
     @property
-    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    def include_prefixes(self) -> google.protobuf.internal.containers.RepeatedScalarFieldContainer[builtins.str]: ...
+    max_time_elapsed_since_last_modification: builtins.str
+    min_time_elapsed_since_last_modification: builtins.str
     def __init__(
         self,
         *,
-        etag: builtins.str = ...,
-        id: builtins.str = ...,
-        location: builtins.str = ...,
-        members: collections.abc.Iterable[builtins.str] | None = ...,
-        project: builtins.str = ...,
-        role: builtins.str = ...,
-        runtime_name: builtins.str = ...,
-        condition: global___NotebooksRuntimeIamBindingXCondition | None = ...,
-        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+        exclude_prefixes: collections.abc.Iterable[builtins.str] | None = ...,
+        include_prefixes: collections.abc.Iterable[builtins.str] | None = ...,
+        max_time_elapsed_since_last_modification: builtins.str = ...,
+        min_time_elapsed_since_last_modification: builtins.str = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "location", b"location", "members", b"members", "project", b"project", "resource_info", b"resource_info", "role", b"role", "runtime_name", b"runtime_name"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["exclude_prefixes", b"exclude_prefixes", "include_prefixes", b"include_prefixes", "max_time_elapsed_since_last_modification", b"max_time_elapsed_since_last_modification", "min_time_elapsed_since_last_modification", b"min_time_elapsed_since_last_modification"]) -> None: ...
 
-global___NotebooksRuntimeIamBinding = NotebooksRuntimeIamBinding
+global___StorageTransferJobXTransferSpecXObjectConditions = StorageTransferJobXTransferSpecXObjectConditions
 
 @typing_extensions.final
-class NotebooksRuntimeIamMemberXCondition(google.protobuf.message.Message):
+class StorageTransferJobXTransferSpecXPosixDataSink(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    DESCRIPTION_FIELD_NUMBER: builtins.int
-    EXPRESSION_FIELD_NUMBER: builtins.int
-    TITLE_FIELD_NUMBER: builtins.int
-    description: builtins.str
-    expression: builtins.str
-    title: builtins.str
+    ROOT_DIRECTORY_FIELD_NUMBER: builtins.int
+    root_directory: builtins.str
     def __init__(
         self,
         *,
-        description: builtins.str = ...,
-        expression: builtins.str = ...,
-        title: builtins.str = ...,
+        root_directory: builtins.str = ...,
     ) -> None: ...
-    def ClearField(self, field_name: typing_extensions.Literal["description", b"description", "expression", b"expression", "title", b"title"]) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["root_directory", b"root_directory"]) -> None: ...
 
-global___NotebooksRuntimeIamMemberXCondition = NotebooksRuntimeIamMemberXCondition
+global___StorageTransferJobXTransferSpecXPosixDataSink = StorageTransferJobXTransferSpecXPosixDataSink
 
 @typing_extensions.final
-class NotebooksRuntimeIamMember(google.protobuf.message.Message):
+class StorageTransferJobXTransferSpecXPosixDataSource(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ETAG_FIELD_NUMBER: builtins.int
-    ID_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
-    MEMBER_FIELD_NUMBER: builtins.int
-    PROJECT_FIELD_NUMBER: builtins.int
-    ROLE_FIELD_NUMBER: builtins.int
-    RUNTIME_NAME_FIELD_NUMBER: builtins.int
-    CONDITION_FIELD_NUMBER: builtins.int
-    RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    etag: builtins.str
-    id: builtins.str
-    location: builtins.str
-    member: builtins.str
-    project: builtins.str
-    role: builtins.str
-    runtime_name: builtins.str
+    ROOT_DIRECTORY_FIELD_NUMBER: builtins.int
+    root_directory: builtins.str
+    def __init__(
+        self,
+        *,
+        root_directory: builtins.str = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["root_directory", b"root_directory"]) -> None: ...
+
+global___StorageTransferJobXTransferSpecXPosixDataSource = StorageTransferJobXTransferSpecXPosixDataSource
+
+@typing_extensions.final
+class StorageTransferJobXTransferSpecXTransferOptions(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    DELETE_OBJECTS_FROM_SOURCE_AFTER_TRANSFER_FIELD_NUMBER: builtins.int
+    DELETE_OBJECTS_UNIQUE_IN_SINK_FIELD_NUMBER: builtins.int
+    OVERWRITE_OBJECTS_ALREADY_EXISTING_IN_SINK_FIELD_NUMBER: builtins.int
+    delete_objects_from_source_after_transfer: builtins.bool
+    delete_objects_unique_in_sink: builtins.bool
+    overwrite_objects_already_existing_in_sink: builtins.bool
+    def __init__(
+        self,
+        *,
+        delete_objects_from_source_after_transfer: builtins.bool = ...,
+        delete_objects_unique_in_sink: builtins.bool = ...,
+        overwrite_objects_already_existing_in_sink: builtins.bool = ...,
+    ) -> None: ...
+    def ClearField(self, field_name: typing_extensions.Literal["delete_objects_from_source_after_transfer", b"delete_objects_from_source_after_transfer", "delete_objects_unique_in_sink", b"delete_objects_unique_in_sink", "overwrite_objects_already_existing_in_sink", b"overwrite_objects_already_existing_in_sink"]) -> None: ...
+
+global___StorageTransferJobXTransferSpecXTransferOptions = StorageTransferJobXTransferSpecXTransferOptions
+
+@typing_extensions.final
+class StorageTransferJobXTransferSpec(google.protobuf.message.Message):
+    DESCRIPTOR: google.protobuf.descriptor.Descriptor
+
+    AWS_S3_DATA_SOURCE_FIELD_NUMBER: builtins.int
+    AZURE_BLOB_STORAGE_DATA_SOURCE_FIELD_NUMBER: builtins.int
+    GCS_DATA_SINK_FIELD_NUMBER: builtins.int
+    GCS_DATA_SOURCE_FIELD_NUMBER: builtins.int
+    HTTP_DATA_SOURCE_FIELD_NUMBER: builtins.int
+    OBJECT_CONDITIONS_FIELD_NUMBER: builtins.int
+    POSIX_DATA_SINK_FIELD_NUMBER: builtins.int
+    POSIX_DATA_SOURCE_FIELD_NUMBER: builtins.int
+    TRANSFER_OPTIONS_FIELD_NUMBER: builtins.int
     @property
-    def condition(self) -> global___NotebooksRuntimeIamMemberXCondition: ...
+    def aws_s3_data_source(self) -> global___StorageTransferJobXTransferSpecXAwsS3DataSource: ...
     @property
-    def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
+    def azure_blob_storage_data_source(self) -> global___StorageTransferJobXTransferSpecXAzureBlobStorageDataSource: ...
+    @property
+    def gcs_data_sink(self) -> global___StorageTransferJobXTransferSpecXGcsDataSink: ...
+    @property
+    def gcs_data_source(self) -> global___StorageTransferJobXTransferSpecXGcsDataSource: ...
+    @property
+    def http_data_source(self) -> global___StorageTransferJobXTransferSpecXHttpDataSource: ...
+    @property
+    def object_conditions(self) -> global___StorageTransferJobXTransferSpecXObjectConditions: ...
+    @property
+    def posix_data_sink(self) -> global___StorageTransferJobXTransferSpecXPosixDataSink: ...
+    @property
+    def posix_data_source(self) -> global___StorageTransferJobXTransferSpecXPosixDataSource: ...
+    @property
+    def transfer_options(self) -> global___StorageTransferJobXTransferSpecXTransferOptions: ...
     def __init__(
         self,
         *,
-        etag: builtins.str = ...,
-        id: builtins.str = ...,
-        location: builtins.str = ...,
-        member: builtins.str = ...,
-        project: builtins.str = ...,
-        role: builtins.str = ...,
-        runtime_name: builtins.str = ...,
-        condition: global___NotebooksRuntimeIamMemberXCondition | None = ...,
-        resource_info: shared.shared_pb2.ResourceInfo | None = ...,
+        aws_s3_data_source: global___StorageTransferJobXTransferSpecXAwsS3DataSource | None = ...,
+        azure_blob_storage_data_source: global___StorageTransferJobXTransferSpecXAzureBlobStorageDataSource | None = ...,
+        gcs_data_sink: global___StorageTransferJobXTransferSpecXGcsDataSink | None = ...,
+        gcs_data_source: global___StorageTransferJobXTransferSpecXGcsDataSource | None = ...,
+        http_data_source: global___StorageTransferJobXTransferSpecXHttpDataSource | None = ...,
+        object_conditions: global___StorageTransferJobXTransferSpecXObjectConditions | None = ...,
+        posix_data_sink: global___StorageTransferJobXTransferSpecXPosixDataSink | None = ...,
+        posix_data_source: global___StorageTransferJobXTransferSpecXPosixDataSource | None = ...,
+        transfer_options: global___StorageTransferJobXTransferSpecXTransferOptions | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["condition", b"condition", "resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["condition", b"condition", "etag", b"etag", "id", b"id", "location", b"location", "member", b"member", "project", b"project", "resource_info", b"resource_info", "role", b"role", "runtime_name", b"runtime_name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["aws_s3_data_source", b"aws_s3_data_source", "azure_blob_storage_data_source", b"azure_blob_storage_data_source", "gcs_data_sink", b"gcs_data_sink", "gcs_data_source", b"gcs_data_source", "http_data_source", b"http_data_source", "object_conditions", b"object_conditions", "posix_data_sink", b"posix_data_sink", "posix_data_source", b"posix_data_source", "transfer_options", b"transfer_options"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["aws_s3_data_source", b"aws_s3_data_source", "azure_blob_storage_data_source", b"azure_blob_storage_data_source", "gcs_data_sink", b"gcs_data_sink", "gcs_data_source", b"gcs_data_source", "http_data_source", b"http_data_source", "object_conditions", b"object_conditions", "posix_data_sink", b"posix_data_sink", "posix_data_source", b"posix_data_source", "transfer_options", b"transfer_options"]) -> None: ...
 
-global___NotebooksRuntimeIamMember = NotebooksRuntimeIamMember
+global___StorageTransferJobXTransferSpec = StorageTransferJobXTransferSpec
 
 @typing_extensions.final
-class NotebooksRuntimeIamPolicy(google.protobuf.message.Message):
+class StorageTransferJob(google.protobuf.message.Message):
     DESCRIPTOR: google.protobuf.descriptor.Descriptor
 
-    ETAG_FIELD_NUMBER: builtins.int
+    CREATION_TIME_FIELD_NUMBER: builtins.int
+    DELETION_TIME_FIELD_NUMBER: builtins.int
+    DESCRIPTION_FIELD_NUMBER: builtins.int
     ID_FIELD_NUMBER: builtins.int
-    LOCATION_FIELD_NUMBER: builtins.int
-    POLICY_DATA_FIELD_NUMBER: builtins.int
+    LAST_MODIFICATION_TIME_FIELD_NUMBER: builtins.int
+    NAME_FIELD_NUMBER: builtins.int
     PROJECT_FIELD_NUMBER: builtins.int
-    RUNTIME_NAME_FIELD_NUMBER: builtins.int
+    STATUS_FIELD_NUMBER: builtins.int
+    SCHEDULE_FIELD_NUMBER: builtins.int
+    TRANSFER_SPEC_FIELD_NUMBER: builtins.int
     RESOURCE_INFO_FIELD_NUMBER: builtins.int
-    etag: builtins.str
+    creation_time: builtins.str
+    deletion_time: builtins.str
+    description: builtins.str
     id: builtins.str
-    location: builtins.str
-    policy_data: builtins.str
+    last_modification_time: builtins.str
+    name: builtins.str
     project: builtins.str
-    runtime_name: builtins.str
+    status: builtins.str
+    @property
+    def schedule(self) -> global___StorageTransferJobXSchedule: ...
+    @property
+    def transfer_spec(self) -> global___StorageTransferJobXTransferSpec: ...
     @property
     def resource_info(self) -> shared.shared_pb2.ResourceInfo: ...
     def __init__(
         self,
         *,
-        etag: builtins.str = ...,
+        creation_time: builtins.str = ...,
+        deletion_time: builtins.str = ...,
+        description: builtins.str = ...,
         id: builtins.str = ...,
-        location: builtins.str = ...,
-        policy_data: builtins.str = ...,
+        last_modification_time: builtins.str = ...,
+        name: builtins.str = ...,
         project: builtins.str = ...,
-        runtime_name: builtins.str = ...,
+        status: builtins.str = ...,
+        schedule: global___StorageTransferJobXSchedule | None = ...,
+        transfer_spec: global___StorageTransferJobXTransferSpec | None = ...,
         resource_info: shared.shared_pb2.ResourceInfo | None = ...,
     ) -> None: ...
-    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info"]) -> builtins.bool: ...
-    def ClearField(self, field_name: typing_extensions.Literal["etag", b"etag", "id", b"id", "location", b"location", "policy_data", b"policy_data", "project", b"project", "resource_info", b"resource_info", "runtime_name", b"runtime_name"]) -> None: ...
+    def HasField(self, field_name: typing_extensions.Literal["resource_info", b"resource_info", "schedule", b"schedule", "transfer_spec", b"transfer_spec"]) -> builtins.bool: ...
+    def ClearField(self, field_name: typing_extensions.Literal["creation_time", b"creation_time", "deletion_time", b"deletion_time", "description", b"description", "id", b"id", "last_modification_time", b"last_modification_time", "name", b"name", "project", b"project", "resource_info", b"resource_info", "schedule", b"schedule", "status", b"status", "transfer_spec", b"transfer_spec"]) -> None: ...
 
-global___NotebooksRuntimeIamPolicy = NotebooksRuntimeIamPolicy
+global___StorageTransferJob = StorageTransferJob
```

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_org_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_org_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_org_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_org_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_organization_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_organization_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_organization_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_organization_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_os_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_os_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_os_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_os_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_privateca_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_privateca_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_privateca_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_privateca_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_project_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_project_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_project_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_pubsub_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_pubsub_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_pubsub_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_recaptcha_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_recaptcha_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_recaptcha_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_redis_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_redis_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_redis_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_redis_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_resource_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_resource_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_resource_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_scc_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_scc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_scc_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_scc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_secret_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_secret_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_secret_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_secret_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_service_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_service_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_service_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sourcerepo_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sourcerepo_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_spanner_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_spanner_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_spanner_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_spanner_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sql_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sql_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_sql_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_sql_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_storage_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_storage_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tags_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tags_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tags_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tags_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tpu_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tpu_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_tpu_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_tpu_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vertex_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vertex_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vertex_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vertex_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vpc_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vpc_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_vpc_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_vpc_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_workflows_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_workflows_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/gcp/gcp_workflows_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/gcp/gcp_workflows_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/admissionregistration/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apiserverinternal/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/apps/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authentication/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/authorization/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/autoscaling/v2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/batch/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/certificates/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/coordination/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/core/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/discovery/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/events/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta2_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/flowcontrol/v1beta3_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/networking/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/node/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/policy/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/rbac/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/resource/v1alpha1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/scheduling/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/api/storage/v1beta1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apiextensionsapiserver/pkg/apis/apiextensions/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/api/resource_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/apis/meta/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/runtime_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/util/intstr_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/apimachinery/pkg/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_io/k8s/kubeaggregator/pkg/apis/apiregistration/v1_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_namespaced_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/kubernetes/kubernetes_kubernetes_nonnamespaced_bundle_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/shared/shared_pb2.py` & `oak9_tython-1.0.5/oak9/tython/models/shared/shared_pb2.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/shared/shared_pb2.pyi` & `oak9_tython-1.0.5/oak9/tython/models/shared/shared_pb2.pyi`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/models/shared/shared_pb2_grpc.py` & `oak9_tython-1.0.5/oak9/tython/models/shared/shared_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/oak9/tython/runner.py` & `oak9_tython-1.0.5/oak9/tython/runner.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import json
 import os
 import sys
 from typing import Protocol, runtime_checkable, Set, Optional, List
 from colorama import Fore, Style, init
 from core.services.runner_input_service import RunnerInputService
-
 from core.bp_metadata_utils.customer_blueprint_repo import CustomerBlueprintRepo
 from core.bp_metadata_utils.python_source_file_utils import get_blueprint_classes
 from core.types import Blueprint, Finding
-
-BLUEPRINT_DIR = ''
-CURRENT_DIR = os.path.dirname(os.path.realpath(__file__))
-REPO_DIR = '/'
+import core.utilities as Utilities
 
 @runtime_checkable
 class SupportsValidation(Protocol):
     def validate(self) -> Set[Finding]:
         """
         Entry point into component's validation logic
         """
@@ -33,50 +29,53 @@
     print(f"    Running oak9's Python Framework                        ")
     print(f"************************************************************************{Style.RESET_ALL}")
 
 
     try:
         init(convert=True) # Ensure that colorama works on Windows
 
-        argsPath = None
+        args_path = None
         
         if len(argv) > 0:
-            argsPath = argv[0]
+            args_path = argv[0]
         
-        argsObj = None
+        args_obj = None
         try:
-            argsFile = open(argsPath)
-            argsObj = json.load(argsFile)
-            argsFile.close()
+            args_file = open(args_path)
+            args_obj = json.load(args_file)
+            args_file.close()
+            Utilities.verify_config_arguments(args_obj)
         except:
             # TODO: CLOUD-9058 save back a JSON instead with understandable errors for CLI to deal with
             print("Runner arguments not found or could not be understood.")
             return
         
-        path = argsObj["blueprint_package_path"]
+        path = args_obj["blueprint_package_path"]
+        command = args_obj["command"] if "command" in args_obj else "test"
         
         runner = Runner()
+        blueprint_dir = ""
 
         if path:
             blueprint_dir = path
         else:
             # TODO: We could default to /blueprints here
             raise Exception("Blueprints directory was not provided.")
 
         findings = set()
 
-        blueprint_repo = CustomerBlueprintRepo(path)
+        blueprint_repo = CustomerBlueprintRepo(blueprint_dir)
 
         # TODO: make this conditional on a CLI command
         blueprint_repo.print_blueprint_summary()
 
         # Verify config/credentials for runner endpoint
 
         # Fetch runner input data
-        runner_inputs = RunnerInputService.fetch_runner_input(argsObj)
+        runner_inputs = RunnerInputService.fetch_runner_input(args_obj)
 
         # Runner input available?
 
         # TODO: initialize blueprint properly
         '''
         Run all blueprints
         '''
@@ -103,16 +102,20 @@
                         finding.req_name = runner_input.meta_info.resource_name
                     findings.update(bp_findings)
 
         # TODO: send gaps to validation broker for the apply command
         print(f"\n{Fore.LIGHTBLACK_EX}************************************************************************\n"
               f"    {Fore.BLUE}Found {Style.BRIGHT}{len(findings)}{Style.NORMAL} Findings{Style.RESET_ALL}\n"
               f"{Fore.LIGHTBLACK_EX}************************************************************************{Style.RESET_ALL}")
-        for finding in findings:
-            print(finding)
+
+        if findings:
+            # if command == "test":
+            #     RunnerInputService.apply_findings(args_obj, findings)
+            for finding in findings:
+                print(finding)
         sys.exit(0)
 
     except Exception as e:
         print("Raised Exception: " + str(e))
         sys.exit(1)
```

### Comparing `oak9_tython-1.0.4/oak9_tython.egg-info/PKG-INFO` & `oak9_tython-1.0.5/oak9_tython.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oak9-tython
-Version: 1.0.4
+Version: 1.0.5
 Author: ['Claudio Balbin <cbalbin@oak9.io>', 'Brandon Nicoll <bnicoll@oak9.io>']
 Project-URL: Homepage, https://github.com/oak9io/tython
 Project-URL: Bug Tracker, https://github.com/oak9io/tython/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `oak9_tython-1.0.4/oak9_tython.egg-info/SOURCES.txt` & `oak9_tython-1.0.5/oak9_tython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oak9_tython-1.0.4/setup.py` & `oak9_tython-1.0.5/setup.py`

 * *Files identical despite different names*

