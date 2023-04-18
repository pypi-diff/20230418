# Comparing `tmp/robotnikmq-0.5.1.tar.gz` & `tmp/robotnikmq-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotnikmq-0.5.1.tar", last modified: Mon Apr 10 23:01:26 2023, max compression
+gzip compressed data, was "robotnikmq-0.6.1.tar", last modified: Tue Apr 18 03:04:26 2023, max compression
```

## Comparing `robotnikmq-0.5.1.tar` & `robotnikmq-0.6.1.tar`

### file list

```diff
@@ -1,39 +1,25 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/LICENSE
--rw-r--r--   0        0        0     6369 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/README.md
--rw-r--r--   0        0        0     1217 2023-04-10 22:57:32.564447 robotnikmq-0.5.1/pyproject.toml
--rwxr-xr-x   0        0        0      320 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/__init__.py
--rwxr-xr-x   0        0        0     5330 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/robotnikmq/config.py
--rw-r--r--   0        0        0     6278 2023-04-10 22:59:06.907684 robotnikmq-0.5.1/robotnikmq/core.py
--rwxr-xr-x   0        0        0      652 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/error.py
--rw-r--r--   0        0        0     1230 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/log.py
--rw-r--r--   0        0        0     2649 2022-11-16 02:41:34.714029 robotnikmq-0.5.1/robotnikmq/rpc_client.py
--rw-r--r--   0        0        0    11552 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/robotnikmq/rpc_server.py
--rw-r--r--   0        0        0     4359 2023-04-10 23:00:12.499144 robotnikmq-0.5.1/robotnikmq/subscriber.py
--rwxr-xr-x   0        0        0     1411 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/robotnikmq/topic.py
--rw-r--r--   0        0        0      471 2023-04-10 14:34:22.584553 robotnikmq-0.5.1/robotnikmq/utils.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:18.502194 robotnikmq-0.5.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 14:11:20.222199 robotnikmq-0.5.1/tests/integration/__init__.py
--rwxr-xr-x   0        0        0    16298 2023-04-10 23:00:46.078865 robotnikmq-0.5.1/tests/integration/test_broadcast.py
--rw-r--r--   0        0        0     1632 2023-04-10 22:43:27.085734 robotnikmq-0.5.1/tests/integration/test_disconnects.py
--rw-r--r--   0        0        0    13648 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/test_rpc.py
--rw-r--r--   0        0        0     2435 2023-04-10 23:00:31.458987 robotnikmq-0.5.1/tests/integration/utils.py
--rw-r--r--   0        0        0    13754 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/library/ca.py
--rw-r--r--   0        0        0    12451 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/library/cert.py
--rw-r--r--   0        0        0      739 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/provision.yaml
--rw-r--r--   0        0        0       84 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
--rw-r--r--   0        0        0       19 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
--rw-r--r--   0        0        0      102 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
--rw-r--r--   0        0        0     1609 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
--rw-r--r--   0        0        0     4907 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
--rwxr-xr-x   0        0        0      588 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
--rw-r--r--   0        0        0     1236 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
--rw-r--r--   0        0        0     1012 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0       29 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/tls/tasks/main.yaml
--rw-r--r--   0        0        0     2522 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/roles/tls/tasks/tls.yaml
--rw-r--r--   0        0        0      172 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/integration/vagrant/testing
--rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.5.1/tests/unit/__init__.py
--rw-r--r--   0        0        0     4142 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_config.py
--rw-r--r--   0        0        0      261 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_error.py
--rw-r--r--   0        0        0     1818 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_message.py
--rw-r--r--   0        0        0     1292 2022-11-16 02:41:34.718029 robotnikmq-0.5.1/tests/unit/test_validation.py
--rw-r--r--   0        0        0     6657 1970-01-01 00:00:00.000000 robotnikmq-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/LICENSE
+-rw-r--r--   0        0        0     6128 2023-04-16 21:48:51.582507 robotnikmq-0.6.1/README.md
+-rw-r--r--   0        0        0     1256 2023-04-18 01:40:55.148760 robotnikmq-0.6.1/pyproject.toml
+-rwxr-xr-x   0        0        0      337 2023-04-17 01:22:37.631810 robotnikmq-0.6.1/robotnikmq/__init__.py
+-rwxr-xr-x   0        0        0     6280 2023-04-16 22:02:59.632874 robotnikmq-0.6.1/robotnikmq/config.py
+-rw-r--r--   0        0        0     6278 2023-04-16 22:03:20.340835 robotnikmq-0.6.1/robotnikmq/core.py
+-rwxr-xr-x   0        0        0      652 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/robotnikmq/error.py
+-rw-r--r--   0        0        0     1230 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/robotnikmq/log.py
+-rw-r--r--   0        0        0     2649 2022-11-16 02:41:34.714029 robotnikmq-0.6.1/robotnikmq/rpc_client.py
+-rw-r--r--   0        0        0    11552 2023-04-10 22:43:27.085734 robotnikmq-0.6.1/robotnikmq/rpc_server.py
+-rw-r--r--   0        0        0     3669 2023-04-18 02:34:34.875545 robotnikmq-0.6.1/robotnikmq/subscriber.py
+-rwxr-xr-x   0        0        0     1411 2023-04-10 22:43:27.085734 robotnikmq-0.6.1/robotnikmq/topic.py
+-rw-r--r--   0        0        0      471 2023-04-10 14:34:22.584553 robotnikmq-0.6.1/robotnikmq/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:18.502194 robotnikmq-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:20.222199 robotnikmq-0.6.1/tests/integration/__init__.py
+-rw-r--r--   0        0        0      454 2023-04-16 23:25:18.821810 robotnikmq-0.6.1/tests/integration/conftest.py
+-rwxr-xr-x   0        0        0    16105 2023-04-18 02:39:58.179068 robotnikmq-0.6.1/tests/integration/test_broadcast.py
+-rw-r--r--   0        0        0    13569 2023-04-16 22:59:42.127250 robotnikmq-0.6.1/tests/integration/test_rpc.py
+-rw-r--r--   0        0        0      622 2023-04-16 22:26:51.861392 robotnikmq-0.6.1/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 14:11:21.330203 robotnikmq-0.6.1/tests/unit/__init__.py
+-rw-r--r--   0        0        0     4105 2023-04-16 23:26:37.032343 robotnikmq-0.6.1/tests/unit/test_config.py
+-rw-r--r--   0        0        0      261 2022-11-16 02:41:34.718029 robotnikmq-0.6.1/tests/unit/test_error.py
+-rw-r--r--   0        0        0     1818 2022-11-16 02:41:34.718029 robotnikmq-0.6.1/tests/unit/test_message.py
+-rw-r--r--   0        0        0     1292 2022-11-16 02:41:34.718029 robotnikmq-0.6.1/tests/unit/test_validation.py
+-rw-r--r--   0        0        0     6416 1970-01-01 00:00:00.000000 robotnikmq-0.6.1/PKG-INFO
```

### Comparing `robotnikmq-0.5.1/LICENSE` & `robotnikmq-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/README.md` & `robotnikmq-0.6.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -117,22 +117,16 @@
 pdm run pytest tests/unit/test_core.py::test_hello
 ```
 
 For more information on testing, see the `pytest.ini` file as well as the [documentation](https://docs.pytest.org/en/stable/).
 
 ### Integration Testing
 
-RobotnikMQ uses [pytest-rabbitmq](https://pypi.org/project/pytest-rabbitmq/) which requires [`rabbitmq`](https://www.rabbitmq.com/) to be installed. An easy way to install it on Ubuntu and most other Debian-based Linux distros without configuring the service to auto-start is:
+For integration testing, this code uses [testcontainers-rabbitmq](https://testcontainers-python.readthedocs.io/en/latest/rabbitmq/README.html). In order to enable this, you will need to install docker, and ensure that your user has the ability to interact with the docker service:
 
 ```bash
