# Comparing `tmp/caikit-0.1.2.tar.gz` & `tmp/caikit-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-0.1.2.tar", last modified: Thu Apr 13 23:42:59 2023, max compression
+gzip compressed data, was "caikit-0.1.3.tar", last modified: Mon Apr 17 22:12:49 2023, max compression
```

## Comparing `caikit-0.1.2.tar` & `caikit-0.1.3.tar`

### file list

```diff
@@ -1,300 +1,295 @@
--rw-r--r--   0        0        0       60 2023-04-13 23:42:51.860106 caikit-0.1.2/.coveragerc
--rw-r--r--   0        0        0      676 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      579 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      519 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0        0        0     1272 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/workflows/build-library.yml
--rw-r--r--   0        0        0     1141 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/workflows/lint-code.yml
--rw-r--r--   0        0        0     1136 2023-04-13 23:42:51.860106 caikit-0.1.2/.github/workflows/publish-library.yml
--rw-r--r--   0        0        0      191 2023-04-13 23:42:51.860106 caikit-0.1.2/.gitignore
--rw-r--r--   0        0        0      310 2023-04-13 23:42:51.860106 caikit-0.1.2/.isort.cfg
--rw-r--r--   0        0        0      370 2023-04-13 23:42:51.860106 caikit-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      122 2023-04-13 23:42:51.860106 caikit-0.1.2/.prettierignore
--rw-r--r--   0        0        0       12 2023-04-13 23:42:51.860106 caikit-0.1.2/.prettierrc.yaml
--rw-r--r--   0        0        0    21434 2023-04-13 23:42:51.860106 caikit-0.1.2/.pylintrc
--rw-r--r--   0        0        0       78 2023-04-13 23:42:51.860106 caikit-0.1.2/.whitesource
--rw-r--r--   0        0        0     3358 2023-04-13 23:42:51.860106 caikit-0.1.2/CODE-OF-CONDUCT.md
--rw-r--r--   0        0        0     6510 2023-04-13 23:42:51.860106 caikit-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0    11357 2023-04-13 23:42:51.860106 caikit-0.1.2/LICENSE
--rw-r--r--   0        0        0       18 2023-04-13 23:42:51.860106 caikit-0.1.2/OWNERS
--rw-r--r--   0        0        0     3757 2023-04-13 23:42:51.860106 caikit-0.1.2/README.md
--rw-r--r--   0        0        0    44878 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit-overview.png
--rw-r--r--   0        0        0      323 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/__init__.py
--rw-r--r--   0        0        0     1861 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/__init__.py
--rw-r--r--   0        0        0      812 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/__init__.py
--rw-r--r--   0        0        0     3506 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/base.py
--rw-r--r--   0        0        0     2828 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/merged_augmentor.py
--rw-r--r--   0        0        0      355 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/__init__.py
--rw-r--r--   0        0        0     2052 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/always_selection_scheme.py
--rw-r--r--   0        0        0     3164 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/base.py
--rw-r--r--   0        0        0     3264 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
--rw-r--r--   0        0        0     2898 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py
--rw-r--r--   0        0        0      974 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/blocks/__init__.py
--rw-r--r--   0        0        0     1552 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/blocks/base.py
--rw-r--r--   0        0        0     1104 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/config/__init__.py
--rw-r--r--   0        0        0     2551 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/config/config.py
--rw-r--r--   0        0        0     1010 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/config/config.yml
--rw-r--r--   0        0        0      962 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/__init__.py
--rw-r--r--   0        0        0    29207 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/base.py
--rw-r--r--   0        0        0      750 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     2207 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/data_backends/base.py
--rw-r--r--   0        0        0     3962 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/data_backends/dict_backend.py
--rw-r--r--   0        0        0    13676 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/dataobject.py
--rw-r--r--   0        0        0     5340 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/enums.py
--rw-r--r--   0        0        0     1471 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/producer.py
--rw-r--r--   0        0        0     3914 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/protobufs/__init__.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/__init__.py
--rw-r--r--   0        0        0     5500 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/converter.py
--rw-r--r--   0        0        0     4788 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/csv_column_formatter.py
--rw-r--r--   0        0        0    40187 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/data_stream.py
--rw-r--r--   0        0        0     3606 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/resolver.py
--rw-r--r--   0        0        0     5245 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/data_model/streams/validator.py
--rw-r--r--   0        0        0    20773 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/model_manager.py
--rw-r--r--   0        0        0    51860 2023-04-13 23:42:51.860106 caikit-0.1.2/caikit/core/module.py
--rw-r--r--   0        0        0     7643 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backend_config.py
--rw-r--r--   0        0        0      684 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/__init__.py
--rw-r--r--   0        0        0     3399 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/backend_types.py
--rw-r--r--   0        0        0     1786 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/base.py
--rw-r--r--   0        0        0     1493 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_backends/local_backend.py
--rw-r--r--   0        0        0     5493 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_config.py
--rw-r--r--   0        0        0     6247 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/module_meta.py
--rw-r--r--   0        0        0      709 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/resources/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/resources/base.py
--rw-r--r--   0        0        0     1110 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/__init__.py
--rw-r--r--   0        0        0     4716 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/compatibility.py
--rw-r--r--   0        0        0     1787 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/config_utils.py
--rw-r--r--   0        0        0      637 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/errors/__init__.py
--rw-r--r--   0        0        0    18275 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/errors/error_handler.py
--rw-r--r--   0        0        0     1400 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/errors/validation_error.py
--rw-r--r--   0        0        0     5439 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/extension_utils.py
--rw-r--r--   0        0        0     4935 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/fileio.py
--rw-r--r--   0        0        0     2292 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/isa.py
--rw-r--r--   0        0        0     1864 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/logging.py
--rw-r--r--   0        0        0      630 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/__init__.py
--rw-r--r--   0        0        0     1459 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/json_test_data.py
--rw-r--r--   0        0        0     4278 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/performance.py
--rw-r--r--   0        0        0     1013 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/test_data.py
--rw-r--r--   0        0        0     1476 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance/text_test_data.py
--rw-r--r--   0        0        0      950 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/performance_metrics.py
--rw-r--r--   0        0        0    32214 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/quality_evaluation.py
--rw-r--r--   0        0        0     3439 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/serializers.py
--rw-r--r--   0        0        0     5979 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/toolkit/wip_decorator.py
--rw-r--r--   0        0        0     1022 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/workflows/__init__.py
--rw-r--r--   0        0        0     9298 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/core/workflows/base.py
--rw-r--r--   0        0        0      530 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/__init__.py
--rw-r--r--   0        0        0      748 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/common/__init__.py
--rw-r--r--   0        0        0     1211 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/common/data_model/__init__.py
--rw-r--r--   0        0        0     1377 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/common/data_model/producer.py
--rw-r--r--   0        0        0      611 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/runtime/__init__.py
--rw-r--r--   0        0        0      763 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/runtime/data_model/__init__.py
--rw-r--r--   0        0        0     2070 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/interfaces/runtime/data_model/training_management.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/__init__.py
--rw-r--r--   0        0        0     5379 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/config/config.yml
--rw-r--r--   0        0        0     1716 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/dump_services.py
--rw-r--r--   0        0        0    13853 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/grpc_server.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/interceptors/__init__.py
--rw-r--r--   0        0        0    16502 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     4703 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/metrics/rpc_meter.py
--rw-r--r--   0        0        0     2370 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/metrics/throughput.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    17143 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/batcher.py
--rw-r--r--   0        0        0     2648 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/loaded_model.py
--rw-r--r--   0        0        0     6068 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/model_loader.py
--rw-r--r--   0        0        0    12138 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/model_manager.py
--rw-r--r--   0        0        0     4194 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/model_sizer.py
--rw-r--r--   0        0        0     1587 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/model_management/training_manager.py
--rw-r--r--   0        0        0      367 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/README.md
--rw-r--r--   0        0        0      698 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/__init__.py
--rw-r--r--   0        0        0    11375 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2.py
--rw-r--r--   0        0        0    12846 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
--rw-r--r--   0        0        0    10107 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2.py
--rw-r--r--   0        0        0    10556 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     5535 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/process_pb2.py
--rw-r--r--   0        0        0     2569 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/process_pb2_grpc.py
--rw-r--r--   0        0        0     8844 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/protos/model-mesh.proto
--rw-r--r--   0        0        0     6795 2023-04-13 23:42:51.864106 caikit-0.1.2/caikit/runtime/protobufs/protos/model-runtime.proto
--rw-r--r--   0        0        0     2479 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/protobufs/protos/process.proto
--rw-r--r--   0        0        0    17157 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_factory.py
--rw-r--r--   0        0        0      109 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0     1779 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/compatibility_checker.py
--rw-r--r--   0        0        0     3083 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/core_module_helpers.py
--rw-r--r--   0        0        0     5611 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/create_service.py
--rw-r--r--   0        0        0    12289 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/data_stream_source.py
--rw-r--r--   0        0        0     5768 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/primitives.py
--rw-r--r--   0        0        0    10121 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/serializers.py
--rw-r--r--   0        0        0      666 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0    10301 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/docstrings.py
--rw-r--r--   0        0        0     4911 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/module_signature.py
--rw-r--r--   0        0        0     8296 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/parsers.py
--rw-r--r--   0        0        0     2571 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/service_generation/type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/__init__.py
--rw-r--r--   0        0        0    12326 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/global_predict_servicer.py
--rw-r--r--   0        0        0    14523 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/global_train_servicer.py
--rw-r--r--   0        0        0    10554 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/model_runtime_servicer.py
--rw-r--r--   0        0        0     5496 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/model_train_servicer.py
--rw-r--r--   0        0        0     1696 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/servicers/training_management_servicer.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/__init__.py
--rw-r--r--   0        0        0      957 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/aborted_exception.py
--rw-r--r--   0        0        0     1558 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/caikit_runtime_exception.py
--rw-r--r--   0        0        0      960 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/types/thread_destroyed_exception.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/__init__.py
--rw-r--r--   0        0        0     4223 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/config_parser.py
--rw-r--r--   0        0        0     6692 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/import_util.py
--rw-r--r--   0        0        0     1686 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/log_config.py
--rw-r--r--   0        0        0    17900 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/utils/servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     3732 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/abortable_action.py
--rw-r--r--   0        0        0     2969 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/call_aborter.py
--rw-r--r--   0        0        0     7596 2023-04-13 23:42:51.868106 caikit-0.1.2/caikit/runtime/work_management/destroyable_thread.py
--rw-r--r--   0        0        0      837 2023-04-13 23:42:51.868106 caikit-0.1.2/examples/start_runtime_with_sample_lib.py
--rw-r--r--   0        0        0     1154 2023-04-13 23:42:55.448182 caikit-0.1.2/pyproject.toml
--rwxr-xr-x   0        0        0      720 2023-04-13 23:42:51.868106 caikit-0.1.2/scripts/fmt.sh
--rw-r--r--   0        0        0       33 2023-04-13 23:42:51.868106 caikit-0.1.2/setup_requirements.txt
--rw-r--r--   0        0        0     1006 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     3783 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/base.py
--rw-r--r--   0        0        0     8909 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/__init__.py
--rw-r--r--   0        0        0     2853 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/augmentors/test_augmentor_base.py
--rw-r--r--   0        0        0     9114 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/augmentors/test_merged_augmentors.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/blocks/__init__.py
--rw-r--r--   0        0        0    12691 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/blocks/test_base.py
--rw-r--r--   0        0        0        0 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/data_backends/__init__.py
--rw-r--r--   0        0        0     4559 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/data_backends/test_dict_backend.py
--rw-r--r--   0        0        0     3306 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_converter.py
--rw-r--r--   0        0        0     3314 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_csv_column_formatter.py
--rw-r--r--   0        0        0    26013 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_data_stream.py
--rw-r--r--   0        0        0     3498 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_resolver.py
--rw-r--r--   0        0        0     2908 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/streams/test_validator.py
--rw-r--r--   0        0        0    13070 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/test_base.py
--rw-r--r--   0        0        0    13533 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/data_model/test_dataobject.py
--rw-r--r--   0        0        0     2909 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/helpers.py
--rw-r--r--   0        0        0     2320 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/module_backends/test_backend_types.py
--rw-r--r--   0        0        0     3080 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_config.py
--rw-r--r--   0        0        0      521 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_imports.py
--rw-r--r--   0        0        0    18331 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_model_manager.py
--rw-r--r--   0        0        0    17317 2023-04-13 23:42:51.868106 caikit-0.1.2/tests/core/test_module.py
--rw-r--r--   0        0        0     4751 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/test_module_backend_config.py
--rw-r--r--   0        0        0     8441 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/test_module_metadata.py
--rw-r--r--   0        0        0     1038 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/test_no_write_permissions.py
--rw-r--r--   0        0        0     7967 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_compatibility.py
--rw-r--r--   0        0        0     1953 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_config_utils.py
--rw-r--r--   0        0        0    14999 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_error_handler.py
--rw-r--r--   0        0        0     4408 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_extension_utils.py
--rw-r--r--   0        0        0     4972 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_fileio.py
--rw-r--r--   0        0        0    25851 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_quality_evaluation.py
--rw-r--r--   0        0        0     2634 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_serializers.py
--rw-r--r--   0        0        0     7824 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/toolkit/test_wip_decorator.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/workflows/__init__.py
--rw-r--r--   0        0        0    15618 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/core/workflows/test_base.py
--rw-r--r--   0        0        0     5655 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/data_model_helpers.py
--rw-r--r--   0        0        0       39 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/__init__.py
--rw-r--r--   0        0        0       27 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/bad_file.json
--rw-r--r--   0        0        0      106 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.csv
--rw-r--r--   0        0        0       66 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.json
--rw-r--r--   0        0        0      233 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.jsonl
--rw-r--r--   0        0        0     1322 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.txt
--rw-r--r--   0        0        0       11 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
--rw-r--r--   0        0        0       11 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
--rw-r--r--   0        0        0       11 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
--rw-r--r--   0        0        0       27 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
--rw-r--r--   0        0        0       27 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
--rw-r--r--   0        0        0       63 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
--rw-r--r--   0        0        0      147 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
--rw-r--r--   0        0        0      218 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
--rw-r--r--   0        0        0       87 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
--rw-r--r--   0        0        0       52 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
--rw-r--r--   0        0        0       56 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
--rw-r--r--   0        0        0       55 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
--rw-r--r--   0        0        0      125 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/data_stream_inputs/sample_w_header.csv
--rw-r--r--   0        0        0     1016 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block.zip
--rw-r--r--   0        0        0      671 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block/data.pkl
--rw-r--r--   0        0        0      189 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_backend/config.yml
--rw-r--r--   0        0        0      177 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_foo/config.yml
--rw-r--r--   0        0        0      506 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_no_nesting.zip
--rw-r--r--   0        0        0      566 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_singleton/config.yml
--rw-r--r--   0        0        0      299 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_singleton/data.json
--rw-r--r--   0        0        0       14 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_block_singleton/data.pkl
--rw-r--r--   0        0        0      222 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_dataset.json
--rw-r--r--   0        0        0      717 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_resource.zip
--rw-r--r--   0        0        0      230 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_resource/config.yml
--rw-r--r--   0        0        0     1991 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow.zip
--rw-r--r--   0        0        0      497 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/config.yml
--rw-r--r--   0        0        0      541 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/config.yml
--rw-r--r--   0        0        0      299 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/data.json
--rw-r--r--   0        0        0       14 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/data.pkl
--rw-r--r--   0        0        0     3033 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/fixtures.py
--rw-r--r--   0        0        0      918 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/invalid.zip
--rw-r--r--   0        0        0     2551 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/linux.txt
--rw-r--r--   0        0        0       10 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/bad_archive.zip
--rw-r--r--   0        0        0      376 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/bad_model.zip
--rw-r--r--   0        0        0      355 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/bar/config.yml
--rw-r--r--   0        0        0      359 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/foo/config.yml
--rw-r--r--   0        0        0      422 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/models/foo_archive.zip
--rw-r--r--   0        0        0     2142 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/primitive_party.proto
--rw-r--r--   0        0        0      145 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/__init__.py
--rw-r--r--   0        0        0     2080 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2.py
--rw-r--r--   0        0        0     2447 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
--rw-r--r--   0        0        0     2217 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
--rw-r--r--   0        0        0     2602 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
--rw-r--r--   0        0        0     5995 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protobufs/primitive_party_pb2.py
--rw-r--r--   0        0        0      416 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protos/caikit_runtime.proto
--rw-r--r--   0        0        0      437 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/protos/caikit_runtime_train.proto
--rw-r--r--   0        0        0       24 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample.csv
--rw-r--r--   0        0        0      359 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_block/config.yml
--rw-r--r--   0        0        0      176 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/__init__.py
--rw-r--r--   0        0        0      114 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/__init__.py
--rw-r--r--   0        0        0       88 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/other_task/__init__.py
--rw-r--r--   0        0        0     1852 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
--rw-r--r--   0        0        0      199 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
--rw-r--r--   0        0        0      616 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
--rw-r--r--   0        0        0     2411 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
--rw-r--r--   0        0        0     1404 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
--rw-r--r--   0        0        0     2498 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      202 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/config.py
--rw-r--r--   0        0        0      141 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/data_model/__init__.py
--rw-r--r--   0        0        0      859 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/data_model/sample.py
--rw-r--r--   0        0        0        0 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/resources/__init__.py
--rw-r--r--   0        0        0       58 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/resources/sample_type/__init__.py
--rw-r--r--   0        0        0       74 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/workflows/__init__.py
--rw-r--r--   0        0        0       58 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
--rw-r--r--   0        0        0     1763 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
--rw-r--r--   0        0        0      933 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/fixtures/studio_models/studio_block
--rw-r--r--   0        0        0        0 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/__init__.py
--rw-r--r--   0        0        0      756 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/generated/__init__.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/metrics/__init__.py
--rw-r--r--   0        0        0     3843 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/metrics/test_rpc_meter.py
--rw-r--r--   0        0        0     6439 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/metrics/test_throughput.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/model_management/__init__.py
--rw-r--r--   0        0        0    14115 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/model_management/test_batcher.py
--rw-r--r--   0        0        0    11774 2023-04-13 23:42:51.872106 caikit-0.1.2/tests/runtime/model_management/test_model_loader.py
--rw-r--r--   0        0        0    18079 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/model_management/test_model_manager.py
--rw-r--r--   0        0        0     5053 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/model_management/test_model_sizer.py
--rw-r--r--   0        0        0     2254 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/model_management/test_training_manager.py
--rw-r--r--   0        0        0        0 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/__init__.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/signature_parsing/__init__.py
--rw-r--r--   0        0        0     1654 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py
--rw-r--r--   0        0        0     3326 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/signature_parsing/test_parsers.py
--rw-r--r--   0        0        0     3280 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/test_create_service.py
--rw-r--r--   0        0        0    18350 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/test_data_stream_source.py
--rw-r--r--   0        0        0     1372 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/service_generation/test_type_helpers.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/__init__.py
--rw-r--r--   0        0        0     9610 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_global_predict_servicer_impl.py
--rw-r--r--   0        0        0    12985 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_global_train_servicer_impl.py
--rw-r--r--   0        0        0     3533 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py
--rw-r--r--   0        0        0     7386 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_model_train_servicer_impl.py
--rw-r--r--   0        0        0     4180 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/servicers/test_training_management_servicer.py
--rw-r--r--   0        0        0    29936 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/test_grpc_server.py
--rw-r--r--   0        0        0     5570 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/test_service_factory.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/__init__.py
--rw-r--r--   0        0        0     3891 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/test_configs.py
--rw-r--r--   0        0        0     5041 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/test_import_util.py
--rw-r--r--   0        0        0    26086 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/utils/test_servicer_util.py
--rw-r--r--   0        0        0      577 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/__init__.py
--rw-r--r--   0        0        0     2807 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/test_abortable_action.py
--rw-r--r--   0        0        0     1868 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/test_call_aborter.py
--rw-r--r--   0        0        0     3355 2023-04-13 23:42:51.876106 caikit-0.1.2/tests/runtime/work_management/test_destroyable_thread.py
--rw-r--r--   0        0        0     1025 2023-04-13 23:42:51.876106 caikit-0.1.2/tox.ini
--rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       60 2023-04-17 22:12:38.150926 caikit-0.1.3/.coveragerc
+-rw-r--r--   0        0        0      676 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      579 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      519 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0        0        0     1272 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/workflows/build-library.yml
+-rw-r--r--   0        0        0     1141 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/workflows/lint-code.yml
+-rw-r--r--   0        0        0     1136 2023-04-17 22:12:38.150926 caikit-0.1.3/.github/workflows/publish-library.yml
+-rw-r--r--   0        0        0      212 2023-04-17 22:12:38.154926 caikit-0.1.3/.gitignore
+-rw-r--r--   0        0        0      310 2023-04-17 22:12:38.154926 caikit-0.1.3/.isort.cfg
+-rw-r--r--   0        0        0      370 2023-04-17 22:12:38.154926 caikit-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      122 2023-04-17 22:12:38.154926 caikit-0.1.3/.prettierignore
+-rw-r--r--   0        0        0       12 2023-04-17 22:12:38.154926 caikit-0.1.3/.prettierrc.yaml
+-rw-r--r--   0        0        0    21434 2023-04-17 22:12:38.154926 caikit-0.1.3/.pylintrc
+-rw-r--r--   0        0        0       78 2023-04-17 22:12:38.154926 caikit-0.1.3/.whitesource
+-rw-r--r--   0        0        0     3358 2023-04-17 22:12:38.154926 caikit-0.1.3/CODE-OF-CONDUCT.md
+-rw-r--r--   0        0        0     6510 2023-04-17 22:12:38.154926 caikit-0.1.3/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11357 2023-04-17 22:12:38.154926 caikit-0.1.3/LICENSE
+-rw-r--r--   0        0        0       18 2023-04-17 22:12:38.154926 caikit-0.1.3/OWNERS
+-rw-r--r--   0        0        0     3757 2023-04-17 22:12:38.154926 caikit-0.1.3/README.md
+-rw-r--r--   0        0        0    44878 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit-overview.png
+-rw-r--r--   0        0        0      323 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/__init__.py
+-rw-r--r--   0        0        0     1861 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/__init__.py
+-rw-r--r--   0        0        0      812 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/__init__.py
+-rw-r--r--   0        0        0     3506 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/base.py
+-rw-r--r--   0        0        0     2828 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/merged_augmentor.py
+-rw-r--r--   0        0        0      355 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/__init__.py
+-rw-r--r--   0        0        0     2052 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/always_selection_scheme.py
+-rw-r--r--   0        0        0     3164 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/base.py
+-rw-r--r--   0        0        0     3264 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py
+-rw-r--r--   0        0        0     2898 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py
+-rw-r--r--   0        0        0      974 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/blocks/__init__.py
+-rw-r--r--   0        0        0     1552 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/blocks/base.py
+-rw-r--r--   0        0        0     1104 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/config/__init__.py
+-rw-r--r--   0        0        0     2551 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/config/config.py
+-rw-r--r--   0        0        0     1010 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/config/config.yml
+-rw-r--r--   0        0        0      962 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/__init__.py
+-rw-r--r--   0        0        0    29207 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/base.py
+-rw-r--r--   0        0        0      750 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     2207 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/data_backends/base.py
+-rw-r--r--   0        0        0     3962 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/data_backends/dict_backend.py
+-rw-r--r--   0        0        0    13676 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/dataobject.py
+-rw-r--r--   0        0        0     5340 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/enums.py
+-rw-r--r--   0        0        0     1471 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/producer.py
+-rw-r--r--   0        0        0     3914 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/protobufs/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/__init__.py
+-rw-r--r--   0        0        0     5500 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/converter.py
+-rw-r--r--   0        0        0     4788 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/csv_column_formatter.py
+-rw-r--r--   0        0        0    40187 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/data_stream.py
+-rw-r--r--   0        0        0     3606 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/resolver.py
+-rw-r--r--   0        0        0     5245 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/data_model/streams/validator.py
+-rw-r--r--   0        0        0    20773 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/model_manager.py
+-rw-r--r--   0        0        0    51860 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module.py
+-rw-r--r--   0        0        0     7643 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backend_config.py
+-rw-r--r--   0        0        0      684 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/__init__.py
+-rw-r--r--   0        0        0     3399 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/backend_types.py
+-rw-r--r--   0        0        0     1786 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/base.py
+-rw-r--r--   0        0        0     1493 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_backends/local_backend.py
+-rw-r--r--   0        0        0     5493 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_config.py
+-rw-r--r--   0        0        0     6247 2023-04-17 22:12:38.154926 caikit-0.1.3/caikit/core/module_meta.py
+-rw-r--r--   0        0        0      709 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/resources/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/resources/base.py
+-rw-r--r--   0        0        0     1032 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/__init__.py
+-rw-r--r--   0        0        0     4716 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/compatibility.py
+-rw-r--r--   0        0        0     1787 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/config_utils.py
+-rw-r--r--   0        0        0      637 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/errors/__init__.py
+-rw-r--r--   0        0        0    18275 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/errors/error_handler.py
+-rw-r--r--   0        0        0     1400 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/errors/validation_error.py
+-rw-r--r--   0        0        0     5439 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/extension_utils.py
+-rw-r--r--   0        0        0     4935 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/fileio.py
+-rw-r--r--   0        0        0     2292 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/isa.py
+-rw-r--r--   0        0        0     1864 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/logging.py
+-rw-r--r--   0        0        0    32214 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/quality_evaluation.py
+-rw-r--r--   0        0        0     3439 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/serializers.py
+-rw-r--r--   0        0        0     5979 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/toolkit/wip_decorator.py
+-rw-r--r--   0        0        0     1022 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/workflows/__init__.py
+-rw-r--r--   0        0        0     9298 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/core/workflows/base.py
+-rw-r--r--   0        0        0      530 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/__init__.py
+-rw-r--r--   0        0        0      748 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/common/__init__.py
+-rw-r--r--   0        0        0     1211 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/common/data_model/__init__.py
+-rw-r--r--   0        0        0     1377 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/common/data_model/producer.py
+-rw-r--r--   0        0        0      611 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/runtime/__init__.py
+-rw-r--r--   0        0        0      763 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/runtime/data_model/__init__.py
+-rw-r--r--   0        0        0     2070 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/interfaces/runtime/data_model/training_management.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/__init__.py
+-rw-r--r--   0        0        0     5353 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/config/config.yml
+-rw-r--r--   0        0        0     1716 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/dump_services.py
+-rw-r--r--   0        0        0    13853 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/grpc_server.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/interceptors/__init__.py
+-rw-r--r--   0        0        0    16502 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     4703 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/metrics/rpc_meter.py
+-rw-r--r--   0        0        0     2370 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/metrics/throughput.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    17143 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/batcher.py
+-rw-r--r--   0        0        0     2648 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/loaded_model.py
+-rw-r--r--   0        0        0     6068 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/model_loader.py
+-rw-r--r--   0        0        0    12138 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/model_manager.py
+-rw-r--r--   0        0        0     4194 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/model_sizer.py
+-rw-r--r--   0        0        0     1587 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/model_management/training_manager.py
+-rw-r--r--   0        0        0      367 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/README.md
+-rw-r--r--   0        0        0      698 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/__init__.py
+-rw-r--r--   0        0        0    11375 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2.py
+-rw-r--r--   0        0        0    12846 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py
+-rw-r--r--   0        0        0    10107 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2.py
+-rw-r--r--   0        0        0    10556 2023-04-17 22:12:38.158926 caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     5535 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/process_pb2.py
+-rw-r--r--   0        0        0     2569 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/process_pb2_grpc.py
+-rw-r--r--   0        0        0     8844 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/protos/model-mesh.proto
+-rw-r--r--   0        0        0     6795 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/protos/model-runtime.proto
+-rw-r--r--   0        0        0     2479 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/protobufs/protos/process.proto
+-rw-r--r--   0        0        0    20064 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_factory.py
+-rw-r--r--   0        0        0      109 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0     1779 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/compatibility_checker.py
+-rw-r--r--   0        0        0     3083 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/core_module_helpers.py
+-rw-r--r--   0        0        0     5611 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/create_service.py
+-rw-r--r--   0        0        0    12289 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/data_stream_source.py
+-rw-r--r--   0        0        0     5768 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/primitives.py
+-rw-r--r--   0        0        0    10121 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/serializers.py
+-rw-r--r--   0        0        0      666 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0    10301 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/docstrings.py
+-rw-r--r--   0        0        0     4911 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/module_signature.py
+-rw-r--r--   0        0        0     8296 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/parsers.py
+-rw-r--r--   0        0        0     2571 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/service_generation/type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0    12008 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/global_predict_servicer.py
+-rw-r--r--   0        0        0    14523 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/global_train_servicer.py
+-rw-r--r--   0        0        0    10554 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/model_runtime_servicer.py
+-rw-r--r--   0        0        0     5496 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/model_train_servicer.py
+-rw-r--r--   0        0        0     1696 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/servicers/training_management_servicer.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/__init__.py
+-rw-r--r--   0        0        0      957 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/aborted_exception.py
+-rw-r--r--   0        0        0     1558 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/caikit_runtime_exception.py
+-rw-r--r--   0        0        0      960 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/types/thread_destroyed_exception.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     4223 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/config_parser.py
+-rw-r--r--   0        0        0     6692 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/import_util.py
+-rw-r--r--   0        0        0     1686 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/log_config.py
+-rw-r--r--   0        0        0    17900 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/utils/servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     3732 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/abortable_action.py
+-rw-r--r--   0        0        0     2969 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/call_aborter.py
+-rw-r--r--   0        0        0     7596 2023-04-17 22:12:38.162926 caikit-0.1.3/caikit/runtime/work_management/destroyable_thread.py
+-rw-r--r--   0        0        0      837 2023-04-17 22:12:38.162926 caikit-0.1.3/examples/start_runtime_with_sample_lib.py
+-rw-r--r--   0        0        0     1154 2023-04-17 22:12:43.871383 caikit-0.1.3/pyproject.toml
+-rwxr-xr-x   0        0        0      720 2023-04-17 22:12:38.162926 caikit-0.1.3/scripts/fmt.sh
+-rw-r--r--   0        0        0       33 2023-04-17 22:12:38.162926 caikit-0.1.3/setup_requirements.txt
+-rw-r--r--   0        0        0     1006 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     3783 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/base.py
+-rw-r--r--   0        0        0     8909 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/__init__.py
+-rw-r--r--   0        0        0     2853 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/augmentors/test_augmentor_base.py
+-rw-r--r--   0        0        0     9114 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/augmentors/test_merged_augmentors.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/blocks/__init__.py
+-rw-r--r--   0        0        0    12691 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/blocks/test_base.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/data_backends/__init__.py
+-rw-r--r--   0        0        0     4559 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/data_backends/test_dict_backend.py
+-rw-r--r--   0        0        0     3306 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_converter.py
+-rw-r--r--   0        0        0     3314 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_csv_column_formatter.py
+-rw-r--r--   0        0        0    26013 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_data_stream.py
+-rw-r--r--   0        0        0     3498 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_resolver.py
+-rw-r--r--   0        0        0     2908 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/streams/test_validator.py
+-rw-r--r--   0        0        0    13070 2023-04-17 22:12:38.162926 caikit-0.1.3/tests/core/data_model/test_base.py
+-rw-r--r--   0        0        0    13533 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/data_model/test_dataobject.py
+-rw-r--r--   0        0        0     1104 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/data_model/test_producer.py
+-rw-r--r--   0        0        0     2909 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/helpers.py
+-rw-r--r--   0        0        0     2320 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/module_backends/test_backend_types.py
+-rw-r--r--   0        0        0     3080 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_config.py
+-rw-r--r--   0        0        0      521 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_imports.py
+-rw-r--r--   0        0        0    18331 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_model_manager.py
+-rw-r--r--   0        0        0    17317 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_module.py
+-rw-r--r--   0        0        0     4751 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_module_backend_config.py
+-rw-r--r--   0        0        0     8441 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_module_metadata.py
+-rw-r--r--   0        0        0     1038 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/test_no_write_permissions.py
+-rw-r--r--   0        0        0     7967 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_compatibility.py
+-rw-r--r--   0        0        0     1953 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_config_utils.py
+-rw-r--r--   0        0        0    14999 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_error_handler.py
+-rw-r--r--   0        0        0     4408 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_extension_utils.py
+-rw-r--r--   0        0        0     4972 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_fileio.py
+-rw-r--r--   0        0        0    25851 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_quality_evaluation.py
+-rw-r--r--   0        0        0     2634 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_serializers.py
+-rw-r--r--   0        0        0     7824 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/toolkit/test_wip_decorator.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/workflows/__init__.py
+-rw-r--r--   0        0        0    15618 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/core/workflows/test_base.py
+-rw-r--r--   0        0        0     5655 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/data_model_helpers.py
+-rw-r--r--   0        0        0       39 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0       27 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/bad_file.json
+-rw-r--r--   0        0        0      106 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.csv
+-rw-r--r--   0        0        0       66 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.json
+-rw-r--r--   0        0        0      233 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.jsonl
+-rw-r--r--   0        0        0     1322 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.txt
+-rw-r--r--   0        0        0       11 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_csv_collection/a.csv
+-rw-r--r--   0        0        0       11 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_csv_collection/b.csv
+-rw-r--r--   0        0        0       11 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_csv_collection/c.csv
+-rw-r--r--   0        0        0       27 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_json_collection/a.json
+-rw-r--r--   0        0        0       27 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_json_collection/b.json
+-rw-r--r--   0        0        0       63 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_json_collection/c.json
+-rw-r--r--   0        0        0      147 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/a.jsonl
+-rw-r--r--   0        0        0      218 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/b.jsonl
+-rw-r--r--   0        0        0       87 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_jsonl_collection/c.jsonl
+-rw-r--r--   0        0        0       52 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_txt_collection/a.txt
+-rw-r--r--   0        0        0       56 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_txt_collection/b.txt
+-rw-r--r--   0        0        0       55 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_txt_collection/c.txt
+-rw-r--r--   0        0        0      125 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/data_stream_inputs/sample_w_header.csv
+-rw-r--r--   0        0        0     1016 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block.zip
+-rw-r--r--   0        0        0      671 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block/data.pkl
+-rw-r--r--   0        0        0      189 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_backend/config.yml
+-rw-r--r--   0        0        0      177 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_foo/config.yml
+-rw-r--r--   0        0        0      506 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_no_nesting.zip
+-rw-r--r--   0        0        0      566 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_singleton/config.yml
+-rw-r--r--   0        0        0      299 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_singleton/data.json
+-rw-r--r--   0        0        0       14 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_block_singleton/data.pkl
+-rw-r--r--   0        0        0      222 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_dataset.json
+-rw-r--r--   0        0        0      717 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_resource.zip
+-rw-r--r--   0        0        0      230 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_resource/config.yml
+-rw-r--r--   0        0        0     1991 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow.zip
+-rw-r--r--   0        0        0      497 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/config.yml
+-rw-r--r--   0        0        0      541 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/config.yml
+-rw-r--r--   0        0        0      299 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/data.json
+-rw-r--r--   0        0        0       14 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/data.pkl
+-rw-r--r--   0        0        0     3033 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/fixtures.py
+-rw-r--r--   0        0        0      918 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/invalid.zip
+-rw-r--r--   0        0        0     2551 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/linux.txt
+-rw-r--r--   0        0        0       10 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/bad_archive.zip
+-rw-r--r--   0        0        0      376 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/bad_model.zip
+-rw-r--r--   0        0        0      355 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/bar/config.yml
+-rw-r--r--   0        0        0      359 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/foo/config.yml
+-rw-r--r--   0        0        0      422 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/models/foo_archive.zip
+-rw-r--r--   0        0        0     2142 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/primitive_party.proto
+-rw-r--r--   0        0        0      145 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/__init__.py
+-rw-r--r--   0        0        0     2080 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2.py
+-rw-r--r--   0        0        0     2447 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py
+-rw-r--r--   0        0        0     2217 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py
+-rw-r--r--   0        0        0     2602 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py
+-rw-r--r--   0        0        0     5995 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protobufs/primitive_party_pb2.py
+-rw-r--r--   0        0        0      416 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protos/caikit_runtime.proto
+-rw-r--r--   0        0        0      437 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/protos/caikit_runtime_train.proto
+-rw-r--r--   0        0        0       24 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample.csv
+-rw-r--r--   0        0        0      359 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_block/config.yml
+-rw-r--r--   0        0        0      176 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/__init__.py
+-rw-r--r--   0        0        0      114 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/other_task/__init__.py
+-rw-r--r--   0        0        0     1852 2023-04-17 22:12:38.166926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py
+-rw-r--r--   0        0        0      199 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/__init__.py
+-rw-r--r--   0        0        0      616 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py
+-rw-r--r--   0        0        0     2411 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py
+-rw-r--r--   0        0        0     1404 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py
+-rw-r--r--   0        0        0     2498 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      202 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/config.py
+-rw-r--r--   0        0        0      141 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/data_model/__init__.py
+-rw-r--r--   0        0        0      859 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/data_model/sample.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/resources/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/resources/sample_type/__init__.py
+-rw-r--r--   0        0        0       74 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/workflows/__init__.py
+-rw-r--r--   0        0        0       58 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/workflows/sample_task/__init__.py
+-rw-r--r--   0        0        0     1763 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py
+-rw-r--r--   0        0        0      933 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/fixtures/studio_models/studio_block
+-rw-r--r--   0        0        0        0 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/__init__.py
+-rw-r--r--   0        0        0      756 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/generated/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/metrics/__init__.py
+-rw-r--r--   0        0        0     3843 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/metrics/test_rpc_meter.py
+-rw-r--r--   0        0        0     6439 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/metrics/test_throughput.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/__init__.py
+-rw-r--r--   0        0        0    14115 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_batcher.py
+-rw-r--r--   0        0        0    11774 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_model_loader.py
+-rw-r--r--   0        0        0    18079 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_model_manager.py
+-rw-r--r--   0        0        0     5053 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_model_sizer.py
+-rw-r--r--   0        0        0     2254 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/model_management/test_training_manager.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/__init__.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/signature_parsing/__init__.py
+-rw-r--r--   0        0        0     1654 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py
+-rw-r--r--   0        0        0     3326 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_parsers.py
+-rw-r--r--   0        0        0     3280 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/test_create_service.py
+-rw-r--r--   0        0        0    18350 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/test_data_stream_source.py
+-rw-r--r--   0        0        0     1372 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/service_generation/test_type_helpers.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/__init__.py
+-rw-r--r--   0        0        0     7923 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_global_predict_servicer_impl.py
+-rw-r--r--   0        0        0    12985 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_global_train_servicer_impl.py
+-rw-r--r--   0        0        0     3533 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py
+-rw-r--r--   0        0        0     7386 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_model_train_servicer_impl.py
+-rw-r--r--   0        0        0     4180 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/servicers/test_training_management_servicer.py
+-rw-r--r--   0        0        0    29936 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/test_grpc_server.py
+-rw-r--r--   0        0        0    10451 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/test_service_factory.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/__init__.py
+-rw-r--r--   0        0        0     3785 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/test_configs.py
+-rw-r--r--   0        0        0     5041 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/test_import_util.py
+-rw-r--r--   0        0        0    26086 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/utils/test_servicer_util.py
+-rw-r--r--   0        0        0      577 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/__init__.py
+-rw-r--r--   0        0        0     2807 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/test_abortable_action.py
+-rw-r--r--   0        0        0     1868 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/test_call_aborter.py
+-rw-r--r--   0        0        0     3355 2023-04-17 22:12:38.170926 caikit-0.1.3/tests/runtime/work_management/test_destroyable_thread.py
+-rw-r--r--   0        0        0     1025 2023-04-17 22:12:38.170926 caikit-0.1.3/tox.ini
+-rw-r--r--   0        0        0     4874 1970-01-01 00:00:00.000000 caikit-0.1.3/PKG-INFO
```

### Comparing `caikit-0.1.2/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-0.1.3/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-0.1.3/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-0.1.3/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/.github/workflows/build-library.yml` & `caikit-0.1.3/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/.github/workflows/lint-code.yml` & `caikit-0.1.3/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/.github/workflows/publish-library.yml` & `caikit-0.1.3/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/.pylintrc` & `caikit-0.1.3/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/CODE-OF-CONDUCT.md` & `caikit-0.1.3/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/CONTRIBUTING.md` & `caikit-0.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/LICENSE` & `caikit-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/README.md` & `caikit-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit-overview.png` & `caikit-0.1.3/caikit-overview.png`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/__init__.py` & `caikit-0.1.3/caikit/core/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/__init__.py` & `caikit-0.1.3/caikit/core/augmentors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/base.py` & `caikit-0.1.3/caikit/core/augmentors/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/merged_augmentor.py` & `caikit-0.1.3/caikit/core/augmentors/merged_augmentor.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/schemes/always_selection_scheme.py` & `caikit-0.1.3/caikit/core/augmentors/schemes/always_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/schemes/base.py` & `caikit-0.1.3/caikit/core/augmentors/schemes/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/schemes/random_multi_selection_scheme.py` & `caikit-0.1.3/caikit/core/augmentors/schemes/random_multi_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/augmentors/schemes/random_single_selection_scheme.py` & `caikit-0.1.3/caikit/core/augmentors/schemes/random_single_selection_scheme.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/blocks/__init__.py` & `caikit-0.1.3/caikit/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/blocks/base.py` & `caikit-0.1.3/caikit/core/blocks/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/config/__init__.py` & `caikit-0.1.3/caikit/core/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/config/config.py` & `caikit-0.1.3/caikit/core/config/config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/config/config.yml` & `caikit-0.1.3/caikit/core/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/__init__.py` & `caikit-0.1.3/caikit/core/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/base.py` & `caikit-0.1.3/caikit/core/data_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/data_backends/__init__.py` & `caikit-0.1.3/caikit/core/data_model/data_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/data_backends/base.py` & `caikit-0.1.3/caikit/core/data_model/data_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/data_backends/dict_backend.py` & `caikit-0.1.3/caikit/core/data_model/data_backends/dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/dataobject.py` & `caikit-0.1.3/caikit/core/data_model/dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/enums.py` & `caikit-0.1.3/caikit/core/data_model/enums.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/producer.py` & `caikit-0.1.3/caikit/core/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/protobufs/__init__.py` & `caikit-0.1.3/caikit/core/data_model/protobufs/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/streams/__init__.py` & `caikit-0.1.3/caikit/core/data_model/streams/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/streams/converter.py` & `caikit-0.1.3/caikit/core/data_model/streams/converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/streams/csv_column_formatter.py` & `caikit-0.1.3/caikit/core/data_model/streams/csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/streams/data_stream.py` & `caikit-0.1.3/caikit/core/data_model/streams/data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/streams/resolver.py` & `caikit-0.1.3/caikit/core/data_model/streams/resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/data_model/streams/validator.py` & `caikit-0.1.3/caikit/core/data_model/streams/validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/model_manager.py` & `caikit-0.1.3/caikit/core/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module.py` & `caikit-0.1.3/caikit/core/module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_backend_config.py` & `caikit-0.1.3/caikit/core/module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_backends/__init__.py` & `caikit-0.1.3/caikit/core/module_backends/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_backends/backend_types.py` & `caikit-0.1.3/caikit/core/module_backends/backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_backends/base.py` & `caikit-0.1.3/caikit/core/module_backends/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_backends/local_backend.py` & `caikit-0.1.3/caikit/core/module_backends/local_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_config.py` & `caikit-0.1.3/caikit/core/module_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/module_meta.py` & `caikit-0.1.3/caikit/core/module_meta.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/resources/__init__.py` & `caikit-0.1.3/caikit/core/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/resources/base.py` & `caikit-0.1.3/caikit/core/resources/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/__init__.py` & `caikit-0.1.3/caikit/core/toolkit/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -18,16 +18,14 @@
 """
 # Local
 from . import compatibility, logging
 from .errors import *
 from .extension_utils import *
 from .fileio import *
 from .isa import *
-from .performance import PerformanceRunner
-from .performance_metrics import *
 from .quality_evaluation import (
     EvalTypes,
     F1Metrics,
     F1MetricsContainer,
     QualityEvaluator,
 )
 from .serializers import *
```

