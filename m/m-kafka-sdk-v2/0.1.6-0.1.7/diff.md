# Comparing `tmp/m-kafka-sdk-v2-0.1.6.tar.gz` & `tmp/m-kafka-sdk-v2-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-kafka-sdk-v2-0.1.6.tar", last modified: Wed Apr  5 04:34:12 2023, max compression
+gzip compressed data, was "m-kafka-sdk-v2-0.1.7.tar", last modified: Tue Apr 18 07:26:34 2023, max compression
```

## Comparing `m-kafka-sdk-v2-0.1.6.tar` & `m-kafka-sdk-v2-0.1.7.tar`

### file list

```diff
@@ -1,29 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.721241 m-kafka-sdk-v2-0.1.6/
--rw-r--r--   0 root         (0) root         (0)     5101 2023-04-05 04:34:12.720241 m-kafka-sdk-v2-0.1.6/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)     3523 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.713241 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5101 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      721 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)       74 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.706241 m-kafka-sdk-v2-0.1.6/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.714241 m-kafka-sdk-v2-0.1.6/mobio/libs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.714241 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/
--rw-r--r--   0 root         (0) root         (0)      945 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.717241 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/
--rw-r--r--   0 root         (0) root         (0)     1326 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     7683 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py
--rw-r--r--   0 root         (0) root         (0)     5741 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.717241 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-05 04:34:12.719241 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/mongo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/mongo/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     6321 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/mongo/base_model.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/mongo/requeue_consumer_model.py
--rw-r--r--   0 root         (0) root         (0)      103 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.6/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-05 04:34:12.721241 m-kafka-sdk-v2-0.1.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9285 2023-04-05 04:34:12.000000 m-kafka-sdk-v2-0.1.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.567829 m-kafka-sdk-v2-0.1.7/
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-04-18 07:26:34.567829 m-kafka-sdk-v2-0.1.7/PKG-INFO
+-rwxr-xr-x   0 root         (0) root         (0)     3806 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.558828 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5416 2023-04-18 07:26:34.000000 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      766 2023-04-18 07:26:34.000000 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 07:26:34.000000 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-18 07:26:34.000000 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-18 07:26:34.000000 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-18 07:26:34.000000 m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.549828 m-kafka-sdk-v2-0.1.7/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.558828 m-kafka-sdk-v2-0.1.7/mobio/libs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.559828 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.562828 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/
+-rw-r--r--   0 root         (0) root         (0)     1326 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     8054 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py
+-rw-r--r--   0 root         (0) root         (0)     5714 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py
+-rw-r--r--   0 root         (0) root         (0)     1736 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.563829 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.565829 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/mongo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/mongo/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     6321 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/mongo/base_model.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/mongo/requeue_consumer_model.py
+-rw-r--r--   0 root         (0) root         (0)      103 2023-04-05 04:32:23.000000 m-kafka-sdk-v2-0.1.7/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 07:26:34.568829 m-kafka-sdk-v2-0.1.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9245 2023-04-18 07:26:33.000000 m-kafka-sdk-v2-0.1.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 07:26:34.566829 m-kafka-sdk-v2-0.1.7/test/
+-rw-r--r--   0 root         (0) root         (0)      655 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/test/test_consumer.py
+-rw-r--r--   0 root         (0) root         (0)      829 2023-04-18 07:24:54.000000 m-kafka-sdk-v2-0.1.7/test/test_singleton.py
```

### Comparing `m-kafka-sdk-v2-0.1.6/PKG-INFO` & `m-kafka-sdk-v2-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-kafka-sdk-v2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mobio Kafka SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: - **Thư viện Consumer của JB. Chạy consumer ở Process, phù hợp cho môi trường K8s** :
@@ -80,14 +80,18 @@
             client_mongo = MongoClient(url_connection, connect=False)
         
             TestConsumer(topic_name="test", group_id="test", client_mongo=client_mongo, retryable=False)
             sleep(1000)
         ```
         
         # change logs
+        * 0.1.7 (2023-04-18):
+            * cho phép truyền vào broker khi khởi tạo consumer, producer. Nếu không truyền thì sẽ lấy mặc định trong ENV KAFKA_BROKER
+            * singleton producer với *args && **kwargs
+            * bỏ requirements "m-singleton>=0.3", "m-caching>=0.1.8"
         * 0.1.6 (2023-04-05):
             * k8s liveness v2
         * 0.1.5 (2022-10-12):
             * raise exception khi close kafka, đảm bảo k8s sẽ restart lại pod
         * 0.1.4.2 (2022-09-19):
             * fix bug topic được tạo đang random vào cả các broker isolate cho module khác.
         * 0.1.4.1 (2022-09-19):
```

