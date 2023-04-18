# Comparing `tmp/djpykafka-0.0.8.tar.gz` & `tmp/djpykafka-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djpykafka-0.0.8.tar", last modified: Thu Jul 28 09:30:00 2022, max compression
+gzip compressed data, was "djpykafka-0.0.9.tar", last modified: Thu Jul 28 10:03:28 2022, max compression
```

## Comparing `djpykafka-0.0.8.tar` & `djpykafka-0.0.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.672526 djpykafka-0.0.8/
--rw-rw-rw-   0        0        0    26438 2022-05-05 06:07:09.000000 djpykafka-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      332 2021-04-29 13:46:13.000000 djpykafka-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0      578 2022-07-28 09:30:00.673526 djpykafka-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-05-04 09:33:38.000000 djpykafka-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.639526 djpykafka-0.0.8/djpykafka/
--rw-rw-rw-   0        0        0       47 2022-05-04 09:44:14.000000 djpykafka-0.0.8/djpykafka/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.654527 djpykafka-0.0.8/djpykafka/events/
--rw-rw-rw-   0        0        0       48 2022-05-04 12:48:57.000000 djpykafka-0.0.8/djpykafka/events/__init__.py
--rw-rw-rw-   0        0        0     8148 2022-06-27 06:36:03.000000 djpykafka-0.0.8/djpykafka/events/publish.py
--rw-rw-rw-   0        0        0     6247 2022-07-28 09:28:46.000000 djpykafka-0.0.8/djpykafka/events/subscribe.py
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.658527 djpykafka-0.0.8/djpykafka/handlers/
--rw-rw-rw-   0        0        0       32 2022-05-04 11:53:09.000000 djpykafka-0.0.8/djpykafka/handlers/__init__.py
--rw-rw-rw-   0        0        0     3896 2022-06-07 07:46:15.000000 djpykafka-0.0.8/djpykafka/handlers/event_consumer.py
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.663525 djpykafka-0.0.8/djpykafka/models/
--rw-rw-rw-   0        0        0       37 2022-06-23 07:51:49.000000 djpykafka-0.0.8/djpykafka/models/__init__.py
--rw-rw-rw-   0        0        0      238 2022-06-27 06:34:08.000000 djpykafka-0.0.8/djpykafka/models/kafka_mixin.py
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.667525 djpykafka-0.0.8/djpykafka/schemas/
--rw-rw-rw-   0        0        0       65 2022-05-04 09:42:39.000000 djpykafka-0.0.8/djpykafka/schemas/__init__.py
--rw-rw-rw-   0        0        0     2052 2022-05-04 09:43:11.000000 djpykafka-0.0.8/djpykafka/schemas/event.py
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.671526 djpykafka-0.0.8/djpykafka/utils/
--rw-rw-rw-   0        0        0       21 2022-06-07 14:41:13.000000 djpykafka-0.0.8/djpykafka/utils/__init__.py
--rw-rw-rw-   0        0        0      290 2022-06-08 07:04:35.000000 djpykafka-0.0.8/djpykafka/utils/kafka.py
-drwxrwxrwx   0        0        0        0 2022-07-28 09:30:00.649526 djpykafka-0.0.8/djpykafka.egg-info/
--rw-rw-rw-   0        0        0      578 2022-07-28 09:30:00.000000 djpykafka-0.0.8/djpykafka.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      592 2022-07-28 09:30:00.000000 djpykafka-0.0.8/djpykafka.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-28 09:30:00.000000 djpykafka-0.0.8/djpykafka.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-05-04 09:36:24.000000 djpykafka-0.0.8/djpykafka.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       56 2022-07-28 09:30:00.000000 djpykafka-0.0.8/djpykafka.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-07-28 09:30:00.000000 djpykafka-0.0.8/djpykafka.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      762 2022-07-28 09:30:00.674525 djpykafka-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0       41 2021-04-29 13:46:21.000000 djpykafka-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.347280 djpykafka-0.0.9/
+-rw-rw-rw-   0        0        0    26438 2022-05-05 06:07:09.000000 djpykafka-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      332 2021-04-29 13:46:13.000000 djpykafka-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0      578 2022-07-28 10:03:28.347280 djpykafka-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-05-04 09:33:38.000000 djpykafka-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.304282 djpykafka-0.0.9/djpykafka/
+-rw-rw-rw-   0        0        0       47 2022-05-04 09:44:14.000000 djpykafka-0.0.9/djpykafka/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.324279 djpykafka-0.0.9/djpykafka/events/
+-rw-rw-rw-   0        0        0       48 2022-05-04 12:48:57.000000 djpykafka-0.0.9/djpykafka/events/__init__.py
+-rw-rw-rw-   0        0        0     8364 2022-07-28 09:38:34.000000 djpykafka-0.0.9/djpykafka/events/publish.py
+-rw-rw-rw-   0        0        0     6701 2022-07-28 09:53:57.000000 djpykafka-0.0.9/djpykafka/events/subscribe.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.330280 djpykafka-0.0.9/djpykafka/handlers/
+-rw-rw-rw-   0        0        0       32 2022-05-04 11:53:09.000000 djpykafka-0.0.9/djpykafka/handlers/__init__.py
+-rw-rw-rw-   0        0        0     4075 2022-07-28 09:59:27.000000 djpykafka-0.0.9/djpykafka/handlers/event_consumer.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.335279 djpykafka-0.0.9/djpykafka/models/
+-rw-rw-rw-   0        0        0       65 2022-07-28 09:35:55.000000 djpykafka-0.0.9/djpykafka/models/__init__.py
+-rw-rw-rw-   0        0        0      335 2022-07-28 09:35:49.000000 djpykafka-0.0.9/djpykafka/models/kafka_mixin.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.340281 djpykafka-0.0.9/djpykafka/schemas/
+-rw-rw-rw-   0        0        0       65 2022-05-04 09:42:39.000000 djpykafka-0.0.9/djpykafka/schemas/__init__.py
+-rw-rw-rw-   0        0        0     2052 2022-05-04 09:43:11.000000 djpykafka-0.0.9/djpykafka/schemas/event.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.345281 djpykafka-0.0.9/djpykafka/utils/
+-rw-rw-rw-   0        0        0       21 2022-06-07 14:41:13.000000 djpykafka-0.0.9/djpykafka/utils/__init__.py
+-rw-rw-rw-   0        0        0      290 2022-06-08 07:04:35.000000 djpykafka-0.0.9/djpykafka/utils/kafka.py
+drwxrwxrwx   0        0        0        0 2022-07-28 10:03:28.317281 djpykafka-0.0.9/djpykafka.egg-info/
+-rw-rw-rw-   0        0        0      578 2022-07-28 10:03:28.000000 djpykafka-0.0.9/djpykafka.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      592 2022-07-28 10:03:28.000000 djpykafka-0.0.9/djpykafka.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-28 10:03:28.000000 djpykafka-0.0.9/djpykafka.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-05-04 09:36:24.000000 djpykafka-0.0.9/djpykafka.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       56 2022-07-28 10:03:28.000000 djpykafka-0.0.9/djpykafka.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2022-07-28 10:03:28.000000 djpykafka-0.0.9/djpykafka.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      762 2022-07-28 10:03:28.349281 djpykafka-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0       41 2021-04-29 13:46:21.000000 djpykafka-0.0.9/setup.py
```

### Comparing `djpykafka-0.0.8/LICENSE` & `djpykafka-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `djpykafka-0.0.8/PKG-INFO` & `djpykafka-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpykafka
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django + Pydantic + Kafka
 Home-page: https://github.com/Voltane-EU/djpykafka
 Author: Manuel Stingl
 Author-email: info+opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djpykafka-0.0.8/djpykafka/events/publish.py` & `djpykafka-0.0.9/djpykafka/events/publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import logging
 from typing import Type, TypeVar
 from functools import partial, cached_property
+import warnings
 from kafka import KafkaProducer
 from kafka.errors import KafkaTimeoutError
 from kafka.producer.future import FutureRecordMetadata
 from pydantic import BaseModel
 from django.dispatch import receiver, Signal
 from django.db.models.signals import post_save, post_delete
 from django.db import models
@@ -12,15 +13,15 @@
 from django.db.utils import OperationalError
 from django.utils import timezone
 from djfapi.utils.pydantic_django import transfer_from_orm
 from djfapi.utils.sentry import instrument_span, capture_exception
 from djfapi.utils.typing import with_typehint
 from djutils.transaction import on_transaction_complete
 from ..schemas import DataChangeEvent, EventMetadata
-from ..models import KafkaMixin
+from ..models import KafkaPublishMixin
 
 
 TBaseModel = TypeVar('TBaseModel', bound=BaseModel)
 TDjangoModel = TypeVar('TDjangoModel', bound=models.Model)
 
 
 class EventPublisher:
@@ -51,14 +52,17 @@
         cls.is_tenant_bound = hasattr(cls.orm_model, 'tenant_id')
         cls.logger = logging.getLogger(f'{cls.__module__}.{cls.__name__}')
         cls._kwargs = kwargs
 
         cls.register()
         cls.logger.info("Registered EventPublisher %s", cls.__name__)
 
+        if not isinstance(cls.orm_model, KafkaPublishMixin):
+            warnings.warn("Using EventPublisher with a model that doesnt has the KafkaPublishMixin is not recommended")
+
     @classmethod
     def register(cls):
         raise NotImplementedError
 
     @classmethod
     @on_transaction_complete()
     @instrument_span(
@@ -174,15 +178,15 @@
         self.logger.debug("Publish DataChangeEvent for %s with schema %s on %r", self.orm_model, self.event_schema, self.topic)
 
         data = self.get_message_data()  # prepare data to allow measuring just self.connection.send
 
         with start_span(op='KafkaProducer.send'):
             future_message: FutureRecordMetadata = self.connection.send(**data)
 
-        if isinstance(self.orm_model, KafkaMixin) and self.data_op != DataChangeEvent.DataOperation.DELETE:
+        if isinstance(self.orm_model, KafkaPublishMixin) and self.data_op != DataChangeEvent.DataOperation.DELETE:
             future_message.add_callback(self.send_callback)
 
         else:
             with start_span(op='FutureRecordMetadata.get'):
                 try:
                     future_message.get()
```