### Comparing `caikit-0.1.2/caikit/core/toolkit/compatibility.py` & `caikit-0.1.3/caikit/core/toolkit/compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/config_utils.py` & `caikit-0.1.3/caikit/core/toolkit/config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/errors/__init__.py` & `caikit-0.1.3/caikit/core/toolkit/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/errors/error_handler.py` & `caikit-0.1.3/caikit/core/toolkit/errors/error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/errors/validation_error.py` & `caikit-0.1.3/caikit/core/toolkit/errors/validation_error.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/extension_utils.py` & `caikit-0.1.3/caikit/core/toolkit/extension_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/fileio.py` & `caikit-0.1.3/caikit/core/toolkit/fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/isa.py` & `caikit-0.1.3/caikit/core/toolkit/isa.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/logging.py` & `caikit-0.1.3/caikit/core/toolkit/logging.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/performance/__init__.py` & `caikit-0.1.3/caikit/runtime/protobufs/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,11 +7,13 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+# Standard
+import os
+import sys
 
-
-# Local
-from .performance import PerformanceRunner
+script_loc = os.path.dirname(os.path.realpath(__file__))
+sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.1.2/caikit/core/toolkit/performance/test_data.py` & `caikit-0.1.3/caikit/runtime/types/thread_destroyed_exception.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,25 +9,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-# Standard
-import os
-
-# Local
-from . import json_test_data, text_test_data
-
-
-def test_data_iter(directory):
-    if os.path.isdir(directory):
-        return text_test_data.TextDirIterator(directory)
-
-    if directory.endswith(".json"):
-        return json_test_data.JsonDataIterator(directory)
-
-    raise ValueError(
-        "Incorrect test directory. Must be either a directory or a .json file "
-        "with `text` attribute"
-    )
+class ThreadDestroyedException(RuntimeError):
+    """Exception raised inside a DestroyableThread when it is destroyed by the thread managing
+    its lifecycle."""
+
+    def __init__(self):
+        super().__init__(
+            "Work thread intentionally destroyed by its lifecycle manager. "
+            "This exception was not raised by the code running in this thread."
+        )
```

### Comparing `caikit-0.1.2/caikit/core/toolkit/quality_evaluation.py` & `caikit-0.1.3/caikit/core/toolkit/quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/serializers.py` & `caikit-0.1.3/caikit/core/toolkit/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/toolkit/wip_decorator.py` & `caikit-0.1.3/caikit/core/toolkit/wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/workflows/__init__.py` & `caikit-0.1.3/caikit/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/core/workflows/base.py` & `caikit-0.1.3/caikit/core/workflows/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/__init__.py` & `caikit-0.1.3/caikit/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/common/__init__.py` & `caikit-0.1.3/caikit/interfaces/common/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/common/data_model/__init__.py` & `caikit-0.1.3/caikit/interfaces/common/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/common/data_model/producer.py` & `caikit-0.1.3/caikit/interfaces/common/data_model/producer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/runtime/__init__.py` & `caikit-0.1.3/caikit/interfaces/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/runtime/data_model/__init__.py` & `caikit-0.1.3/caikit/interfaces/runtime/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/interfaces/runtime/data_model/training_management.py` & `caikit-0.1.3/caikit/interfaces/runtime/data_model/training_management.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/__init__.py` & `caikit-0.1.3/caikit/runtime/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/config/config.yml` & `caikit-0.1.3/caikit/runtime/config/config.yml`

 * *Files 12% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 
 # Configuration items for service generation:
 service_generation:
     enabled: true
     client_package_name: ""
     module_types:
         included: ["blocks", "workflows"]
-    modules:
+    module_guids:
+        included: []
         excluded: []
     primitive_data_model_types: []
     task_types:
+        included: []
         excluded: []
 
 use_abortable_threads: true
 
-strict_rpc_mode: false
-
 metering:
     # Switch off metering by default
     enabled: false
     # Directory to save metrics files
     log_dir: "metering_logs"
     # Write to log file every N seconds
     log_interval: 3600
@@ -123,15 +123,14 @@
 
 # gRPC Server shutdown grace period
 server_shutdown_grace_period_seconds: 45
 
 # Per-environment configurations
 environment: prod
 test:
-    grpc_server_sleep_interval: 1
     find_available_port: true
     runtime_version: mock
     caikit_library: sample_lib
     service_proto_gen_module_dir: tests.fixtures.protobufs
     metering:
         # Switch on metering by default
         enabled: true
@@ -139,29 +138,29 @@
         log_dir: "test/metering_logs"
         # Write to log file every N seconds
         log_interval: 5
     service_generation:
         client_package_name: ""
         module_types:
             included: ["blocks", "workflows"]
-        modules:
+        module_guids:
+            included: []
             excluded: []
         primitive_data_model_types:
             - "sample_lib.data_model.SampleInputType"
         task_types:
+            included: []
             excluded: []
     # training configs for tests
     training:
         auto_load_trained_model: true
         output_dir: test/training_output
 dev:
-    grpc_server_sleep_interval: 45
     runtime_version: real_implementation
 prod:
-    grpc_server_sleep_interval: 45
     runtime_version: real
 
 # TLS configs
 tls:
     server:
         key: ""
         cert: ""
```

