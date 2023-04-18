# Comparing `tmp/gcn-kafka-0.3.0.tar.gz` & `tmp/gcn-kafka-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcn-kafka-0.3.0.tar", last modified: Fri Oct  7 16:15:05 2022, max compression
+gzip compressed data, was "gcn-kafka-0.3.1.tar", last modified: Tue Apr 18 00:53:21 2023, max compression
```

## Comparing `gcn-kafka-0.3.0.tar` & `gcn-kafka-0.3.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 16:15:05.963262 gcn-kafka-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 16:15:05.959261 gcn-kafka-0.3.0/.github/
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 16:15:05.959261 gcn-kafka-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-10-07 16:15:05.963262 gcn-kafka-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6309 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 16:15:05.959261 gcn-kafka-0.3.0/gcn_kafka/
--rw-r--r--   0 runner    (1001) docker     (121)      234 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      176 2022-10-07 16:15:05.000000 gcn-kafka-0.3.0/gcn_kafka/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)     4738 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/core.py
--rw-r--r--   0 runner    (1001) docker     (121)     1558 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/env.py
--rw-r--r--   0 runner    (1001) docker     (121)     1061 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/oidc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 16:15:05.963262 gcn-kafka-0.3.0/gcn_kafka/test/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      896 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/test/test_core.py
--rw-r--r--   0 runner    (1001) docker     (121)      428 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/test/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/gcn_kafka/test/test_oidc.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 16:15:05.959261 gcn-kafka-0.3.0/gcn_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6978 2022-10-07 16:15:05.000000 gcn-kafka-0.3.0/gcn_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-10-07 16:15:05.000000 gcn-kafka-0.3.0/gcn_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 16:15:05.000000 gcn-kafka-0.3.0/gcn_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-10-07 16:15:05.000000 gcn-kafka-0.3.0/gcn_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-10-07 16:15:05.000000 gcn-kafka-0.3.0/gcn_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1136 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-07 16:15:05.963262 gcn-kafka-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-10-07 16:14:48.000000 gcn-kafka-0.3.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      473 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7048 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6475 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/gcn_kafka/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/oidc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/gcn_kafka/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/gcn_kafka/test/test_oidc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/gcn_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-18 00:53:21.000000 gcn-kafka-0.3.1/gcn_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:53:21.387466 gcn-kafka-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-18 00:53:04.000000 gcn-kafka-0.3.1/tox.ini
```

### Comparing `gcn-kafka-0.3.0/.github/workflows/codeql-analysis.yml` & `gcn-kafka-0.3.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/LICENSE.txt` & `gcn-kafka-0.3.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/PKG-INFO` & `gcn-kafka-0.3.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcn-kafka
-Version: 0.3.0
+Version: 0.3.1
 Summary: Kafka client for NASA's General Coordinates Network (GCN)
 Author-email: Leo Singer <leo.p.singer@nasa.gov>, Tom Barclay <tb@umbc.edu>, Eric Burns <ericburns@lsu.edu>
 License: CC0-1.0
 Project-URL: source, https://github.com/nasa-gcn/gcn-kafka-python
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
@@ -54,21 +54,28 @@
 
 Subscribe to topics and receive alerts:
 
 ```python
 consumer.subscribe(['gcn.classic.text.FERMI_GBM_FIN_POS',
                     'gcn.classic.text.LVC_INITIAL'])
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
 ```
 
+The `timeout` argument to `consume()`, given as an integer number of seconds,
+will allow the program to exit quickly once it has reached the end of the
+existing message buffer. This is useful for users who just want to recover an
+older message from the stream. `timeout` will also make the `while True`
+infinite loop interruptible via the standard ctrl-c key sequence, which
+`consume()` ignores.
+
 ## Testing and Development Kafka Clusters
 
