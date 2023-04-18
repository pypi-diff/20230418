# Comparing `tmp/taskiq_aio_kafka-0.1.0.tar.gz` & `tmp/taskiq_aio_kafka-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq_aio_kafka-0.1.0.tar", max compression
+gzip compressed data, was "taskiq_aio_kafka-0.1.1.tar", max compression
```

## Comparing `taskiq_aio_kafka-0.1.0.tar` & `taskiq_aio_kafka-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-04-16 11:23:05.788663 taskiq_aio_kafka-0.1.0/LICENSE
--rw-r--r--   0        0        0      779 2023-04-16 11:23:05.788663 taskiq_aio_kafka-0.1.0/README.md
--rw-r--r--   0        0        0     1728 2023-04-16 11:23:05.788663 taskiq_aio_kafka-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-04-16 11:23:05.788663 taskiq_aio_kafka-0.1.0/taskiq_aio_kafka/__init__.py
--rw-r--r--   0        0        0     6969 2023-04-16 11:23:05.788663 taskiq_aio_kafka-0.1.0/taskiq_aio_kafka/broker.py
--rw-r--r--   0        0        0      178 2023-04-16 11:23:05.788663 taskiq_aio_kafka-0.1.0/taskiq_aio_kafka/exceptions.py
--rw-r--r--   0        0        0     2105 1970-01-01 00:00:00.000000 taskiq_aio_kafka-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1388 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/README.md
+-rw-r--r--   0        0        0     1749 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/__init__.py
+-rw-r--r--   0        0        0     8007 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/broker.py
+-rw-r--r--   0        0        0      178 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/exceptions.py
+-rw-r--r--   0        0        0     2964 2023-04-18 08:23:01.045210 taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/models.py
+-rw-r--r--   0        0        0     2756 1970-01-01 00:00:00.000000 taskiq_aio_kafka-0.1.1/PKG-INFO
```

### Comparing `taskiq_aio_kafka-0.1.0/LICENSE` & `taskiq_aio_kafka-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq_aio_kafka-0.1.0/pyproject.toml` & `taskiq_aio_kafka-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "taskiq-aio-kafka"
 description = "Kafka broker for taskiq"
 authors = ["Taskiq team <taskiq@no-reply.com>"]
 maintainers = ["Taskiq team <taskiq@no-reply.com>"]