### Comparing `caikit-0.1.2/caikit/runtime/dump_services.py` & `caikit-0.1.3/caikit/runtime/dump_services.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/grpc_server.py` & `caikit-0.1.3/caikit/runtime/grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/interceptors/__init__.py` & `caikit-0.1.3/caikit/runtime/interceptors/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py` & `caikit-0.1.3/caikit/runtime/interceptors/caikit_runtime_server_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/metrics/__init__.py` & `caikit-0.1.3/caikit/runtime/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/metrics/rpc_meter.py` & `caikit-0.1.3/caikit/runtime/metrics/rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/metrics/throughput.py` & `caikit-0.1.3/caikit/runtime/metrics/throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/__init__.py` & `caikit-0.1.3/caikit/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/batcher.py` & `caikit-0.1.3/caikit/runtime/model_management/batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/loaded_model.py` & `caikit-0.1.3/caikit/runtime/model_management/loaded_model.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/model_loader.py` & `caikit-0.1.3/caikit/runtime/model_management/model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/model_manager.py` & `caikit-0.1.3/caikit/runtime/model_management/model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/model_sizer.py` & `caikit-0.1.3/caikit/runtime/model_management/model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/model_management/training_manager.py` & `caikit-0.1.3/caikit/runtime/model_management/training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/__init__.py` & `caikit-0.1.3/tests/runtime/generated/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,9 +11,10 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # Standard
 import os
 import sys
 
