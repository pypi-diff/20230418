# Comparing `tmp/polarismesh_specification-1.3.0a5.tar.gz` & `tmp/polarismesh_specification-1.3.0a6.tar.gz`

## Comparing `polarismesh_specification-1.3.0a5.tar` & `polarismesh_specification-1.3.0a6.tar`

### file list

```diff
@@ -1,75 +1,75 @@
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/__about__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
--rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
--rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
--rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
--rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
--rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
--rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/__init__.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/__init__.pyi
--rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.py
--rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.py
--rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/__init__.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/__init__.pyi
--rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.py
--rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/__init__.py
--rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
--rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
--rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
--rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
--rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
--rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
--rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
--rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
--rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
--rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
--rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
--rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
--rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
--rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
--rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/.gitignore
--rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/LICENSE.txt
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/README.md
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/pyproject.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a5/PKG-INFO
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/__about__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/__init__.pyi
+-rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py
+-rw-r--r--   0        0        0    15838 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2_grpc.py
+-rw-r--r--   0        0        0     4675 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2_grpc.py
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.pyi
+-rw-r--r--   0        0        0     4281 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/__init__.py
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/__init__.pyi
+-rw-r--r--   0        0        0    12836 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py
+-rw-r--r--   0        0        0    21477 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2_grpc.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py
+-rw-r--r--   0        0        0     5050 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2_grpc.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/__init__.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/__init__.pyi
+-rw-r--r--   0        0        0     9500 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.py
+-rw-r--r--   0        0        0     4864 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2_grpc.py
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.py
+-rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2_grpc.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.py
+-rw-r--r--   0        0        0     3331 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2_grpc.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/__init__.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/__init__.pyi
+-rw-r--r--   0        0        0     8640 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.py
+-rw-r--r--   0        0        0    14132 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2_grpc.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/__init__.py
+-rw-r--r--   0        0        0      428 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/__init__.pyi
+-rw-r--r--   0        0        0     2514 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2_grpc.py
+-rw-r--r--   0        0        0     2114 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py
+-rw-r--r--   0        0        0     1795 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2_grpc.py
+-rw-r--r--   0        0        0     2342 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.pyi
+-rw-r--r--   0        0        0    13092 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py
+-rw-r--r--   0        0        0     2623 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2_grpc.py
+-rw-r--r--   0        0        0     1980 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.py
+-rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2_grpc.py
+-rw-r--r--   0        0        0     7810 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.py
+-rw-r--r--   0        0        0    13032 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2_grpc.py
+-rw-r--r--   0        0        0     7373 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.py
+-rw-r--r--   0        0        0    11915 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2_grpc.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/__init__.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/__init__.pyi
+-rw-r--r--   0        0        0     9567 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py
+-rw-r--r--   0        0        0    15322 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2_grpc.py
+-rw-r--r--   0        0        0     9246 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py
+-rw-r--r--   0        0        0    13498 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2_grpc.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/.gitignore
+-rw-r--r--   0        0        0    48229 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/LICENSE.txt
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/README.md
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/pyproject.toml
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 polarismesh_specification-1.3.0a6/PKG-INFO
```

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/config_file_response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/config_manage/grpc_config_api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/circuitbreaker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/fault_tolerance/fault_detector_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/code_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/code_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/model_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/model/namespace_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/security/auth_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/security/auth_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/configrelease_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/grpcapi_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/heartbeat_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from ..model import model_pb2 as model__pb2
 from ..service_manage import client_pb2 as client__pb2
 from ..service_manage import configrelease_pb2 as configrelease__pb2
 from ..fault_tolerance import fault_detector_pb2 as fault__detector__pb2
 from ..security import auth_pb2 as auth__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eresponse.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/protobuf/any.proto\x1a\x0fnamespace.proto\x1a\rservice.proto\x1a\rrouting.proto\x1a\x0fratelimit.proto\x1a\x14\x63ircuitbreaker.proto\x1a\x0bmodel.proto\x1a\x0c\x63lient.proto\x1a\x13\x63onfigrelease.proto\x1a\x14\x66\x61ult_detector.proto\x1a\nauth.proto\"\xcf\x06\n\x08Response\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1a\n\x06\x63lient\x18\x03 \x01(\x0b\x32\n.v1.Client\x12 \n\tnamespace\x18\x04 \x01(\x0b\x32\r.v1.Namespace\x12\x1c\n\x07service\x18\x05 \x01(\x0b\x32\x0b.v1.Service\x12\x1e\n\x08instance\x18\x06 \x01(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x07 \x01(\x0b\x32\x0b.v1.Routing\x12\x1f\n\x05\x61lias\x18\x08 \x01(\x0b\x32\x10.v1.ServiceAlias\x12\x1b\n\trateLimit\x18\t \x01(\x0b\x32\x08.v1.Rule\x12*\n\x0e\x63ircuitBreaker\x18\n \x01(\x0b\x32\x12.v1.CircuitBreaker\x12(\n\rconfigRelease\x18\x0b \x01(\x0b\x32\x11.v1.ConfigRelease\x12\x16\n\x04user\x18\x13 \x01(\x0b\x32\x08.v1.User\x12 \n\tuserGroup\x18\x14 \x01(\x0b\x32\r.v1.UserGroup\x12&\n\x0c\x61uthStrategy\x18\x15 \x01(\x0b\x32\x10.v1.AuthStrategy\x12\'\n\x08relation\x18\x16 \x01(\x0b\x32\x15.v1.UserGroupRelation\x12(\n\rloginResponse\x18\x17 \x01(\x0b\x32\x11.v1.LoginResponse\x12\x32\n\x12modifyAuthStrategy\x18\x18 \x01(\x0b\x32\x16.v1.ModifyAuthStrategy\x12,\n\x0fmodifyUserGroup\x18\x19 \x01(\x0b\x32\x13.v1.ModifyUserGroup\x12(\n\tresources\x18\x1a \x01(\x0b\x32\x15.v1.StrategyResources\x12&\n\x0coptionSwitch\x18\x1b \x01(\x0b\x32\x10.v1.OptionSwitch\x12*\n\x0einstanceLabels\x18\x1c \x01(\x0b\x32\x12.v1.InstanceLabels\x12\"\n\x04\x64\x61ta\x18\x1d \x01(\x0b\x32\x14.google.protobuf.AnyJ\x04\x08\x0c\x10\x13\"\xb9\x01\n\x12\x42\x61tchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04size\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x1f\n\tresponses\x18\x04 \x03(\x0b\x32\x0c.v1.Response\"\x87\x05\n\x12\x42\x61tchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04size\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12!\n\nnamespaces\x18\x05 \x03(\x0b\x32\r.v1.Namespace\x12\x1d\n\x08services\x18\x06 \x03(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x07 \x03(\x0b\x32\x0c.v1.Instance\x12\x1d\n\x08routings\x18\x08 \x03(\x0b\x32\x0b.v1.Routing\x12!\n\x07\x61liases\x18\t \x03(\x0b\x32\x10.v1.ServiceAlias\x12\x1c\n\nrateLimits\x18\n \x03(\x0b\x32\x08.v1.Rule\x12\x31\n\x12\x63onfigWithServices\x18\x0b \x03(\x0b\x32\x15.v1.ConfigWithService\x12\x17\n\x05users\x18\x12 \x03(\x0b\x32\x08.v1.User\x12!\n\nuserGroups\x18\x13 \x03(\x0b\x32\r.v1.UserGroup\x12(\n\x0e\x61uthStrategies\x18\x14 \x03(\x0b\x32\x10.v1.AuthStrategy\x12\x1b\n\x07\x63lients\x18\x15 \x03(\x0b\x32\n.v1.Client\x12\"\n\x04\x64\x61ta\x18\x16 \x03(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x07summary\x18\x17 \x01(\x0b\x32\x0b.v1.SummaryJ\x04\x08\x0c\x10\x12\"\xbe\x05\n\x10\x44iscoverResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).v1.DiscoverResponse.DiscoverResponseType\x12\x1c\n\x07service\x18\x04 \x01(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x05 \x03(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x06 \x01(\x0b\x32\x0b.v1.Routing\x12 \n\trateLimit\x18\x07 \x01(\x0b\x32\r.v1.RateLimit\x12*\n\x0e\x63ircuitBreaker\x18\x08 \x01(\x0b\x32\x12.v1.CircuitBreaker\x12\x1d\n\x08services\x18\t \x03(\x0b\x32\x0b.v1.Service\x12!\n\nnamespaces\x18\n \x03(\x0b\x32\r.v1.Namespace\x12(\n\rfaultDetector\x18\x0b \x01(\x0b\x32\x11.v1.FaultDetector\x12\x1d\n\x08\x61liasFor\x18\x0c \x01(\x0b\x32\x0b.v1.Service\"\xe2\x01\n\x14\x44iscoverResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\"\x04\x08\x07\x10\x0b*\x04MESH*\x0bMESH_CONFIG*\x0e\x46LUX_DBREFRESH*\x08\x46LUX_SDK*\x0b\x46LUX_SERVER\"n\n\x0cOptionSwitch\x12.\n\x07options\x18\x01 \x03(\x0b\x32\x1d.v1.OptionSwitch.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\x0eInstanceLabels\x12.\n\x06labels\x18\x01 \x03(\x0b\x32\x1e.v1.InstanceLabels.LabelsEntry\x1a=\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.v1.StringList:\x02\x38\x01\x42\x8e\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eresponse.proto\x12\x02v1\x1a\x1egoogle/protobuf/wrappers.proto\x1a\x19google/protobuf/any.proto\x1a\x0fnamespace.proto\x1a\rservice.proto\x1a\rrouting.proto\x1a\x0fratelimit.proto\x1a\x14\x63ircuitbreaker.proto\x1a\x0bmodel.proto\x1a\x0c\x63lient.proto\x1a\x13\x63onfigrelease.proto\x1a\x14\x66\x61ult_detector.proto\x1a\nauth.proto\"\xcf\x06\n\x08Response\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x1a\n\x06\x63lient\x18\x03 \x01(\x0b\x32\n.v1.Client\x12 \n\tnamespace\x18\x04 \x01(\x0b\x32\r.v1.Namespace\x12\x1c\n\x07service\x18\x05 \x01(\x0b\x32\x0b.v1.Service\x12\x1e\n\x08instance\x18\x06 \x01(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x07 \x01(\x0b\x32\x0b.v1.Routing\x12\x1f\n\x05\x61lias\x18\x08 \x01(\x0b\x32\x10.v1.ServiceAlias\x12\x1b\n\trateLimit\x18\t \x01(\x0b\x32\x08.v1.Rule\x12*\n\x0e\x63ircuitBreaker\x18\n \x01(\x0b\x32\x12.v1.CircuitBreaker\x12(\n\rconfigRelease\x18\x0b \x01(\x0b\x32\x11.v1.ConfigRelease\x12\x16\n\x04user\x18\x13 \x01(\x0b\x32\x08.v1.User\x12 \n\tuserGroup\x18\x14 \x01(\x0b\x32\r.v1.UserGroup\x12&\n\x0c\x61uthStrategy\x18\x15 \x01(\x0b\x32\x10.v1.AuthStrategy\x12\'\n\x08relation\x18\x16 \x01(\x0b\x32\x15.v1.UserGroupRelation\x12(\n\rloginResponse\x18\x17 \x01(\x0b\x32\x11.v1.LoginResponse\x12\x32\n\x12modifyAuthStrategy\x18\x18 \x01(\x0b\x32\x16.v1.ModifyAuthStrategy\x12,\n\x0fmodifyUserGroup\x18\x19 \x01(\x0b\x32\x13.v1.ModifyUserGroup\x12(\n\tresources\x18\x1a \x01(\x0b\x32\x15.v1.StrategyResources\x12&\n\x0coptionSwitch\x18\x1b \x01(\x0b\x32\x10.v1.OptionSwitch\x12*\n\x0einstanceLabels\x18\x1c \x01(\x0b\x32\x12.v1.InstanceLabels\x12\"\n\x04\x64\x61ta\x18\x1d \x01(\x0b\x32\x14.google.protobuf.AnyJ\x04\x08\x0c\x10\x13\"\xb9\x01\n\x12\x42\x61tchWriteResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12*\n\x04size\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12\x1f\n\tresponses\x18\x04 \x03(\x0b\x32\x0c.v1.Response\"\x87\x05\n\x12\x42\x61tchQueryResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12,\n\x06\x61mount\x18\x03 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04size\x18\x04 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12!\n\nnamespaces\x18\x05 \x03(\x0b\x32\r.v1.Namespace\x12\x1d\n\x08services\x18\x06 \x03(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x07 \x03(\x0b\x32\x0c.v1.Instance\x12\x1d\n\x08routings\x18\x08 \x03(\x0b\x32\x0b.v1.Routing\x12!\n\x07\x61liases\x18\t \x03(\x0b\x32\x10.v1.ServiceAlias\x12\x1c\n\nrateLimits\x18\n \x03(\x0b\x32\x08.v1.Rule\x12\x31\n\x12\x63onfigWithServices\x18\x0b \x03(\x0b\x32\x15.v1.ConfigWithService\x12\x17\n\x05users\x18\x12 \x03(\x0b\x32\x08.v1.User\x12!\n\nuserGroups\x18\x13 \x03(\x0b\x32\r.v1.UserGroup\x12(\n\x0e\x61uthStrategies\x18\x14 \x03(\x0b\x32\x10.v1.AuthStrategy\x12\x1b\n\x07\x63lients\x18\x15 \x03(\x0b\x32\n.v1.Client\x12\"\n\x04\x64\x61ta\x18\x16 \x03(\x0b\x32\x14.google.protobuf.Any\x12\x1c\n\x07summary\x18\x17 \x01(\x0b\x32\x0b.v1.SummaryJ\x04\x08\x0c\x10\x12\"\xc4\x05\n\x10\x44iscoverResponse\x12*\n\x04\x63ode\x18\x01 \x01(\x0b\x32\x1c.google.protobuf.UInt32Value\x12*\n\x04info\x18\x02 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x37\n\x04type\x18\x03 \x01(\x0e\x32).v1.DiscoverResponse.DiscoverResponseType\x12\x1c\n\x07service\x18\x04 \x01(\x0b\x32\x0b.v1.Service\x12\x1f\n\tinstances\x18\x05 \x03(\x0b\x32\x0c.v1.Instance\x12\x1c\n\x07routing\x18\x06 \x01(\x0b\x32\x0b.v1.Routing\x12 \n\trateLimit\x18\x07 \x01(\x0b\x32\r.v1.RateLimit\x12*\n\x0e\x63ircuitBreaker\x18\x08 \x01(\x0b\x32\x12.v1.CircuitBreaker\x12\x1d\n\x08services\x18\t \x03(\x0b\x32\x0b.v1.Service\x12!\n\nnamespaces\x18\n \x03(\x0b\x32\r.v1.Namespace\x12(\n\rfaultDetector\x18\x0b \x01(\x0b\x32\x11.v1.FaultDetector\x12\x1d\n\x08\x61liasFor\x18\x15 \x01(\x0b\x32\x0b.v1.Service\"\xe2\x01\n\x14\x44iscoverResponseType\x12\x0b\n\x07UNKNOWN\x10\x00\x12\x0c\n\x08INSTANCE\x10\x01\x12\x0b\n\x07\x43LUSTER\x10\x02\x12\x0b\n\x07ROUTING\x10\x03\x12\x0e\n\nRATE_LIMIT\x10\x04\x12\x13\n\x0f\x43IRCUIT_BREAKER\x10\x05\x12\x0c\n\x08SERVICES\x10\x06\x12\x0e\n\nNAMESPACES\x10\x0c\x12\x12\n\x0e\x46\x41ULT_DETECTOR\x10\r\"\x04\x08\x07\x10\x0b*\x04MESH*\x0bMESH_CONFIG*\x0e\x46LUX_DBREFRESH*\x08\x46LUX_SDK*\x0b\x46LUX_SERVERJ\x04\x08\x0c\x10\x15\"n\n\x0cOptionSwitch\x12.\n\x07options\x18\x01 \x03(\x0b\x32\x1d.v1.OptionSwitch.OptionsEntry\x1a.\n\x0cOptionsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\x7f\n\x0eInstanceLabels\x12.\n\x06labels\x18\x01 \x03(\x0b\x32\x1e.v1.InstanceLabels.LabelsEntry\x1a=\n\x0bLabelsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x1d\n\x05value\x18\x02 \x01(\x0b\x32\x0e.v1.StringList:\x02\x38\x01\x42\x8e\x01\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manageb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'response_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n7com.tencent.polaris.specification.api.v1.service.manageB\rResponseProtoZDgithub.com/polarismesh/specification/source/go/api/v1/service_manage'
