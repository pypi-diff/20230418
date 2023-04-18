# Comparing `tmp/tigeropen-2.3.6.tar.gz` & `tmp/tigeropen-2.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tigeropen-2.3.6.tar", last modified: Tue Apr 11 08:56:40 2023, max compression
+gzip compressed data, was "tigeropen-2.3.7.tar", last modified: Tue Apr 18 08:29:48 2023, max compression
```

## Comparing `tigeropen-2.3.6.tar` & `tigeropen-2.3.7.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.852808 tigeropen-2.3.6/
--rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.6/MANIFEST.in
--rw-r--r--   0 sukai      (501) staff       (20)     6807 2023-04-11 08:56:40.852337 tigeropen-2.3.6/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.6/README.md
--rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.6/requirements.txt
--rw-r--r--   0 sukai      (501) staff       (20)       38 2023-04-11 08:56:40.852957 tigeropen-2.3.6/setup.cfg
--rw-r--r--   0 sukai      (501) staff       (20)     1407 2023-02-16 07:36:42.000000 tigeropen-2.3.6/setup.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.780294 tigeropen-2.3.6/tigeropen/
--rw-r--r--   0 sukai      (501) staff       (20)       91 2023-04-11 08:56:25.000000 tigeropen-2.3.6/tigeropen/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.784104 tigeropen-2.3.6/tigeropen/common/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/common/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.788206 tigeropen-2.3.6/tigeropen/common/consts/
--rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.6/tigeropen/common/consts/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    18954 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/consts/filter_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/consts/fundamental_fields.py
--rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/common/consts/params.py
--rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/consts/push_destinations.py
--rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/consts/push_subscriptions.py
--rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/common/consts/push_types.py
--rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.6/tigeropen/common/consts/quote_keys.py
--rw-r--r--   0 sukai      (501) staff       (20)     2887 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/common/consts/service_types.py
--rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/consts/tick_constants.py
--rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/common/exceptions.py
--rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/model.py
--rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/request.py
--rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.6/tigeropen/common/response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.792018 tigeropen-2.3.6/tigeropen/common/util/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/common/util/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/util/account_util.py
--rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/util/common_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-02-16 07:36:42.000000 tigeropen-2.3.6/tigeropen/common/util/contract_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.6/tigeropen/common/util/order_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/common/util/price_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.6/tigeropen/common/util/signature_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/common/util/string_utils.py
--rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.6/tigeropen/common/util/tick_util.py
--rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/common/util/web_utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.793868 tigeropen-2.3.6/tigeropen/examples/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/examples/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/client_config.py
--rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/nasdaq100.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.794345 tigeropen-2.3.6/tigeropen/examples/option_helpers/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/option_helpers/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/examples/option_helpers/helpers.py
--rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/examples/push_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/examples/push_client_stomp_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/examples/quote_client_demo.py
--rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/examples/trade_client_demo.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.794764 tigeropen-2.3.6/tigeropen/fundamental/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.795037 tigeropen-2.3.6/tigeropen/fundamental/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/domain/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.795594 tigeropen-2.3.6/tigeropen/fundamental/request/
--rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/fundamental/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.798237 tigeropen-2.3.6/tigeropen/fundamental/response/
--rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.6/tigeropen/fundamental/response/corporate_dividend_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.6/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/fundamental/response/corporate_split_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/fundamental/response/financial_daily_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/fundamental/response/financial_report_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/fundamental/response/industry_response.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.799595 tigeropen-2.3.6/tigeropen/push/
--rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/push/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.803032 tigeropen-2.3.6/tigeropen/push/network/
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/connect.py
--rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/exception.py
--rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/listener.py
--rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/protocal.py
--rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/transport.py
--rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/network/utils.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.817382 tigeropen-2.3.6/tigeropen/push/pb/
--rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/AssetData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1030 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PositionData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1749 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2314 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PushData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Request.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Response.proto
--rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/SocketCommon.proto
--rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/TradeTickData.proto
--rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.py
--rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.pyi
--rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.6/tigeropen/push/pb/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/readme.md
--rw-r--r--   0 sukai      (501) staff       (20)     8946 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/pb/util.py
--rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/protobuf_push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/push_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.6/tigeropen/push/stomp_push_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.817969 tigeropen-2.3.6/tigeropen/quote/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/quote/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.823029 tigeropen-2.3.6/tigeropen/quote/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/quote/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/bar.py
--rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/domain/capital_distribution.py
--rw-r--r--   0 sukai      (501) staff       (20)     9598 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/domain/filter.py
--rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/market_status.py
--rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/quote_brief.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/domain/stock_broker.py
--rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/tick.py
--rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/domain/timeline.py
--rw-r--r--   0 sukai      (501) staff       (20)    76032 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/quote_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.823956 tigeropen-2.3.6/tigeropen/quote/request/
--rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    33338 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.842691 tigeropen-2.3.6/tigeropen/quote/response/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/quote/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/capital_distribution_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/capital_flow_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.6/tigeropen/quote/response/future_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.6/tigeropen/quote/response/future_contract_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/future_exchange_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/future_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/future_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.6/tigeropen/quote/response/future_trading_times_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1129 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/market_scanner_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/market_status_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/quote/response/option_chains_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_expirations_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/option_quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_bar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_brief_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_delay_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_depth_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_grab_permission_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_hour_trading_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_ticks_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_history_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_broker_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_details_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_short_interest_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/stock_trade_meta_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/symbol_names_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/quote/response/symbols_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/quote/response/trading_calendar_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/response/warrant_briefs_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/quote/response/warrant_filter_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.6/tigeropen/tiger_open_client.py
--rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.6/tigeropen/tiger_open_config.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.843402 tigeropen-2.3.6/tigeropen/trade/
--rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/trade/__init__.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.845848 tigeropen-2.3.6/tigeropen/trade/domain/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/trade/domain/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/domain/account.py
--rw-r--r--   0 sukai      (501) staff       (20)     4117 2023-01-11 10:23:46.000000 tigeropen-2.3.6/tigeropen/trade/domain/contract.py
--rw-r--r--   0 sukai      (501) staff       (20)     9743 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/domain/order.py
--rw-r--r--   0 sukai      (501) staff       (20)     1682 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/trade/domain/position.py
--rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/trade/domain/prime_account.py
--rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/domain/profile.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.847154 tigeropen-2.3.6/tigeropen/trade/request/
--rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.6/tigeropen/trade/request/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)    29977 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/request/model.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.851624 tigeropen-2.3.6/tigeropen/trade/response/
--rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/__init__.py
--rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/account_profile_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/analytics_asset_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/contracts_response.py
--rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/response/forex_order_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/order_id_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.6/tigeropen/trade/response/order_preview_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     6627 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/response/orders_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     3878 2021-08-30 08:30:28.000000 tigeropen-2.3.6/tigeropen/trade/response/positions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.6/tigeropen/trade/response/prime_assets_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/response/segment_fund_response.py
--rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.6/tigeropen/trade/response/transactions_response.py
--rw-r--r--   0 sukai      (501) staff       (20)    39340 2023-04-11 08:55:54.000000 tigeropen-2.3.6/tigeropen/trade/trade_client.py
-drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-11 08:56:40.782340 tigeropen-2.3.6/tigeropen.egg-info/
--rw-r--r--   0 sukai      (501) staff       (20)     6807 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/PKG-INFO
--rw-r--r--   0 sukai      (501) staff       (20)     7360 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/SOURCES.txt
--rw-r--r--   0 sukai      (501) staff       (20)        1 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/dependency_links.txt
--rw-r--r--   0 sukai      (501) staff       (20)      130 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/requires.txt
--rw-r--r--   0 sukai      (501) staff       (20)       10 2023-04-11 08:56:40.000000 tigeropen-2.3.6/tigeropen.egg-info/top_level.txt
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.101903 tigeropen-2.3.7/
+-rw-r--r--   0 sukai      (501) staff       (20)       25 2020-06-01 05:09:25.000000 tigeropen-2.3.7/MANIFEST.in
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-04-18 08:29:48.101671 tigeropen-2.3.7/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     6033 2022-11-30 08:21:30.000000 tigeropen-2.3.7/README.md
+-rw-r--r--   0 sukai      (501) staff       (20)      129 2023-03-29 02:32:08.000000 tigeropen-2.3.7/requirements.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       38 2023-04-18 08:29:48.101977 tigeropen-2.3.7/setup.cfg
+-rw-r--r--   0 sukai      (501) staff       (20)     1358 2023-04-18 08:29:36.000000 tigeropen-2.3.7/setup.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.027768 tigeropen-2.3.7/tigeropen/
+-rw-r--r--   0 sukai      (501) staff       (20)       91 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.030847 tigeropen-2.3.7/tigeropen/common/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/common/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.033441 tigeropen-2.3.7/tigeropen/common/consts/
+-rw-r--r--   0 sukai      (501) staff       (20)     4255 2023-03-31 07:32:01.000000 tigeropen-2.3.7/tigeropen/common/consts/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    18954 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/consts/filter_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)    30001 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/consts/fundamental_fields.py
+-rw-r--r--   0 sukai      (501) staff       (20)      521 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/common/consts/params.py
+-rw-r--r--   0 sukai      (501) staff       (20)      272 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/consts/push_destinations.py
+-rw-r--r--   0 sukai      (501) staff       (20)      376 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/consts/push_subscriptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1395 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/common/consts/push_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)      784 2021-11-01 11:55:38.000000 tigeropen-2.3.7/tigeropen/common/consts/quote_keys.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2945 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/common/consts/service_types.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3368 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/consts/tick_constants.py
+-rw-r--r--   0 sukai      (501) staff       (20)      411 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/common/exceptions.py
+-rw-r--r--   0 sukai      (501) staff       (20)      686 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/model.py
+-rw-r--r--   0 sukai      (501) staff       (20)      857 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/request.py
+-rw-r--r--   0 sukai      (501) staff       (20)      549 2021-11-16 06:27:09.000000 tigeropen-2.3.7/tigeropen/common/response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.035800 tigeropen-2.3.7/tigeropen/common/util/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/common/util/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      331 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/util/account_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)      984 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/util/common_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3942 2023-02-16 07:36:42.000000 tigeropen-2.3.7/tigeropen/common/util/contract_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6676 2023-03-29 02:32:08.000000 tigeropen-2.3.7/tigeropen/common/util/order_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2993 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/common/util/price_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2126 2022-06-02 11:07:24.000000 tigeropen-2.3.7/tigeropen/common/util/signature_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      850 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/common/util/string_utils.py
+-rw-r--r--   0 sukai      (501) staff       (20)      615 2023-03-02 08:06:25.000000 tigeropen-2.3.7/tigeropen/common/util/tick_util.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3580 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/common/util/web_utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.039547 tigeropen-2.3.7/tigeropen/examples/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/examples/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      877 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/client_config.py
+-rw-r--r--   0 sukai      (501) staff       (20)    15007 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/nasdaq100.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.040220 tigeropen-2.3.7/tigeropen/examples/option_helpers/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/option_helpers/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    13524 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/examples/option_helpers/helpers.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9532 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/examples/push_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11030 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/examples/push_client_stomp_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)    12782 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/examples/quote_client_demo.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8402 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/examples/trade_client_demo.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.040548 tigeropen-2.3.7/tigeropen/fundamental/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.041054 tigeropen-2.3.7/tigeropen/fundamental/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/domain/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.041931 tigeropen-2.3.7/tigeropen/fundamental/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       23 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6390 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/fundamental/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.045929 tigeropen-2.3.7/tigeropen/fundamental/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       24 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1342 2023-03-03 09:45:35.000000 tigeropen-2.3.7/tigeropen/fundamental/response/corporate_dividend_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1392 2021-05-18 09:54:41.000000 tigeropen-2.3.7/tigeropen/fundamental/response/corporate_earnings_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1142 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/fundamental/response/corporate_split_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      945 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/fundamental/response/financial_daily_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1108 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/fundamental/response/financial_report_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2715 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/fundamental/response/industry_response.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.048777 tigeropen-2.3.7/tigeropen/push/
+-rw-r--r--   0 sukai      (501) staff       (20)      812 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/push/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.052043 tigeropen-2.3.7/tigeropen/push/network/
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2499 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/connect.py
+-rw-r--r--   0 sukai      (501) staff       (20)      523 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/exception.py
+-rw-r--r--   0 sukai      (501) staff       (20)     7693 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/listener.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1492 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/protocal.py
+-rw-r--r--   0 sukai      (501) staff       (20)    31491 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/transport.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2633 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/network/utils.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.071329 tigeropen-2.3.7/tigeropen/push/pb/
+-rw-r--r--   0 sukai      (501) staff       (20)     1100 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/AssetData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1572 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1887 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1567 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2199 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3433 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      878 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1729 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2102 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1117 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/push/pb/PositionData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1824 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2418 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      826 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/PushData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3277 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2985 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      451 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1702 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1397 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3046 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3115 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     2372 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     3573 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4265 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      326 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1490 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1503 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      622 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/Request.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2412 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2457 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/Response.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     4204 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1717 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)      726 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/SocketCommon.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     2049 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1478 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)     1239 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/TradeTickData.proto
+-rw-r--r--   0 sukai      (501) staff       (20)     1760 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2502 2023-04-18 06:52:53.000000 tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.pyi
+-rw-r--r--   0 sukai      (501) staff       (20)        0 2023-03-29 02:32:08.000000 tigeropen-2.3.7/tigeropen/push/pb/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      125 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/readme.md
+-rw-r--r--   0 sukai      (501) staff       (20)     8946 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/pb/util.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11569 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/protobuf_push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)     8097 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/push_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    27606 2023-03-03 09:45:38.000000 tigeropen-2.3.7/tigeropen/push/stomp_push_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.072200 tigeropen-2.3.7/tigeropen/quote/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/quote/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.076959 tigeropen-2.3.7/tigeropen/quote/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/quote/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      396 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/bar.py
+-rw-r--r--   0 sukai      (501) staff       (20)      484 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/domain/capital_distribution.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9598 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/domain/filter.py
+-rw-r--r--   0 sukai      (501) staff       (20)      443 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/market_status.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1897 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/quote_brief.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/domain/stock_broker.py
+-rw-r--r--   0 sukai      (501) staff       (20)      322 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/tick.py
+-rw-r--r--   0 sukai      (501) staff       (20)      298 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/domain/timeline.py
+-rw-r--r--   0 sukai      (501) staff       (20)    76032 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/quote_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.077894 tigeropen-2.3.7/tigeropen/quote/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       71 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    33338 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.093978 tigeropen-2.3.7/tigeropen/quote/response/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/quote/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)      840 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/capital_distribution_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      818 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/capital_flow_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2251 2023-01-11 10:48:57.000000 tigeropen-2.3.7/tigeropen/quote/response/future_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2521 2023-01-11 10:48:57.000000 tigeropen-2.3.7/tigeropen/quote/response/future_contract_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1222 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/future_exchange_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1719 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/future_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      770 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/future_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1403 2020-04-24 06:35:28.000000 tigeropen-2.3.7/tigeropen/quote/response/future_trading_times_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1129 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/market_scanner_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1998 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/market_status_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2505 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1635 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/quote/response/option_chains_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1131 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_expirations_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2402 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2170 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/option_quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1574 2023-03-02 08:06:25.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_bar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2528 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_brief_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      863 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_delay_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1366 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_depth_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      719 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_grab_permission_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2742 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_hour_trading_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2463 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_ticks_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1064 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_history_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2837 2022-04-13 02:06:02.000000 tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1517 2021-11-11 02:55:37.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1857 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_broker_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4953 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_details_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1770 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_short_interest_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1270 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/stock_trade_meta_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      740 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/symbol_names_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      655 2021-08-30 08:30:28.000000 tigeropen-2.3.7/tigeropen/quote/response/symbols_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      701 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/quote/response/trading_calendar_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      802 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/response/warrant_briefs_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      979 2023-04-11 09:03:52.000000 tigeropen-2.3.7/tigeropen/quote/response/warrant_filter_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11305 2023-03-10 10:02:27.000000 tigeropen-2.3.7/tigeropen/tiger_open_client.py
+-rw-r--r--   0 sukai      (501) staff       (20)    16406 2023-03-23 03:30:06.000000 tigeropen-2.3.7/tigeropen/tiger_open_config.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.094816 tigeropen-2.3.7/tigeropen/trade/
+-rw-r--r--   0 sukai      (501) staff       (20)       68 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/trade/__init__.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.096677 tigeropen-2.3.7/tigeropen/trade/domain/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/trade/domain/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    11655 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/trade/domain/account.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4117 2023-01-11 10:23:46.000000 tigeropen-2.3.7/tigeropen/trade/domain/contract.py
+-rw-r--r--   0 sukai      (501) staff       (20)     9811 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/domain/order.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2257 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/domain/position.py
+-rw-r--r--   0 sukai      (501) staff       (20)     3197 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/trade/domain/prime_account.py
+-rw-r--r--   0 sukai      (501) staff       (20)      452 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/domain/profile.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.097528 tigeropen-2.3.7/tigeropen/trade/request/
+-rw-r--r--   0 sukai      (501) staff       (20)       69 2019-01-23 09:28:35.000000 tigeropen-2.3.7/tigeropen/trade/request/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)    32706 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/request/model.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.101366 tigeropen-2.3.7/tigeropen/trade/response/
+-rw-r--r--   0 sukai      (501) staff       (20)      657 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/__init__.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1179 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/account_profile_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      961 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/analytics_asset_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4484 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1633 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/contracts_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)      664 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/trade/response/forex_order_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1163 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/order_id_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1336 2020-06-01 05:09:25.000000 tigeropen-2.3.7/tigeropen/trade/response/order_preview_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     6736 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/response/orders_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     4864 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/response/positions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1408 2022-09-27 12:08:43.000000 tigeropen-2.3.7/tigeropen/trade/response/prime_assets_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     2539 2023-04-11 08:55:54.000000 tigeropen-2.3.7/tigeropen/trade/response/segment_fund_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)     1472 2022-11-30 08:21:30.000000 tigeropen-2.3.7/tigeropen/trade/response/transactions_response.py
+-rw-r--r--   0 sukai      (501) staff       (20)    40415 2023-04-18 08:29:36.000000 tigeropen-2.3.7/tigeropen/trade/trade_client.py
+drwxr-xr-x   0 sukai      (501) staff       (20)        0 2023-04-18 08:29:48.029840 tigeropen-2.3.7/tigeropen.egg-info/
+-rw-r--r--   0 sukai      (501) staff       (20)     6757 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/PKG-INFO
+-rw-r--r--   0 sukai      (501) staff       (20)     7360 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/SOURCES.txt
+-rw-r--r--   0 sukai      (501) staff       (20)        1 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/dependency_links.txt
+-rw-r--r--   0 sukai      (501) staff       (20)      130 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/requires.txt
+-rw-r--r--   0 sukai      (501) staff       (20)       10 2023-04-18 08:29:47.000000 tigeropen-2.3.7/tigeropen.egg-info/top_level.txt
```

### Comparing `tigeropen-2.3.6/PKG-INFO` & `tigeropen-2.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.6
+Version: 2.3.7
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `tigeropen-2.3.6/README.md` & `tigeropen-2.3.7/README.md`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/setup.py` & `tigeropen-2.3.7/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     url='https://github.com/tigerbrokers/openapi-python-sdk',
     platforms='any',
     install_requires=install_requires,
     classifiers=[
         'Programming Language :: Python',
         'Operating System :: Microsoft :: Windows',
         'Operating System :: Unix',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
     ],
