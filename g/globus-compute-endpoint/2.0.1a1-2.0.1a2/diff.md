# Comparing `tmp/globus-compute-endpoint-2.0.1a1.tar.gz` & `tmp/globus-compute-endpoint-2.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "globus-compute-endpoint-2.0.1a1.tar", last modified: Mon Apr 17 19:01:13 2023, max compression
+gzip compressed data, was "globus-compute-endpoint-2.0.1a2.tar", last modified: Tue Apr 18 21:51:21 2023, max compression
```

## Comparing `globus-compute-endpoint-2.0.1a1.tar` & `globus-compute-endpoint-2.0.1a2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.176264 globus-compute-endpoint-2.0.1a1/
--rw-r--r--   0 chris      (501) staff       (20)    11330 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/LICENSE
--rw-r--r--   0 chris      (501) staff       (20)       16 2023-04-17 18:57:51.000000 globus-compute-endpoint-2.0.1a1/MANIFEST.in
--rw-r--r--   0 chris      (501) staff       (20)     1646 2023-04-17 19:01:13.176355 globus-compute-endpoint-2.0.1a1/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)      871 2023-04-17 18:38:33.000000 globus-compute-endpoint-2.0.1a1/PyPI.md
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.165547 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/
--rw-r--r--   0 chris      (501) staff       (20)      131 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    18802 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/cli.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.168805 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2895 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/config.py
--rw-r--r--   0 chris      (501) staff       (20)      772 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/default_config.py
--rw-r--r--   0 chris      (501) staff       (20)    26053 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint.py
--rw-r--r--   0 chris      (501) staff       (20)    19658 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint_manager.py
--rw-r--r--   0 chris      (501) staff       (20)    24955 2023-04-12 19:39:07.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/interchange.py
--rw-r--r--   0 chris      (501) staff       (20)     2773 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/messages_compat.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.169844 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/
--rw-r--r--   0 chris      (501) staff       (20)      307 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)      689 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py
--rw-r--r--   0 chris      (501) staff       (20)    11834 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
--rw-r--r--   0 chris      (501) staff       (20)     3068 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
--rw-r--r--   0 chris      (501) staff       (20)    14076 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
--rw-r--r--   0 chris      (501) staff       (20)     5184 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/result_store.py
--rw-r--r--   0 chris      (501) staff       (20)     7275 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/taskqueue.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.170257 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/
--rw-r--r--   0 chris      (501) staff       (20)     1017 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     6026 2023-04-13 15:26:40.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/config.py
--rw-r--r--   0 chris      (501) staff       (20)     1834 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/exception_handling.py
--rw-r--r--   0 chris      (501) staff       (20)      220 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/exceptions.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.170457 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/
--rw-r--r--   0 chris      (501) staff       (20)      141 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.173398 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2104 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/container_sched.py
--rw-r--r--   0 chris      (501) staff       (20)    34995 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/executor.py
--rw-r--r--   0 chris      (501) staff       (20)    48886 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange.py
--rw-r--r--   0 chris      (501) staff       (20)     9712 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
--rw-r--r--   0 chris      (501) staff       (20)      267 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
--rwxr-xr-x   0 chris      (501) staff       (20)    35860 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/manager.py
--rw-r--r--   0 chris      (501) staff       (20)     9114 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/messages.py
--rw-r--r--   0 chris      (501) staff       (20)     8401 2023-04-17 18:38:33.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker.py
--rw-r--r--   0 chris      (501) staff       (20)    18606 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker_map.py
--rw-r--r--   0 chris      (501) staff       (20)     5433 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
--rw-r--r--   0 chris      (501) staff       (20)     8219 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/logging_config.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.173695 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/
--rw-r--r--   0 chris      (501) staff       (20)      115 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/__init__.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.174298 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)    12874 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/kube.py
--rw-r--r--   0 chris      (501) staff       (20)       50 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/template.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.175416 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/
--rw-r--r--   0 chris      (501) staff       (20)      280 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     7018 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/base.py
--rw-r--r--   0 chris      (501) staff       (20)     5106 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/kube_simple.py
--rw-r--r--   0 chris      (501) staff       (20)     6145 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/simple.py
--rw-r--r--   0 chris      (501) staff       (20)     1610 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/test.py
--rw-r--r--   0 chris      (501) staff       (20)      806 2023-04-17 19:00:11.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/version.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.166460 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/
--rw-r--r--   0 chris      (501) staff       (20)     1646 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/PKG-INFO
--rw-r--r--   0 chris      (501) staff       (20)     2657 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/SOURCES.txt
--rw-r--r--   0 chris      (501) staff       (20)        1 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/dependency_links.txt
--rw-r--r--   0 chris      (501) staff       (20)      359 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/entry_points.txt
--rw-r--r--   0 chris      (501) staff       (20)      305 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/requires.txt
--rw-r--r--   0 chris      (501) staff       (20)       30 2023-04-17 19:01:13.000000 globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/top_level.txt
--rw-r--r--   0 chris      (501) staff       (20)      282 2023-04-17 19:01:13.176709 globus-compute-endpoint-2.0.1a1/setup.cfg
--rw-r--r--   0 chris      (501) staff       (20)     3384 2023-04-17 18:38:33.000000 globus-compute-endpoint-2.0.1a1/setup.py
-drwxr-xr-x   0 chris      (501) staff       (20)        0 2023-04-17 19:01:13.175990 globus-compute-endpoint-2.0.1a1/tests/
--rw-r--r--   0 chris      (501) staff       (20)        0 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/tests/__init__.py
--rw-r--r--   0 chris      (501) staff       (20)     2693 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/tests/conftest.py
--rw-r--r--   0 chris      (501) staff       (20)     2276 2023-04-12 14:51:48.000000 globus-compute-endpoint-2.0.1a1/tests/utils.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.891209 globus-compute-endpoint-2.0.1a2/
+-rw-r--r--   0 lei        (501) staff       (20)    11330 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/LICENSE
+-rw-r--r--   0 lei        (501) staff       (20)       16 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a2/MANIFEST.in
+-rw-r--r--   0 lei        (501) staff       (20)     1646 2023-04-18 21:51:21.891309 globus-compute-endpoint-2.0.1a2/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)      871 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a2/PyPI.md
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.875094 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)      131 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    18802 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/cli.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.877507 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2895 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/config.py
+-rw-r--r--   0 lei        (501) staff       (20)      772 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/default_config.py
+-rw-r--r--   0 lei        (501) staff       (20)    26053 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint.py
+-rw-r--r--   0 lei        (501) staff       (20)    19658 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint_manager.py
+-rw-r--r--   0 lei        (501) staff       (20)    25351 2023-04-18 19:39:56.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     2773 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/messages_compat.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.878262 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)      689 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/base.py
+-rw-r--r--   0 lei        (501) staff       (20)    11834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     3068 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py
+-rw-r--r--   0 lei        (501) staff       (20)    14076 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py
+-rw-r--r--   0 lei        (501) staff       (20)     5184 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/result_store.py
+-rw-r--r--   0 lei        (501) staff       (20)     7275 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/taskqueue.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.878549 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/
+-rw-r--r--   0 lei        (501) staff       (20)     1017 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     6026 2023-04-13 13:57:47.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/config.py
+-rw-r--r--   0 lei        (501) staff       (20)     1834 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/exception_handling.py
+-rw-r--r--   0 lei        (501) staff       (20)      220 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/exceptions.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.878692 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/
+-rw-r--r--   0 lei        (501) staff       (20)      141 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.889230 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2104 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/container_sched.py
+-rw-r--r--   0 lei        (501) staff       (20)    34995 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/executor.py
+-rw-r--r--   0 lei        (501) staff       (20)    48886 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange.py
+-rw-r--r--   0 lei        (501) staff       (20)     9712 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py
+-rw-r--r--   0 lei        (501) staff       (20)      267 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/mac_safe_queue.py
+-rwxr-xr-x   0 lei        (501) staff       (20)    35860 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/manager.py
+-rw-r--r--   0 lei        (501) staff       (20)     9114 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/messages.py
+-rw-r--r--   0 lei        (501) staff       (20)     8401 2023-04-14 16:35:15.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker.py
+-rw-r--r--   0 lei        (501) staff       (20)    18606 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker_map.py
+-rw-r--r--   0 lei        (501) staff       (20)     5433 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py
+-rw-r--r--   0 lei        (501) staff       (20)     8219 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/logging_config.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.889389 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/
+-rw-r--r--   0 lei        (501) staff       (20)      115 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/__init__.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.889855 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)    12874 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/kube.py
+-rw-r--r--   0 lei        (501) staff       (20)       50 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/template.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.890593 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/
+-rw-r--r--   0 lei        (501) staff       (20)      280 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     7018 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/base.py
+-rw-r--r--   0 lei        (501) staff       (20)     5106 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/kube_simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     6145 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/simple.py
+-rw-r--r--   0 lei        (501) staff       (20)     1610 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/test.py
+-rw-r--r--   0 lei        (501) staff       (20)      806 2023-04-18 21:17:41.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/version.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.875903 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/
+-rw-r--r--   0 lei        (501) staff       (20)     1646 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/PKG-INFO
+-rw-r--r--   0 lei        (501) staff       (20)     2657 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/SOURCES.txt
+-rw-r--r--   0 lei        (501) staff       (20)        1 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/dependency_links.txt
+-rw-r--r--   0 lei        (501) staff       (20)      359 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/entry_points.txt
+-rw-r--r--   0 lei        (501) staff       (20)      307 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/requires.txt
+-rw-r--r--   0 lei        (501) staff       (20)       30 2023-04-18 21:51:21.000000 globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/top_level.txt
+-rw-r--r--   0 lei        (501) staff       (20)      282 2023-04-18 21:51:21.891612 globus-compute-endpoint-2.0.1a2/setup.cfg
+-rw-r--r--   0 lei        (501) staff       (20)     3386 2023-04-18 21:17:41.000000 globus-compute-endpoint-2.0.1a2/setup.py
+drwxr-xr-x   0 lei        (501) staff       (20)        0 2023-04-18 21:51:21.891072 globus-compute-endpoint-2.0.1a2/tests/
+-rw-r--r--   0 lei        (501) staff       (20)        0 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/tests/__init__.py
+-rw-r--r--   0 lei        (501) staff       (20)     2693 2023-04-13 00:34:31.000000 globus-compute-endpoint-2.0.1a2/tests/conftest.py
+-rw-r--r--   0 lei        (501) staff       (20)     2276 2023-04-10 19:02:41.000000 globus-compute-endpoint-2.0.1a2/tests/utils.py
```

### Comparing `globus-compute-endpoint-2.0.1a1/LICENSE` & `globus-compute-endpoint-2.0.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/PKG-INFO` & `globus-compute-endpoint-2.0.1a2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a1
+Version: 2.0.1a2
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
@@ -19,10 +19,10 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # Globus Compute Endpoint
 
 [Globus Compute](https://globus-compute.readthedocs.io/en/latest/) is a distributed Function as a Service (FaaS) platform that enables flexible, scalable, and high performance remote function execution. Unlike centralized FaaS platforms, Globus Compute allows users to execute functions on heterogeneous remote computers, from laptops to campus clusters, clouds, and supercomputers.
 
-This package provides the [Compute Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which recieves user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing compute endpoints.
+This package provides the [Compute Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which receives user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing compute endpoints.
 
 To submit functions for execution on compute endpoints, use the companion [Globus Compute SDK](https://pypi.org/project/globus-compute-sdk/) package.
```

### Comparing `globus-compute-endpoint-2.0.1a1/PyPI.md` & `globus-compute-endpoint-2.0.1a2/PyPI.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 # Globus Compute Endpoint
 
 [Globus Compute](https://globus-compute.readthedocs.io/en/latest/) is a distributed Function as a Service (FaaS) platform that enables flexible, scalable, and high performance remote function execution. Unlike centralized FaaS platforms, Globus Compute allows users to execute functions on heterogeneous remote computers, from laptops to campus clusters, clouds, and supercomputers.
 
-This package provides the [Compute Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which recieves user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing compute endpoints.
+This package provides the [Compute Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which receives user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing compute endpoints.
 
 To submit functions for execution on compute endpoints, use the companion [Globus Compute SDK](https://pypi.org/project/globus-compute-sdk/) package.
```

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/cli.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/cli.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/config.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/default_config.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/default_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/endpoint_manager.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/interchange.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/interchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,18 +32,15 @@
     try_convert_to_messagepack,
 )
 from globus_compute_endpoint.endpoint.rabbit_mq import (
     ResultQueuePublisher,
     TaskQueueSubscriber,
 )
 from globus_compute_endpoint.endpoint.result_store import ResultStore
-from globus_compute_endpoint.exception_handling import (
-    get_error_string,
-    get_result_error_details,
-)
+from globus_compute_endpoint.exception_handling import get_result_error_details
 from globus_compute_endpoint.executors.high_throughput.mac_safe_queue import mpQueue
 from globus_compute_sdk import __version__ as funcx_sdk_version
 from parsl.version import VERSION as PARSL_VERSION
 
 log = logging.getLogger(__name__)
 
 
@@ -404,35 +401,44 @@
                     try:
                         task = convert_to_internaltask(task_msg, ctype)
                         executor.submit_raw(task)
                         num_tasks_forwarded += 1  # Safe given GIL
 
                     except Exception as exc:
                         log.exception(f"Failed to process {task_msg.task_id}")
-                        result = {
+                        code, msg = get_result_error_details()
+                        failed_result = Result(
+                            task_id=task_msg.task_id,
+                            data=f"Failed to start task: {exc}",
+                            error_details=ResultErrorDetails(
+                                code=code, user_message=msg
+                            ),
+                        )
+                        res = {
                             "task_id": task_msg.task_id,
-                            "exception": f"Failed to start task: {get_error_string()}",
-                            "error_details": get_result_error_details(),
-                            "message": f"Failed to start task.  Exception text: {exc}",
+                            "message": pack(failed_result),
                         }
-                        self.results_passthrough.put(result)
+                        self.results_passthrough.put(res)
 
                 log.debug("Exit process-pending-tasks thread.")
 
             def process_pending_results():
                 # Forward incoming results from the globus-compute-manager to the
                 # Globus Compute services. For graceful handling of shutdown
                 # (or "reboot"), wait up to a second or incoming results before
                 # iterating the loop regardless.
                 nonlocal num_results_forwarded
                 while not self._quiesce_event.is_set():
                     try:
                         result = self.results_passthrough.get(timeout=1)
-                        task_id = result["task_id"]
-                        packed_result = result["message"]
+                        task_id: str | None = result["task_id"]
+                        packed_result: bytes = result["message"]
+
+                        if not task_id:
+                            raise AssertionError("task_id: empty or None")
 
                     except queue.Empty:
                         # Empty queue!  Let's see if we have any prior results to send
                         continue
 
                     except Exception as exc:
                         log.warning(
@@ -448,17 +454,19 @@
 
                     except Exception as exc:
                         log.exception(
                             f"Unable to parse result message for task {task_id}."
                             "   Marking task as failed."
                         )
 
+                        err = f"[Task ID: {task_id}] ({exc.__class__.__name__}) {exc}"
+
                         kwargs = {
                             "task_id": task_id,
-                            "data": packed_result,
+                            "data": err,
                             "error_details": ResultErrorDetails(
                                 code=0,
                                 user_message=(
                                     "Endpoint failed to serialize."
                                     f"  Exception text: {exc}"
                                 ),
                             ),
```

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/messages_compat.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/messages_compat.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/base.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/command_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/result_queue_publisher.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/rabbit_mq/task_queue_subscriber.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/result_store.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/result_store.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/taskqueue.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/taskqueue.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/__init__.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/endpoint/utils/config.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/endpoint/utils/config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/exception_handling.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/exception_handling.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/container_sched.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/container_sched.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/executor.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/executor.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/interchange_task_dispatch.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/manager.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/manager.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/messages.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/messages.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/worker_map.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/worker_map.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/executors/high_throughput/zmq_pipes.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/logging_config.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/logging_config.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/providers/kubernetes/kube.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/providers/kubernetes/kube.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/base.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/base.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/kube_simple.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/kube_simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/simple.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/simple.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/strategies/test.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/strategies/test.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint/version.py` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # single source of truth for package version,
 # see https://packaging.python.org/en/latest/single_source_version/
-__version__ = "2.0.1a1"
+__version__ = "2.0.1a2"
 
 # TODO: remove after a `globus-compute-sdk` release
 # this is needed because it's imported by `globus-compute-sdk` to do the version check
 VERSION = __version__
 
 # Here as it's the easier way for funcx-endpoint cli to display it
 DEPRECATION_FUNCX_ENDPOINT = """
```

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/PKG-INFO` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: globus-compute-endpoint
-Version: 2.0.1a1
+Version: 2.0.1a2
 Summary: Globus Compute: High Performance Function Serving for Science
 Home-page: https://github.com/funcx-faas/funcx
 Author: Globus Compute Team
 Author-email: support@globus.org
 License: Apache License, Version 2.0
 Keywords: Globus Compute,FaaS,Function Serving
 Classifier: Development Status :: 3 - Alpha
@@ -19,10 +19,10 @@
 Provides-Extra: test
 License-File: LICENSE
 
 # Globus Compute Endpoint
 
 [Globus Compute](https://globus-compute.readthedocs.io/en/latest/) is a distributed Function as a Service (FaaS) platform that enables flexible, scalable, and high performance remote function execution. Unlike centralized FaaS platforms, Globus Compute allows users to execute functions on heterogeneous remote computers, from laptops to campus clusters, clouds, and supercomputers.
 
-This package provides the [Compute Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which recieves user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing compute endpoints.
+This package provides the [Compute Endpoint](https://globus-compute.readthedocs.io/en/latest/endpoints.html) agent — the software which receives user-submitted tasks (functions + arguments) and manages their execution on target machines — in addition to command line tools for managing compute endpoints.
 
 To submit functions for execution on compute endpoints, use the companion [Globus Compute SDK](https://pypi.org/project/globus-compute-sdk/) package.
```

### Comparing `globus-compute-endpoint-2.0.1a1/globus_compute_endpoint.egg-info/SOURCES.txt` & `globus-compute-endpoint-2.0.1a2/globus_compute_endpoint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/setup.py` & `globus-compute-endpoint-2.0.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 REQUIRES = [
     "requests>=2.20.0,<3",
     "globus-sdk",  # version will be bounded by `globus-compute-sdk`
-    "globus-compute-sdk>=2.0.0",
+    "globus-compute-sdk>=2.0.1a2",
     "globus-compute-common==0.1.0",
     # table printing used in list-endpoints
     "texttable>=1.6.4,<2",
     # although psutil does not declare itself to use semver, it appears to offer
     # strong backwards-compatibility promises based on its changelog, usage, and
     # history
     #
```

### Comparing `globus-compute-endpoint-2.0.1a1/tests/conftest.py` & `globus-compute-endpoint-2.0.1a2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `globus-compute-endpoint-2.0.1a1/tests/utils.py` & `globus-compute-endpoint-2.0.1a2/tests/utils.py`

 * *Files identical despite different names*

