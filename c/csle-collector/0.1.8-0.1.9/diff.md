# Comparing `tmp/csle_collector-0.1.8.tar.gz` & `tmp/csle_collector-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csle_collector-0.1.8.tar", last modified: Mon Mar 20 15:26:37 2023, max compression
+gzip compressed data, was "csle_collector-0.1.9.tar", last modified: Tue Mar 21 08:09:08 2023, max compression
```

## Comparing `csle_collector-0.1.8.tar` & `csle_collector-0.1.9.tar`

### file list

```diff
@@ -1,92 +1,92 @@
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.217188 csle_collector-0.1.8/
--rw-r--r--   0 kimham     (501) staff       (20)      803 2023-03-20 15:26:37.217312 csle_collector-0.1.8/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     5807 2023-03-05 07:26:30.000000 csle_collector-0.1.8/README.md
--rw-r--r--   0 kimham     (501) staff       (20)      674 2023-02-12 08:59:32.000000 csle_collector-0.1.8/pyproject.toml
--rw-r--r--   0 kimham     (501) staff       (20)     1454 2023-03-20 15:26:37.217878 csle_collector-0.1.8/setup.cfg
--rw-r--r--   0 kimham     (501) staff       (20)       69 2022-11-28 13:00:49.000000 csle_collector-0.1.8/setup.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.176883 csle_collector-0.1.8/src/
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.180409 csle_collector-0.1.8/src/csle_collector/
--rw-r--r--   0 kimham     (501) staff       (20)       37 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)       22 2023-03-20 15:26:11.000000 csle_collector-0.1.8/src/csle_collector/__version__.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.186931 csle_collector-0.1.8/src/csle_collector/client_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/client_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    16588 2023-03-20 15:23:29.000000 csle_collector-0.1.8/src/csle_collector/client_manager/client_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4671 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/client_manager/client_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8592 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/client_manager/client_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     2179 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/client_manager/client_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3633 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/client_manager/client_population_metrics.py
--rw-r--r--   0 kimham     (501) staff       (20)     4292 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/client_manager/query_clients.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.187617 csle_collector-0.1.8/src/csle_collector/constants/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/constants/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    33168 2023-03-20 14:07:19.000000 csle_collector-0.1.8/src/csle_collector/constants/constants.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.192445 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2023-02-12 12:41:34.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    12394 2023-03-15 11:36:56.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats.py
--rw-r--r--   0 kimham     (501) staff       (20)    13540 2023-03-05 11:13:10.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4589 2023-02-12 12:41:34.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     6193 2023-02-12 12:41:34.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     8801 2023-02-12 12:41:34.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3994 2023-03-20 09:39:38.000000 csle_collector-0.1.8/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.195547 csle_collector-0.1.8/src/csle_collector/elk_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/elk_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)    10730 2023-03-20 15:23:29.000000 csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     5923 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    14300 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1540 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     5768 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/elk_manager/query_elk_server.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.201065 csle_collector-0.1.8/src/csle_collector/host_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/host_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)      875 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/host_manager/failed_login_attempt.py
--rw-r--r--   0 kimham     (501) staff       (20)    59894 2023-03-20 15:23:53.000000 csle_collector-0.1.8/src/csle_collector/host_manager/host_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)    12978 2022-12-07 07:23:42.000000 csle_collector-0.1.8/src/csle_collector/host_manager/host_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    25786 2022-12-07 07:23:42.000000 csle_collector-0.1.8/src/csle_collector/host_manager/host_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    33850 2023-03-05 07:26:30.000000 csle_collector-0.1.8/src/csle_collector/host_manager/host_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     7783 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/host_manager/host_metrics.py
--rw-r--r--   0 kimham     (501) staff       (20)    15344 2022-12-07 07:23:42.000000 csle_collector-0.1.8/src/csle_collector/host_manager/query_host_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     1292 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/host_manager/successful_login.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.203155 csle_collector-0.1.8/src/csle_collector/kafka_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/kafka_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     6606 2023-03-20 15:24:02.000000 csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4116 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8484 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1442 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     3233 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/kafka_manager/query_kafka_server.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.206795 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2931 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
--rw-r--r--   0 kimham     (501) staff       (20)    10847 2023-03-16 08:28:05.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)    11376 2023-03-20 15:24:15.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7479 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    13329 2022-11-30 17:44:15.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
--rw-r--r--   0 kimham     (501) staff       (20)     5377 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.210579 csle_collector-0.1.8/src/csle_collector/ryu_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/ryu_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     3936 2022-12-07 13:13:59.000000 csle_collector-0.1.8/src/csle_collector/ryu_manager/query_ryu_server.py
--rw-r--r--   0 kimham     (501) staff       (20)    12104 2023-03-20 15:24:25.000000 csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     4363 2022-12-07 08:23:15.000000 csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     8368 2022-12-07 08:23:40.000000 csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     2086 2022-12-07 08:18:55.000000 csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.214057 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     5390 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7053 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_alert.py
--rw-r--r--   0 kimham     (501) staff       (20)    11754 2023-03-16 08:28:38.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
--rw-r--r--   0 kimham     (501) staff       (20)    11533 2023-03-20 15:25:13.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     8152 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)    10801 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)    15997 2022-11-30 17:44:15.000000 csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.216852 csle_collector-0.1.8/src/csle_collector/traffic_manager/
--rw-r--r--   0 kimham     (501) staff       (20)        0 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/traffic_manager/__init__.py
--rw-r--r--   0 kimham     (501) staff       (20)     2534 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/traffic_manager/query_traffic_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     7482 2023-03-20 15:22:56.000000 csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager.py
--rw-r--r--   0 kimham     (501) staff       (20)     3087 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager_pb2.py
--rw-r--r--   0 kimham     (501) staff       (20)     5596 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
--rw-r--r--   0 kimham     (501) staff       (20)     1477 2022-11-28 13:00:49.000000 csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager_util.py
-drwxr-xr-x   0 kimham     (501) staff       (20)        0 2023-03-20 15:26:37.182770 csle_collector-0.1.8/src/csle_collector.egg-info/
--rw-r--r--   0 kimham     (501) staff       (20)      803 2023-03-20 15:26:36.000000 csle_collector-0.1.8/src/csle_collector.egg-info/PKG-INFO
--rw-r--r--   0 kimham     (501) staff       (20)     3954 2023-03-20 15:26:37.000000 csle_collector-0.1.8/src/csle_collector.egg-info/SOURCES.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2023-03-20 15:26:36.000000 csle_collector-0.1.8/src/csle_collector.egg-info/dependency_links.txt
--rw-r--r--   0 kimham     (501) staff       (20)        1 2022-11-29 18:03:14.000000 csle_collector-0.1.8/src/csle_collector.egg-info/not-zip-safe
--rw-r--r--   0 kimham     (501) staff       (20)      293 2023-03-20 15:26:37.000000 csle_collector-0.1.8/src/csle_collector.egg-info/requires.txt
--rw-r--r--   0 kimham     (501) staff       (20)       15 2023-03-20 15:26:37.000000 csle_collector-0.1.8/src/csle_collector.egg-info/top_level.txt
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.025203 csle_collector-0.1.9/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-03-21 08:09:08.025203 csle_collector-0.1.9/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5807 2023-03-04 17:48:16.000000 csle_collector-0.1.9/README.md
+-rw-rw-r--   0 kim       (1000) kim       (1000)      674 2023-02-11 20:28:41.000000 csle_collector-0.1.9/pyproject.toml
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1454 2023-03-21 08:09:08.025203 csle_collector-0.1.9/setup.cfg
+-rw-rw-r--   0 kim       (1000) kim       (1000)       69 2022-11-28 13:03:16.000000 csle_collector-0.1.9/setup.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.009203 csle_collector-0.1.9/src/
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.009203 csle_collector-0.1.9/src/csle_collector/
+-rw-rw-r--   0 kim       (1000) kim       (1000)       37 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)       22 2023-03-21 08:08:55.000000 csle_collector-0.1.9/src/csle_collector/__version__.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector/client_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    16588 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4671 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8592 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2179 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3633 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/client_population_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4292 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/client_manager/query_clients.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector/constants/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/constants/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33268 2023-03-21 07:35:53.000000 csle_collector-0.1.9/src/csle_collector/constants/constants.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12394 2023-03-17 07:49:22.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13540 2023-03-06 06:25:37.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4589 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6193 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8801 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3994 2023-03-17 14:04:50.000000 csle_collector-0.1.9/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.017203 csle_collector-0.1.9/src/csle_collector/elk_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10730 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5923 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    14300 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1540 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5768 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/elk_manager/query_elk_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.017203 csle_collector-0.1.9/src/csle_collector/host_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)      875 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/failed_login_attempt.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    60179 2023-03-21 07:55:28.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12978 2022-12-02 11:02:24.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    25786 2022-12-02 11:02:35.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    33850 2023-03-04 10:28:54.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7783 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/host_metrics.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15344 2022-12-02 15:50:47.000000 csle_collector-0.1.9/src/csle_collector/host_manager/query_host_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1292 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/host_manager/successful_login.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.017203 csle_collector-0.1.9/src/csle_collector/kafka_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     6606 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4116 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8484 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1442 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3233 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/kafka_manager/query_kafka_server.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.021203 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2931 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10847 2023-03-17 07:49:22.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11376 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7479 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    13329 2022-12-01 06:44:23.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5377 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.021203 csle_collector-0.1.9/src/csle_collector/ryu_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3936 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/query_ryu_server.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    12104 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     4363 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8368 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2086 2022-12-11 08:32:31.000000 csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.021203 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5390 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7053 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11754 2023-03-17 07:49:22.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    11533 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     8152 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    10801 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)    15997 2022-12-01 06:44:23.000000 csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.025203 csle_collector-0.1.9/src/csle_collector/traffic_manager/
+-rw-rw-r--   0 kim       (1000) kim       (1000)        0 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/__init__.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     2534 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/query_traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     7482 2023-03-21 06:33:58.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3087 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     5596 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py
+-rw-rw-r--   0 kim       (1000) kim       (1000)     1477 2022-11-28 13:03:16.000000 csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_util.py
+drwxrwxr-x   0 kim       (1000) kim       (1000)        0 2023-03-21 08:09:08.013203 csle_collector-0.1.9/src/csle_collector.egg-info/
+-rw-rw-r--   0 kim       (1000) kim       (1000)      803 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/PKG-INFO
+-rw-rw-r--   0 kim       (1000) kim       (1000)     3954 2023-03-21 08:09:08.000000 csle_collector-0.1.9/src/csle_collector.egg-info/SOURCES.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/dependency_links.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)        1 2022-11-28 13:35:37.000000 csle_collector-0.1.9/src/csle_collector.egg-info/not-zip-safe
+-rw-rw-r--   0 kim       (1000) kim       (1000)      293 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/requires.txt
+-rw-rw-r--   0 kim       (1000) kim       (1000)       15 2023-03-21 08:09:07.000000 csle_collector-0.1.9/src/csle_collector.egg-info/top_level.txt
```

### Comparing `csle_collector-0.1.8/PKG-INFO` & `csle_collector-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle_collector
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.1.8/README.md` & `csle_collector-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/pyproject.toml` & `csle_collector-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/setup.cfg` & `csle_collector-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/client_manager/client_manager.py` & `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/client_manager/client_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/client_manager/client_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/client_manager/client_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/client_manager/client_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/client_manager/client_population_metrics.py` & `csle_collector-0.1.9/src/csle_collector/client_manager/client_population_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/client_manager/query_clients.py` & `csle_collector-0.1.9/src/csle_collector/client_manager/query_clients.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/constants/constants.py` & `csle_collector-0.1.9/src/csle_collector/constants/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -238,14 +238,15 @@
     CLIENT_MANAGER_LOG_FILE = "client_manager.log"
     CLIENT_MANAGER_LOG_DIR = "/"
     TRAFFIC_MANAGER_LOG_FILE = "traffic_manager.log"
     TRAFFIC_MANAGER_LOG_DIR = "/"
     KAFKA_LOG_FILE = "/usr/local/kafka/logs/server.log"
     RYU_MANAGER_LOG_FILE = "ryu_manager.log"
     RYU_MANAGER_LOG_DIR = "/"