```

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/__init__.py` & `tigeropen-2.3.7/tigeropen/common/consts/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/filter_fields.py` & `tigeropen-2.3.7/tigeropen/common/consts/filter_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/fundamental_fields.py` & `tigeropen-2.3.7/tigeropen/common/consts/fundamental_fields.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/params.py` & `tigeropen-2.3.7/tigeropen/common/consts/params.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/push_types.py` & `tigeropen-2.3.7/tigeropen/common/consts/push_types.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/quote_keys.py` & `tigeropen-2.3.7/tigeropen/common/consts/quote_keys.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/service_types.py` & `tigeropen-2.3.7/tigeropen/common/consts/service_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 ORDER_TRANSACTIONS = "order_transactions"  # 订单成交记录
 ANALYTICS_ASSET = "analytics_asset"
 SEGMENT_FUND_HISTORY = "segment_fund_history"
 SEGMENT_FUND_AVAILABLE = "segment_fund_available"
 TRANSFER_SEGMENT_FUND = "transfer_segment_fund"
 CANCEL_SEGMENT_FUND = "cancel_segment_fund"
 PLACE_FOREX_ORDER = "place_forex_order"
+ESTIMATE_TRADABLE_QUANTITY = "estimate_tradable_quantity"
 
 USER_LICENSE = "user_license"
 
 """
 合约
 """
 CONTRACT = "contract"
```

