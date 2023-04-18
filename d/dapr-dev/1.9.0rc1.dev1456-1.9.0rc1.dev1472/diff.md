# Comparing `tmp/dapr-dev-1.9.0rc1.dev1456.tar.gz` & `tmp/dapr-dev-1.9.0rc1.dev1472.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1456.tar", last modified: Tue Apr 11 18:05:50 2023, max compression
+gzip compressed data, was "dist/dapr-dev-1.9.0rc1.dev1472.tar", last modified: Tue Apr 18 17:05:03 2023, max compression
```

## Comparing `dapr-dev-1.9.0rc1.dev1456.tar` & `dapr-dev-1.9.0rc1.dev1472.tar`

### file list

```diff
@@ -1,83 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/
--rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/actor_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/client/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/client/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_call_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_method_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_reminder_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_state_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_timer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_type_information.py
--rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/actor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/method_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/reentrancy_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/remindable.py
--rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/state_change.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/state_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/
--rw-r--r--   0 runner    (1001) docker     (123)     7021 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    28997 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    47859 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/dapr_actor_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/dapr_invocation_http_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/conf/
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/conf/global_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/v1/common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/v1/common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/appcallback_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/dapr_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/dapr_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/serializers/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/serializers/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr/version/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/version/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/dapr/version/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-11 18:05:49.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1961 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:05:49.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-11 18:05:49.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-11 18:05:49.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-11 18:05:49.000000 dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-11 18:05:50.000000 dapr-dev-1.9.0rc1.dev1456/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-11 18:05:37.000000 dapr-dev-1.9.0rc1.dev1456/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/
+-rw-r--r--   0 runner    (1001) docker     (123)    11378 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/actor_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7084 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/client/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_call_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_method_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_reminder_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_state_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_timer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2707 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_type_information.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3847 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10127 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4721 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6112 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1851 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/method_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/reentrancy_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/remindable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7173 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/state_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/state_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/grpc/_asynchelpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48802 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29839 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47931 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/dapr_actor_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5760 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/dapr_invocation_http_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/conf/
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/conf/global_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8257 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/v1/common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/v1/common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18118 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/appcallback_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/appcallback_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71113 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/dapr_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57502 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/dapr_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/serializers/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2541 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/serializers/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr/version/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/version/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/dapr/version/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-04-18 17:05:03.000000 dapr-dev-1.9.0rc1.dev1472/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-18 17:04:51.000000 dapr-dev-1.9.0rc1.dev1472/setup.py
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/LICENSE` & `dapr-dev-1.9.0rc1.dev1472/LICENSE`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1472/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1456
+Version: 1.9.0rc1.dev1472
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/README.md` & `dapr-dev-1.9.0rc1.dev1472/README.md`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/actor_interface.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/actor_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/client/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/client/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/client/proxy.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/client/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/id.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_call_type.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_call_type.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_method_context.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_method_context.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_reminder_data.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_reminder_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_state_provider.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_state_provider.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_timer_data.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_timer_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_type_information.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_type_information.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/_type_utils.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/_type_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/actor.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/actor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/config.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/context.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/manager.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/method_dispatcher.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/method_dispatcher.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/reentrancy_context.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/reentrancy_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/remindable.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/remindable.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/runtime.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/state_change.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/state_change.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/actor/runtime/state_manager.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/actor/runtime/state_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
 
 from typing import Callable, Dict, List, Optional, Union
+from warnings import warn
 
 from dapr.clients.base import DaprActorClientBase
 from dapr.clients.exceptions import DaprInternalError, ERROR_CODE_UNKNOWN
 from dapr.clients.grpc.client import DaprGrpcClient, MetadataTuple, InvokeMethodResponse
 from dapr.clients.http.dapr_actor_http_client import DaprActorHttpClient
 from dapr.clients.http.dapr_invocation_http_client import DaprInvocationHttpClient
 from dapr.conf import settings
@@ -114,53 +115,60 @@
             return self.invocation_client.invoke_method(
                 app_id,
                 method_name,
                 data,
                 content_type=content_type,
                 metadata=metadata,
                 http_verb=http_verb,
-                http_querystring=http_querystring)
+                http_querystring=http_querystring,
+                timeout=timeout)
         else:
             return super().invoke_method(
                 app_id,
                 method_name,
                 data,
                 content_type=content_type,
                 metadata=metadata,
                 http_verb=http_verb,
-                http_querystring=http_querystring)
+                http_querystring=http_querystring,
+                timeout=timeout)
 
     async def invoke_method_async(
             self,
             app_id: str,
             method_name: str,
             data: Union[bytes, str, GrpcMessage],
             content_type: Optional[str] = None,
             metadata: Optional[MetadataTuple] = None,
             http_verb: Optional[str] = None,
-            http_querystring: Optional[MetadataTuple] = None) -> InvokeMethodResponse:
+            http_querystring: Optional[MetadataTuple] = None,
+            timeout: Optional[int] = None) -> InvokeMethodResponse:
         """Invoke a service method over gRPC or HTTP.
 
         Args:
             app_id (str): Application Id.
             method_name (str): Method to be invoked.
             data (bytes or str or GrpcMessage, optional): Data for requet's body.
             content_type (str, optional): Content type of the data.
             metadata (MetadataTuple, optional): Additional metadata or headers.
             http_verb (str, optional): HTTP verb for the request.
             http_querystring (MetadataTuple, optional): Query parameters.
+            timeout (int, optional): Request timeout in seconds.
 
         Returns:
             InvokeMethodResponse: the method invocation response.
         """
         if self.invocation_client:
+            warn('Async invocation is deprecated. Please use `dapr.aio.clients.DaprClient`.',
+                 DeprecationWarning, stacklevel=2)
             return await self.invocation_client.invoke_method_async(
                 app_id,
                 method_name,
                 data,
                 content_type=content_type,
                 metadata=metadata,
                 http_verb=http_verb,
-                http_querystring=http_querystring)
+                http_querystring=http_querystring,
+                timeout=timeout)
         else:
             raise NotImplementedError(
-                'invoke_method_async is not implemented for gRPC')
+                'Please use `dapr.aio.clients.DaprClient` for async invocation')
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/base.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/exceptions.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/exceptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/aio/clients/grpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_helpers.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_request.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_response.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
@@ -847,14 +847,32 @@
         your own ContextManager that logs or otherwise raises exceptions
         if unlock doesn't return `UnlockResponseStatus.success`.
         '''
         if self._success:
             self._client.unlock(self._store_name, self._resource_id, self._lock_owner)
         # else: there is no point unlocking a lock we did not acquire.
 
+    async def __aexit__(self, *exc) -> None:
+        ''''Automatically unlocks the lock if this TryLockResponse was used as
+        a ContextManager / `with` statement.
+
+        Notice: we are not checking the result of the unlock operation.
+        If this is something  you care about it might be wiser creating
+        your own ContextManager that logs or otherwise raises exceptions
+        if unlock doesn't return `UnlockResponseStatus.success`.
+        '''
+        if self._success:
+            await self._client.unlock(self._store_name,   # type: ignore
+                                      self._resource_id, self._lock_owner)
+        # else: there is no point unlocking a lock we did not acquire.
+
+    async def __aenter__(self) -> 'TryLockResponse':
+        '''Returns self as the context manager object.'''
+        return self
+
 
 class GetMetadataResponse(DaprResponse):
     '''GetMetadataResponse is a message that is returned on GetMetadata rpc call.'''
 
     def __init__(
         self,
         application_id: str,
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/_state.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/_state.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/grpc/client.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
@@ -402,15 +402,15 @@
             store_name: str,
             key: str,
             state_metadata: Optional[Dict[str, str]] = dict(),
             metadata: Optional[MetadataTuple] = None) -> StateResponse:
         """Gets value from a statestore with a key
 
         The example gets value from a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.get_state(
                     store_name='state_store'
                     key='key_1',
                     state={"key": "value"},
                     state_metadata={"metakey": "metavalue"},
                 )
@@ -444,15 +444,15 @@
             keys: Sequence[str],
             parallelism: int = 1,
             states_metadata: Optional[Dict[str, str]] = dict(),
             metadata: Optional[MetadataTuple] = None) -> BulkStatesResponse:
         """Gets values from a statestore with keys
 
         The example gets value from a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.get_bulk_state(
                     store_name='state_store',
                     keys=['key_1', key_2],
                     parallelism=2,
                     states_metadata={"metakey": "metavalue"},
                 )
@@ -499,15 +499,15 @@
             query: str,
             states_metadata: Optional[Dict[str, str]] = dict()) -> QueryResponse:
         """Queries a statestore with a query
 
         For details on supported queries see https://docs.dapr.io/
 
         This example queries a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
 
             query = '''
             {
                 "filter": {
                     "EQ": { "state": "CA" }
                 },
                 "sort": [
@@ -574,15 +574,15 @@
         """Saves key-value pairs to a statestore
 
         This saves a value to the statestore with a given key and state store name.
         Options for request can be passed with the options field and custom
         metadata can be passed with metadata field.
 
         The example saves states to a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.save_state(
                     store_name='state_store',
                     key='key1',
                     value='value1',
                     etag='etag',
                     state_metadata={"metakey": "metavalue"},
@@ -640,15 +640,15 @@
             states: List[StateItem],
             metadata: Optional[MetadataTuple] = None) -> DaprResponse:
         """Saves state items to a statestore
 
         This saves a given state item into the statestore specified by store_name.
 
         The example saves states to a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.save_bulk_state(
                     store_name='state_store',
                     states=[StateItem(key='key1', value='value1'),
                         StateItem(key='key2', value='value2', etag='etag'),],
                 )
 
@@ -695,15 +695,15 @@
         """Saves or deletes key-value pairs to a statestore as a transaction
 
         This saves or deletes key-values to the statestore as part of a single transaction,
         transaction_metadata is used for the transaction operation, while metadata is used
         for the GRPC call.
 
         The example saves states to a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.execute_state_transaction(
                     store_name='state_store',
                     operations=[
                         TransactionalStateOperation(key=key, data=value),
                         TransactionalStateOperation(key=another_key, data=another_value),
                         TransactionalStateOperation(
@@ -755,15 +755,15 @@
         """Deletes key-value pairs from a statestore
 
         This deletes a value from the statestore with a given key and state store name.
         Options for request can be passed with the options field and custom
         metadata can be passed with metadata field.
 
         The example deletes states from a statestore:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.delete_state(
                     store_name='state_store',
                     key='key1',
                     etag='etag',
                     state_metadata={"header1": "value1"},
                 )
@@ -909,15 +909,15 @@
             self,
             store_name: str,
             keys: List[str],
             config_metadata: Optional[Dict[str, str]] = dict()) -> ConfigurationResponse:
         """Gets value from a config store with a key
 
         The example gets value from a config store:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.get_configuration(
                     store_name='state_store'
                     keys=['key_1'],
                     config_metadata={"metakey": "metavalue"}
                 )
 
@@ -946,15 +946,15 @@
             self,
             store_name: str,
             keys: List[str],
             config_metadata: Optional[Dict[str, str]] = dict()) -> ConfigurationWatcher:
         """Gets changed value from a config store with a key
 
         The example gets value from a config store:
-            from dapr import DaprClient
+            from dapr.clients import DaprClient
             with DaprClient() as d:
                 resp = d.subscribe_config(
                     store_name='state_store'
                     key='key_1',
                     config_metadata={"metakey": "metavalue"}
                 )
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/grpc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/client.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/dapr_actor_http_client.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/dapr_actor_http_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/clients/http/dapr_invocation_http_client.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/dapr_invocation_http_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/conf/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/conf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/conf/global_settings.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/conf/global_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/clients/http/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/common/v1/common_pb2.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/v1/common_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/common/v1/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/appcallback_pb2.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/appcallback_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/appcallback_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/appcallback_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/dapr_pb2.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/dapr_pb2.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/proto/runtime/v1/dapr_pb2_grpc.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/proto/runtime/v1/dapr_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/serializers/__init__.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/serializers/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/serializers/base.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/serializers/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/serializers/json.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/serializers/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/serializers/util.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/serializers/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr/version/version.py` & `dapr-dev-1.9.0rc1.dev1472/dapr/version/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 
 """
-Copyright 2021 The Dapr Authors
+Copyright 2023 The Dapr Authors
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
     http://www.apache.org/licenses/LICENSE-2.0
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/PKG-INFO` & `dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: dapr-dev
-Version: 1.9.0rc1.dev1456
+Version: 1.9.0rc1.dev1472
 Summary: The developmental release for Dapr Python SDK.
 Home-page: https://dapr.io/
 Author: Dapr Authors
 Author-email: daprweb@microsoft.com
 License: Apache
 Project-URL: Documentation, https://github.com/dapr/docs
 Project-URL: Source, https://github.com/dapr/python-sdk
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/dapr_dev.egg-info/SOURCES.txt` & `dapr-dev-1.9.0rc1.dev1472/dapr_dev.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,18 @@
 dapr/actor/runtime/manager.py
 dapr/actor/runtime/method_dispatcher.py
 dapr/actor/runtime/reentrancy_context.py
 dapr/actor/runtime/remindable.py
 dapr/actor/runtime/runtime.py
 dapr/actor/runtime/state_change.py
 dapr/actor/runtime/state_manager.py
+dapr/aio/clients/__init__.py
+dapr/aio/clients/grpc/__init__.py
+dapr/aio/clients/grpc/_asynchelpers.py
+dapr/aio/clients/grpc/client.py
 dapr/clients/__init__.py
 dapr/clients/base.py
 dapr/clients/exceptions.py
 dapr/clients/grpc/__init__.py
 dapr/clients/grpc/_helpers.py
 dapr/clients/grpc/_request.py
 dapr/clients/grpc/_response.py
```

### Comparing `dapr-dev-1.9.0rc1.dev1456/setup.cfg` & `dapr-dev-1.9.0rc1.dev1472/setup.cfg`

 * *Files identical despite different names*

### Comparing `dapr-dev-1.9.0rc1.dev1456/setup.py` & `dapr-dev-1.9.0rc1.dev1472/setup.py`

 * *Files identical despite different names*

