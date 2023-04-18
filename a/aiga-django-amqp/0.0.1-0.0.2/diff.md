# Comparing `tmp/aiga-django-amqp-0.0.1.tar.gz` & `tmp/aiga-django-amqp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiga-django-amqp-0.0.1.tar", last modified: Thu Sep  8 19:34:05 2022, max compression
+gzip compressed data, was "aiga-django-amqp-0.0.2.tar", last modified: Tue Mar 28 15:00:59 2023, max compression
```

## Comparing `aiga-django-amqp-0.0.1.tar` & `aiga-django-amqp-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2022-09-08 19:34:05.396963 aiga-django-amqp-0.0.1/
--rw-rw-rw-   0        0        0     1088 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      109 2022-09-08 18:07:36.000000 aiga-django-amqp-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3112 2022-09-08 19:34:05.397966 aiga-django-amqp-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2136 2022-09-08 19:24:51.000000 aiga-django-amqp-0.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2022-09-08 19:34:05.385963 aiga-django-amqp-0.0.1/aiga_amqp/
--rw-rw-rw-   0        0        0        0 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/aiga_amqp/__init__.py
--rw-rw-rw-   0        0        0      155 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/aiga_amqp/apps.py
--rw-rw-rw-   0        0        0     4793 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/aiga_amqp/core.py
--rw-rw-rw-   0        0        0       63 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/aiga_amqp/tests.py
-drwxrwxrwx   0        0        0        0 2022-09-08 19:34:05.395963 aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/
--rw-rw-rw-   0        0        0     3112 2022-09-08 19:34:05.000000 aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2022-09-08 19:34:05.000000 aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-09-08 19:34:05.000000 aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2022-09-08 19:34:05.000000 aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-09-08 19:34:05.000000 aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      110 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      990 2022-09-08 19:34:05.398965 aiga-django-amqp-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0       37 2022-09-08 17:50:06.000000 aiga-django-amqp-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-28 15:00:59.130000 aiga-django-amqp-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-03-28 14:58:38.000000 aiga-django-amqp-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      109 2022-09-08 18:07:38.000000 aiga-django-amqp-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     3089 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2136 2022-09-08 19:24:52.000000 aiga-django-amqp-0.0.2/README.rst
+drwxrwxrwx   0        0        0        0 2023-03-28 15:00:59.130000 aiga-django-amqp-0.0.2/aiga_amqp/
+-rw-rw-rw-   0        0        0        0 2022-09-08 17:50:08.000000 aiga-django-amqp-0.0.2/aiga_amqp/__init__.py
+-rw-rw-rw-   0        0        0      155 2022-09-08 17:50:08.000000 aiga-django-amqp-0.0.2/aiga_amqp/apps.py
+-rw-rw-rw-   0        0        0     4585 2023-03-28 14:54:00.000000 aiga-django-amqp-0.0.2/aiga_amqp/core.py
+-rw-rw-rw-   0        0        0       63 2022-09-08 17:50:08.000000 aiga-django-amqp-0.0.2/aiga_amqp/tests.py
+drwxrwxrwx   0        0        0        0 2023-03-28 15:00:59.140000 aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/
+-rw-rw-rw-   0        0        0     3089 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      110 2022-09-08 17:50:08.000000 aiga-django-amqp-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      990 2023-03-28 15:01:00.000000 aiga-django-amqp-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       37 2022-09-08 17:50:08.000000 aiga-django-amqp-0.0.2/setup.py
```

### Comparing `aiga-django-amqp-0.0.1/LICENSE` & `aiga-django-amqp-0.0.2/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Arik Subagia
+Copyright (c) 2023 Arik Subagia
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `aiga-django-amqp-0.0.1/PKG-INFO` & `aiga-django-amqp-0.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: aiga-django-amqp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django app yang digunakan untuk mempermudah penggunaan rabbit mq
 Home-page: https://github.com/ariksubagia/aiga-django-amqp
 Author: I Putu Arik Subagia, S.kom
 Author-email: ariksubagia@ymail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -93,9 +92,7 @@
         'PORT' : 5672,          //port dari rabbitmq
         'CREDENTIAL' : False,   //set menjadi True jika menggunakan USERNAME dan PASSWORD
         'USERNAME' : None,      //username untuk mengakses rabbitmq
         'PASSWORD' : None,      //password untuk mengakses rabbitmq
         'HEARTBEAT' : 600,
         'TIMEOUT' : 300
     }
-
-
```