### Comparing `tigeropen-2.3.6/tigeropen/common/consts/tick_constants.py` & `tigeropen-2.3.7/tigeropen/common/consts/tick_constants.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/model.py` & `tigeropen-2.3.7/tigeropen/common/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/request.py` & `tigeropen-2.3.7/tigeropen/common/request.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/response.py` & `tigeropen-2.3.7/tigeropen/common/response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/common_utils.py` & `tigeropen-2.3.7/tigeropen/common/util/common_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/contract_utils.py` & `tigeropen-2.3.7/tigeropen/common/util/contract_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/order_utils.py` & `tigeropen-2.3.7/tigeropen/common/util/order_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/price_util.py` & `tigeropen-2.3.7/tigeropen/common/util/price_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/signature_utils.py` & `tigeropen-2.3.7/tigeropen/common/util/signature_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/string_utils.py` & `tigeropen-2.3.7/tigeropen/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/tick_util.py` & `tigeropen-2.3.7/tigeropen/common/util/tick_util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/common/util/web_utils.py` & `tigeropen-2.3.7/tigeropen/common/util/web_utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/client_config.py` & `tigeropen-2.3.7/tigeropen/examples/client_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/nasdaq100.py` & `tigeropen-2.3.7/tigeropen/examples/nasdaq100.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/option_helpers/helpers.py` & `tigeropen-2.3.7/tigeropen/examples/option_helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/push_client_demo.py` & `tigeropen-2.3.7/tigeropen/examples/push_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/push_client_stomp_demo.py` & `tigeropen-2.3.7/tigeropen/examples/push_client_stomp_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/quote_client_demo.py` & `tigeropen-2.3.7/tigeropen/examples/quote_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/examples/trade_client_demo.py` & `tigeropen-2.3.7/tigeropen/examples/trade_client_demo.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/request/model.py` & `tigeropen-2.3.7/tigeropen/fundamental/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/response/corporate_dividend_response.py` & `tigeropen-2.3.7/tigeropen/fundamental/response/corporate_dividend_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/response/corporate_earnings_calendar_response.py` & `tigeropen-2.3.7/tigeropen/fundamental/response/corporate_earnings_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/response/corporate_split_response.py` & `tigeropen-2.3.7/tigeropen/fundamental/response/corporate_split_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/response/financial_daily_response.py` & `tigeropen-2.3.7/tigeropen/fundamental/response/financial_daily_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/response/financial_report_response.py` & `tigeropen-2.3.7/tigeropen/fundamental/response/financial_report_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/fundamental/response/industry_response.py` & `tigeropen-2.3.7/tigeropen/fundamental/response/industry_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/__init__.py` & `tigeropen-2.3.7/tigeropen/push/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/network/connect.py` & `tigeropen-2.3.7/tigeropen/push/network/connect.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/network/exception.py` & `tigeropen-2.3.7/tigeropen/push/network/exception.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/network/listener.py` & `tigeropen-2.3.7/tigeropen/push/network/listener.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/network/protocal.py` & `tigeropen-2.3.7/tigeropen/push/network/protocal.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/network/transport.py` & `tigeropen-2.3.7/tigeropen/push/network/transport.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/network/utils.py` & `tigeropen-2.3.7/tigeropen/push/network/utils.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/AssetData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/AssetData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/AssetData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/AssetData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/OrderStatusData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/OrderStatusData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/OrderTransactionData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/OrderTransactionData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/PositionData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/PositionData.proto`

 * *Files 24% similar despite different names*