### Comparing `m-kafka-sdk-v2-0.1.6/README.md` & `m-kafka-sdk-v2-0.1.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,14 +71,18 @@
     client_mongo = MongoClient(url_connection, connect=False)
 
     TestConsumer(topic_name="test", group_id="test", client_mongo=client_mongo, retryable=False)
     sleep(1000)
 ```
 
 # change logs
+* 0.1.7 (2023-04-18):
+    * cho phép truyền vào broker khi khởi tạo consumer, producer. Nếu không truyền thì sẽ lấy mặc định trong ENV KAFKA_BROKER
+    * singleton producer với *args && **kwargs
+    * bỏ requirements "m-singleton>=0.3", "m-caching>=0.1.8"
 * 0.1.6 (2023-04-05):
     * k8s liveness v2
 * 0.1.5 (2022-10-12):
     * raise exception khi close kafka, đảm bảo k8s sẽ restart lại pod
 * 0.1.4.2 (2022-09-19):
     * fix bug topic được tạo đang random vào cả các broker isolate cho module khác.
 * 0.1.4.1 (2022-09-19):
```

### Comparing `m-kafka-sdk-v2-0.1.6/m_kafka_sdk_v2.egg-info/PKG-INFO` & `m-kafka-sdk-v2-0.1.7/m_kafka_sdk_v2.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-kafka-sdk-v2
-Version: 0.1.6
+Version: 0.1.7
 Summary: Mobio Kafka SDK
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: - **Thư viện Consumer của JB. Chạy consumer ở Process, phù hợp cho môi trường K8s** :
@@ -80,14 +80,18 @@
             client_mongo = MongoClient(url_connection, connect=False)
         
             TestConsumer(topic_name="test", group_id="test", client_mongo=client_mongo, retryable=False)
             sleep(1000)
         ```
         
         # change logs
+        * 0.1.7 (2023-04-18):
+            * cho phép truyền vào broker khi khởi tạo consumer, producer. Nếu không truyền thì sẽ lấy mặc định trong ENV KAFKA_BROKER
+            * singleton producer với *args && **kwargs
+            * bỏ requirements "m-singleton>=0.3", "m-caching>=0.1.8"
         * 0.1.6 (2023-04-05):
             * k8s liveness v2
         * 0.1.5 (2022-10-12):
             * raise exception khi close kafka, đảm bảo k8s sẽ restart lại pod
         * 0.1.4.2 (2022-09-19):
             * fix bug topic được tạo đang random vào cả các broker isolate cho module khác.
         * 0.1.4.1 (2022-09-19):
```

### Comparing `m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/__init__.py` & `m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py` & `m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/ensure_kafka_topic.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,20 @@
 from confluent_kafka.cimpl import NewTopic
 import random
 from mobio.libs.kafka_lib import MobioEnvironment, KAFKA_BOOTSTRAP
 import inspect
 
 
 class EnsureKafkaTopic:
+    def __init__(self, bootstrap_server=None):
+        if bootstrap_server:
+            self.bootstrap_server = bootstrap_server
+        else:
+            self.bootstrap_server = KAFKA_BOOTSTRAP
+
     TOPIC_NAME = "topic"
     NUM_PARTITIONS = "num_partitions"
     REPLICATION_FACTOR = "replication_factor"
     CONFIG = "config"
     REPLICATION_ASSIGNMENT = "replica_assignment"
 
     @classmethod