-GCN has three Kafka clusters: production, testing, and an internal development deployment. Use the optional ``domain`` keyword argument to select which broker to connect to.
+GCN has three Kafka clusters: production, testing, and an internal development deployment. Use the optional `domain` keyword argument to select which broker to connect to.
 
 ```python
 # Production (default)
 consumer = Consumer(client_id='fill me in',
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
@@ -102,15 +109,15 @@
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
 topics = ['gcn.classic.voevent.FERMI_GBM_SUBTHRESH']
 consumer.subscribe(topics)
 
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
         consumer.commit(message)
 ```
 
 **How can I read messages beginning at the earliest available messages for a given stream?**
 
 You can begin reading a given topic stream from the earliest message that is present in the stream buffer by setting the Group ID to an empty string and applying the ‘earliest’ setting for the auto offset reset option in the configuration dictionary argument for the Consumer class. This feature allows the user to scan for older messages for testing purposes or to recover messages that may have been missed due to a crash or network outage. Just keep in mind that the stream buffers are finite in size. They currently hold messages from the past few days.
@@ -127,23 +134,21 @@
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
 topics = ['gcn.classic.voevent.INTEGRAL_SPIACS']
 consumer.subscribe(topics)
 
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
 ```
 
-Note: Adding a timeout argument, given as an integer number of seconds, to consume() will allow the program to exit quickly once it has reached the end of the existing message buffer. This is useful for users who just want to recover an older message from the stream.
-
 **How can I search for messages occurring within a given date range?**
 
-To search for messages in a given date range, you can use the offsets_for_times() function from the Consumer class to get the message offsets for the desired date range. You can then assign the starting offset to the Consumer and read the desired number of messages. When doing so, keep in mind that the stream buffers are finite in size. It is not possible to recover messages prior to the start of the stream buffer. The GCN stream buffers are currently set to hold messages from the past few days.
+To search for messages in a given date range, you can use the `offsets_for_times()` function from the Consumer class to get the message offsets for the desired date range. You can then assign the starting offset to the Consumer and read the desired number of messages. When doing so, keep in mind that the stream buffers are finite in size. It is not possible to recover messages prior to the start of the stream buffer. The GCN stream buffers are currently set to hold messages from the past few days.
 
 Example code:
 ```python3
 import datetime
 from gcn_kafka import Consumer
 from confluent_kafka import TopicPartition
 
@@ -158,10 +163,10 @@
 topic = 'gcn.classic.voevent.INTEGRAL_SPIACS'
 start = consumer.offsets_for_times(
     [TopicPartition(topic, 0, timestamp1)])
 end = consumer.offsets_for_times(
     [TopicPartition(topic, 0, timestamp2)])
 
 consumer.assign(start)
-for message in consumer.consume(end[0].offset - start[0].offset):
+for message in consumer.consume(end[0].offset - start[0].offset, timeout=1):
     print(message.value())
 ```
```

### Comparing `gcn-kafka-0.3.0/README.md` & `gcn-kafka-0.3.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -37,21 +37,28 @@
 
 Subscribe to topics and receive alerts:
 
 ```python
 consumer.subscribe(['gcn.classic.text.FERMI_GBM_FIN_POS',
                     'gcn.classic.text.LVC_INITIAL'])
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
 ```
 
+The `timeout` argument to `consume()`, given as an integer number of seconds,
+will allow the program to exit quickly once it has reached the end of the
+existing message buffer. This is useful for users who just want to recover an
+older message from the stream. `timeout` will also make the `while True`
+infinite loop interruptible via the standard ctrl-c key sequence, which
+`consume()` ignores.
+
 ## Testing and Development Kafka Clusters
 
-GCN has three Kafka clusters: production, testing, and an internal development deployment. Use the optional ``domain`` keyword argument to select which broker to connect to.
+GCN has three Kafka clusters: production, testing, and an internal development deployment. Use the optional `domain` keyword argument to select which broker to connect to.
 
 ```python
 # Production (default)
 consumer = Consumer(client_id='fill me in',
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
@@ -85,15 +92,15 @@
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
 topics = ['gcn.classic.voevent.FERMI_GBM_SUBTHRESH']
 consumer.subscribe(topics)
 
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
         consumer.commit(message)
 ```
 
 **How can I read messages beginning at the earliest available messages for a given stream?**
 
 You can begin reading a given topic stream from the earliest message that is present in the stream buffer by setting the Group ID to an empty string and applying the ‘earliest’ setting for the auto offset reset option in the configuration dictionary argument for the Consumer class. This feature allows the user to scan for older messages for testing purposes or to recover messages that may have been missed due to a crash or network outage. Just keep in mind that the stream buffers are finite in size. They currently hold messages from the past few days.