-version = "0.1.0"
+version = "0.1.1"
 readme = "README.md"
 license = "LICENSE"
 classifiers = [
     "Typing :: Typed",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -23,14 +23,15 @@
 keywords = ["taskiq", "tasks", "distributed", "async", "kafka", "aiokafka"]
 packages = [{ include = "taskiq_aio_kafka" }]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 taskiq = "^0"
 aiokafka = "^0.8.0"
+pydantic = "^1.10.7"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.2"
 flake8 = "^4.0.1"
 isort = "^5.10.1"
 mypy = "^1.2.0"
 pre-commit = "^2.20.0"
```

### Comparing `taskiq_aio_kafka-0.1.0/taskiq_aio_kafka/broker.py` & `taskiq_aio_kafka-0.1.1/taskiq_aio_kafka/broker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import asyncio
 import pickle  # noqa: S403
 from logging import getLogger
-from typing import AsyncGenerator, Callable, List, Optional, Set, TypeVar, Union
+from typing import Any, AsyncGenerator, Callable, List, Optional, Set, TypeVar, Union
 
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from kafka.admin import KafkaAdminClient, NewTopic
 from taskiq import AsyncResultBackend, BrokerMessage
 from taskiq.abc.broker import AsyncBroker
 
 from taskiq_aio_kafka.exceptions import WrongAioKafkaBrokerParametersError
+from taskiq_aio_kafka.models import KafkaConsumerParameters, KafkaProducerParameters
 
 _T = TypeVar("_T")  # noqa: WPS111
 
 
 logger = getLogger("taskiq.kafka_broker")
 
 
@@ -82,29 +83,20 @@
 
         self._kafka_topic: NewTopic = kafka_topic or NewTopic(
             name="taskiq_topic",
             num_partitions=1,
             replication_factor=1,
         )
 
-        self._aiokafka_producer: AIOKafkaProducer = (
-            aiokafka_producer
-            or AIOKafkaProducer(
-                bootstrap_servers=self._bootstrap_servers,
-                loop=self._loop,
-            )
+        self._aiokafka_producer_params: KafkaProducerParameters = (
+            KafkaProducerParameters()
         )
 
-        self._aiokafka_consumer: AIOKafkaConsumer = (
-            aiokafka_consumer
-            or AIOKafkaConsumer(
-                self._kafka_topic.name,
-                bootstrap_servers=self._bootstrap_servers,
-                loop=self._loop,
-            )
+        self._aiokafka_consumer_params: KafkaConsumerParameters = (
+            KafkaConsumerParameters()
         )
 
         self._kafka_admin_client: KafkaAdminClient = (
             kafka_admin_client
             or KafkaAdminClient(
                 bootstrap_servers=self._bootstrap_servers,
                 client_id="kafka-python-taskiq",
@@ -114,48 +106,83 @@
         self._delete_topic_on_shutdown: bool = delete_topic_on_shutdown
 
         self._delay_kick_tasks: Set[asyncio.Task[None]] = set()
 
         self._is_producer_started = False
         self._is_consumer_started = False
 
+    def configure_producer(self, **producer_parameters: Any) -> None:
+        """Configure kafka producer.
+
+        You can pass here any configuration parameters
+        accepted by the kafka producer.
+
+        :param producer_parameters: producer parameters kwargs.
+        """
+        self._aiokafka_producer_params = KafkaProducerParameters(
+            **producer_parameters,
+        )
+
+    def configure_consumer(self, **consumer_parameters: Any) -> None:
+        """Configure kafka consumer.
+
+        You can pass here any configuration parameters
+        accepted by the kafka consumer.
+
+        :param consumer_parameters: consumer parameters kwargs.
+        """
+        self._aiokafka_consumer_params = KafkaConsumerParameters(
+            **consumer_parameters,
+        )
+
     async def startup(self) -> None:
         """Setup AIOKafkaProducer, AIOKafkaConsumer and kafka topics.
 
         We will have 2 topics for default and high priority.
 
         Also we need to create AIOKafkaProducer and AIOKafkaConsumer
         if there are no producer and consumer passed.
         """
         await super().startup()
-
-        is_topic_available: bool = bool(
-            self._kafka_admin_client.describe_topics([self._kafka_topic.name]),
+        available_condition: bool = (
+            self._kafka_topic.name not in self._kafka_admin_client.list_topics()
         )
-        if not is_topic_available:
+        if available_condition:
             self._kafka_admin_client.create_topics(
                 new_topics=[self._kafka_topic],
                 validate_only=False,
             )
-
+        self._aiokafka_producer = AIOKafkaProducer(
+            bootstrap_servers=self._bootstrap_servers,
+            loop=self._loop,
+            **self._aiokafka_producer_params.dict(),
+        )
         await self._aiokafka_producer.start()
+
         if self.is_worker_process:
+            self._aiokafka_consumer = AIOKafkaConsumer(
+                self._kafka_topic.name,
+                bootstrap_servers=self._bootstrap_servers,
+                loop=self._loop,
+                **self._aiokafka_consumer_params.dict(),
+            )
+
             await self._aiokafka_consumer.start()
             self._is_consumer_started = True
 
         self._is_producer_started = True
 
     async def shutdown(self) -> None:
         """Close all connections on shutdown."""
         await super().shutdown()
 
-        if self._aiokafka_producer:
+        if self._is_producer_started:
             await self._aiokafka_producer.stop()
 
-        if self._aiokafka_consumer:
+        if self._is_consumer_started:
             await self._aiokafka_consumer.stop()
 
         topic_delete_condition: bool = all(
             (
                 self._delete_topic_on_shutdown,
                 self._kafka_topic.name  # type: ignore
                 in self._kafka_admin_client.list_topics(),  # type: ignore
@@ -179,20 +206,19 @@
 
         :raises ValueError: if startup wasn't called.
         :param message: message to send.
         """
         if not self._is_producer_started:
             raise ValueError("Please run startup before kicking.")
 
-        kafka_message: bytes = pickle.dumps(message)
         topic_name: str = self._kafka_topic.name
 
-        await self._aiokafka_producer.send(
+        await self._aiokafka_producer.send(  # type: ignore
             topic=topic_name,
-            value=kafka_message,
+            value=message.message,
         )
 
     async def listen(
         self,
     ) -> AsyncGenerator[bytes, None]:
         """Listen to topic.
 
@@ -201,9 +227,9 @@
 
         :yields: parsed broker message.
         :raises ValueError: if no aiokafka_consumer or startup wasn't called.
         """
         if not self._is_consumer_started:
             raise ValueError("Please run startup before listening.")
 
-        async for raw_kafka_message in self._aiokafka_consumer:
+        async for raw_kafka_message in self._aiokafka_consumer:  # type: ignore
             yield raw_kafka_message.value
```