+# Allow generated _pb2 files in here to import each other
 script_loc = os.path.dirname(os.path.realpath(__file__))
 sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2.py` & `caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/model_mesh_pb2_grpc.py` & `caikit-0.1.3/caikit/runtime/protobufs/model_mesh_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2.py` & `caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/model_runtime_pb2_grpc.py` & `caikit-0.1.3/caikit/runtime/protobufs/model_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/process_pb2.py` & `caikit-0.1.3/caikit/runtime/protobufs/process_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/process_pb2_grpc.py` & `caikit-0.1.3/caikit/runtime/protobufs/process_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/protos/model-mesh.proto` & `caikit-0.1.3/caikit/runtime/protobufs/protos/model-mesh.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/protos/model-runtime.proto` & `caikit-0.1.3/caikit/runtime/protobufs/protos/model-runtime.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/protobufs/protos/process.proto` & `caikit-0.1.3/caikit/runtime/protobufs/protos/process.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_factory.py` & `caikit-0.1.3/caikit/runtime/service_factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """This module is responsible for creating service objects for the runtime to consume"""
 # Standard
 from enum import Enum
 from types import ModuleType
-from typing import Callable, Dict, List, Type
+from typing import Callable, Dict, List, Set, Type
 import dataclasses
 import inspect
 
 # Third Party
 import google.protobuf.descriptor
 import google.protobuf.service
 import grpc
