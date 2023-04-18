# Comparing `tmp/panini-0.8.0a2.tar.gz` & `tmp/panini-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panini-0.8.0a2.tar", last modified: Tue Nov 22 00:35:24 2022, max compression
+gzip compressed data, was "panini-0.8.1.tar", last modified: Tue Apr 18 16:20:08 2023, max compression
```

## Comparing `panini-0.8.0a2.tar` & `panini-0.8.1.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.048634 panini-0.8.0a2/
--rw-r--r--   0 artas      (502) staff       (20)     3176 2022-07-22 01:01:04.000000 panini-0.8.0a2/CHANGELOG.md
--rw-r--r--   0 artas      (502) staff       (20)     1223 2021-03-30 12:13:12.000000 panini-0.8.0a2/CONTRIBUTING.md
--rw-r--r--   0 artas      (502) staff       (20)     1091 2021-03-30 12:13:12.000000 panini-0.8.0a2/LICENSE.md
--rw-r--r--   0 artas      (502) staff       (20)      105 2021-03-30 12:13:12.000000 panini-0.8.0a2/MANIFEST.in
--rw-r--r--   0 artas      (502) staff       (20)     1616 2022-11-22 00:35:24.048845 panini-0.8.0a2/PKG-INFO
--rw-r--r--   0 artas      (502) staff       (20)    11821 2022-07-22 01:01:04.000000 panini-0.8.0a2/README.md
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.037106 panini-0.8.0a2/panini/
--rw-r--r--   0 artas      (502) staff       (20)        0 2022-11-20 17:29:37.000000 panini-0.8.0a2/panini/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)    14121 2022-11-21 23:01:29.000000 panini-0.8.0a2/panini/app.py
--rw-r--r--   0 artas      (502) staff       (20)    13391 2022-11-21 23:01:29.000000 panini-0.8.0a2/panini/async_test_client.py
--rw-r--r--   0 artas      (502) staff       (20)     5449 2021-05-25 01:00:47.000000 panini-0.8.0a2/panini/emulator_client.py
--rw-r--r--   0 artas      (502) staff       (20)     2209 2022-11-21 23:01:29.000000 panini-0.8.0a2/panini/exceptions.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.039663 panini-0.8.0a2/panini/http_server/
--rw-r--r--   0 artas      (502) staff       (20)        0 2021-03-30 12:13:12.000000 panini-0.8.0a2/panini/http_server/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     1084 2022-07-22 01:01:04.000000 panini-0.8.0a2/panini/http_server/http_server_app.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.042725 panini-0.8.0a2/panini/managers/
--rw-r--r--   0 artas      (502) staff       (20)        0 2022-11-20 17:29:29.000000 panini-0.8.0a2/panini/managers/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     2733 2022-11-21 23:01:29.000000 panini-0.8.0a2/panini/managers/event_manager.py
--rw-r--r--   0 artas      (502) staff       (20)     6361 2022-09-16 19:16:55.000000 panini-0.8.0a2/panini/managers/middleware_manager.py
--rw-r--r--   0 artas      (502) staff       (20)    17818 2022-11-21 23:31:18.000000 panini-0.8.0a2/panini/managers/nats_client.py
--rw-r--r--   0 artas      (502) staff       (20)     3709 2022-11-22 00:32:44.000000 panini-0.8.0a2/panini/managers/schema_manager.py
--rw-r--r--   0 artas      (502) staff       (20)     2251 2022-11-21 23:01:29.000000 panini-0.8.0a2/panini/managers/task_manager.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.046282 panini-0.8.0a2/panini/middleware/
--rw-r--r--   0 artas      (502) staff       (20)     1563 2021-03-30 12:13:12.000000 panini-0.8.0a2/panini/middleware/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     1383 2022-07-22 01:01:04.000000 panini-0.8.0a2/panini/middleware/debug_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)     1355 2021-03-30 12:13:12.000000 panini-0.8.0a2/panini/middleware/error.py
--rw-r--r--   0 artas      (502) staff       (20)     1200 2022-11-22 00:14:35.000000 panini-0.8.0a2/panini/middleware/nats_timeout.py
--rw-r--r--   0 artas      (502) staff       (20)     3281 2022-11-22 00:18:24.000000 panini-0.8.0a2/panini/middleware/prometheus_monitoring.py
--rw-r--r--   0 artas      (502) staff       (20)     1716 2022-11-21 23:59:52.000000 panini-0.8.0a2/panini/middleware/reader_emulator_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)     3810 2022-07-22 01:01:04.000000 panini-0.8.0a2/panini/middleware/writer_emulator_middleware.py
--rw-r--r--   0 artas      (502) staff       (20)    11241 2022-11-21 23:01:29.000000 panini-0.8.0a2/panini/test_client.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.048185 panini-0.8.0a2/panini/utils/
--rw-r--r--   0 artas      (502) staff       (20)        0 2021-03-30 12:13:12.000000 panini-0.8.0a2/panini/utils/__init__.py
--rw-r--r--   0 artas      (502) staff       (20)     3133 2021-03-30 12:13:12.000000 panini-0.8.0a2/panini/utils/helper.py
--rw-r--r--   0 artas      (502) staff       (20)     9207 2022-07-22 01:01:04.000000 panini-0.8.0a2/panini/utils/logger.py
--rw-r--r--   0 artas      (502) staff       (20)      185 2021-03-30 12:13:12.000000 panini-0.8.0a2/panini/utils/singleton.py
-drwxr-xr-x   0 artas      (502) staff       (20)        0 2022-11-22 00:35:24.039089 panini-0.8.0a2/panini.egg-info/
--rw-r--r--   0 artas      (502) staff       (20)     1616 2022-11-22 00:35:23.000000 panini-0.8.0a2/panini.egg-info/PKG-INFO
--rw-r--r--   0 artas      (502) staff       (20)     1033 2022-11-22 00:35:23.000000 panini-0.8.0a2/panini.egg-info/SOURCES.txt
--rw-r--r--   0 artas      (502) staff       (20)        1 2022-11-22 00:35:23.000000 panini-0.8.0a2/panini.egg-info/dependency_links.txt
--rw-r--r--   0 artas      (502) staff       (20)        1 2022-11-22 00:35:23.000000 panini-0.8.0a2/panini.egg-info/not-zip-safe
--rw-r--r--   0 artas      (502) staff       (20)      204 2022-11-22 00:35:23.000000 panini-0.8.0a2/panini.egg-info/requires.txt
--rw-r--r--   0 artas      (502) staff       (20)        7 2022-11-22 00:35:23.000000 panini-0.8.0a2/panini.egg-info/top_level.txt
--rw-r--r--   0 artas      (502) staff       (20)      180 2021-03-30 12:13:12.000000 panini-0.8.0a2/pyproject.toml
--rw-r--r--   0 artas      (502) staff       (20)       79 2022-11-22 00:35:24.049662 panini-0.8.0a2/setup.cfg
--rw-r--r--   0 artas      (502) staff       (20)     2432 2022-11-22 00:35:18.000000 panini-0.8.0a2/setup.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.728312 panini-0.8.1/
+-rw-r--r--   0 artas      (502) staff       (20)     4249 2023-03-06 14:18:48.000000 panini-0.8.1/CHANGELOG.md
+-rw-r--r--   0 artas      (502) staff       (20)     1223 2021-03-30 12:13:12.000000 panini-0.8.1/CONTRIBUTING.md
+-rw-r--r--   0 artas      (502) staff       (20)     1091 2021-03-30 12:13:12.000000 panini-0.8.1/LICENSE.md
+-rw-r--r--   0 artas      (502) staff       (20)      105 2021-03-30 12:13:12.000000 panini-0.8.1/MANIFEST.in
+-rw-r--r--   0 artas      (502) staff       (20)     1614 2023-04-18 16:20:08.728475 panini-0.8.1/PKG-INFO
+-rw-r--r--   0 artas      (502) staff       (20)    11821 2023-03-06 14:18:48.000000 panini-0.8.1/README.md
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.710236 panini-0.8.1/panini/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2022-11-20 17:29:37.000000 panini-0.8.1/panini/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)    14741 2023-04-18 16:04:08.000000 panini-0.8.1/panini/app.py
+-rw-r--r--   0 artas      (502) staff       (20)    13391 2023-03-06 14:18:48.000000 panini-0.8.1/panini/async_test_client.py
+-rw-r--r--   0 artas      (502) staff       (20)     5449 2021-05-25 01:00:47.000000 panini-0.8.1/panini/emulator_client.py
+-rw-r--r--   0 artas      (502) staff       (20)     2209 2023-03-06 14:18:48.000000 panini-0.8.1/panini/exceptions.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.715406 panini-0.8.1/panini/http_server/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2021-03-30 12:13:12.000000 panini-0.8.1/panini/http_server/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     1084 2023-03-06 14:18:48.000000 panini-0.8.1/panini/http_server/http_server_app.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.721051 panini-0.8.1/panini/managers/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2022-11-20 17:29:29.000000 panini-0.8.1/panini/managers/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     2826 2023-04-18 16:04:08.000000 panini-0.8.1/panini/managers/event_manager.py
+-rw-r--r--   0 artas      (502) staff       (20)     6361 2022-09-16 19:16:55.000000 panini-0.8.1/panini/managers/middleware_manager.py
+-rw-r--r--   0 artas      (502) staff       (20)    18198 2023-04-18 16:04:08.000000 panini-0.8.1/panini/managers/nats_client.py
+-rw-r--r--   0 artas      (502) staff       (20)     3709 2023-03-06 14:18:48.000000 panini-0.8.1/panini/managers/schema_manager.py
+-rw-r--r--   0 artas      (502) staff       (20)     2251 2023-03-06 14:18:48.000000 panini-0.8.1/panini/managers/task_manager.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.725748 panini-0.8.1/panini/middleware/
+-rw-r--r--   0 artas      (502) staff       (20)     1563 2021-03-30 12:13:12.000000 panini-0.8.1/panini/middleware/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     1383 2023-03-06 14:18:48.000000 panini-0.8.1/panini/middleware/debug_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)     1355 2021-03-30 12:13:12.000000 panini-0.8.1/panini/middleware/error.py
+-rw-r--r--   0 artas      (502) staff       (20)     1200 2023-03-06 14:18:48.000000 panini-0.8.1/panini/middleware/nats_timeout.py
+-rw-r--r--   0 artas      (502) staff       (20)     3281 2023-03-06 14:18:48.000000 panini-0.8.1/panini/middleware/prometheus_monitoring.py
+-rw-r--r--   0 artas      (502) staff       (20)     1716 2023-03-06 14:18:48.000000 panini-0.8.1/panini/middleware/reader_emulator_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)     5990 2023-04-18 16:04:08.000000 panini-0.8.1/panini/middleware/tracing_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)     3810 2023-03-06 14:18:48.000000 panini-0.8.1/panini/middleware/writer_emulator_middleware.py
+-rw-r--r--   0 artas      (502) staff       (20)    11241 2023-03-06 14:18:48.000000 panini-0.8.1/panini/test_client.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.727818 panini-0.8.1/panini/utils/
+-rw-r--r--   0 artas      (502) staff       (20)        0 2021-03-30 12:13:12.000000 panini-0.8.1/panini/utils/__init__.py
+-rw-r--r--   0 artas      (502) staff       (20)     3133 2021-03-30 12:13:12.000000 panini-0.8.1/panini/utils/helper.py
+-rw-r--r--   0 artas      (502) staff       (20)     9207 2023-03-06 14:18:48.000000 panini-0.8.1/panini/utils/logger.py
+-rw-r--r--   0 artas      (502) staff       (20)      185 2021-03-30 12:13:12.000000 panini-0.8.1/panini/utils/singleton.py
+drwxr-xr-x   0 artas      (502) staff       (20)        0 2023-04-18 16:20:08.714484 panini-0.8.1/panini.egg-info/
+-rw-r--r--   0 artas      (502) staff       (20)     1614 2023-04-18 16:20:08.000000 panini-0.8.1/panini.egg-info/PKG-INFO
+-rw-r--r--   0 artas      (502) staff       (20)     1073 2023-04-18 16:20:08.000000 panini-0.8.1/panini.egg-info/SOURCES.txt
+-rw-r--r--   0 artas      (502) staff       (20)        1 2023-04-18 16:20:08.000000 panini-0.8.1/panini.egg-info/dependency_links.txt
+-rw-r--r--   0 artas      (502) staff       (20)        1 2022-11-22 00:35:23.000000 panini-0.8.1/panini.egg-info/not-zip-safe
+-rw-r--r--   0 artas      (502) staff       (20)      204 2023-04-18 16:20:08.000000 panini-0.8.1/panini.egg-info/requires.txt
+-rw-r--r--   0 artas      (502) staff       (20)        7 2023-04-18 16:20:08.000000 panini-0.8.1/panini.egg-info/top_level.txt
+-rw-r--r--   0 artas      (502) staff       (20)      180 2021-03-30 12:13:12.000000 panini-0.8.1/pyproject.toml
+-rw-r--r--   0 artas      (502) staff       (20)       79 2023-04-18 16:20:08.729044 panini-0.8.1/setup.cfg
+-rw-r--r--   0 artas      (502) staff       (20)     2430 2023-04-18 16:15:48.000000 panini-0.8.1/setup.py
```

### Comparing `panini-0.8.0a2/CHANGELOG.md` & `panini-0.8.1/CHANGELOG.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,32 @@
 # Changelog