@@ -110,23 +117,21 @@
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
 topics = ['gcn.classic.voevent.INTEGRAL_SPIACS']
 consumer.subscribe(topics)
 
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
 ```
 
-Note: Adding a timeout argument, given as an integer number of seconds, to consume() will allow the program to exit quickly once it has reached the end of the existing message buffer. This is useful for users who just want to recover an older message from the stream.
-
 **How can I search for messages occurring within a given date range?**
 
-To search for messages in a given date range, you can use the offsets_for_times() function from the Consumer class to get the message offsets for the desired date range. You can then assign the starting offset to the Consumer and read the desired number of messages. When doing so, keep in mind that the stream buffers are finite in size. It is not possible to recover messages prior to the start of the stream buffer. The GCN stream buffers are currently set to hold messages from the past few days.
+To search for messages in a given date range, you can use the `offsets_for_times()` function from the Consumer class to get the message offsets for the desired date range. You can then assign the starting offset to the Consumer and read the desired number of messages. When doing so, keep in mind that the stream buffers are finite in size. It is not possible to recover messages prior to the start of the stream buffer. The GCN stream buffers are currently set to hold messages from the past few days.
 
 Example code:
 ```python3
 import datetime
 from gcn_kafka import Consumer
 from confluent_kafka import TopicPartition
 
@@ -141,10 +146,10 @@
 topic = 'gcn.classic.voevent.INTEGRAL_SPIACS'
 start = consumer.offsets_for_times(
     [TopicPartition(topic, 0, timestamp1)])
 end = consumer.offsets_for_times(
     [TopicPartition(topic, 0, timestamp2)])
 
 consumer.assign(start)
-for message in consumer.consume(end[0].offset - start[0].offset):
+for message in consumer.consume(end[0].offset - start[0].offset, timeout=1):
     print(message.value())
 ```
```

### Comparing `gcn-kafka-0.3.0/gcn_kafka/core.py` & `gcn-kafka-0.3.1/gcn_kafka/core.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/gcn_kafka/env.py` & `gcn-kafka-0.3.1/gcn_kafka/env.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/gcn_kafka/oidc.py` & `gcn-kafka-0.3.1/gcn_kafka/oidc.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/gcn_kafka/test/test_core.py` & `gcn-kafka-0.3.1/gcn_kafka/test/test_core.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/gcn_kafka/test/test_oidc.py` & `gcn-kafka-0.3.1/gcn_kafka/test/test_oidc.py`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/gcn_kafka.egg-info/PKG-INFO` & `gcn-kafka-0.3.1/gcn_kafka.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcn-kafka
-Version: 0.3.0
+Version: 0.3.1
 Summary: Kafka client for NASA's General Coordinates Network (GCN)
 Author-email: Leo Singer <leo.p.singer@nasa.gov>, Tom Barclay <tb@umbc.edu>, Eric Burns <ericburns@lsu.edu>
 License: CC0-1.0
 Project-URL: source, https://github.com/nasa-gcn/gcn-kafka-python
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
@@ -54,21 +54,28 @@
 
 Subscribe to topics and receive alerts:
 
 ```python
 consumer.subscribe(['gcn.classic.text.FERMI_GBM_FIN_POS',
                     'gcn.classic.text.LVC_INITIAL'])
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
 ```
 