@@ -32,19 +32,21 @@
     service_descriptor_to_service,
 )
 import alog
 
 # Local
 from caikit.core import dataobject
 from caikit.core.data_model.base import DataBase
+from caikit.core.module import ModuleBase
 from caikit.interfaces.runtime.data_model import (
     TrainingInfoRequest,
     TrainingInfoResponse,
 )
 from caikit.runtime import service_generation
+from caikit.runtime.service_generation.core_module_helpers import get_module_info
 from caikit.runtime.service_generation.serializers import (
     RPCSerializerBase,
     snake_to_upper_camel,
 )
 from caikit.runtime.types.caikit_runtime_exception import CaikitRuntimeException
 from caikit.runtime.utils import import_util
 from caikit.runtime.utils.config_parser import ConfigParser
@@ -183,29 +185,29 @@
             )
 
         if source == cls.ServiceSource.GENERATED:
             # First make sure we import the data model for the correct library
             # !!!! This will use the `caikit_library` config
             _ = import_util.get_data_model()
 
-            lib = ConfigParser.get_instance().caikit_library
+            config_parser = ConfigParser.get_instance()
+            lib = config_parser.caikit_library
             ai_domain_name = snake_to_upper_camel(lib.replace("caikit_", ""))
             package_name = f"caikit.runtime.{ai_domain_name}"
 
             # Then do API introspection to come up with all the API definitions to support