```diff
@@ -19,9 +19,9 @@
   sint32 positionScale = 13; // total position scale
   double averageCost = 14; // average holding cost
   double latestPrice = 15; // last price of the asset
   double marketValue = 16; // market value of the asset
   double unrealizedPnl = 17; // unrealized profit and loss
   string name = 18; // symbol name
   uint64 timestamp = 19;
-
+  optional sint64 saleable = 20; // saleable quantity for Chinese A-share market stocks
 }
```

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tigeropen/push/pb/PositionData.proto\x12\x11tigeropen.push.pb\"\xea\x02\n\x0cPositionData\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x0e\n\x06\x65xpiry\x18\x03 \x01(\t\x12\x0e\n\x06strike\x18\x04 \x01(\t\x12\r\n\x05right\x18\x05 \x01(\t\x12\x12\n\nidentifier\x18\x06 \x01(\t\x12\x12\n\nmultiplier\x18\x07 \x01(\r\x12\x0e\n\x06market\x18\x08 \x01(\t\x12\x10\n\x08\x63urrency\x18\t \x01(\t\x12\x0f\n\x07segType\x18\n \x01(\t\x12\x0f\n\x07secType\x18\x0b \x01(\t\x12\x10\n\x08position\x18\x0c \x01(\x12\x12\x15\n\rpositionScale\x18\r \x01(\x11\x12\x13\n\x0b\x61verageCost\x18\x0e \x01(\x01\x12\x13\n\x0blatestPrice\x18\x0f \x01(\x01\x12\x13\n\x0bmarketValue\x18\x10 \x01(\x01\x12\x15\n\runrealizedPnl\x18\x11 \x01(\x01\x12\x0c\n\x04name\x18\x12 \x01(\t\x12\x11\n\ttimestamp\x18\x13 \x01(\x04\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n$tigeropen/push/pb/PositionData.proto\x12\x11tigeropen.push.pb\"\x8e\x03\n\x0cPositionData\x12\x0f\n\x07\x61\x63\x63ount\x18\x01 \x01(\t\x12\x0e\n\x06symbol\x18\x02 \x01(\t\x12\x0e\n\x06\x65xpiry\x18\x03 \x01(\t\x12\x0e\n\x06strike\x18\x04 \x01(\t\x12\r\n\x05right\x18\x05 \x01(\t\x12\x12\n\nidentifier\x18\x06 \x01(\t\x12\x12\n\nmultiplier\x18\x07 \x01(\r\x12\x0e\n\x06market\x18\x08 \x01(\t\x12\x10\n\x08\x63urrency\x18\t \x01(\t\x12\x0f\n\x07segType\x18\n \x01(\t\x12\x0f\n\x07secType\x18\x0b \x01(\t\x12\x10\n\x08position\x18\x0c \x01(\x12\x12\x15\n\rpositionScale\x18\r \x01(\x11\x12\x13\n\x0b\x61verageCost\x18\x0e \x01(\x01\x12\x13\n\x0blatestPrice\x18\x0f \x01(\x01\x12\x13\n\x0bmarketValue\x18\x10 \x01(\x01\x12\x15\n\runrealizedPnl\x18\x11 \x01(\x01\x12\x0c\n\x04name\x18\x12 \x01(\t\x12\x11\n\ttimestamp\x18\x13 \x01(\x04\x12\x15\n\x08saleable\x18\x14 \x01(\x12H\x00\x88\x01\x01\x42\x0b\n\t_saleableb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tigeropen.push.pb.PositionData_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _POSITIONDATA._serialized_start=60
-  _POSITIONDATA._serialized_end=422
+  _POSITIONDATA._serialized_end=458
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/PositionData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/PositionData_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class PositionData(_message.Message):
-    __slots__ = ["account", "averageCost", "currency", "expiry", "identifier", "latestPrice", "market", "marketValue", "multiplier", "name", "position", "positionScale", "right", "secType", "segType", "strike", "symbol", "timestamp", "unrealizedPnl"]
+    __slots__ = ["account", "averageCost", "currency", "expiry", "identifier", "latestPrice", "market", "marketValue", "multiplier", "name", "position", "positionScale", "right", "saleable", "secType", "segType", "strike", "symbol", "timestamp", "unrealizedPnl"]
     ACCOUNT_FIELD_NUMBER: _ClassVar[int]
     AVERAGECOST_FIELD_NUMBER: _ClassVar[int]
     CURRENCY_FIELD_NUMBER: _ClassVar[int]
     EXPIRY_FIELD_NUMBER: _ClassVar[int]
     IDENTIFIER_FIELD_NUMBER: _ClassVar[int]
     LATESTPRICE_FIELD_NUMBER: _ClassVar[int]
     MARKETVALUE_FIELD_NUMBER: _ClassVar[int]
     MARKET_FIELD_NUMBER: _ClassVar[int]
     MULTIPLIER_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     POSITIONSCALE_FIELD_NUMBER: _ClassVar[int]
     POSITION_FIELD_NUMBER: _ClassVar[int]
     RIGHT_FIELD_NUMBER: _ClassVar[int]