+
+## [v0.8.0](https://github.com/lwinterface/panini/tree/v0.7.0) (2022-12-20)
+
+- Parameter data_type "json" removed
+- No need to declare "data_type" for "publish" and "request"
+- New parameter for “request” method - “response_data_type”
+- Panini supports Dataclass as data_type
+- Experimental: Custom data_type with Callable object
+- Panini Validator has been removed
+- JetStream syntax support
+- Removed "validation_error_cb"
+
+## [v0.7.2](https://github.com/lwinterface/panini/tree/v0.7.0) (2022-02-14)
+
+- Fixed reconnection problem
+
+## [v0.7.0](https://github.com/lwinterface/panini/tree/v0.7.0) (2022-02-14)
+
+- Support NATS 2.0🎉. Now the panini stands on shoulders of nats-py v2.0.0
+- Support Python 3.10
+- Introducing on_start_task
+- Introducing minimal JetStream support
+Since Panini switched from asyncio-nats-client to nats-py, it has become possible to support one of the most important features of NATS 2.0 - JetStream. Panini v0.7.0 does not implement an interface to JetStream at the framework level. Instead, it is suggested to use directly nats-py.
+
 ## [v0.6.2](https://github.com/lwinterface/panini/tree/v0.6.2) (2021-11-11)
 
 - Fixed bug: tasks doesn't works with HTTP server
 - Fixed package incompatibility
 
 ## [v0.6.0](https://github.com/lwinterface/panini/tree/v0.6.0) (2021-11-04)
