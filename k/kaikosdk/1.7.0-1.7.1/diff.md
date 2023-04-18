# Comparing `tmp/kaikosdk-1.7.0.tar.gz` & `tmp/kaikosdk-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kaikosdk-1.7.0.tar", last modified: Fri Mar 31 08:17:39 2023, max compression
+gzip compressed data, was "kaikosdk-1.7.1.tar", last modified: Tue Apr 18 08:27:10 2023, max compression
```

## Comparing `kaikosdk-1.7.0.tar` & `kaikosdk-1.7.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.715396 kaikosdk-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-31 08:17:39.715396 kaikosdk-1.7.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.695396 kaikosdk-1.7.0/kaikosdk/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.699396 kaikosdk-1.7.0/kaikosdk/core/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/data_interval_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/data_interval_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/instrument_criteria_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/instrument_criteria_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/sort_criteria_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/sort_criteria_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/source_data_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/source_data_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/source_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/source_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/wrappers_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/core/wrappers_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/sdk_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/sdk_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.699396 kaikosdk-1.7.0/kaikosdk/stream/
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.703396 kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.703396 kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.707396 kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.707396 kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.707396 kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.711396 kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.711396 kaikosdk-1.7.0/kaikosdk/stream/index_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/commodity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/commodity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/index_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.715396 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/commodity_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/commodity_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.715396 kaikosdk-1.7.0/kaikosdk/stream/trades_v1/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/trades_v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/trades_v1/request_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/trades_v1/request_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/trades_v1/response_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-31 08:17:27.000000 kaikosdk-1.7.0/kaikosdk/stream/trades_v1/response_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 08:17:39.695396 kaikosdk-1.7.0/kaikosdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-31 08:17:39.000000 kaikosdk-1.7.0/kaikosdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-03-31 08:17:39.000000 kaikosdk-1.7.0/kaikosdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 08:17:39.000000 kaikosdk-1.7.0/kaikosdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 08:17:39.000000 kaikosdk-1.7.0/kaikosdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 08:17:39.000000 kaikosdk-1.7.0/kaikosdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-31 08:17:39.715396 kaikosdk-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-03-31 08:17:30.000000 kaikosdk-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.897806 kaikosdk-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.885806 kaikosdk-1.7.1/kaikosdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/core/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/data_interval_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/data_interval_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/instrument_criteria_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/instrument_criteria_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/sort_criteria_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/sort_criteria_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_data_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_data_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/source_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/wrappers_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/core/wrappers_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/sdk_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26534 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/sdk_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1728 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1718 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/index_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/commodity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/commodity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1797 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/index_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/commodity_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/commodity_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.893806 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/request_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/request_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/response_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-18 08:27:01.000000 kaikosdk-1.7.1/kaikosdk/stream/trades_v1/response_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 08:27:10.889806 kaikosdk-1.7.1/kaikosdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-18 08:27:10.000000 kaikosdk-1.7.1/kaikosdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 08:27:10.897806 kaikosdk-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-04-18 08:27:03.000000 kaikosdk-1.7.1/setup.py
```

### Comparing `kaikosdk-1.7.0/kaikosdk/core/data_interval_pb2.py` & `kaikosdk-1.7.1/kaikosdk/core/data_interval_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/core/instrument_criteria_pb2.py` & `kaikosdk-1.7.1/kaikosdk/core/instrument_criteria_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/core/sort_criteria_pb2.py` & `kaikosdk-1.7.1/kaikosdk/core/sort_criteria_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/core/source_data_pb2.py` & `kaikosdk-1.7.1/kaikosdk/core/source_data_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/core/source_pb2.py` & `kaikosdk-1.7.1/kaikosdk/core/source_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/core/wrappers_pb2.py` & `kaikosdk-1.7.1/kaikosdk/core/wrappers_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/sdk_pb2.py` & `kaikosdk-1.7.1/kaikosdk/sdk_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/sdk_pb2_grpc.py` & `kaikosdk-1.7.1/kaikosdk/sdk_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregated_price_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregated_price_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregated_quote_v2/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregated_quote_v2/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_direct_exchange_rate_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_ohlcv_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_spot_exchange_rate_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/aggregates_vwap_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/index_v1/commodity_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/index_v1/commodity_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/index_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/index_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/index_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/index_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/commodity_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/commodity_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/market_update_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/market_update_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/trades_v1/request_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/trades_v1/request_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk/stream/trades_v1/response_pb2.py` & `kaikosdk-1.7.1/kaikosdk/stream/trades_v1/response_pb2.py`

 * *Files identical despite different names*

### Comparing `kaikosdk-1.7.0/kaikosdk.egg-info/SOURCES.txt` & `kaikosdk-1.7.1/kaikosdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