+    SALEABLE_FIELD_NUMBER: _ClassVar[int]
     SECTYPE_FIELD_NUMBER: _ClassVar[int]
     SEGTYPE_FIELD_NUMBER: _ClassVar[int]
     STRIKE_FIELD_NUMBER: _ClassVar[int]
     SYMBOL_FIELD_NUMBER: _ClassVar[int]
     TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     UNREALIZEDPNL_FIELD_NUMBER: _ClassVar[int]
     account: str
@@ -34,14 +35,15 @@
     market: str
     marketValue: float
     multiplier: int
     name: str
     position: int
     positionScale: int
     right: str
+    saleable: int
     secType: str
     segType: str
     strike: str
     symbol: str
     timestamp: int
     unrealizedPnl: float
-    def __init__(self, account: _Optional[str] = ..., symbol: _Optional[str] = ..., expiry: _Optional[str] = ..., strike: _Optional[str] = ..., right: _Optional[str] = ..., identifier: _Optional[str] = ..., multiplier: _Optional[int] = ..., market: _Optional[str] = ..., currency: _Optional[str] = ..., segType: _Optional[str] = ..., secType: _Optional[str] = ..., position: _Optional[int] = ..., positionScale: _Optional[int] = ..., averageCost: _Optional[float] = ..., latestPrice: _Optional[float] = ..., marketValue: _Optional[float] = ..., unrealizedPnl: _Optional[float] = ..., name: _Optional[str] = ..., timestamp: _Optional[int] = ...) -> None: ...
+    def __init__(self, account: _Optional[str] = ..., symbol: _Optional[str] = ..., expiry: _Optional[str] = ..., strike: _Optional[str] = ..., right: _Optional[str] = ..., identifier: _Optional[str] = ..., multiplier: _Optional[int] = ..., market: _Optional[str] = ..., currency: _Optional[str] = ..., segType: _Optional[str] = ..., secType: _Optional[str] = ..., position: _Optional[int] = ..., positionScale: _Optional[int] = ..., averageCost: _Optional[float] = ..., latestPrice: _Optional[float] = ..., marketValue: _Optional[float] = ..., unrealizedPnl: _Optional[float] = ..., name: _Optional[str] = ..., timestamp: _Optional[int] = ..., saleable: _Optional[int] = ...) -> None: ...
```

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/PushData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/PushData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/PushData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/PushData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteBBOData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteBBOData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteBasicData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteBasicData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/QuoteDepthData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/QuoteDepthData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/Request.proto` & `tigeropen-2.3.7/tigeropen/push/pb/Request.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/Request_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/Request_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/Response_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/Response_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/SocketCommon.proto` & `tigeropen-2.3.7/tigeropen/push/pb/SocketCommon.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/SocketCommon_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/SocketCommon_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/TradeTickData.proto` & `tigeropen-2.3.7/tigeropen/push/pb/TradeTickData.proto`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.py` & `tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/TradeTickData_pb2.pyi` & `tigeropen-2.3.7/tigeropen/push/pb/TradeTickData_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/pb/util.py` & `tigeropen-2.3.7/tigeropen/push/pb/util.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/protobuf_push_client.py` & `tigeropen-2.3.7/tigeropen/push/protobuf_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/push_client.py` & `tigeropen-2.3.7/tigeropen/push/push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/push/stomp_push_client.py` & `tigeropen-2.3.7/tigeropen/push/stomp_push_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/domain/filter.py` & `tigeropen-2.3.7/tigeropen/quote/domain/filter.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/domain/quote_brief.py` & `tigeropen-2.3.7/tigeropen/quote/domain/quote_brief.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/domain/stock_broker.py` & `tigeropen-2.3.7/tigeropen/quote/domain/stock_broker.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/quote_client.py` & `tigeropen-2.3.7/tigeropen/quote/quote_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/request/model.py` & `tigeropen-2.3.7/tigeropen/quote/request/model.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/capital_distribution_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/capital_distribution_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/capital_flow_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/capital_flow_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/future_briefs_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/future_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/future_contract_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/future_contract_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/future_exchange_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/future_exchange_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/future_quote_bar_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/future_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/future_quote_ticks_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/future_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/future_trading_times_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/future_trading_times_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/market_scanner_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/market_scanner_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/market_status_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/market_status_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/option_briefs_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/option_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/option_chains_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/option_chains_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/option_expirations_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/option_expirations_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/option_quote_bar_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/option_quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/option_quote_ticks_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/option_quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_bar_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_bar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_brief_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_brief_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_delay_briefs_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_delay_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_depth_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_depth_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_grab_permission_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_grab_permission_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_hour_trading_timeline_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_hour_trading_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_ticks_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_ticks_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_history_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_history_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/quote_timeline_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/quote_timeline_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/stock_briefs_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/stock_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/stock_broker_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/stock_broker_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/stock_details_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/stock_details_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/stock_short_interest_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/stock_short_interest_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/stock_trade_meta_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/stock_trade_meta_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/symbol_names_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/symbol_names_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/symbols_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/symbols_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/trading_calendar_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/trading_calendar_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/warrant_briefs_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/warrant_briefs_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/quote/response/warrant_filter_response.py` & `tigeropen-2.3.7/tigeropen/quote/response/warrant_filter_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/tiger_open_client.py` & `tigeropen-2.3.7/tigeropen/tiger_open_client.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/tiger_open_config.py` & `tigeropen-2.3.7/tigeropen/tiger_open_config.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/domain/account.py` & `tigeropen-2.3.7/tigeropen/trade/domain/account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/domain/contract.py` & `tigeropen-2.3.7/tigeropen/trade/domain/contract.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/domain/order.py` & `tigeropen-2.3.7/tigeropen/trade/domain/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class Order:
     __slots__ = ["account", "id", "order_id", "parent_id", "order_time", "reason", "trade_time", "contract", "action",
                  "quantity", "filled", "_remaining", "avg_fill_price", "commission", "realized_pnl", "_status",
                  "trail_stop_price", "limit_price", "aux_price", "trailing_percent", "percent_offset", "action",
                  "order_type", "time_in_force", "outside_rth", "order_legs", "algo_params", "algo_strategy",
                  "secret_key", "liquidation", "discount", "attr_desc", "source", 'adjust_limit', 'sub_ids', "user_mark",
-                 "update_time", "expire_time", "can_modify"]
+                 "update_time", "expire_time", "can_modify", "external_id"]
 
     def __init__(self, account, contract, action, order_type, quantity, limit_price=None, aux_price=None,
                  trail_stop_price=None, trailing_percent=None, percent_offset=None, time_in_force=None,
                  outside_rth=None, filled=0, avg_fill_price=0, commission=None, realized_pnl=None,
                  id=None, order_id=None, parent_id=None, order_time=None, trade_time=None, order_legs=None,
                  algo_params=None, secret_key=None, **kwargs):
         """
@@ -97,14 +97,15 @@
         self.attr_desc = kwargs.get('attr_desc')
         self.source = kwargs.get('source')
         self.adjust_limit = kwargs.get('adjust_limit')
         self.sub_ids = kwargs.get('sub_ids')
         self.user_mark = kwargs.get('user_mark')
         self.expire_time = kwargs.get('expire_time')
         self.can_modify = kwargs.get('can_modify')
+        self.external_id = kwargs.get('external_id')
 
     def to_dict(self):
         dct = {name: getattr(self, name) for name in self.__slots__ if name not in ORDER_FIELDS_TO_IGNORE}
 
         dct['contract'] = self.contract
         if self.status:
             dct['status'] = self.status.name
```

### Comparing `tigeropen-2.3.6/tigeropen/trade/domain/position.py` & `tigeropen-2.3.7/tigeropen/trade/domain/position.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 @author: gaoan
 """
 
 
 class Position:
     def __init__(self, account, contract, quantity=0, average_cost=None, market_price=None, market_value=None,
-                 realized_pnl=None, unrealized_pnl=None):
+                 realized_pnl=None, unrealized_pnl=None, saleable=None, position_scale=None):
         """
         - account: 对应的账户ID
         - contract: 合约对象
         - quantity: 合约数量
         - average_cost: 含佣金的平均成本
         - market_price: 市价
         - market_value: 市值
@@ -23,14 +23,16 @@
         self.contract = contract
         self.quantity = quantity
         self.average_cost = average_cost
         self.market_price = market_price
         self.market_value = market_value
         self.realized_pnl = realized_pnl
         self.unrealized_pnl = unrealized_pnl
+        self.saleable = saleable
+        self.position_scale = position_scale
     
     def __repr__(self):
         template = "contract: {contract}, quantity: {quantity}, average_cost: {average_cost}, " \
                    "market_price: {market_price}"
         return template.format(
             contract=self.contract,
             quantity=self.quantity,
@@ -48,7 +50,18 @@
         """
         return {
             'contract': self.contract,
             'quantity': self.quantity,
             'average_cost': self.average_cost,
             'market_price': self.market_price
         }