-RUNLEVEL=1 apt install -y rabbitmq-server
-```
-
-## Documentation
-
-Documentation is generated using [`mkdocs`](https://www.mkdocs.org/). When code/docstrings change, you should re-generate the documentation with:
-
-```bash
-pdm run mkdocs build
-```
-
-which will put the HTML files for the documentation into the gitignored `sites/` directory. Also, you can use `pdm run mkdocs serve` while editing the documentation to see results live in your browser.
+sudo apt install docker
+sudo groupadd docker # may fail if the docker group already exists
+sudo usermod -aG docker $USER
+newgrp docker
+docker run hello-world # verify that everything is working well
+```
```

### Comparing `robotnikmq-0.5.1/pyproject.toml` & `robotnikmq-0.6.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "robotnikmq"
-version = "0.5.1"
+version = "0.6.1"
 description = "Utilities for safe, efficient, and scalable infrastructure using RabbitMQ"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "typeguard>=3.0.2",
     "pyyaml>=6.0",
@@ -35,14 +35,15 @@
     "flake8<5.0.0,>=3.0.0",
     "mkdocs>=1.0.0",
     "mkdocstrings[python]>=0.10.0",
     "mkdocs-cinder>=1.2.0",
     "pytest-rabbitmq>=2.2.1",
     "pudb>=2022.1.2",
     "types-retry>=0.9.9.3",