@@ -24,15 +30,15 @@
             if not (a[0].startswith("__") and a[0].endswith("__"))
         ]
         return values
 
     def create_kafka_topics(self, lst_topic: list):
         all_property = self.get_all_property()
         new_topics = []
-        admin_client = AdminClient({"bootstrap.servers": KAFKA_BOOTSTRAP})
+        admin_client = AdminClient({"bootstrap.servers": self.bootstrap_server})
         existing_topics = list(admin_client.list_topics().topics.keys())
         for topic in lst_topic:
             if topic.get(self.TOPIC_NAME) not in existing_topics:
                 if not topic.get(self.REPLICATION_FACTOR):
                     topic[self.REPLICATION_FACTOR] = int(
                         os.getenv(MobioEnvironment.KAFKA_REPLICATION_FACTOR)
                     )
@@ -67,28 +73,28 @@
                 try:
                     f.result()  # The result itself is None
                     print("New Topic {} created".format(topic))
                 except Exception as e:
                     print("Failed to create new topic {}: {}".format(topic, e))
 
     def delete_kafka_topics(self, lst_topic: list):
-        admin_client = AdminClient({"bootstrap.servers": KAFKA_BOOTSTRAP})
+        admin_client = AdminClient({"bootstrap.servers": self.bootstrap_server})
         fs = admin_client.delete_topics(lst_topic, operation_timeout=30)
 
         # Wait for each operation to finish.
         for topic, f in fs.items():
             try:
                 f.result()  # The result itself is None
                 print("Topic {} deleted".format(topic))
             except Exception as e:
                 print("Failed to delete topic {}: {}".format(topic, e))
 
 