```

### Comparing `panini-0.8.0a2/CONTRIBUTING.md` & `panini-0.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/LICENSE.md` & `panini-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/PKG-INFO` & `panini-0.8.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panini
-Version: 0.8.0a2
+Version: 0.8.1
 Summary: A python messaging framework for microservices based on NATS
 Home-page: https://github.com/lwinterface/panini
 Author: Op Return SA, developers: Andrii Volotskov, Danylo Tiutiushkin
 Author-email: example@example.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/lwinterface/panini/issues
 Project-URL: Source, https://github.com/lwinterface/panini/
```

### Comparing `panini-0.8.0a2/README.md` & `panini-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/app.py` & `panini-0.8.1/panini/app.py`

 * *Files 7% similar despite different names*

```diff
@@ -192,32 +192,35 @@
             )
         self.logger.logger = logging.getLogger(service_name)
 
     def listen(
             self,
             subject: list or str,
             data_type=dict,
+            **kwargs
     ):
         return self._event_manager.listen(
             subject=subject,
             data_type=data_type,
+            **kwargs
         )
 
     def js_listen(
             self,
             subject: str = None,
             data_type=dict,
             queue: str = None,
             durable: Optional[str] = None,
             stream: Optional[str] = None,
             config: Optional[api.ConsumerConfig] = None,
             manual_ack: Optional[bool] = False,
             ordered_consumer: Optional[bool] = False,
             idle_heartbeat: Optional[float] = None,
             flow_control: Optional[bool] = False,
+            **kwargs
     ):
         """
         "PUSH" JetStream listen(subscribe)
 
         :param subject: Subject from a stream from JetStream.
         :param data_type: Type of message to convert to.
         :param queue: Deliver group name from a set a of queue subscribers.
@@ -237,125 +240,150 @@
             durable=durable,
             stream=stream,
             config=config,
             manual_ack=manual_ack,
             ordered_consumer=ordered_consumer,
             idle_heartbeat=idle_heartbeat,
             flow_control=flow_control,
+            **kwargs
         )
 
     async def publish(
             self,
             subject: str,
             message,
             reply_to: str = "",
             force: bool = False,
-            headers: dict = None
+            headers: dict = None,
+            *args,
+            **kwargs
     ):
         return await self.nats.publish(
             subject=subject,
             message=message,
             reply_to=reply_to,
             force=force,
-            headers=headers
+            headers=headers,
+            *args,
+            **kwargs
         )
 
     def publish_sync(
             self,
             subject: str,
             message,
             reply_to: str = "",
             force: bool = False,
-            headers: dict = None
+            headers: dict = None,
+            *args,
+            **kwargs
     ):
         return self.nats.publish_sync(
             subject=subject,
             message=message,
             reply_to=reply_to,
             force=force,
-            headers=headers
+            headers=headers,
+            *args,
+            **kwargs
         )
 
     async def request(
             self,
             subject: str,
             message,
             timeout: int = 10,
             response_data_type: type = dict,
-            headers: dict = None
+            headers: dict = None,
+            *args,
+            **kwargs
     ):
         return await self.nats.request(
             subject=subject,
             message=message,
             timeout=timeout,
             response_data_type=response_data_type,
-            headers=headers
+            headers=headers,
+            *args,
+            **kwargs
         )
 
     def request_sync(
             self,
             subject: str,
             message,
             timeout: int = 10,
             response_data_type: type = dict,
-            headers: dict = None
+            headers: dict = None,
+            *args,
+            **kwargs
     ):
         return self.nats.request_sync(
             subject=subject,
             message=message,
             timeout=timeout,
             response_data_type=response_data_type,
-            headers=headers
+            headers=headers,
+            *args,
+            **kwargs
         )
 
     async def publish_js(
             self,
             subject: str,
             message,
             timeout: float = None,
             stream: str = None,
             headers: dict = None,
+            *args,
+            **kwargs
     ):
         return await self.nats.publish_js(
             subject=subject,
             message=message,
             timeout=timeout,
             stream=stream,
             headers=headers,
+            *args,
+            **kwargs
         )
 
     def subscribe_new_subject_sync(
             self,
             subject: str,
             callback: Callable,
             data_type=dict,
             queue="",
+            **listen_kwargs
     ):
         return self.nats.subscribe_new_subject_sync(
             listener=Listen(
                 callback=callback,
                 subject=subject,
                 data_type=data_type,
                 queue=queue,
+                _meta=listen_kwargs
             )
         )
 
     async def subscribe_new_subject(
             self,
             subject: str,
             callback: Callable,
             data_type=dict,
             queue="",
+            **listen_kwargs
     ):
         return await self.nats.subscribe_new_subject(
             listener=Listen(
                 callback=callback,
                 subject=subject,
                 data_type=data_type,
                 queue=queue,
+                _meta=listen_kwargs
             ),
         )
 
     def unsubscribe_subject_sync(self, subject: str):
         return self.nats.unsubscribe_subject_sync(subject)
 
     async def unsubscribe_subject(self, subject: str):
```

### Comparing `panini-0.8.0a2/panini/async_test_client.py` & `panini-0.8.1/panini/async_test_client.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/emulator_client.py` & `panini-0.8.1/panini/emulator_client.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/exceptions.py` & `panini-0.8.1/panini/exceptions.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/http_server/http_server_app.py` & `panini-0.8.1/panini/http_server/http_server_app.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/managers/event_manager.py` & `panini-0.8.1/panini/managers/event_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 
 @dataclass
 class Listen:
     callback: Callable
     subject: str
     data_type: type = dict
     queue: str = ""
+    _meta: dict = dict
 
 @dataclass
 class JsListen(Listen):
     durable: Optional[str] = None
     stream: Optional[str] = None
     config: Optional[api.ConsumerConfig] = None
     manual_ack: Optional[bool] = False
     ordered_consumer: Optional[bool] = False
     idle_heartbeat: Optional[float] = None
     flow_control: Optional[bool] = False
+    _meta: dict = dict
 
 
 class EventManager:
     """
     Collect all functions from each module wrapped by @app.subscription or @EventManager.subscribe
     """
 
@@ -38,52 +40,52 @@
     def js_subscriptions(self):
         return self._js_subscriptions
 
     def listen(
         self,
         subject: list or str,
         data_type: type = dict,
-        **kwargs
+        **listen_kwargs
     ):
         def wrapper(callback):
             if isinstance(subject, list):
                 for s in subject:
                     self._create_subscription_if_missing(s)
                     listen_obj = Listen(
                         callback=callback,
                         subject=s,
                         data_type=data_type,
-                        **kwargs
+                        _meta=listen_kwargs
                     )
                     self._subscriptions[s].append(listen_obj)
             else:
                 self._create_subscription_if_missing(subject)
                 listen_obj = Listen(
                     callback=callback,
                     subject=subject,
                     data_type=data_type,
-                    **kwargs
+                    _meta=listen_kwargs
                 )
                 self._subscriptions[subject].append(listen_obj)
             return callback
         return wrapper
 
     def js_listen(
         self,
         subject: list or str,
         data_type: type = dict,
-        **kwargs,
+        **listen_kwargs,
     ):
         def wrapper(callback):
             self._create_subscription_if_missing(subject, js=True)
             js_listen_obj = JsListen(
                 callback=callback,
                 subject=subject,
                 data_type=data_type,
-                **kwargs
+                _meta=listen_kwargs
             )
             self._js_subscriptions[subject].append(js_listen_obj)
             return callback
         return wrapper
 
 
     def _create_subscription_if_missing(self, subscription, js=False):
```

### Comparing `panini-0.8.0a2/panini/managers/middleware_manager.py` & `panini-0.8.1/panini/managers/middleware_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/managers/nats_client.py` & `panini-0.8.1/panini/managers/nats_client.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,18 +166,18 @@
         print("======================================================================================\n")
 
     def subscribe_new_subject_sync(self, listener: Listen):
         self.loop.run_until_complete(self.subscribe_new_subject(listener))
 
     async def subscribe_new_subject(self, listener: Listen):
         params = listener.__dict__
-        subject = params.pop("subject")
-        callback = params.pop("callback")
-        data_type = params.pop("data_type")
-        queue = params.pop("queue")
+        subject = params.get("subject")
+        callback = params.get("callback")
+        data_type = params.get("data_type")
+        queue = params.get("queue")
         if not queue:
             queue = self.queue
 
         callback_with_middleware = self._middleware_manager.wrap_function_by_middleware("listen")(callback)
         wrapped_callback = _ReceivedMessageHandler(self._publish, callback_with_middleware, data_type).call
         sub = await self.client.subscribe(
             subject,
@@ -189,17 +189,17 @@
         if subject not in self.sub_map:
             self.sub_map[subject] = []
         self.sub_map[subject].append(sub)
         return sub
 
     async def subscribe_new_js(self, js_listener: JsListen):
         params = js_listener.__dict__
-        callback = params.pop("callback")
-        data_type = params.pop("data_type")
-        queue = params.pop("queue")
+        callback = params.get("callback")
+        data_type = params.get("data_type")
+        queue = params.get("queue")
         if not queue:
             queue = self.queue
         callback_with_middleware = self._middleware_manager.wrap_function_by_middleware("listen")(callback)
         wrapped_callback = _ReceivedMessageHandler(self._publish, callback_with_middleware, data_type).call_js
 
         sub = await self.js.subscribe(
             queue=queue,
@@ -233,32 +233,38 @@
     def publish_sync(
             self,
             subject: str,
             message,
             reply_to: str = "",
             force: bool = False,
             headers: dict = None,
+            *args,
+            **kwargs
     ):
         asyncio.ensure_future(
-            self.publish(subject, message, reply_to, force, headers)
+            self.publish(subject, message, reply_to, force, headers, *args,
+            **kwargs)
         )
 
     def publish_from_another_thread(self, subject: str, message):
         self.loop.call_soon_threadsafe(self.publish_sync, subject, message)
 
     def request_sync(
             self,
             subject: str,
             message,
             timeout: int = 10,
             response_data_type: type = dict,
             headers: dict = None,
+            *args,
+            **kwargs
     ):
         return self.loop.run_until_complete(
-            self.request(subject, message, timeout, response_data_type, headers)
+            self.request(subject, message, timeout, response_data_type, headers, *args,
+            **kwargs)
         )
 
     def request_from_another_thread_sync(
             self,
             subject: str,
             message,
             timeout: int = 10,
@@ -315,21 +321,25 @@
     async def publish(
             self,
             subject: str,
             message,
             reply_to: str = None,
             force: bool = False,
             headers: dict = None,
+            *args,
+            **kwargs
     ):
         return await self._publish_wrapped(
             subject=subject,
             message=message,
             reply_to=reply_to,
             force=force,
-            headers=headers
+            headers=headers,
+            *args,
+            **kwargs
         )
 
     async def _request(
             self,
             subject: str,
             message,
             timeout: int = 10,
@@ -343,21 +353,25 @@
     async def request(
             self,
             subject: str,
             message,
             timeout: int = 10,
             response_data_type: type = dict,
             headers: dict = None,
+            *args,
+            **kwargs
     ):
         return await self._request_wrapped(
             subject=subject,
             message=message,
             timeout=timeout,
             response_data_type=response_data_type,
             headers=headers,
+            *args,
+            **kwargs
         )
 
     async def _publish_js(
             self,
             subject: str,
             message,
             timeout: float = None,
@@ -376,14 +390,16 @@
     async def publish_js(
             self,
             subject: str,
             message,
             timeout: float = None,
             stream: str = None,
             headers: dict = None,
+            *args,
+            **kwargs
     ):
         return await self._publish_js(
             subject=subject,
             message=message,
             timeout=timeout,
             stream=stream,
             headers=headers,
@@ -392,15 +408,17 @@
     async def _publish_js(
             self,
             subject: str,
             message,
             timeout: float = None,
             stream: str = None,
             data_type: type = dict,
-            headers: dict = None
+            headers: dict = None,
+            *args,
+            **kwargs
     ) :
         payload: bytes = self.format_message_data_type(message, data_type)
         return await self._js.publish(
                 subject=subject,
                 payload=payload,
                 timeout=timeout,
                 stream=stream,
```

### Comparing `panini-0.8.0a2/panini/managers/schema_manager.py` & `panini-0.8.1/panini/managers/schema_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/managers/task_manager.py` & `panini-0.8.1/panini/managers/task_manager.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/__init__.py` & `panini-0.8.1/panini/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/debug_middleware.py` & `panini-0.8.1/panini/middleware/debug_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/error.py` & `panini-0.8.1/panini/middleware/error.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/nats_timeout.py` & `panini-0.8.1/panini/middleware/nats_timeout.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/prometheus_monitoring.py` & `panini-0.8.1/panini/middleware/prometheus_monitoring.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/reader_emulator_middleware.py` & `panini-0.8.1/panini/middleware/reader_emulator_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/middleware/writer_emulator_middleware.py` & `panini-0.8.1/panini/middleware/writer_emulator_middleware.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/test_client.py` & `panini-0.8.1/panini/test_client.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/utils/helper.py` & `panini-0.8.1/panini/utils/helper.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini/utils/logger.py` & `panini-0.8.1/panini/utils/logger.py`

 * *Files identical despite different names*

### Comparing `panini-0.8.0a2/panini.egg-info/PKG-INFO` & `panini-0.8.1/panini.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panini
-Version: 0.8.0a2
+Version: 0.8.1
 Summary: A python messaging framework for microservices based on NATS
 Home-page: https://github.com/lwinterface/panini
 Author: Op Return SA, developers: Andrii Volotskov, Danylo Tiutiushkin
 Author-email: example@example.com
 License: MIT
 Project-URL: Bug Reports, https://github.com/lwinterface/panini/issues
 Project-URL: Source, https://github.com/lwinterface/panini/
```

### Comparing `panini-0.8.0a2/panini.egg-info/SOURCES.txt` & `panini-0.8.1/panini.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -28,12 +28,13 @@
 panini/managers/task_manager.py
 panini/middleware/__init__.py
 panini/middleware/debug_middleware.py
 panini/middleware/error.py
 panini/middleware/nats_timeout.py
 panini/middleware/prometheus_monitoring.py
 panini/middleware/reader_emulator_middleware.py
+panini/middleware/tracing_middleware.py
 panini/middleware/writer_emulator_middleware.py
 panini/utils/__init__.py
 panini/utils/helper.py
 panini/utils/logger.py
 panini/utils/singleton.py
```

### Comparing `panini-0.8.0a2/setup.py` & `panini-0.8.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - middlewares
 - HTTP server
 
 """
 
 setup(
     name="panini",
-    version="0.8.0a2",
+    version="0.8.1",
     description="A python messaging framework for microservices based on NATS",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/lwinterface/panini",
     author="Op Return SA, developers: Andrii Volotskov, Danylo Tiutiushkin",
     author_email="example@example.com",
     python_requires=">=3.8.3",
```