-            modules = [
-                module_class
-                for module_class in caikit.core.MODULE_REGISTRY.values()
-                if module_class.__module__.partition(".")[0] == lib
-            ]
+            clean_modules = ServicePackageFactory._get_and_filter_modules(
+                config_parser, lib
+            )
+
             if service_type == cls.ServiceType.INFERENCE:
-                task_rpc_list = service_generation.create_inference_rpcs(modules)
+                task_rpc_list = service_generation.create_inference_rpcs(clean_modules)
                 service_name = f"{ai_domain_name}Service"
             else:  # service_type == cls.ServiceType.TRAINING
-                task_rpc_list = service_generation.create_training_rpcs(modules)
+                task_rpc_list = service_generation.create_training_rpcs(clean_modules)
                 service_name = f"{ai_domain_name}TrainingService"
 
             for rpc in task_rpc_list:
                 if rpc.return_type is None:
                     # TODO: need to hook up the excluded tasks / modules configs and add some
                     # more handling here to ensure good RPCs generated
                     log.info("Skipping rpc %s, no return type on method!", rpc.name)
@@ -239,14 +241,83 @@
                 ),
                 stub_class=service_descriptor_to_client_stub(service_descriptor),
                 messages=client_module,
             )
 
     # Implementation details for pure python service packages #
     @staticmethod
+    def _get_and_filter_modules(
+        config_parser: ConfigParser, lib: str
+    ) -> Set[Type[ModuleBase]]:
+        clean_modules = set()
+        modules = [
+            module_class
+            for module_class in caikit.core.MODULE_REGISTRY.values()
+            if module_class.__module__.partition(".")[0] == lib
+        ]
+        log.debug("Found all modules %s for library %s.", modules, lib)
+
+        # Check config for any explicit inclusions
+        included_task_types = (
+            config_parser.service_generation
+            and config_parser.service_generation.task_types
+            and config_parser.service_generation.task_types.included
+        )
+        included_modules = (
+            config_parser.service_generation
+            and config_parser.service_generation.module_guids
+            and config_parser.service_generation.module_guids.included
+        )
+
+        # Check config for any exclusions
+        excluded_task_types = (
+            config_parser.service_generation
+            and config_parser.service_generation.task_types
+            and config_parser.service_generation.task_types.excluded
+        )
+        excluded_modules = (
+            config_parser.service_generation
+            and config_parser.service_generation.module_guids
+            and config_parser.service_generation.module_guids.excluded
+        )
+
+        for ck_module in modules:
+            # Only create for modules from defined included and exclusion list
+            module_info = get_module_info(ck_module)
+            if excluded_task_types and module_info.type in excluded_task_types:
+                log.debug("Skipping module %s of type %s", ck_module, module_info.type)
+                continue
+
+            if excluded_modules and ck_module.MODULE_ID in excluded_modules:
+                log.debug("Skipping module %s of id %s", ck_module, ck_module.MODULE_ID)
+                continue
+
+            # no inclusions specified means include everything
+            if (included_task_types is None or included_task_types == []) and (
+                included_modules is None or included_modules == []
+            ):
+                clean_modules.add(ck_module)
+
+            # if inclusion is specified, use that
+            else:
+                if (included_modules and ck_module.MODULE_ID in included_modules) or (
+                    included_task_types and module_info.type in included_task_types
+                ):
+                    clean_modules.add(ck_module)
+
+        log.debug(
+            "Filtered list of modules %s after excluding task types: %s and modules ids: %s. \
+                Exclusions are defined in config",
+            clean_modules,
+            excluded_task_types,
+            excluded_modules,
+        )
+        return clean_modules
+
+    @staticmethod
     def _create_request_message_types(
         rpcs_list: List[RPCSerializerBase],
         package_name: str,
     ) -> List[Type[DataBase]]:
         """Dynamically create data model classes for the inputs to these RPCs"""
         data_model_classes = []
         for task in rpcs_list:
```

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/compatibility_checker.py` & `caikit-0.1.3/caikit/runtime/service_generation/compatibility_checker.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/core_module_helpers.py` & `caikit-0.1.3/caikit/runtime/service_generation/core_module_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/create_service.py` & `caikit-0.1.3/caikit/runtime/service_generation/create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/data_stream_source.py` & `caikit-0.1.3/caikit/runtime/service_generation/data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/primitives.py` & `caikit-0.1.3/caikit/runtime/service_generation/primitives.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/serializers.py` & `caikit-0.1.3/caikit/runtime/service_generation/serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/docstrings.py` & `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/module_signature.py` & `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/module_signature.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/signature_parsing/parsers.py` & `caikit-0.1.3/caikit/runtime/service_generation/signature_parsing/parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/service_generation/type_helpers.py` & `caikit-0.1.3/caikit/runtime/service_generation/type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/servicers/__init__.py` & `caikit-0.1.3/caikit/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/servicers/global_predict_servicer.py` & `caikit-0.1.3/caikit/runtime/servicers/global_predict_servicer.py`

 * *Files 3% similar despite different names*