+
+
+class TradableQuantityItem:
+    def __init__(self, tradable_quantity=0, financing_quantity=0, position_quantity=0, tradable_position_quantity=0):
+        self.tradable_quantity = tradable_quantity
+        self.financing_quantity = financing_quantity
+        self.position_quantity = position_quantity
+        self.tradable_position_quantity = tradable_position_quantity
+
+    def __repr__(self):
+        return 'TradableQuantityItem<{0}>'.format(self.__dict__)
```

### Comparing `tigeropen-2.3.6/tigeropen/trade/domain/prime_account.py` & `tigeropen-2.3.7/tigeropen/trade/domain/prime_account.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/request/model.py` & `tigeropen-2.3.7/tigeropen/trade/request/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1222,8 +1222,114 @@
             params['target_currency'] = self.target_currency
         if self.seg_type:
             params['seg_type'] = self.seg_type
         if self.external_id:
             params['external_id'] = self.external_id
         if self.time_in_force:
             params['time_in_force'] = self.time_in_force
-        return params
+        return params
+
+
+class EstimateTradableQuantityModel(BaseParams):
+    def __init__(self):
+        super().__init__()
+        self._account = None
+        self._secret_key = None
+        self._contract = None
+        self._seg_type = None
+        self._action = None
+        self._order_type = None
+        self._limit_price = None
+        self._stop_price = None
+
+    @property
+    def account(self):
+        return self._account
+
+    @account.setter
+    def account(self, value):
+        self._account = value
+
+    @property
+    def secret_key(self):
+        return self._secret_key
+
+    @secret_key.setter
+    def secret_key(self, value):
+        self._secret_key = value
+
+    @property
+    def contract(self):
+        return self._contract
+
+    @contract.setter
+    def contract(self, value):
+        self._contract = value
+
+    @property
+    def seg_type(self):
+        return self._seg_type
+
+    @seg_type.setter
+    def seg_type(self, value):
+        self._seg_type = value
+
+    @property
+    def action(self):
+        return self._action
+
+    @action.setter
+    def action(self, value):
+        self._action = value
+
+    @property
+    def order_type(self):
+        return self._order_type
+
+    @order_type.setter
+    def order_type(self, value):
+        self._order_type = value
+
+    @property
+    def limit_price(self):
+        return self._limit_price
+
+    @limit_price.setter
+    def limit_price(self, value):
+        self._limit_price = value
+
+    @property
+    def stop_price(self):
+        return self._stop_price
+
+    @stop_price.setter
+    def stop_price(self, value):
+        self._stop_price = value
+
+    def to_openapi_dict(self):
+        params = super().to_openapi_dict()
+        if self.account:
+            params['account'] = self.account
+        if self.secret_key:
+            params['secret_key'] = self.secret_key
+        if self.contract:
+            if self.contract.symbol:
+                params['symbol'] = self.contract.symbol
+            if self.contract.expiry:
+                params['expiry'] = self.contract.expiry
+            if self.contract.strike:
+                params['strike'] = self.contract.strike
+            if self.contract.put_call:
+                params['right'] = self.contract.put_call
+            if self.contract.sec_type:
+                params['sec_type'] = self.contract.sec_type
+        if self.seg_type:
+            params['seg_type'] = self.seg_type
+        if self.action:
+            params['action'] = self.action
+        if self.order_type:
+            params['order_type'] = self.order_type
+        if self.limit_price:
+            params['limit_price'] = self.limit_price
+        if self.stop_price:
+            params['stop_price'] = self.stop_price
+        return params
```

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/__init__.py` & `tigeropen-2.3.7/tigeropen/trade/response/__init__.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/account_profile_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/account_profile_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/analytics_asset_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/analytics_asset_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/assets_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/contracts_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/contracts_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/forex_order_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/forex_order_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/order_id_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/order_id_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/order_preview_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/order_preview_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/orders_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/orders_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                         'remark': 'reason',
                         'localSymbol': 'local_symbol', 'originSymbol': 'origin_symbol', 'outsideRth': 'outside_rth',
                         'timeInForce': 'time_in_force', 'openTime': 'order_time', 'latestTime': 'trade_time',
                         'contractId': 'contract_id', 'algoStrategy': 'algo_strategy',
                         'trailStopPrice': 'trail_stop_price', 'trailingPercent': 'trailing_percent',
                         'percentOffset': 'percent_offset', 'identifier': 'identifier', 'algoParameters': 'algo_params',
                         'userMark': 'user_mark', 'updateTime': 'update_time', 'expireTime': 'expire_time',
-                        'canModify': 'can_modify'
+                        'canModify': 'can_modify', 'externalId': 'external_id',
                         }
 
 
 class OrdersResponse(TigerResponse):
     def __init__(self):
         super(OrdersResponse, self).__init__()
         self.orders = []
@@ -102,23 +102,24 @@
         liquidation = order_fields.get('liquidation')
         algo_strategy = order_fields.get('algo_strategy')
         discount = order_fields.get('discount')
         attr_desc = order_fields.get('attr_desc')
         source = order_fields.get('source')
         user_mark = order_fields.get('user_mark')
         can_modify = order_fields.get('can_modify')
+        external_id = order_fields.get('external_id')
 
         order = Order(account, contract, action, order_type, quantity, limit_price=limit_price, aux_price=aux_price,
                       trail_stop_price=trail_stop_price, trailing_percent=trailing_percent,
                       percent_offset=percent_offset, time_in_force=time_in_force, outside_rth=outside_rth,
                       filled=filled, avg_fill_price=avg_fill_price, commission=commission,
                       realized_pnl=realized_pnl, id=id_, order_id=order_id, parent_id=parent_id,
                       algo_params=algo_params, liquidation=liquidation, algo_strategy=algo_strategy, discount=discount,
                       attr_desc=attr_desc, source=source, user_mark=user_mark, expire_time=expire_time,
-                      can_modify=can_modify)
+                      can_modify=can_modify, external_id=external_id)
         if 'order_time' in order_fields:
             order.order_time = order_fields.get('order_time')
         if 'trade_time' in order_fields:
             order.trade_time = order_fields.get('trade_time')
         if 'update_time' in order_fields:
             order.update_time = order_fields.get('update_time')
         if 'reason' in order_fields:
```

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/positions_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/positions_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,22 +3,24 @@
 Created on 2018/10/31
 
 @author: gaoan
 """
 import json
 
 from tigeropen.common.response import TigerResponse
+from tigeropen.common.util import string_utils
 from tigeropen.trade.domain.contract import Contract
-from tigeropen.trade.domain.position import Position
+from tigeropen.trade.domain.position import Position, TradableQuantityItem
 from tigeropen.trade.response import CONTRACT_FIELDS
 
 POSITION_FIELD_MAPPINGS = {'averageCost': 'average_cost', 'position': 'quantity', 'latestPrice': 'market_price',
                            'marketValue': 'market_value', 'orderType': 'order_type', 'realizedPnl': 'realized_pnl',
                            'unrealizedPnl': 'unrealized_pnl', 'secType': 'sec_type', 'localSymbol': 'local_symbol',
-                           'originSymbol': 'origin_symbol', 'contractId': 'contract_id', 'identifier': 'identifier'}
+                           'originSymbol': 'origin_symbol', 'contractId': 'contract_id', 'identifier': 'identifier',
+                           'salable': 'saleable', 'positionScale': 'position_scale'}
 
 
 class PositionsResponse(TigerResponse):
     def __init__(self):
         super(PositionsResponse, self).__init__()
         self.positions = []
         self._is_success = None
@@ -62,12 +64,30 @@
                     account = position_fields.get('account')
                     quantity = position_fields.get('quantity')
                     average_cost = position_fields.get('average_cost')
                     market_price = position_fields.get('market_price')
                     market_value = position_fields.get('market_value')
                     realized_pnl = position_fields.get('realized_pnl')
                     unrealized_pnl = position_fields.get('unrealized_pnl')
-                    
+                    saleable = position_fields.get('saleable')
+                    position_scale = position_fields.get('position_scale')
                     position = Position(account, contract, quantity, average_cost=average_cost,
                                         market_price=market_price, market_value=market_value,
-                                        realized_pnl=realized_pnl, unrealized_pnl=unrealized_pnl)
+                                        realized_pnl=realized_pnl, unrealized_pnl=unrealized_pnl,
+                                        saleable=saleable, position_scale=position_scale)
                     self.positions.append(position)
+
+
+class EstimateTradableQuantityResponse(TigerResponse):
+    def __init__(self):
+        super(EstimateTradableQuantityResponse, self).__init__()
+        self.result = None
+        self._is_success = None
+
+    def parse_response_content(self, response_content):
+        response = super(EstimateTradableQuantityResponse, self).parse_response_content(response_content)
+        if 'is_success' in response:
+            self._is_success = response['is_success']
+
+        if self.data:
+            data_json = json.loads(self.data)
+            self.result = TradableQuantityItem(**string_utils.camel_to_underline_obj(data_json))
```

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/prime_assets_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/prime_assets_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/segment_fund_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/segment_fund_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/response/transactions_response.py` & `tigeropen-2.3.7/tigeropen/trade/response/transactions_response.py`

 * *Files identical despite different names*

### Comparing `tigeropen-2.3.6/tigeropen/trade/trade_client.py` & `tigeropen-2.3.7/tigeropen/trade/trade_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,33 +6,33 @@
 """
 import logging
 
 from tigeropen.common.consts import THREAD_LOCAL, SecurityType, Market, Currency, Language, OPEN_API_SERVICE_VERSION_V3
 from tigeropen.common.consts.service_types import CONTRACTS, ACCOUNTS, POSITIONS, ASSETS, ORDERS, ORDER_NO, \
     CANCEL_ORDER, MODIFY_ORDER, PLACE_ORDER, ACTIVE_ORDERS, INACTIVE_ORDERS, FILLED_ORDERS, CONTRACT, PREVIEW_ORDER, \
     PRIME_ASSETS, ORDER_TRANSACTIONS, QUOTE_CONTRACT, ANALYTICS_ASSET, SEGMENT_FUND_AVAILABLE, SEGMENT_FUND_HISTORY, \
