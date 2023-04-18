# Comparing `tmp/hagworm-5.4.6.tar.gz` & `tmp/hagworm-5.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagworm-5.4.6.tar", last modified: Sat Apr 15 05:15:43 2023, max compression
+gzip compressed data, was "hagworm-5.4.7.tar", last modified: Tue Apr 18 08:48:59 2023, max compression
```

## Comparing `hagworm-5.4.6.tar` & `hagworm-5.4.7.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.862124 hagworm-5.4.6/
--rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.6/LICENSE
--rw-rw-rw-   0        0        0     7509 2023-04-15 05:15:43.861125 hagworm-5.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.751127 hagworm-5.4.6/c_extend/
--rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.6/c_extend/math.c
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.754125 hagworm-5.4.6/example/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.760125 hagworm-5.4.6/example/fastapi_demo/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.763126 hagworm-5.4.6/example/fastapi_demo/controller/
--rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/controller/__init__.py
--rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/controller/home.py
--rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/gunicorn.config.py
--rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/main.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.764125 hagworm-5.4.6/example/fastapi_demo/model/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.766125 hagworm-5.4.6/example/fastapi_demo/service/
--rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/service/__init__.py
--rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/fastapi_demo/setting.py
--rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.6/example/main_test.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.767125 hagworm-5.4.6/hagworm/
--rw-rw-rw-   0        0        0      510 2023-04-15 03:09:52.000000 hagworm-5.4.6/hagworm/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.804126 hagworm-5.4.6/hagworm/extend/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.831155 hagworm-5.4.6/hagworm/extend/asyncio/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/__init__.py
--rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.6/hagworm/extend/asyncio/base.py
--rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.6/hagworm/extend/asyncio/buffer.py
--rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/command.py
--rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.6/hagworm/extend/asyncio/event.py
--rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.6/hagworm/extend/asyncio/file.py
--rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/future.py
--rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/mail.py
--rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/mongo.py
--rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.6/hagworm/extend/asyncio/mysql.py
--rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/net.py
--rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/ntp.py
--rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/pool.py
--rw-rw-rw-   0        0        0    12069 2023-04-14 02:51:40.000000 hagworm-5.4.6/hagworm/extend/asyncio/redis.py
--rw-rw-rw-   0        0        0     3787 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/socket.py
--rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.6/hagworm/extend/asyncio/task.py
--rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/transaction.py
--rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/asyncio/zmq.py
--rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.6/hagworm/extend/base.py
--rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/cache.py
--rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.6/hagworm/extend/compile.py
--rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/config.py
--rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/crypto.py
--rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.6/hagworm/extend/error.py
--rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/event.py
--rw-rw-rw-   0        0        0     4375 2023-04-13 02:37:21.000000 hagworm-5.4.6/hagworm/extend/igraph.py
--rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.6/hagworm/extend/interface.py
--rw-rw-rw-   0        0        0    14859 2023-04-13 09:17:30.000000 hagworm-5.4.6/hagworm/extend/logging.py
--rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/media.py
--rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.6/hagworm/extend/metaclass.py
--rw-rw-rw-   0        0        0     4500 2023-04-15 03:28:39.000000 hagworm-5.4.6/hagworm/extend/process.py
--rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/qrcode.py
--rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.6/hagworm/extend/struct.py
--rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.6/hagworm/extend/text.py
--rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/trace.py
--rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/transaction.py
--rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/extend/validator.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.836125 hagworm-5.4.6/hagworm/frame/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.843125 hagworm-5.4.6/hagworm/frame/fastapi/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/fastapi/__init__.py
--rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.6/hagworm/frame/fastapi/base.py
--rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/fastapi/field.py
--rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/fastapi/model.py
--rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/fastapi/response.py
--rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/gunicorn.py
--rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/frame/stress_tests.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.845125 hagworm-5.4.6/hagworm/static/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/static/__init__.py
--rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/static/cacert.pem
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.847124 hagworm-5.4.6/hagworm/third/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.852128 hagworm-5.4.6/hagworm/third/aliyun/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/aliyun/__init__.py
--rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/aliyun/logging.py
--rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.6/hagworm/third/aliyun/rocketmq.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.855125 hagworm-5.4.6/hagworm/third/consul/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/consul/__init__.py
--rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/consul/config.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.860125 hagworm-5.4.6/hagworm/third/rabbitmq/
--rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/rabbitmq/__init__.py
--rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.6/hagworm/third/rabbitmq/consume.py
--rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.6/hagworm/third/rabbitmq/publish.py
--rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.6/hagworm/third/rabbitmq/rpc.py
-drwxrwxrwx   0        0        0        0 2023-04-15 05:15:43.774125 hagworm-5.4.6/hagworm.egg-info/
--rw-rw-rw-   0        0        0     7509 2023-04-15 05:15:43.000000 hagworm-5.4.6/hagworm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2262 2023-04-15 05:15:43.000000 hagworm-5.4.6/hagworm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-15 05:15:43.000000 hagworm-5.4.6/hagworm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      707 2023-04-15 05:15:43.000000 hagworm-5.4.6/hagworm.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-04-15 05:15:43.000000 hagworm-5.4.6/hagworm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-15 05:15:43.862124 hagworm-5.4.6/setup.cfg
--rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.822271 hagworm-5.4.7/
+-rw-rw-rw-   0        0        0    11362 2023-03-01 02:07:14.000000 hagworm-5.4.7/LICENSE
+-rw-rw-rw-   0        0        0     7509 2023-04-18 08:48:59.821271 hagworm-5.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6065 2023-04-08 01:06:26.000000 hagworm-5.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.717270 hagworm-5.4.7/c_extend/
+-rw-rw-rw-   0        0        0      847 2023-03-01 02:07:14.000000 hagworm-5.4.7/c_extend/math.c
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.719274 hagworm-5.4.7/example/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.725270 hagworm-5.4.7/example/fastapi_demo/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.728271 hagworm-5.4.7/example/fastapi_demo/controller/
+-rw-rw-rw-   0        0        0      211 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/controller/__init__.py
+-rw-rw-rw-   0        0        0      397 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/controller/home.py
+-rw-rw-rw-   0        0        0      840 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/gunicorn.config.py
+-rw-rw-rw-   0        0        0     1417 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/main.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.729270 hagworm-5.4.7/example/fastapi_demo/model/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.730270 hagworm-5.4.7/example/fastapi_demo/service/
+-rw-rw-rw-   0        0        0     3496 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/service/__init__.py
+-rw-rw-rw-   0        0        0     2096 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/fastapi_demo/setting.py
+-rw-rw-rw-   0        0        0      788 2023-03-01 02:07:14.000000 hagworm-5.4.7/example/main_test.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.732270 hagworm-5.4.7/hagworm/
+-rw-rw-rw-   0        0        0      510 2023-04-18 02:11:41.000000 hagworm-5.4.7/hagworm/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.767271 hagworm-5.4.7/hagworm/extend/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.792272 hagworm-5.4.7/hagworm/extend/asyncio/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/__init__.py
+-rw-rw-rw-   0        0        0    16082 2023-04-11 09:03:03.000000 hagworm-5.4.7/hagworm/extend/asyncio/base.py
+-rw-rw-rw-   0        0        0     4773 2023-04-11 08:20:16.000000 hagworm-5.4.7/hagworm/extend/asyncio/buffer.py
+-rw-rw-rw-   0        0        0     2008 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/command.py
+-rw-rw-rw-   0        0        0     3073 2023-04-12 08:05:02.000000 hagworm-5.4.7/hagworm/extend/asyncio/event.py
+-rw-rw-rw-   0        0        0     1308 2023-04-11 09:00:40.000000 hagworm-5.4.7/hagworm/extend/asyncio/file.py
+-rw-rw-rw-   0        0        0     4232 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/future.py
+-rw-rw-rw-   0        0        0     2603 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/mail.py
+-rw-rw-rw-   0        0        0     3897 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/mongo.py
+-rw-rw-rw-   0        0        0    14412 2023-04-12 08:15:17.000000 hagworm-5.4.7/hagworm/extend/asyncio/mysql.py
+-rw-rw-rw-   0        0        0    13489 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/net.py
+-rw-rw-rw-   0        0        0     4149 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/ntp.py
+-rw-rw-rw-   0        0        0     1490 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/pool.py
+-rw-rw-rw-   0        0        0    12069 2023-04-14 02:51:40.000000 hagworm-5.4.7/hagworm/extend/asyncio/redis.py
+-rw-rw-rw-   0        0        0     5019 2023-04-18 06:23:31.000000 hagworm-5.4.7/hagworm/extend/asyncio/socket.py
+-rw-rw-rw-   0        0        0     6170 2023-04-11 07:28:18.000000 hagworm-5.4.7/hagworm/extend/asyncio/task.py
+-rw-rw-rw-   0        0        0     1360 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/transaction.py
+-rw-rw-rw-   0        0        0     3792 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/asyncio/zmq.py
+-rw-rw-rw-   0        0        0    22551 2023-04-12 08:21:47.000000 hagworm-5.4.7/hagworm/extend/base.py
+-rw-rw-rw-   0        0        0     2365 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/cache.py
+-rw-rw-rw-   0        0        0     1759 2023-04-12 08:23:58.000000 hagworm-5.4.7/hagworm/extend/compile.py
+-rw-rw-rw-   0        0        0     3857 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/config.py
+-rw-rw-rw-   0        0        0     1487 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/crypto.py
+-rw-rw-rw-   0        0        0     1699 2023-04-12 08:24:47.000000 hagworm-5.4.7/hagworm/extend/error.py
+-rw-rw-rw-   0        0        0     1220 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/event.py
+-rw-rw-rw-   0        0        0     4375 2023-04-13 02:37:21.000000 hagworm-5.4.7/hagworm/extend/igraph.py
+-rw-rw-rw-   0        0        0     2208 2023-04-12 08:06:38.000000 hagworm-5.4.7/hagworm/extend/interface.py
+-rw-rw-rw-   0        0        0    14859 2023-04-13 09:17:30.000000 hagworm-5.4.7/hagworm/extend/logging.py
+-rw-rw-rw-   0        0        0     1791 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/media.py
+-rw-rw-rw-   0        0        0     1603 2023-04-08 01:06:26.000000 hagworm-5.4.7/hagworm/extend/metaclass.py
+-rw-rw-rw-   0        0        0     4500 2023-04-15 03:28:39.000000 hagworm-5.4.7/hagworm/extend/process.py
+-rw-rw-rw-   0        0        0      551 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/qrcode.py
+-rw-rw-rw-   0        0        0     6909 2023-04-12 08:32:50.000000 hagworm-5.4.7/hagworm/extend/struct.py
+-rw-rw-rw-   0        0        0     3620 2023-04-12 08:40:57.000000 hagworm-5.4.7/hagworm/extend/text.py
+-rw-rw-rw-   0        0        0     2409 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/trace.py
+-rw-rw-rw-   0        0        0     2677 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/transaction.py
+-rw-rw-rw-   0        0        0     6411 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/extend/validator.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.797270 hagworm-5.4.7/hagworm/frame/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.803270 hagworm-5.4.7/hagworm/frame/fastapi/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/fastapi/__init__.py
+-rw-rw-rw-   0        0        0     7849 2023-04-12 08:55:19.000000 hagworm-5.4.7/hagworm/frame/fastapi/base.py
+-rw-rw-rw-   0        0        0     8494 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/fastapi/field.py
+-rw-rw-rw-   0        0        0     1389 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/fastapi/model.py
+-rw-rw-rw-   0        0        0     1000 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/fastapi/response.py
+-rw-rw-rw-   0        0        0     1304 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/gunicorn.py
+-rw-rw-rw-   0        0        0     3822 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/frame/stress_tests.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.806270 hagworm-5.4.7/hagworm/static/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/static/__init__.py
+-rw-rw-rw-   0        0        0   208075 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/static/cacert.pem
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.807270 hagworm-5.4.7/hagworm/third/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.811270 hagworm-5.4.7/hagworm/third/aliyun/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/aliyun/__init__.py
+-rw-rw-rw-   0        0        0     2111 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/aliyun/logging.py
+-rw-rw-rw-   0        0        0    10141 2023-04-12 08:57:49.000000 hagworm-5.4.7/hagworm/third/aliyun/rocketmq.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.814270 hagworm-5.4.7/hagworm/third/consul/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/consul/__init__.py
+-rw-rw-rw-   0        0        0     1288 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/consul/config.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.820272 hagworm-5.4.7/hagworm/third/rabbitmq/
+-rw-rw-rw-   0        0        0       58 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/rabbitmq/__init__.py
+-rw-rw-rw-   0        0        0     3437 2023-04-12 09:00:41.000000 hagworm-5.4.7/hagworm/third/rabbitmq/consume.py
+-rw-rw-rw-   0        0        0     5350 2023-03-01 02:07:14.000000 hagworm-5.4.7/hagworm/third/rabbitmq/publish.py
+-rw-rw-rw-   0        0        0     5743 2023-04-12 08:59:35.000000 hagworm-5.4.7/hagworm/third/rabbitmq/rpc.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:48:59.739270 hagworm-5.4.7/hagworm.egg-info/
+-rw-rw-rw-   0        0        0     7509 2023-04-18 08:48:59.000000 hagworm-5.4.7/hagworm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2262 2023-04-18 08:48:59.000000 hagworm-5.4.7/hagworm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:48:59.000000 hagworm-5.4.7/hagworm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      707 2023-04-18 08:48:59.000000 hagworm-5.4.7/hagworm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-04-18 08:48:59.000000 hagworm-5.4.7/hagworm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 08:48:59.822271 hagworm-5.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     2291 2023-03-01 02:07:14.000000 hagworm-5.4.7/setup.py
```

### Comparing `hagworm-5.4.6/LICENSE` & `hagworm-5.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/PKG-INFO` & `hagworm-5.4.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.6
+Version: 5.4.7
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.6/README.md` & `hagworm-5.4.7/README.md`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/c_extend/math.c` & `hagworm-5.4.7/c_extend/math.c`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/example/fastapi_demo/gunicorn.config.py` & `hagworm-5.4.7/example/fastapi_demo/gunicorn.config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/example/fastapi_demo/main.py` & `hagworm-5.4.7/example/fastapi_demo/main.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/example/fastapi_demo/service/__init__.py` & `hagworm-5.4.7/example/fastapi_demo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/example/fastapi_demo/setting.py` & `hagworm-5.4.7/example/fastapi_demo/setting.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/example/main_test.py` & `hagworm-5.4.7/example/main_test.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/base.py` & `hagworm-5.4.7/hagworm/extend/asyncio/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/buffer.py` & `hagworm-5.4.7/hagworm/extend/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/command.py` & `hagworm-5.4.7/hagworm/extend/asyncio/command.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/event.py` & `hagworm-5.4.7/hagworm/extend/asyncio/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/file.py` & `hagworm-5.4.7/hagworm/extend/asyncio/file.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/future.py` & `hagworm-5.4.7/hagworm/extend/asyncio/future.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/mail.py` & `hagworm-5.4.7/hagworm/extend/asyncio/mail.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/mongo.py` & `hagworm-5.4.7/hagworm/extend/asyncio/mongo.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/mysql.py` & `hagworm-5.4.7/hagworm/extend/asyncio/mysql.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/net.py` & `hagworm-5.4.7/hagworm/extend/asyncio/net.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/ntp.py` & `hagworm-5.4.7/hagworm/extend/asyncio/ntp.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/pool.py` & `hagworm-5.4.7/hagworm/extend/asyncio/pool.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/redis.py` & `hagworm-5.4.7/hagworm/extend/asyncio/redis.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/socket.py` & `hagworm-5.4.7/hagworm/extend/asyncio/socket.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 __author__ = r'wsb310@gmail.com'
 
 import signal
 import socket
 import asyncio
 
