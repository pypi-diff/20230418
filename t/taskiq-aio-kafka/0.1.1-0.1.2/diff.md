# Comparing `tmp/taskiq_aio_kafka-0.1.1.tar.gz` & `tmp/taskiq_aio_kafka-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_kafka-0.1.1.tar", max compression
+gzip compressed data, was "taskiq_aio_kafka-0.1.2.tar", max compression
```

## Comparing `taskiq_aio_kafka-0.1.1.tar` & `taskiq_aio_kafka-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/LICENSE
--rw-r--r--   0        0        0     1388 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/README.md
--rw-r--r--   0        0        0     1749 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      121 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/__init__.py
--rw-r--r--   0        0        0     8007 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/broker.py
--rw-r--r--   0        0        0      178 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/exceptions.py
--rw-r--r--   0        0        0     2964 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/models.py
--rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 taskiq_aio_kafka-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1284 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/README.md
+-rw-r--r--   0        0        0     1749 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/__init__.py
+-rw-r--r--   0        0        0     7709 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/broker.py
+-rw-r--r--   0        0        0      178 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/exceptions.py
+-rw-r--r--   0        0        0     2964 2023-04-18 08:40:14.883449 taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/models.py
+-rw-r--r--   0        0        0     2652 1970-01-01 00:00:00.000000 taskiq_aio_kafka-0.1.2/PKG-INFO
```

### Comparing `taskiq_aio_kafka-0.1.1/LICENSE` & `taskiq_aio_kafka-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aio_kafka-0.1.1/README.md` & `taskiq_aio_kafka-0.1.2/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -34,11 +34,9 @@
 ## Configuration
 
 AioKafkaBroker parameters:
 * `bootstrap_servers` - url to kafka nodes. Can be either string or list of strings.
 * `kafka_topic` - custom topic in kafka.
 * `result_backend` - custom result backend.
 * `task_id_generator` - custom task_id genertaor.
-* `aiokafka_producer` - custom `aiokafka` producer.
-* `aiokafka_consumer` - custom `aiokafka` consumer.
 * `kafka_admin_client` - custom `kafka` admin client.
 * `delete_topic_on_shutdown` - flag to delete topic on broker shutdown.
```

### Comparing `taskiq_aio_kafka-0.1.1/pyproject.toml` & `taskiq_aio_kafka-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-aio-kafka"
 description = "Kafka broker for taskiq"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.1"
+version = "0.1.2"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
```

### Comparing `taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/broker.py` & `taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/broker.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,41 +42,37 @@
 
     def __init__(  # noqa: WPS211
         self,
         bootstrap_servers: Optional[Union[str, List[str]]],
         kafka_topic: Optional[NewTopic] = None,
         result_backend: Optional[AsyncResultBackend[_T]] = None,
         task_id_generator: Optional[Callable[[], str]] = None,
-        aiokafka_producer: Optional[AIOKafkaProducer] = None,
-        aiokafka_consumer: Optional[AIOKafkaConsumer] = None,
         kafka_admin_client: Optional[KafkaAdminClient] = None,
         loop: Optional[asyncio.AbstractEventLoop] = None,
         delete_topic_on_shutdown: bool = False,
     ) -> None:
         """Construct a new broker.
 
         :param bootstrap_servers: string with url to kafka or list with urls.
         :param kafka_topic: kafka topic.
         :param result_backend: custom result backend.
         :param task_id_generator: custom task_id generator.
-        :param aiokafka_producer: configured AIOKafkaProducer.
-        :param aiokafka_consumer: configured AIOKafkaConsumer.
         :param kafka_admin_client: configured KafkaAdminClient.
         :param loop: specific even loop.
         :param delete_topic_on_shutdown: delete or don't delete topic on shutdown.
 
         :raises WrongAioKafkaBrokerParametersError: if aiokafka_producer and/or
             aiokafka_consumer were specified but bootstrap_servers wasn't specified.
         """
         super().__init__(result_backend, task_id_generator)
 
-        if (aiokafka_producer or aiokafka_consumer) and not bootstrap_servers:
+        if kafka_admin_client and not bootstrap_servers:
             raise WrongAioKafkaBrokerParametersError(
                 (
-                    "If you specify `aiokafka_producer` and/or `aiokafka_consumer`, "
+                    "If you specify `kafka_admin_client`, "
                     "you must specify `bootstrap_servers`."
                 ),
             )
 
         self._bootstrap_servers: Optional[Union[str, List[str]]] = bootstrap_servers
 
         self._loop: Optional[asyncio.AbstractEventLoop] = loop
```

### Comparing `taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/models.py` & `taskiq_aio_kafka-0.1.2/taskiq_aio_kafka/models.py`

 * *Files identical despite different names*

### Comparing `taskiq_aio_kafka-0.1.1/PKG-INFO` & `taskiq_aio_kafka-0.1.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq-aio-kafka
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kafka broker for taskiq
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async,kafka,aiokafka
 Author: Taskiq team
 Author-email: taskiq@no-reply.com
 Maintainer: Taskiq team
 Maintainer-email: taskiq@no-reply.com
@@ -69,12 +69,10 @@
 ## Configuration
 
 AioKafkaBroker parameters:
 * `bootstrap_servers` - url to kafka nodes. Can be either string or list of strings.
 * `kafka_topic` - custom topic in kafka.
 * `result_backend` - custom result backend.
 * `task_id_generator` - custom task_id genertaor.
-* `aiokafka_producer` - custom `aiokafka` producer.
-* `aiokafka_consumer` - custom `aiokafka` consumer.
 * `kafka_admin_client` - custom `kafka` admin client.
 * `delete_topic_on_shutdown` - flag to delete topic on broker shutdown.
```