-    TRANSFER_SEGMENT_FUND, CANCEL_SEGMENT_FUND, PLACE_FOREX_ORDER
+    TRANSFER_SEGMENT_FUND, CANCEL_SEGMENT_FUND, PLACE_FOREX_ORDER, ESTIMATE_TRADABLE_QUANTITY
 from tigeropen.common.exceptions import ApiException
 from tigeropen.common.util.common_utils import get_enum_value, date_str_to_timestamp
 from tigeropen.common.request import OpenApiRequest
 from tigeropen.tiger_open_client import TigerOpenClient
 from tigeropen.tiger_open_config import LANGUAGE
 from tigeropen.trade.domain.order import Order
 from tigeropen.trade.request.model import ContractParams, AccountsParams, AssetParams, PositionParams, OrdersParams, \
     OrderParams, PlaceModifyOrderParams, CancelOrderParams, TransactionsParams, AnalyticsAssetParams, SegmentFundParams, \
-    ForexTradeOrderParams
+    ForexTradeOrderParams, EstimateTradableQuantityModel
 from tigeropen.trade.response.account_profile_response import ProfilesResponse
 from tigeropen.trade.response.analytics_asset_response import AnalyticsAssetResponse
 from tigeropen.trade.response.assets_response import AssetsResponse
 from tigeropen.trade.response.contracts_response import ContractsResponse
 from tigeropen.trade.response.forex_order_response import ForexOrderResponse
 from tigeropen.trade.response.order_id_response import OrderIdResponse
 from tigeropen.trade.response.order_preview_response import PreviewOrderResponse
 from tigeropen.trade.response.orders_response import OrdersResponse