@@ -40,19 +40,19 @@
   _RESPONSE._serialized_start=250
   _RESPONSE._serialized_end=1097
   _BATCHWRITERESPONSE._serialized_start=1100
   _BATCHWRITERESPONSE._serialized_end=1285
   _BATCHQUERYRESPONSE._serialized_start=1288
   _BATCHQUERYRESPONSE._serialized_end=1935
   _DISCOVERRESPONSE._serialized_start=1938
-  _DISCOVERRESPONSE._serialized_end=2640
+  _DISCOVERRESPONSE._serialized_end=2646
   _DISCOVERRESPONSE_DISCOVERRESPONSETYPE._serialized_start=2414
   _DISCOVERRESPONSE_DISCOVERRESPONSETYPE._serialized_end=2640
-  _OPTIONSWITCH._serialized_start=2642
-  _OPTIONSWITCH._serialized_end=2752
-  _OPTIONSWITCH_OPTIONSENTRY._serialized_start=2706
-  _OPTIONSWITCH_OPTIONSENTRY._serialized_end=2752
-  _INSTANCELABELS._serialized_start=2754
-  _INSTANCELABELS._serialized_end=2881
-  _INSTANCELABELS_LABELSENTRY._serialized_start=2820
-  _INSTANCELABELS_LABELSENTRY._serialized_end=2881
+  _OPTIONSWITCH._serialized_start=2648
+  _OPTIONSWITCH._serialized_end=2758
+  _OPTIONSWITCH_OPTIONSENTRY._serialized_start=2712
+  _OPTIONSWITCH_OPTIONSENTRY._serialized_end=2758
+  _INSTANCELABELS._serialized_start=2760
+  _INSTANCELABELS._serialized_end=2887
+  _INSTANCELABELS_LABELSENTRY._serialized_start=2826
+  _INSTANCELABELS_LABELSENTRY._serialized_end=2887
 # @@protoc_insertion_point(module_scope)
```

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/service_manage/service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.py`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi` & `polarismesh_specification-1.3.0a6/src/polarismesh_specification/api/v1/traffic_manage/routing_pb2.pyi`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/LICENSE.txt` & `polarismesh_specification-1.3.0a6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/README.md` & `polarismesh_specification-1.3.0a6/README.md`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/pyproject.toml` & `polarismesh_specification-1.3.0a6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `polarismesh_specification-1.3.0a5/PKG-INFO` & `polarismesh_specification-1.3.0a6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polarismesh-specification
-Version: 1.3.0a5
+Version: 1.3.0a6
 Project-URL: Documentation, https://github.com/polarismesh/specification#readme
 Project-URL: Issues, https://github.com/polarismesh/specification/issues
 Project-URL: Source, https://github.com/polarismesh/specification
 Author-email: "{authemail@qq.com}" <authemail@qq.com>
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