### Comparing `djpykafka-0.0.8/djpykafka/events/subscribe.py` & `djpykafka-0.0.9/djpykafka/events/subscribe.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from django.db import models
 from djfapi.utils.pydantic_django import transfer_to_orm, TransferAction
 from djfapi.utils.sentry import instrument_span
 from djfapi.security.jwt import access as access_ctx
 from djfapi.schemas import Access, AccessToken
 from ..handlers.event_consumer import message_handler
 from ..schemas import DataChangeEvent
+from ..models import KafkaSubscribeMixin
 try:
     from sentry_sdk import set_extra, Hub
 
 except ImportError:
     def set_extra(key, data):
         pass
 
@@ -26,14 +27,15 @@
 
 class Break(Exception):
     pass
 
 
 class EventSubscription:
     __orm_obj: Optional[TDjangoModel] = None
+    logger: logging.Logger
 
     def __init_subclass__(
         cls,
         event_schema: Type[TBaseModel],
         orm_model: Type[TDjangoModel],
         topic: str,
         delete_on_status: Optional[Any] = None,
@@ -42,15 +44,15 @@
     ):
         super().__init_subclass__(**kwargs)
         cls.event_schema = event_schema
         cls.orm_model = orm_model
         cls.topic = topic
         cls.delete_on_status = delete_on_status
         cls.create_only_on_op_create = create_only_on_op_create