### Comparing `aiga-django-amqp-0.0.1/README.rst` & `aiga-django-amqp-0.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `aiga-django-amqp-0.0.1/aiga_amqp/core.py` & `aiga-django-amqp-0.0.2/aiga_amqp/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,27 +38,22 @@
         self.__connection_parameters = pika.ConnectionParameters(**params)
 
         super().__init__(self.__connection_parameters, None)
 
 class AMQPListener:
     ExchangeType = ExchangeType
 
-    def __init__(self):
-        self.connection = self.__connect()
-
-    def __connect(self):
+    def connect(self):
         return AMQPConnector()
 
-    def __disconnect(self):
-        self.connection.close()
-
     def consume(self, consumer, channel_name = None):
         def runner():
+            connection = self.connect()
             ch_name = channel_name
-            channel = self.connection.channel()
+            channel = connection.channel()
             channel.queue_declare(queue=ch_name)
             channel.basic_qos(prefetch_count=1)
 
             def callback(channel, method, properties, body):
                 consumer(channel, method, properties, body)
                 channel.basic_ack(delivery_tag=method.delivery_tag)
 
@@ -68,16 +63,17 @@
         thread = Thread(name=uuid4(), target=runner)
         thread.daemon = True
         thread.start()
         return thread
 
     def subscribe(self, consumer, exchange_key = None, routing_key = '', exchange_type = ExchangeType.fanout):
         def runner():
+            connection = self.connect()
             ch_name = exchange_key
-            channel = self.connection.channel()
+            channel = connection.channel()
 
             exchange_declaration_params = {
                 'exchange' : ch_name,
                 'exchange_type' : exchange_type
             }
 
             channel.exchange_declare(**exchange_declaration_params)
@@ -101,20 +97,14 @@
             channel.start_consuming()
 
         thread = Thread(name=uuid4(), target=runner)
         thread.daemon = True
         thread.start()
         return thread
 
-    def __enter__(self):
-        print(self.connection)
-
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.__disconnect()
-
 # function untuk mengirim queue ke rabbit mq
 def send_queue(channel : str, message : str):
     connection = AMQPConnector()
     ch = connection.channel()
     ch.queue_declare(queue=channel)
     ch.basic_publish('', routing_key=channel, body=message)
     connection.close()
```

### Comparing `aiga-django-amqp-0.0.1/aiga_django_amqp.egg-info/PKG-INFO` & `aiga-django-amqp-0.0.2/aiga_django_amqp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: aiga-django-amqp
-Version: 0.0.1
+Version: 0.0.2
 Summary: Django app yang digunakan untuk mempermudah penggunaan rabbit mq
 Home-page: https://github.com/ariksubagia/aiga-django-amqp
 Author: I Putu Arik Subagia, S.kom
 Author-email: ariksubagia@ymail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -93,9 +92,7 @@
         'PORT' : 5672,          //port dari rabbitmq
         'CREDENTIAL' : False,   //set menjadi True jika menggunakan USERNAME dan PASSWORD
         'USERNAME' : None,      //username untuk mengakses rabbitmq
         'PASSWORD' : None,      //password untuk mengakses rabbitmq
         'HEARTBEAT' : 600,
         'TIMEOUT' : 300
     }
-
-
```

### Comparing `aiga-django-amqp-0.0.1/setup.cfg` & `aiga-django-amqp-0.0.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 6967 612d 646a 616e 676f 2d61   = aiga-django-a
 00000020: 6d71 700d 0a76 6572 7369 6f6e 203d 2030  mqp..version = 0
-00000030: 2e30 2e31 0d0a 6465 7363 7269 7074 696f  .0.1..descriptio
+00000030: 2e30 2e32 0d0a 6465 7363 7269 7074 696f  .0.2..descriptio
 00000040: 6e20 3d20 446a 616e 676f 2061 7070 2079  n = Django app y
 00000050: 616e 6720 6469 6775 6e61 6b61 6e20 756e  ang digunakan un
 00000060: 7475 6b20 6d65 6d70 6572 6d75 6461 6820  tuk mempermudah 
 00000070: 7065 6e67 6775 6e61 616e 2072 6162 6269  penggunaan rabbi
 00000080: 7420 6d71 0d0a 6c6f 6e67 5f64 6573 6372  t mq..long_descr
 00000090: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 000000a0: 4541 444d 452e 7273 740d 0a75 726c 203d  EADME.rst..url =
```