-def create_kafka_topics(lst_topic):
-    admin_client = AdminClient({"bootstrap.servers": KAFKA_BOOTSTRAP})
+def create_kafka_topics(lst_topic, bootstrap_server=None):
+    admin_client = AdminClient({"bootstrap.servers": bootstrap_server if bootstrap_server else KAFKA_BOOTSTRAP})
     existing_topics = list(admin_client.list_topics().topics.keys())
     new_topics = []
     for required_topic in lst_topic:
         if required_topic not in existing_topics:
             new_topics.append(
                 NewTopic(
                     required_topic,
@@ -109,16 +115,16 @@
             try:
                 f.result()  # The result itself is None
                 print("New Topic {} created".format(topic))
             except Exception as e:
                 print("Failed to create new topic {}: {}".format(topic, e))
 
 
-def create_kafka_topics_v2(lst_topic):
-    admin_client = AdminClient({"bootstrap.servers": KAFKA_BOOTSTRAP})
+def create_kafka_topics_v2(lst_topic, bootstrap_server=None):
+    admin_client = AdminClient({"bootstrap.servers": bootstrap_server if bootstrap_server else KAFKA_BOOTSTRAP})
     existing_topics = list(admin_client.list_topics().topics.keys())
     new_topics = []
     for required_topic in lst_topic:
         if (
             type(required_topic) != tuple
             or len(required_topic) < 2
             or type(required_topic[1]) != int
@@ -151,15 +157,15 @@
                 f.result()  # The result itself is None
                 print("New Topic {} created".format(topic))
             except Exception as e:
                 print("Failed to create new topic {}: {}".format(topic, e))
 
 
 if __name__ == "__main__":
-    EnsureKafkaTopic().create_kafka_topics(
+    EnsureKafkaTopic(bootstrap_server="127.0.0.1:9092").create_kafka_topics(
         [
             # TEST WITH SET replica_assignment
             {
                 EnsureKafkaTopic.TOPIC_NAME: "giang-test1",
                 EnsureKafkaTopic.NUM_PARTITIONS: 8,
                 EnsureKafkaTopic.CONFIG: {"compression.type": "snappy"},
                 EnsureKafkaTopic.REPLICATION_ASSIGNMENT: os.getenv(
```

### Comparing `m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py` & `m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/kafka_consumer_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from mobio.libs.kafka_lib import RequeueStatus, KAFKA_BOOTSTRAP
 from mobio.libs.kafka_lib.helpers import consumer_warning_slack
 from mobio.libs.kafka_lib.models.mongo.requeue_consumer_model import (
     RequeueConsumerModel,
 )
 from time import time, sleep
 from uuid import uuid4
-from os.path import exists
 import os
 
 
 class BaseKafkaConsumer:
     def __init__(
             self,
             topic_name: object,
```

### Comparing `m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py` & `m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/helpers/kafka_producer_manager.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import json
 from confluent_kafka.cimpl import Producer, KafkaException, KafkaError
-from mobio.libs.Singleton import Singleton
-
-from mobio.libs.kafka_lib import KAFKA_BOOTSTRAP
+from mobio.libs.kafka_lib import KAFKA_BOOTSTRAP, SingletonArgs
 
 
 def error_cb(err):
     print("Client error: {}".format(err))
     if err.code() == KafkaError._ALL_BROKERS_DOWN or \
        err.code() == KafkaError._AUTHENTICATION:
         # Any exception raised from this callback will be re-raised from the
         # triggering flush() or poll() call.
         raise KafkaException(err)
 
 
-@Singleton
-class KafkaProducerManager:
-    producer = Producer(
-                {
-                    "request.timeout.ms": 20000,
-                    "bootstrap.servers": KAFKA_BOOTSTRAP,
-                    "compression.type": "zstd",
-                    "linger.ms": 10,
-                    # 'error_cb': error_cb,
-                })
+class KafkaProducerManager(metaclass=SingletonArgs):
+    bootstrap_server = None
+
+    def __init__(self, bootstrap_server=None):
+        if bootstrap_server:
+            self.bootstrap_server = bootstrap_server
+        else:
+            self.bootstrap_server = KAFKA_BOOTSTRAP
+
+        self.producer = Producer(
+                    {
+                        "request.timeout.ms": 20000,
+                        "bootstrap.servers": self.bootstrap_server,
+                        "compression.type": "zstd",
+                        "linger.ms": 10,
+                        # 'error_cb': error_cb,
+                    })
 
     def flush_message(self, topic: str, key: str, value):
         self.producer.produce(
             topic=topic,
             key=key,
             value=json.dumps(value).encode("utf-8"),
             on_delivery=self.kafka_delivery_report,
```

### Comparing `m-kafka-sdk-v2-0.1.6/mobio/libs/kafka_lib/models/mongo/base_model.py` & `m-kafka-sdk-v2-0.1.7/mobio/libs/kafka_lib/models/mongo/base_model.py`

 * *Files identical despite different names*

### Comparing `m-kafka-sdk-v2-0.1.6/setup.py` & `m-kafka-sdk-v2-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,20 +20,20 @@
 
     @staticmethod
     def get():
         """Retrieve all dependencies for this project
         :param filename:
         :return:
         """
-        requirements = ["m-singleton>=0.3", "m-caching>=0.1.8", "requests>=2.25.1", "confluent-kafka>=1.7.0"]
+        requirements = ["requests>=2.25.1", "confluent-kafka>=1.7.0"]
         return requirements
 
 
 version_dev='0.1.5'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
-version_prod='0.1.6'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
+version_prod='0.1.7'  # Giữ nguyên định dạng không được format file có khoảng trống theo Pycharm (version_dev = '1.0.9' là file run.sh sẽ không bắt được current_version)
 
 run_mode = ''
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -48,15 +48,15 @@
     name="m-kafka-sdk-v2" + run_mode,  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='0.1.6',  # Required, Phần này cũng không được format file.
+    version='0.1.7',  # Required, Phần này cũng không được format file.
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Mobio Kafka SDK",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