```diff
@@ -95,15 +95,14 @@
     # Input size in code points, provided by orchestrator
     INPUT_SIZE_KEY = "input-length"
 
     def __init__(
         self,
         inference_service: ServicePackage,
         use_abortable_threads: bool = ConfigParser.get_instance().use_abortable_threads,
-        strict_rpc_mode: bool = ConfigParser.get_instance().strict_rpc_mode,
     ):
         self._model_manager = ModelManager.get_instance()
         if ConfigParser.get_instance().metering.enabled:
             self.rpc_meter = RPCMeter()
             log.info(
                 "<RUN76773775I>",
                 "Metering is enabled, to disable set `metering.enabled` in config to false",
@@ -111,15 +110,14 @@
         else:
             log.info(
                 "<RUN76773776I>",
                 "Metering is disabled, to enable set `metering.enabled` in config to true",
             )
 
         self.use_abortable_threads = use_abortable_threads
-        self.strict_rpc_mode = strict_rpc_mode
         self._inference_service = inference_service
         # Validate that the Caikit Library CDM is compatible with our service descriptor
         validate_data_model(self._inference_service.descriptor)
         log.info("<RUN76773778I>", "Validated Caikit Library CDM successfully")
 
         # Duplicate code in global_train_servicer
         # pylint: disable=duplicate-code
@@ -190,19 +188,14 @@
                                     model.run,
                                     **caikit_library_request,
                                 )
                                 response = work.do()
                             else:
                                 response = model.run(**caikit_library_request)
 
-                if self.strict_rpc_mode:
-                    GlobalPredictServicer._raise_on_wrong_rpc(
-                        desc_name, type(response), model_id, model
-                    )
-
                 # Marshall the response to the necessary return type
                 with PREDICT_TO_PROTO_SUMMARY.labels(
                     grpc_request=desc_name, model_id=model_id
                 ).time():
                     response_proto = build_proto_response(response)
 
             # Update Prometheus metrics
```

### Comparing `caikit-0.1.2/caikit/runtime/servicers/global_train_servicer.py` & `caikit-0.1.3/caikit/runtime/servicers/global_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/servicers/model_runtime_servicer.py` & `caikit-0.1.3/caikit/runtime/servicers/model_runtime_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/servicers/model_train_servicer.py` & `caikit-0.1.3/caikit/runtime/servicers/model_train_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/servicers/training_management_servicer.py` & `caikit-0.1.3/caikit/runtime/servicers/training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/types/__init__.py` & `caikit-0.1.3/caikit/runtime/types/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/types/aborted_exception.py` & `caikit-0.1.3/caikit/runtime/types/aborted_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/types/caikit_runtime_exception.py` & `caikit-0.1.3/caikit/runtime/types/caikit_runtime_exception.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/utils/__init__.py` & `caikit-0.1.3/caikit/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/utils/config_parser.py` & `caikit-0.1.3/caikit/runtime/utils/config_parser.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/utils/import_util.py` & `caikit-0.1.3/caikit/runtime/utils/import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/utils/log_config.py` & `caikit-0.1.3/caikit/runtime/utils/log_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/utils/servicer_util.py` & `caikit-0.1.3/caikit/runtime/utils/servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/work_management/__init__.py` & `caikit-0.1.3/caikit/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/work_management/abortable_action.py` & `caikit-0.1.3/caikit/runtime/work_management/abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/work_management/call_aborter.py` & `caikit-0.1.3/caikit/runtime/work_management/call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/caikit/runtime/work_management/destroyable_thread.py` & `caikit-0.1.3/caikit/runtime/work_management/destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/examples/start_runtime_with_sample_lib.py` & `caikit-0.1.3/examples/start_runtime_with_sample_lib.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/pyproject.toml` & `caikit-0.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "caikit"
 # Not the actual current version: overwritten by CI
-version = "0.1.2"
+version = "0.1.3"
 description = "AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework"
 license = {text = "Apache-2.0"}
 readme = "README.md"
 requires-python = "~=3.8"
 classifiers=[
     "License :: OSI Approved :: Apache Software License"
 ]
@@ -18,15 +18,15 @@
     "alchemy-logging>=1.0.4",
     "anytree>=2.7.0,<3.0",
     "docstring-parser>=0.14.1",
     "grpcio-health-checking>=1.35.0,<2.0",
     "grpcio>=1.35.0,<2.0",
     "ijson>=3.1.4,<3.2.0",
     "munch>=2.5.0,<3.0",
-    "protobuf>=3.20.1,<5",
+    "protobuf>=3.19.0,<5",
     "prometheus_client==0.12.0",
     "py-grpc-prometheus>=0.7.0,<0.8",
     "PyYAML>=6.0,<7.0",
     "requests>=2.26.0,<3.0",
     "semver>=2.13.0,<3.0",
     "six>=1.16.0,<2.0.0",
     "tqdm>=4.59.0,<5.0.0",
```

### Comparing `caikit-0.1.2/scripts/fmt.sh` & `caikit-0.1.3/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/__init__.py` & `caikit-0.1.3/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/base.py` & `caikit-0.1.3/tests/base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/conftest.py` & `caikit-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/augmentors/test_augmentor_base.py` & `caikit-0.1.3/tests/core/augmentors/test_augmentor_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/augmentors/test_merged_augmentors.py` & `caikit-0.1.3/tests/core/augmentors/test_merged_augmentors.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/blocks/__init__.py` & `caikit-0.1.3/tests/core/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/blocks/test_base.py` & `caikit-0.1.3/tests/core/blocks/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/data_backends/test_dict_backend.py` & `caikit-0.1.3/tests/core/data_model/data_backends/test_dict_backend.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/streams/test_converter.py` & `caikit-0.1.3/tests/core/data_model/streams/test_converter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/streams/test_csv_column_formatter.py` & `caikit-0.1.3/tests/core/data_model/streams/test_csv_column_formatter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/streams/test_data_stream.py` & `caikit-0.1.3/tests/core/data_model/streams/test_data_stream.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/streams/test_resolver.py` & `caikit-0.1.3/tests/core/data_model/streams/test_resolver.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/streams/test_validator.py` & `caikit-0.1.3/tests/core/data_model/streams/test_validator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/test_base.py` & `caikit-0.1.3/tests/core/data_model/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/data_model/test_dataobject.py` & `caikit-0.1.3/tests/core/data_model/test_dataobject.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/helpers.py` & `caikit-0.1.3/tests/core/helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/module_backends/test_backend_types.py` & `caikit-0.1.3/tests/core/module_backends/test_backend_types.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_config.py` & `caikit-0.1.3/tests/core/test_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_imports.py` & `caikit-0.1.3/tests/core/test_imports.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_model_manager.py` & `caikit-0.1.3/tests/core/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_module.py` & `caikit-0.1.3/tests/core/test_module.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_module_backend_config.py` & `caikit-0.1.3/tests/core/test_module_backend_config.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_module_metadata.py` & `caikit-0.1.3/tests/core/test_module_metadata.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/test_no_write_permissions.py` & `caikit-0.1.3/tests/core/test_no_write_permissions.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_compatibility.py` & `caikit-0.1.3/tests/core/toolkit/test_compatibility.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_config_utils.py` & `caikit-0.1.3/tests/core/toolkit/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_error_handler.py` & `caikit-0.1.3/tests/core/toolkit/test_error_handler.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_extension_utils.py` & `caikit-0.1.3/tests/core/toolkit/test_extension_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_fileio.py` & `caikit-0.1.3/tests/core/toolkit/test_fileio.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_quality_evaluation.py` & `caikit-0.1.3/tests/core/toolkit/test_quality_evaluation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_serializers.py` & `caikit-0.1.3/tests/core/toolkit/test_serializers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/toolkit/test_wip_decorator.py` & `caikit-0.1.3/tests/core/toolkit/test_wip_decorator.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/workflows/__init__.py` & `caikit-0.1.3/tests/core/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/core/workflows/test_base.py` & `caikit-0.1.3/tests/core/workflows/test_base.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/data_model_helpers.py` & `caikit-0.1.3/tests/data_model_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/data_stream_inputs/sample.txt` & `caikit-0.1.3/tests/fixtures/data_stream_inputs/sample.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/dummy_block.zip` & `caikit-0.1.3/tests/fixtures/dummy_block.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/dummy_block/config.yml` & `caikit-0.1.3/tests/fixtures/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/dummy_block_singleton/config.yml` & `caikit-0.1.3/tests/fixtures/dummy_block_singleton/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/dummy_resource.zip` & `caikit-0.1.3/tests/fixtures/dummy_resource.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/dummy_workflow.zip` & `caikit-0.1.3/tests/fixtures/dummy_workflow.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/dummy_workflow/dummy_block/config.yml` & `caikit-0.1.3/tests/fixtures/dummy_workflow/dummy_block/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/fixtures.py` & `caikit-0.1.3/tests/fixtures/fixtures.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/invalid.zip` & `caikit-0.1.3/tests/fixtures/invalid.zip`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/linux.txt` & `caikit-0.1.3/tests/fixtures/linux.txt`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/primitive_party.proto` & `caikit-0.1.3/tests/fixtures/primitive_party.proto`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2.py` & `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py` & `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2.py` & `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py` & `caikit-0.1.3/tests/fixtures/protobufs/caikit_runtime_train_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/protobufs/primitive_party_pb2.py` & `caikit-0.1.3/tests/fixtures/protobufs/primitive_party_pb2.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py` & `caikit-0.1.3/tests/fixtures/sample_lib/blocks/other_task/other_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py` & `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/inner_block.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py` & `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/list_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py` & `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/primitive_party_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py` & `caikit-0.1.3/tests/fixtures/sample_lib/blocks/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/data_model/sample.py` & `caikit-0.1.3/tests/fixtures/sample_lib/data_model/sample.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py` & `caikit-0.1.3/tests/fixtures/sample_lib/workflows/sample_task/sample_implementation.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/fixtures/studio_models/studio_block` & `caikit-0.1.3/tests/fixtures/studio_models/studio_block`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/generated/__init__.py` & `caikit-0.1.3/tests/runtime/metrics/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-# Standard
-import os
-import sys
-
-# Allow generated _pb2 files in here to import each other
-script_loc = os.path.dirname(os.path.realpath(__file__))
-sys.path.insert(0, script_loc)
```

### Comparing `caikit-0.1.2/tests/runtime/metrics/__init__.py` & `caikit-0.1.3/tests/runtime/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/metrics/test_rpc_meter.py` & `caikit-0.1.3/tests/runtime/metrics/test_rpc_meter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/metrics/test_throughput.py` & `caikit-0.1.3/tests/runtime/metrics/test_throughput.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/model_management/__init__.py` & `caikit-0.1.3/tests/runtime/service_generation/signature_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/model_management/test_batcher.py` & `caikit-0.1.3/tests/runtime/model_management/test_batcher.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/model_management/test_model_loader.py` & `caikit-0.1.3/tests/runtime/model_management/test_model_loader.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/model_management/test_model_manager.py` & `caikit-0.1.3/tests/runtime/model_management/test_model_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/model_management/test_model_sizer.py` & `caikit-0.1.3/tests/runtime/model_management/test_model_sizer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/model_management/test_training_manager.py` & `caikit-0.1.3/tests/runtime/model_management/test_training_manager.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/service_generation/signature_parsing/__init__.py` & `caikit-0.1.3/tests/runtime/servicers/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/service_generation/signature_parsing/test_docstrings.py` & `caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/service_generation/signature_parsing/test_parsers.py` & `caikit-0.1.3/tests/runtime/service_generation/signature_parsing/test_parsers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/service_generation/test_create_service.py` & `caikit-0.1.3/tests/runtime/service_generation/test_create_service.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/service_generation/test_data_stream_source.py` & `caikit-0.1.3/tests/runtime/service_generation/test_data_stream_source.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/service_generation/test_type_helpers.py` & `caikit-0.1.3/tests/runtime/service_generation/test_type_helpers.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/servicers/__init__.py` & `caikit-0.1.3/tests/runtime/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/servicers/test_global_predict_servicer_impl.py` & `caikit-0.1.3/tests/runtime/servicers/test_global_predict_servicer_impl.py`

 * *Files 14% similar despite different names*

```diff
@@ -37,32 +37,14 @@
     return "test-any-model-" + str(uuid.uuid4())
 
 
 HAPPY_PATH_INPUT = SampleInputType(name="Gabe").to_proto()
 HAPPY_PATH_RESPONSE = SampleOutputType(greeting="Hello Gabe").to_proto()
 
 