+from typing import List
+
 from hagworm import hagworm_slogan
 from hagworm import __version__ as hagworm_version
 from hagworm.extend.asyncio.base import Utils, install_uvloop
 from hagworm.extend.interface import RunnableInterface
 
 from ..error import RouterError
 
@@ -57,26 +59,42 @@
 
     def include(self, router):
 
         for method, func in router.items():
             self._reg(method, func)
 
 
+class SocketConfig:
+
+    __slots__ = [r'client_connected_cb', r'address', r'family', r'backlog', r'reuse_port', r'buffer_limit']
+
+    def __init__(self, client_connected_cb, address, family, backlog, reuse_port, buffer_limit):
+
+        self.client_connected_cb = client_connected_cb
+        self.address = address
+        self.family = family
+        self.backlog = backlog
+        self.reuse_port = reuse_port
+        self.buffer_limit = buffer_limit
+
+
 class AsyncTcpServer(RunnableInterface):
 
     def __init__(
             self, client_connected_cb, address, *,
-            backlog=None, buffer_limit=0xffffff,
+            family=socket.AF_INET, backlog=None, reuse_port=True, buffer_limit=0xffffff,
             on_startup=None, on_shutdown=None
     ):
 
-        self._listeners = [(client_connected_cb, address)]
-
-        self._backlog = backlog
-        self._buffer_limit = buffer_limit
+        self._listeners: List[SocketConfig] = [
+            SocketConfig(
+                client_connected_cb, address,
+                family, backlog, reuse_port, buffer_limit
+            )
+        ]
 
         self._on_startup = on_startup
         self._on_shutdown = on_shutdown
 
         self._servers = []
         self._server_tasks = []
 