-from tigeropen.trade.response.positions_response import PositionsResponse
+from tigeropen.trade.response.positions_response import PositionsResponse, EstimateTradableQuantityResponse
 from tigeropen.trade.response.prime_assets_response import PrimeAssetsResponse
 from tigeropen.trade.response.segment_fund_response import SegmentFundAvailableResponse, \
     SegmentFundHistoryResponse, SegmentFundCancelResponse
 from tigeropen.trade.response.segment_fund_response import SegmentFundTransferResponse
 from tigeropen.trade.response.transactions_response import TransactionsResponse
 
 
@@ -851,14 +851,37 @@
             response.parse_response_content(response_content)
             if response.is_success():
                 return response.data
             else:
                 raise ApiException(response.code, response.message)
         return None
 
+    def get_estimate_tradable_quantity(self, order, seg_type=None):
+        params = EstimateTradableQuantityModel()
+        params.account = self._account
+        params.secret_key = self._secret_key
+        params.lang = get_enum_value(self._lang)
+        params.contract = order.contract
+        params.order_type = order.order_type
+        params.action = order.action
+        params.limit_price = order.limit_price
+        params.stop_price = order.aux_price
+        params.seg_type = get_enum_value(seg_type)
+
+        request = OpenApiRequest(ESTIMATE_TRADABLE_QUANTITY, biz_model=params)
+        response_content = self.__fetch_data(request)
+        if response_content:
+            response = EstimateTradableQuantityResponse()
+            response.parse_response_content(response_content)
+            if response.is_success():
+                return response.result
+            else:
+                raise ApiException(response.code, response.message)
+        return None
+
     def __fetch_data(self, request):
         try:
             response = super(TradeClient, self).execute(request)
             return response
         except Exception as e:
             if THREAD_LOCAL.logger:
                 THREAD_LOCAL.logger.error(e, exc_info=True)
```

### Comparing `tigeropen-2.3.6/tigeropen.egg-info/PKG-INFO` & `tigeropen-2.3.7/tigeropen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: tigeropen
-Version: 2.3.6
+Version: 2.3.7
 Summary: TigerBrokers Open API
 Home-page: https://github.com/tigerbrokers/openapi-python-sdk
 Author: TigerBrokers
 Author-email: openapi@tigerbrokers.com
 License: Apache License v2
 Platform: any
 Classifier: Programming Language :: Python
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: Unix
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
```

### Comparing `tigeropen-2.3.6/tigeropen.egg-info/SOURCES.txt` & `tigeropen-2.3.7/tigeropen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