-@pytest.mark.skip("We'd like to just nix the whole strict_rpc_mode check from caikit")
-def test_calling_the_wrong_rpc_for_a_model_raises(
-    sample_inference_service, sample_predict_servicer, loaded_model_id
-):
-    request = sample_inference_service.messages.BobbitRequest(
-        producer_id=TEST_PRODUCER_ID
-    )
-
-    with pytest.raises(CaikitRuntimeException) as context:
-        sample_predict_servicer.Predict(
-            request, Fixtures.build_context(loaded_model_id)
-        )
-
-    assert context.value.status_code == grpc.StatusCode.INVALID_ARGUMENT
-
-    assert "Wrong return type from model" in context.value.message
-
-
 def test_calling_predict_should_raise_if_block_raises(
     sample_inference_service, sample_predict_servicer, loaded_model_id
 ):
     with pytest.raises(CaikitRuntimeException) as context:
         # SampleBlocks will raise a RuntimeError if the throw flag is set
         request = sample_inference_service.messages.SampleTaskRequest(
             sample_input=HAPPY_PATH_INPUT, throw=True
@@ -70,35 +52,14 @@
         sample_predict_servicer.Predict(
             request, Fixtures.build_context(loaded_model_id)
         )
     assert context.value.status_code == grpc.StatusCode.INTERNAL
     assert "Unhandled exception during prediction" in context.value.message
 
 
-@pytest.mark.skip("We'd like to just nix the strict_rpc_mode checking from caikit")
-def test_wrong_rpc_edge_case(sample_inference_service, sample_predict_servicer):
-    """Test that a model that returns a type with a name like ${some_bad_prefix}${expected_type_name} will still
-    raise an invalid argument error"""
-    model_id = _random_test_id()
-    model = DeprecatedWidget()
-    with tempfile.TemporaryDirectory() as tmpdir:
-        model_path = os.path.join(tmpdir, model_id)
-        model.save(model_path)
-        Fixtures.load_model(model_id, model_path, Fixtures().get_good_model_type())
-        with pytest.raises(CaikitRuntimeException) as context:
-            sample_predict_servicer.Predict(
-                sample_inference_service.messages.WidgetRequest(
-                    producer_id=TEST_PRODUCER_ID
-                ),
-                Fixtures.build_context(model_id),
-            )
-        assert context.value.status_code == grpc.StatusCode.INVALID_ARGUMENT
-        assert "Wrong return type from model" in context.value.message
-
-
 def test_invalid_input_to_a_valid_caikit_core_class_method_raises(
     loaded_model_id, sample_inference_service, sample_predict_servicer
 ):
     """Test that a caikit.core block that gets an unexpected input value errors in an expected way"""
     with pytest.raises(CaikitRuntimeException) as context:
         # SampleBlocks will raise a ValueError if the poison pill name is given
         request = sample_inference_service.messages.SampleTaskRequest(
```

### Comparing `caikit-0.1.2/tests/runtime/servicers/test_global_train_servicer_impl.py` & `caikit-0.1.3/tests/runtime/servicers/test_global_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/servicers/test_model_runtime_servicer_impl.py` & `caikit-0.1.3/tests/runtime/servicers/test_model_runtime_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/servicers/test_model_train_servicer_impl.py` & `caikit-0.1.3/tests/runtime/servicers/test_model_train_servicer_impl.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/servicers/test_training_management_servicer.py` & `caikit-0.1.3/tests/runtime/servicers/test_training_management_servicer.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/test_grpc_server.py` & `caikit-0.1.3/tests/runtime/test_grpc_server.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/utils/__init__.py` & `caikit-0.1.3/tests/runtime/work_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/utils/test_configs.py` & `caikit-0.1.3/tests/runtime/utils/test_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,32 +56,31 @@
     def test_it_overrides_deployment_environment_settings(self):
         delete_config_singleton()
         old_deploy_env = os.getenv("ENVIRONMENT")
         try:
             # PROD should set the grpc sleep setting up to 45
             os.environ["ENVIRONMENT"] = "PROD"
             c = ConfigParser()
-            self.assertEqual(45, c.grpc_server_sleep_interval)
+            self.assertEqual("real", c.runtime_version)
         finally:
             # Try to make sure we re-set this to not bork other tests
             os.environ["ENVIRONMENT"] = old_deploy_env
 
     def test_it_can_merge_in_a_config_file(self):
         delete_config_singleton()
         try:
             with TemporaryDirectory() as tempdir:
-                cfg = {"grpc_server_sleep_interval": 7, "new_key": "new_value"}
+                cfg = {"new_key": "new_value"}
                 path = os.path.join(tempdir, "new_config.yml")
                 with open(path, "w") as f:
                     yaml.dump(cfg, f)
 
                 os.environ["CONFIG_FILES"] = path
                 c = ConfigParser()
 
-                self.assertEqual(7, c.grpc_server_sleep_interval)
                 self.assertEqual("new_value", c.new_key)
         finally:
             os.environ["CONFIG_FILES"] = ""
 
     def test_it_can_merge_in_a_dictionary_without_deleting_all_keys(self):
         delete_config_singleton()
         try:
```

### Comparing `caikit-0.1.2/tests/runtime/utils/test_import_util.py` & `caikit-0.1.3/tests/runtime/utils/test_import_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/utils/test_servicer_util.py` & `caikit-0.1.3/tests/runtime/utils/test_servicer_util.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/work_management/test_abortable_action.py` & `caikit-0.1.3/tests/runtime/work_management/test_abortable_action.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/work_management/test_call_aborter.py` & `caikit-0.1.3/tests/runtime/work_management/test_call_aborter.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tests/runtime/work_management/test_destroyable_thread.py` & `caikit-0.1.3/tests/runtime/work_management/test_destroyable_thread.py`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/tox.ini` & `caikit-0.1.3/tox.ini`

 * *Files identical despite different names*

### Comparing `caikit-0.1.2/PKG-INFO` & `caikit-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: caikit
-Version: 0.1.2
+Version: 0.1.3
 Summary: AI toolkit that enables AI users to consume stable task-specific model APIs and enables AI developers build algorithms and models in a modular/composable framework
 Requires-Python: ~=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Dist: alchemy-config>=1.0.0
 Requires-Dist: alchemy-logging>=1.0.4
 Requires-Dist: anytree>=2.7.0,<3.0
 Requires-Dist: docstring-parser>=0.14.1
 Requires-Dist: grpcio-health-checking>=1.35.0,<2.0
 Requires-Dist: grpcio>=1.35.0,<2.0
 Requires-Dist: ijson>=3.1.4,<3.2.0
 Requires-Dist: munch>=2.5.0,<3.0
-Requires-Dist: protobuf>=3.20.1,<5
+Requires-Dist: protobuf>=3.19.0,<5
 Requires-Dist: prometheus_client==0.12.0
 Requires-Dist: py-grpc-prometheus>=0.7.0,<0.8
 Requires-Dist: PyYAML>=6.0,<7.0
 Requires-Dist: requests>=2.26.0,<3.0
 Requires-Dist: semver>=2.13.0,<3.0
 Requires-Dist: six>=1.16.0,<2.0.0
 Requires-Dist: tqdm>=4.59.0,<5.0.0
```