+The `timeout` argument to `consume()`, given as an integer number of seconds,
+will allow the program to exit quickly once it has reached the end of the
+existing message buffer. This is useful for users who just want to recover an
+older message from the stream. `timeout` will also make the `while True`
+infinite loop interruptible via the standard ctrl-c key sequence, which
+`consume()` ignores.
+
 ## Testing and Development Kafka Clusters
 
-GCN has three Kafka clusters: production, testing, and an internal development deployment. Use the optional ``domain`` keyword argument to select which broker to connect to.
+GCN has three Kafka clusters: production, testing, and an internal development deployment. Use the optional `domain` keyword argument to select which broker to connect to.
 
 ```python
 # Production (default)
 consumer = Consumer(client_id='fill me in',
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
@@ -102,15 +109,15 @@
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
 topics = ['gcn.classic.voevent.FERMI_GBM_SUBTHRESH']
 consumer.subscribe(topics)
 
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
         consumer.commit(message)
 ```
 
 **How can I read messages beginning at the earliest available messages for a given stream?**
 
 You can begin reading a given topic stream from the earliest message that is present in the stream buffer by setting the Group ID to an empty string and applying the ‘earliest’ setting for the auto offset reset option in the configuration dictionary argument for the Consumer class. This feature allows the user to scan for older messages for testing purposes or to recover messages that may have been missed due to a crash or network outage. Just keep in mind that the stream buffers are finite in size. They currently hold messages from the past few days.
@@ -127,23 +134,21 @@
                     client_secret='fill me in',
                     domain='gcn.nasa.gov')
 
 topics = ['gcn.classic.voevent.INTEGRAL_SPIACS']
 consumer.subscribe(topics)
 
 while True:
-    for message in consumer.consume():
+    for message in consumer.consume(timeout=1):
         print(message.value())
 ```
 
-Note: Adding a timeout argument, given as an integer number of seconds, to consume() will allow the program to exit quickly once it has reached the end of the existing message buffer. This is useful for users who just want to recover an older message from the stream.
-
 **How can I search for messages occurring within a given date range?**
 
-To search for messages in a given date range, you can use the offsets_for_times() function from the Consumer class to get the message offsets for the desired date range. You can then assign the starting offset to the Consumer and read the desired number of messages. When doing so, keep in mind that the stream buffers are finite in size. It is not possible to recover messages prior to the start of the stream buffer. The GCN stream buffers are currently set to hold messages from the past few days.
+To search for messages in a given date range, you can use the `offsets_for_times()` function from the Consumer class to get the message offsets for the desired date range. You can then assign the starting offset to the Consumer and read the desired number of messages. When doing so, keep in mind that the stream buffers are finite in size. It is not possible to recover messages prior to the start of the stream buffer. The GCN stream buffers are currently set to hold messages from the past few days.
 
 Example code:
 ```python3
 import datetime
 from gcn_kafka import Consumer
 from confluent_kafka import TopicPartition
 
@@ -158,10 +163,10 @@
 topic = 'gcn.classic.voevent.INTEGRAL_SPIACS'
 start = consumer.offsets_for_times(
     [TopicPartition(topic, 0, timestamp1)])
 end = consumer.offsets_for_times(
     [TopicPartition(topic, 0, timestamp2)])
 
 consumer.assign(start)
-for message in consumer.consume(end[0].offset - start[0].offset):
+for message in consumer.consume(end[0].offset - start[0].offset, timeout=1):
     print(message.value())
 ```
```

### Comparing `gcn-kafka-0.3.0/gcn_kafka.egg-info/SOURCES.txt` & `gcn-kafka-0.3.1/gcn_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcn-kafka-0.3.0/pyproject.toml` & `gcn-kafka-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Topic :: Scientific/Engineering :: Astronomy",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: System :: Networking"
 ]
 dependencies = [
     "authlib",
     "certifi",
-    "confluent-kafka >= 1.6.1",
+    "confluent-kafka >= 1.6.1, != 2.1.0",
     "requests",
     "typing-extensions; python_version<='3.7'"
 ]
 requires-python = ">=3.7"
 dynamic = [ "version" ]
 
 [project.urls]
```