@@ -91,17 +109,25 @@
         return self
 
     async def __aexit__(self, exc_type, exc_value, _traceback):
 
         for server in self._servers:
             await server.__aexit__(exc_type, exc_value, _traceback)
 
-    def add_listener(self, client_connected_cb, address):
+    def add_listener(
+            self, client_connected_cb, address, *,
+            family=socket.AF_INET, backlog=None, reuse_port=True, buffer_limit=0xffffff
+    ):
 
-        self._listeners.append((client_connected_cb, address))
+        self._listeners.append(
+            SocketConfig(
+                client_connected_cb, address,
+                family, backlog, reuse_port, buffer_limit
+            )
+        )
 
     def run(self):
 
         environment = Utils.environment()
 
         Utils.log.info(
             f'{hagworm_slogan}'
@@ -115,23 +141,38 @@
         asyncio.run(self._run())
 
     async def _run(self):
 
         if self._on_startup is not None:
             await self._on_startup()
 
-        for client_connected_cb, address in self._listeners:
+        for config in self._listeners:
 
-            sock = socket.create_server(address, family=socket.AF_INET, backlog=self._backlog, reuse_port=True)
+            if config.family == socket.AF_UNIX:
 
-            self._servers.append(
-                await asyncio.start_server(client_connected_cb, limit=self._buffer_limit, sock=sock)
-            )
+                _socket_server = await asyncio.start_unix_server(
+                    config.client_connected_cb, config.address, limit=config.buffer_limit
+                )
 
-            Utils.log.success(f'tcp server [pid:{Utils.getpid()}] startup complete: {sock.getsockname()}')
+                Utils.log.success(f'unix server [pid:{Utils.getpid()}] startup complete: {config.address}')
+
+            else:
+
+                _socket = socket.create_server(
+                    config.address, family=config.family, backlog=config.backlog, reuse_port=config.reuse_port
+                )
+
+                _socket_server = await asyncio.start_server(
+                    config.client_connected_cb,
+                    limit=config.buffer_limit, sock=_socket
+                )
+
+                Utils.log.success(f'socket server [pid:{Utils.getpid()}] startup complete: {config.address}')
+
+            self._servers.append(_socket_server)
 
         async with self:
 
             for _server in self._servers:
                 self._server_tasks.append(
                     asyncio.create_task(_server.serve_forever())
                 )
@@ -142,13 +183,11 @@
                     await _server_task
                 except asyncio.CancelledError as _:
                     pass
 
         if self._on_shutdown is not None:
             await self._on_shutdown()
 
-        Utils.log.success(f'tcp server [pid:{Utils.getpid()}] shutdown')
-
     def _exit(self, *_):
 
         for _server_task in self._server_tasks:
             _server_task.cancel()
```

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/task.py` & `hagworm-5.4.7/hagworm/extend/asyncio/task.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/transaction.py` & `hagworm-5.4.7/hagworm/extend/asyncio/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/asyncio/zmq.py` & `hagworm-5.4.7/hagworm/extend/asyncio/zmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/base.py` & `hagworm-5.4.7/hagworm/extend/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/cache.py` & `hagworm-5.4.7/hagworm/extend/cache.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/compile.py` & `hagworm-5.4.7/hagworm/extend/compile.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/config.py` & `hagworm-5.4.7/hagworm/extend/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/crypto.py` & `hagworm-5.4.7/hagworm/extend/crypto.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/error.py` & `hagworm-5.4.7/hagworm/extend/error.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/event.py` & `hagworm-5.4.7/hagworm/extend/event.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/igraph.py` & `hagworm-5.4.7/hagworm/extend/igraph.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/interface.py` & `hagworm-5.4.7/hagworm/extend/interface.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/logging.py` & `hagworm-5.4.7/hagworm/extend/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/media.py` & `hagworm-5.4.7/hagworm/extend/media.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/metaclass.py` & `hagworm-5.4.7/hagworm/extend/metaclass.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/process.py` & `hagworm-5.4.7/hagworm/extend/process.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/qrcode.py` & `hagworm-5.4.7/hagworm/extend/qrcode.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/struct.py` & `hagworm-5.4.7/hagworm/extend/struct.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/text.py` & `hagworm-5.4.7/hagworm/extend/text.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/trace.py` & `hagworm-5.4.7/hagworm/extend/trace.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/transaction.py` & `hagworm-5.4.7/hagworm/extend/transaction.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/extend/validator.py` & `hagworm-5.4.7/hagworm/extend/validator.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/frame/fastapi/base.py` & `hagworm-5.4.7/hagworm/frame/fastapi/base.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/frame/fastapi/field.py` & `hagworm-5.4.7/hagworm/frame/fastapi/field.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/frame/fastapi/model.py` & `hagworm-5.4.7/hagworm/frame/fastapi/model.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/frame/fastapi/response.py` & `hagworm-5.4.7/hagworm/frame/fastapi/response.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/frame/gunicorn.py` & `hagworm-5.4.7/hagworm/frame/gunicorn.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/frame/stress_tests.py` & `hagworm-5.4.7/hagworm/frame/stress_tests.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/static/cacert.pem` & `hagworm-5.4.7/hagworm/static/cacert.pem`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/third/aliyun/logging.py` & `hagworm-5.4.7/hagworm/third/aliyun/logging.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/third/aliyun/rocketmq.py` & `hagworm-5.4.7/hagworm/third/aliyun/rocketmq.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/third/consul/config.py` & `hagworm-5.4.7/hagworm/third/consul/config.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/third/rabbitmq/consume.py` & `hagworm-5.4.7/hagworm/third/rabbitmq/consume.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/third/rabbitmq/publish.py` & `hagworm-5.4.7/hagworm/third/rabbitmq/publish.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm/third/rabbitmq/rpc.py` & `hagworm-5.4.7/hagworm/third/rabbitmq/rpc.py`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm.egg-info/PKG-INFO` & `hagworm-5.4.7/hagworm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hagworm
-Version: 5.4.6
+Version: 5.4.7
 Summary: Network Development Suite
 Home-page: https://gitee.com/wsb310/hagworm
 Author: Shaobo.Wang
 Author-email: wsb310@gmail.com
 License: Apache License Version 2.0
 Description: # Hagworm
```

### Comparing `hagworm-5.4.6/hagworm.egg-info/SOURCES.txt` & `hagworm-5.4.7/hagworm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/hagworm.egg-info/requires.txt` & `hagworm-5.4.7/hagworm.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hagworm-5.4.6/setup.py` & `hagworm-5.4.7/setup.py`

 * *Files identical despite different names*