-        cls.logger = logging.getLogger(__name__)
+        cls.logger = logging.getLogger(f'{cls.__module__}.{cls.__qualname__}')
 
         message_handler(
             topic=cls.topic,
             transaction_name=f'{cls.__module__}.{cls.__qualname__}',
         )(cls.handle)
 
         if not hasattr(cls.orm_model, 'updated_at'):
@@ -62,22 +64,30 @@
             "Registered EventSubscription %r with event_schema %r and orm_model %s on topic %s",
             cls,
             cls.event_schema,
             cls.orm_model,
             cls.topic,
         )
 
+        if not isinstance(cls.orm_model, KafkaSubscribeMixin):
+            warnings.warn("Using EventSubscription with a model that doesnt has the KafkaSubscribeMixin is not recommended")
+
     @classmethod
     @instrument_span(
         op='EventSubscription',
         description=lambda cls, body, *args, **kwargs: f'{cls}',
     )
     def handle(cls, body):
-        instance = cls(body)
-        instance.process()
+        try:
+            instance = cls(body)
+            instance.process()
+
+        except Exception as error:
+            cls.logger.exception("Error occurred while processing message")
+            raise error
 
     def __init__(self, body):
         self.body = body
         self.event = DataChangeEvent.parse_raw(self.body) if isinstance(self.body, (bytes, str)) else DataChangeEvent.parse_obj(self.body)
 
         self.logger.info(
             "%s %s eid=%s id=%s flow_id=%s",
```

### Comparing `djpykafka-0.0.8/djpykafka/handlers/event_consumer.py` & `djpykafka-0.0.9/djpykafka/handlers/event_consumer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import json
-from typing import Callable, List, Optional, Union
+from typing import Callable, List, Literal, Optional, Union
 from collections import defaultdict
 from functools import wraps
 from kafka import KafkaConsumer
 from kafka.consumer.fetcher import ConsumerRecord
 
 try:
     from sentry_sdk.integrations.serverless import serverless_function
@@ -24,19 +24,20 @@
     @classmethod
     def get_consumer(cls):
         if len(cls.consumers) != 1:
             raise ValueError('more than one consumer defined')
 
         return cls.consumers[0]
 
-    def __init__(self, bootstrap_servers: Union[str, List[str]], client_id: Optional[str] = None, group_id: Optional[str] = None, **kwargs) -> None:
+    def __init__(self, bootstrap_servers: Union[str, List[str]], client_id: Optional[str] = None, group_id: Optional[str] = None, auto_offset_reset: Literal['earliest', 'latest'] = 'earliest', **kwargs) -> None:
         self.handlers: defaultdict[str, List[Callable[[str], None]]] = defaultdict(list)
         self.bootstrap_servers = bootstrap_servers
         self.client_id = client_id
         self.group_id = group_id
+        self.auto_offset_reset = auto_offset_reset
         self._kwargs = kwargs
         self.__class__.consumers.append(self)
         self.logger = logging.getLogger('djpykafka.event')
 
     def register_handler(self, topic: str, handler: callable):
         self.handlers[topic].append(handler)
 
@@ -47,14 +48,15 @@
 
     def run(self):
         self.consumer = KafkaConsumer(
             *self.handlers.keys(),
             bootstrap_servers=self.bootstrap_servers,
             client_id=self.client_id,
             group_id=self.group_id,
+            auto_offset_reset=self.auto_offset_reset,
             **self._kwargs,
         )
 
         for message in self.consumer:
             self._dispatch(message)
```

### Comparing `djpykafka-0.0.8/djpykafka/schemas/event.py` & `djpykafka-0.0.9/djpykafka/schemas/event.py`

 * *Files identical despite different names*

### Comparing `djpykafka-0.0.8/djpykafka.egg-info/PKG-INFO` & `djpykafka-0.0.9/djpykafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djpykafka
-Version: 0.0.8
+Version: 0.0.9
 Summary: Django + Pydantic + Kafka
 Home-page: https://github.com/Voltane-EU/djpykafka
 Author: Manuel Stingl
 Author-email: info+opensource@voltane.eu
 License: GNU LGPLv2.1
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
```

### Comparing `djpykafka-0.0.8/djpykafka.egg-info/SOURCES.txt` & `djpykafka-0.0.9/djpykafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djpykafka-0.0.8/setup.cfg` & `djpykafka-0.0.9/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6a70 796b 6166 6b61 0d0a 7665   = djpykafka..ve
-00000020: 7273 696f 6e20 3d20 302e 302e 380d 0a61  rsion = 0.0.8..a
+00000020: 7273 696f 6e20 3d20 302e 302e 390d 0a61  rsion = 0.0.9..a
 00000030: 7574 686f 7220 3d20 4d61 6e75 656c 2053  uthor = Manuel S
 00000040: 7469 6e67 6c0d 0a61 7574 686f 725f 656d  tingl..author_em
 00000050: 6169 6c20 3d20 696e 666f 2b6f 7065 6e73  ail = info+opens
 00000060: 6f75 7263 6540 766f 6c74 616e 652e 6575  ource@voltane.eu
 00000070: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
 00000080: 446a 616e 676f 202b 2050 7964 616e 7469  Django + Pydanti
 00000090: 6320 2b20 4b61 666b 610d 0a6c 6f6e 675f  c + Kafka..long_
```