+    DEFAULT_LOG_FILE_PATHS = ["/*.log", "/var/log/*.log", "/var/log/*/*.log", "/var/log/*/*/*.log"]
 
 
 class MANAGER_PORTS:
     """
     Constants related to the ports of managers
     """
     TRAFFIC_MANAGER_DEFAULT_PORT = 50043
```

### Comparing `csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats.py` & `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_manager.py` & `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/docker_stats_manager/docker_stats_util.py` & `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/docker_stats_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py` & `csle_collector-0.1.9/src/csle_collector/docker_stats_manager/query_docker_stats_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager.py` & `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/elk_manager/elk_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/elk_manager/elk_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/elk_manager/query_elk_server.py` & `csle_collector-0.1.9/src/csle_collector/elk_manager/query_elk_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/failed_login_attempt.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/failed_login_attempt.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/host_manager.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,21 +51,26 @@
         Main loop of the thread. Parses log files and metrics on the host and pushes it to Kafka periodically
 
         :return: None
         """
         logging.info("HostMonitor [Running]")
         while self.running:
             time.sleep(self.time_step_len_seconds)
-            host_metrics = HostManagerUtil.read_host_metrics(failed_auth_last_ts=self.failed_auth_last_ts,
-                                                             login_last_ts=self.login_last_ts)
-            record = host_metrics.to_kafka_record(ip=self.ip)
-            self.producer.produce(constants.KAFKA_CONFIG.HOST_METRICS_TOPIC_NAME, record)
-            self.producer.poll(0)
-            self.failed_auth_last_ts = HostManagerUtil.read_latest_ts_auth()
-            self.login_last_ts = HostManagerUtil.read_latest_ts_login()
+            try:
+                host_metrics = HostManagerUtil.read_host_metrics(failed_auth_last_ts=self.failed_auth_last_ts,
+                                                                 login_last_ts=self.login_last_ts)
+                record = host_metrics.to_kafka_record(ip=self.ip)
+                self.producer.produce(constants.KAFKA_CONFIG.HOST_METRICS_TOPIC_NAME, record)
+                self.producer.poll(0)
+                self.failed_auth_last_ts = HostManagerUtil.read_latest_ts_auth()
+                self.login_last_ts = HostManagerUtil.read_latest_ts_login()
+            except Exception as e:
+                logging.info(f"[Monitor thread], "
+                             f"There was an exception reading host metrics and producing to kafka: "
+                             f"{str(e)}, {repr(e)}")
 
 
 class HostManagerServicer(csle_collector.host_manager.host_manager_pb2_grpc.HostManagerServicer):
     """
     gRPC server for collecting Host statistics.
     """
```

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/host_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/host_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/host_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/host_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/host_metrics.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/host_metrics.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/query_host_manager.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/query_host_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/host_manager/successful_login.py` & `csle_collector-0.1.9/src/csle_collector/host_manager/successful_login.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager.py` & `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/kafka_manager/kafka_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/kafka_manager/kafka_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/kafka_manager/query_kafka_server.py` & `csle_collector-0.1.9/src/csle_collector/kafka_manager/query_kafka_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/ossec_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py` & `csle_collector-0.1.9/src/csle_collector/ossec_ids_manager/query_ossec_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ryu_manager/query_ryu_server.py` & `csle_collector-0.1.9/src/csle_collector/ryu_manager/query_ryu_server.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager.py` & `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/ryu_manager/ryu_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/ryu_manager/ryu_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/query_snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_alert.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_alert_counters.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/snort_ids_manager/snort_ids_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/traffic_manager/query_traffic_manager.py` & `csle_collector-0.1.9/src/csle_collector/traffic_manager/query_traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager.py` & `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager_pb2.py` & `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py` & `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector/traffic_manager/traffic_manager_util.py` & `csle_collector-0.1.9/src/csle_collector/traffic_manager/traffic_manager_util.py`

 * *Files identical despite different names*

### Comparing `csle_collector-0.1.8/src/csle_collector.egg-info/PKG-INFO` & `csle_collector-0.1.9/src/csle_collector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csle-collector
-Version: 0.1.8
+Version: 0.1.9
 Summary: Scripts for data collection in CSLE
 Author: Kim Hammar
 Author-email: hammar.kim@gmail.com
 License: Creative Commons Attribution-ShareAlike 4.0 International
 Keywords: Reinforcement-Learning Cyber-Security Markov-Games Markov-Decision-Processes
 Platform: unix
 Platform: linux
```

### Comparing `csle_collector-0.1.8/src/csle_collector.egg-info/SOURCES.txt` & `csle_collector-0.1.9/src/csle_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