+    "testcontainers[rabbitmq]>=3.7.1",
 ]
 
 [tool.pdm.scripts.publish-test]
 cmd = "twine upload -r testpypi dist/*"
 
 [tool.pdm.scripts.publish-prod]
 cmd = "twine upload -r pypi dist/*"
```

### Comparing `robotnikmq-0.5.1/robotnikmq/config.py` & `robotnikmq-0.6.1/robotnikmq/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -46,14 +46,15 @@
     port: int
     user: str
     password: str
     vhost: str
     ca_cert: Optional[Path] = None
     cert: Optional[Path] = None
     key: Optional[Path] = None
+    _conn_params: Optional[ConnectionParameters] = None
 
     _existing_ca_cert = validator("ca_cert", pre=True, always=True, allow_reuse=True)(
         _existing_file_or_none
     )
     _existing_cert = validator("cert", pre=True, always=True, allow_reuse=True)(
         _existing_file_or_none
     )
@@ -64,14 +65,16 @@
     class Config:
         json_encoders = {
             Path: str,
         }
 
     @typechecked
     def conn_params(self) -> ConnectionParameters:
+        if self._conn_params is not None:
+            return self._conn_params
         if self.ca_cert is not None and self.cert is not None and self.key is not None:
             context = create_default_context(cafile=str(self.ca_cert))
             context.load_cert_chain(self.cert, self.key)
             return ConnectionParameters(
                 host=self.host,
                 port=self.port,
                 virtual_host=self.vhost,
@@ -82,14 +85,25 @@
         return ConnectionParameters(
             host=self.host,
             port=self.port,
             virtual_host=self.vhost,
             credentials=PlainCredentials(self.user, self.password),
         )
 
+    @typechecked
+    @staticmethod
+    def from_connection_params(conn_params: ConnectionParameters) -> "ServerConfig":
+        return ServerConfig(
+            host=conn_params.host,
+            port=conn_params.port,
+            user=getattr(conn_params.credentials, "username", ""),
+            password=getattr(conn_params.credentials, "password", ""),
+            vhost=conn_params.virtual_host,
+        )
+
 
 @typechecked
 def server_config(
     host: str,
     port: int,
     user: str,
     password: str,
@@ -163,14 +177,28 @@
     def a_server(self, tier: int) -> ServerConfig:
         return choice(self.tier(tier))
 
     @typechecked
     def as_dict(self) -> Dict[str, Any]:
         return self.dict()
 
+    @typechecked
+    @staticmethod
+    def from_tiered(
+        tiers: List[List[ServerConfig]],
+    ) -> "RobotnikConfig":
+        return RobotnikConfig(tiers=tiers)
+
+    @typechecked
+    @staticmethod
+    def from_connection_params(conn_params: ConnectionParameters) -> "RobotnikConfig":
+        return RobotnikConfig(
+            tiers=[[ServerConfig.from_connection_params(conn_params)]]
+        )
+
 
 @typechecked
 def config_of(config_file: Optional[Path]) -> RobotnikConfig:
     if config_file is None or not config_file.exists():
         log.critical("No valid RobotnikMQ configuration file was provided")
         raise NotConfigured("No valid RobotnikMQ configuration file was provided")
     return RobotnikConfig(**safe_load(config_file.open().read()))
```

### Comparing `robotnikmq-0.5.1/robotnikmq/core.py` & `robotnikmq-0.6.1/robotnikmq/core.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/robotnikmq/error.py` & `robotnikmq-0.6.1/robotnikmq/error.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/robotnikmq/log.py` & `robotnikmq-0.6.1/robotnikmq/log.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/robotnikmq/rpc_client.py` & `robotnikmq-0.6.1/robotnikmq/rpc_client.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/robotnikmq/rpc_server.py` & `robotnikmq-0.6.1/robotnikmq/rpc_server.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/robotnikmq/topic.py` & `robotnikmq-0.6.1/robotnikmq/topic.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/tests/integration/test_broadcast.py` & `robotnikmq-0.6.1/tests/integration/test_broadcast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,40 @@
 # pylint: disable=redefined-outer-name
-from functools import partial
 import json
 from multiprocessing import Process, Event
 from pprint import pprint
 from time import sleep
 
 from pytest import raises
-from typeguard import typechecked
 
-from robotnikmq.config import server_config, RobotnikConfig
+from robotnikmq.config import server_config, RobotnikConfig, conn_config
 from robotnikmq.core import Message
 from robotnikmq.error import UnableToConnect
 from robotnikmq.log import log
 from robotnikmq.subscriber import Subscriber
 from robotnikmq.topic import Topic
 
 from tests.integration.utils import META_QUEUE
-from tests.integration.utils import (
-    conn_config,
-    robotnikmq_config,
-)  # pylint: disable=W0611
 
 
 try:
     from pytest_cov.embed import cleanup_on_sigterm  # type: ignore
 except ImportError:
     pass
 else:
     cleanup_on_sigterm()
 
 
 def test_basic_broadcast(robotnikmq_config):
-    medium = Topic(
+    topic = Topic(
         META_QUEUE,
         robotnikmq_config,
         on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
     )
-    medium.broadcast(Message({"stuff": "Hello world!"}))
+    topic.broadcast(Message({"stuff": "Hello world!"}))
 
 
 def test_unable_to_connect():
     config = RobotnikConfig(
         connection=conn_config(1, 1, 2),
         tiers=[
             [
@@ -68,26 +62,26 @@
             ]
         ],
     )
     with raises(UnableToConnect) as exc:
         medium = Topic(META_QUEUE, config)
         medium.broadcast(Message({"stuff": "Hello world!"}))
     log.debug(str(exc))
-    log.debug(str(exc.value.__str__()))
+    log.debug(str(exc.value))
 
 
 def test_basic_broadcast_receive(robotnikmq_config):
     msg_received = Event()
 
-    def callback(msg: Message) -> None:
-        pprint(msg.to_dict())
-        msg_received.set()
-
     def sub():
-        Subscriber(config=robotnikmq_config).bind(exchange=META_QUEUE).run(callback)
+        for msg in (
+            Subscriber(config=robotnikmq_config).bind(exchange=META_QUEUE).consume()
+        ):
+            pprint(msg.to_dict())
+            msg_received.set()
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
@@ -104,23 +98,25 @@
     pub_proc.join()
     sub_proc.join()
 
 
 def test_broadcast_malformed_message(robotnikmq_config):
     msg_received = Event()
 
-    def callback(msg: Message) -> None:
-        pprint(msg.to_dict())
-        msg_received.set()
-
     def sub():
-        Subscriber(
-            config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-        ).bind(exchange=META_QUEUE).run(callback)
+        for msg in (
+            Subscriber(
+                config=robotnikmq_config,
+                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
+            )
+            .bind(exchange=META_QUEUE)
+            .consume()
+        ):
+            pprint(msg.to_dict())
+            msg_received.set()
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
@@ -132,41 +128,34 @@
         )
 
     sub_proc = Process(target=sub)
     sub_proc.start()
     pub_proc = Process(target=pub)
     pub_proc.start()
     assert not msg_received.wait(timeout=1)
-    pub_proc.terminate()
     sub_proc.terminate()
     pub_proc.join()
     sub_proc.join()
 
 
 def test_subscriber_stop(robotnikmq_config):
     first_msg_received = Event()
     second_msg_received = Event()
 
-    @typechecked
-    def callback(sub: Subscriber, msg: Message) -> None:
-        pprint(msg.to_dict())
-        if not first_msg_received.is_set():
-            first_msg_received.set()
-        else:
-            second_msg_received.set()
-        sub.stop()
-
     def sub():
         sub = Subscriber(
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
-        sub.bind(exchange=META_QUEUE).run(
-            partial(callback, sub), inactivity_timeout=0.1
-        )
+        for msg in sub.bind(exchange=META_QUEUE).consume():
+            pprint(msg.to_dict())
+            if not first_msg_received.is_set():
+                first_msg_received.set()
+                break
+            second_msg_received.set()
 
     def pub():
         medium = Topic(
             exchange=META_QUEUE,
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
@@ -240,27 +229,27 @@
     pub_proc.terminate()
     pub_proc.join()
 
 
 def test_multiple_broadcast_single_receive(robotnikmq_config):
     msg_received = Event()
 
-    def callback(msg: Message) -> None:
-        pprint(msg.to_dict())
-        assert msg.contents["stuff"] != "Bad"
-        assert (
-            msg.routing_key == "stuff.something" or msg.routing_key == "stuff.nothing"
-        )
-        msg_received.set()
-
     def sub():
-        Subscriber(
-            config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-        ).bind(exchange="stuff", binding_key="stuff.*").run(callback)
+        for msg in (
+            Subscriber(
+                config=robotnikmq_config,
+                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
+            )
+            .bind(exchange="stuff", binding_key="stuff.*")
+            .consume()
+        ):
+            pprint(msg.to_dict())
+            assert msg.contents["stuff"] != "Bad"
+            assert msg.routing_key in {"stuff.something", "stuff.nothing"}
+            msg_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
@@ -309,33 +298,33 @@
 
 
 def test_multiple_route_receive(robotnikmq_config):
     msg1_received = Event()
     msg2_received = Event()
     msg3_received = Event()
 
-    def callback(msg: Message) -> None:
-        pprint(msg.to_dict())
-        assert msg.contents["stuff"] != "Bad"
-        if msg.route == "message.1":
-            msg1_received.set()
-        if msg.route == "message.2":
-            msg2_received.set()
-        if msg.route == "message.3":
-            msg3_received.set()
-
     def sub():
-        Subscriber(
-            config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-        ).bind("stuff", "message.1").bind("stuff", "message.2").bind(
-            "stuff", "message.3"
-        ).run(
-            callback
-        )
+        for msg in (
+            Subscriber(
+                config=robotnikmq_config,
+                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
+            )
+            .bind("stuff", "message.1")
+            .bind("stuff", "message.2")
+            .bind("stuff", "message.3")
+            .consume()
+        ):
+            pprint(msg.to_dict())
+            assert msg.contents["stuff"] != "Bad"
+            if msg.route == "message.1":
+                msg1_received.set()
+            if msg.route == "message.2":
+                msg2_received.set()
+            if msg.route == "message.3":
+                msg3_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
@@ -401,33 +390,33 @@
 
 
 def test_multiple_queue_receive(robotnikmq_config):
     msg1_received = Event()
     msg2_received = Event()
     msg3_received = Event()
 
-    def callback(msg: Message) -> None:
-        pprint(msg.to_dict())
-        assert msg.contents["stuff"] != "Bad"
-        if msg.route == "message.1":
-            msg1_received.set()
-        if msg.route == "message.2":
-            msg2_received.set()
-        if msg.route == "message.3":
-            msg3_received.set()
-
     def sub():
-        Subscriber(
-            config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-        ).bind("stuff.1", "message.1").bind("stuff.2", "message.2").bind(
-            "stuff.3", "message.3"
-        ).run(
-            callback
-        )
+        for msg in (
+            Subscriber(
+                config=robotnikmq_config,
+                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
+            )
+            .bind("stuff.1", "message.1")
+            .bind("stuff.2", "message.2")
+            .bind("stuff.3", "message.3")
+            .consume()
+        ):
+            pprint(msg.to_dict())
+            assert msg.contents["stuff"] != "Bad"
+            if msg.route == "message.1":
+                msg1_received.set()
+            if msg.route == "message.2":
+                msg2_received.set()
+            if msg.route == "message.3":
+                msg3_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff.1",
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
@@ -491,27 +480,27 @@
     pub_proc_bad.join()
     sub_proc.join()
 
 
 def test_multiple_broadcast_single_receive_msg_routing(robotnikmq_config):
     msg_received = Event()
 
-    def callback(msg: Message) -> None:
-        pprint(msg.to_dict())
-        assert msg.contents["stuff"] != "Bad"
-        assert (
-            msg.routing_key == "stuff.something" or msg.routing_key == "stuff.nothing"
-        )
-        msg_received.set()
-
     def sub():
-        Subscriber(
-            config=robotnikmq_config,
-            on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
-        ).bind(exchange="stuff", binding_key="stuff.*").run(callback)
+        for msg in (
+            Subscriber(
+                config=robotnikmq_config,
+                on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
+            )
+            .bind(exchange="stuff", binding_key="stuff.*")
+            .consume()
+        ):
+            pprint(msg.to_dict())
+            assert msg.contents["stuff"] != "Bad"
+            assert msg.routing_key in {"stuff.something", "stuff.nothing"}
+            msg_received.set()
 
     def pub1():
         medium = Topic(
             exchange="stuff",
             config=robotnikmq_config,
             on_conn_error=lambda a: print(f"Could not connect: {a.args}"),
         )
```

### Comparing `robotnikmq-0.5.1/tests/integration/test_rpc.py` & `robotnikmq-0.6.1/tests/integration/test_rpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 from typeguard import typechecked
 
 from robotnikmq.log import log
 from robotnikmq.rpc_client import RpcClient
 from robotnikmq.rpc_server import RpcServer
 
 from tests.integration.utils import sub_process
-from tests.integration.utils import robotnikmq_config  # pylint: disable=W0611
 
 try:
     from pytest_cov.embed import cleanup_on_sigterm  # type: ignore
 except ImportError:
     pass
 else:
     cleanup_on_sigterm()
```

### Comparing `robotnikmq-0.5.1/tests/unit/test_config.py` & `robotnikmq-0.6.1/tests/unit/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from os import chdir
 from os.path import realpath
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
-from pydantic import ValidationError
 from pytest import raises, mark, param
 
 from robotnikmq.config import config_of, server_config, _existing_file_or_none
 from robotnikmq.core import Robotnik
 from robotnikmq.error import NotConfigured
```

### Comparing `robotnikmq-0.5.1/tests/unit/test_message.py` & `robotnikmq-0.6.1/tests/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/tests/unit/test_validation.py` & `robotnikmq-0.6.1/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `robotnikmq-0.5.1/PKG-INFO` & `robotnikmq-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotnikmq
-Version: 0.5.1
+Version: 0.6.1
 Summary: Utilities for safe, efficient, and scalable infrastructure using RabbitMQ
 License: GPL-3.0-or-later
 Author-email: Eugene Kovalev <eugene@kovalev.systems>
 Requires-Python: >3.8.2,<4.0
 Description-Content-Type: text/markdown
 
 # RobotnikMQ
@@ -126,22 +126,16 @@
 pdm run pytest tests/unit/test_core.py::test_hello
 ```
 
 For more information on testing, see the `pytest.ini` file as well as the [documentation](https://docs.pytest.org/en/stable/).
 
 ### Integration Testing
 
-RobotnikMQ uses [pytest-rabbitmq](https://pypi.org/project/pytest-rabbitmq/) which requires [`rabbitmq`](https://www.rabbitmq.com/) to be installed. An easy way to install it on Ubuntu and most other Debian-based Linux distros without configuring the service to auto-start is:
+For integration testing, this code uses [testcontainers-rabbitmq](https://testcontainers-python.readthedocs.io/en/latest/rabbitmq/README.html). In order to enable this, you will need to install docker, and ensure that your user has the ability to interact with the docker service:
 
 ```bash
-RUNLEVEL=1 apt install -y rabbitmq-server
+sudo apt install docker
+sudo groupadd docker # may fail if the docker group already exists
+sudo usermod -aG docker $USER
+newgrp docker
+docker run hello-world # verify that everything is working well
 ```
-
-## Documentation
-
-Documentation is generated using [`mkdocs`](https://www.mkdocs.org/). When code/docstrings change, you should re-generate the documentation with:
-
-```bash
-pdm run mkdocs build
-```
-
-which will put the HTML files for the documentation into the gitignored `sites/` directory. Also, you can use `pdm run mkdocs serve` while editing the documentation to see results live in your browser.
```

