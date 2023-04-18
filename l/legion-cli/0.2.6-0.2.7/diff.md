# Comparing `tmp/legion-cli-0.2.6.tar.gz` & `tmp/legion-cli-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "legion-cli-0.2.6.tar", last modified: Tue Apr 11 00:03:41 2023, max compression
+gzip compressed data, was "legion-cli-0.2.7.tar", last modified: Tue Apr 18 03:17:33 2023, max compression
```

## Comparing `legion-cli-0.2.6.tar` & `legion-cli-0.2.7.tar`

### file list

```diff
@@ -1,50 +1,21 @@
--rw-r--r--   0        0        0    34500 2022-11-16 02:41:53.005895 legion-cli-0.2.6/LICENSE
--rw-r--r--   0        0        0     2472 2022-11-16 02:41:53.005895 legion-cli-0.2.6/README.md
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.6/legion_cli/__init__.py
--rw-r--r--   0        0        0     4459 2022-11-16 02:41:53.005895 legion-cli-0.2.6/legion_cli/alerts_manager.py
--rw-r--r--   0        0        0     6679 2023-04-10 23:51:16.952762 legion-cli-0.2.6/legion_cli/cli.py
--rw-r--r--   0        0        0      214 2022-11-16 02:41:53.005895 legion-cli-0.2.6/legion_cli/config.py
--rw-r--r--   0        0        0     1451 2022-11-16 02:41:53.005895 legion-cli-0.2.6/legion_cli/log.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.6/legion_cli/tui/__init__.py
--rw-r--r--   0        0        0     8529 2023-04-10 23:51:04.144876 legion-cli-0.2.6/legion_cli/tui/alerts_monitor.py
--rw-r--r--   0        0        0     8791 2023-04-10 23:58:30.245037 legion-cli-0.2.6/legion_cli/tui/detail_list.py
--rw-r--r--   0        0        0      897 2022-11-16 02:41:53.005895 legion-cli-0.2.6/legion_cli/tui/keyboard.py
--rw-r--r--   0        0        0      956 2023-04-11 00:03:23.618603 legion-cli-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/__init__.py
--rw-r--r--   0        0        0     1119 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/test_watch.py
--rw-r--r--   0        0        0     1103 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/utils.py
--rw-r--r--   0        0        0     1184 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/host_files/rabbitmq-vm/legiond/legiond.conf
--rw-r--r--   0        0        0      556 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/host_files/rabbitmq-vm/robotnikmq/robotnikmq.yaml
--rw-r--r--   0        0        0    13754 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/library/ca.py
--rw-r--r--   0        0        0    12451 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/library/cert.py
--rw-r--r--   0        0        0      907 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/provision.yaml
--rw-r--r--   0        0        0      234 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/robotnikmq.yaml
--rw-r--r--   0        0        0       26 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/legion-cli/meta/main.yaml
--rw-r--r--   0        0        0     1064 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/legion-cli/tasks/main.yaml
--rw-r--r--   0        0        0       43 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/legiond/meta/main.yaml
--rw-r--r--   0        0        0     2173 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/legiond/tasks/main.yaml
--rw-r--r--   0        0        0      339 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/legiond/templates/legiond.conf.j2
--rw-r--r--   0        0        0       84 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/handlers/main.yaml
--rw-r--r--   0        0        0       19 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/meta/main.yaml
--rw-r--r--   0        0        0      102 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/tasks/main.yaml
--rw-r--r--   0        0        0     1609 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq-cluster.yaml
--rw-r--r--   0        0        0     4907 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/tasks/rabbitmq.yaml
--rwxr-xr-x   0        0        0      588 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/tasks/vhosts.yaml
--rw-r--r--   0        0        0     1236 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq-env.conf.j2
--rw-r--r--   0        0        0     1012 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/rabbitmq/templates/rabbitmq.conf.j2
--rw-r--r--   0        0        0     2602 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/robotnikmq/files/dk_legion_robotnik_id_rsa
--rw-r--r--   0        0        0      552 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/robotnikmq/files/dk_legion_robotnik_id_rsa.pub
--rw-r--r--   0        0        0       21 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/robotnikmq/meta/main.yaml
--rw-r--r--   0        0        0     1212 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/robotnikmq/tasks/main.yaml
--rw-r--r--   0        0        0       78 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/supervisor/handlers/main.yaml
--rw-r--r--   0        0        0       36 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/supervisor/tasks/main.yaml
--rw-r--r--   0        0        0      385 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/supervisor/tasks/supervisor.yaml
--rw-r--r--   0        0        0       29 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/tls/tasks/main.yaml
--rw-r--r--   0        0        0     2526 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/roles/tls/tasks/tls.yaml
--rw-r--r--   0        0        0      172 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/integration/vagrant/testing
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/unit/__init__.py
--rw-r--r--   0        0        0     8670 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/unit/test_alerts_manager.py
--rw-r--r--   0        0        0      863 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/unit/test_config.py
--rw-r--r--   0        0        0    11550 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/unit/test_detail_list.py
--rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.6/tests/unit/test_keyboard.py
--rw-r--r--   0        0        0     2755 1970-01-01 00:00:00.000000 legion-cli-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0    34500 2022-11-16 02:41:53.005895 legion-cli-0.2.7/LICENSE
+-rw-r--r--   0        0        0     2780 2023-04-16 21:05:35.342704 legion-cli-0.2.7/README.md
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/__init__.py
+-rw-r--r--   0        0        0     4459 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/alerts_manager.py
+-rw-r--r--   0        0        0     6797 2023-04-18 01:29:44.807755 legion-cli-0.2.7/legion_cli/cli.py
+-rw-r--r--   0        0        0      214 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/config.py
+-rw-r--r--   0        0        0     1451 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/log.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/tui/__init__.py
+-rw-r--r--   0        0        0     8529 2023-04-10 23:51:04.144876 legion-cli-0.2.7/legion_cli/tui/alerts_monitor.py
+-rw-r--r--   0        0        0     8791 2023-04-10 23:58:30.245037 legion-cli-0.2.7/legion_cli/tui/detail_list.py
+-rw-r--r--   0        0        0      897 2022-11-16 02:41:53.005895 legion-cli-0.2.7/legion_cli/tui/keyboard.py
+-rw-r--r--   0        0        0     1115 2023-04-18 03:10:43.017132 legion-cli-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/integration/__init__.py
+-rw-r--r--   0        0        0     1507 2023-04-16 20:19:34.157064 legion-cli-0.2.7/tests/integration/test_watch.py
+-rw-r--r--   0        0        0      521 2023-04-16 20:04:09.231827 legion-cli-0.2.7/tests/integration/utils.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/__init__.py
+-rw-r--r--   0        0        0     8670 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_alerts_manager.py
+-rw-r--r--   0        0        0      863 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_config.py
+-rw-r--r--   0        0        0    11550 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_detail_list.py
+-rw-r--r--   0        0        0        0 2022-11-16 02:41:53.005895 legion-cli-0.2.7/tests/unit/test_keyboard.py
+-rw-r--r--   0        0        0     3063 1970-01-01 00:00:00.000000 legion-cli-0.2.7/PKG-INFO
```

### Comparing `legion-cli-0.2.6/LICENSE` & `legion-cli-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/README.md` & `legion-cli-0.2.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,27 @@
+Metadata-Version: 2.1
+Name: legion-cli
+Version: 0.2.7
+Summary: Commandline Utilities for the Legion Alerting and Monitoring System
+License: GPL-3.0-or-later
+Author-email: Eugene Kovalev <eugene@kovalev.systems>
+Requires-Python: >=3.8.3,<4.0
+Description-Content-Type: text/markdown
+
 # Legion CLI
 
 Commandline Utilities for the Legion Alerting and Monitoring System
 
 ## Setup & Usage
 
 ### Installation
 
-TODO
+```bash
+pip install -U legion-cli --user
+```
 
 ### Configuration
 
 TODO
 
 ### Usage
 
@@ -36,53 +47,61 @@
 - All internal arguments passing should be typechecked whenever possible with `typeguard.typechecked`
 
 ### Development Setup
 
 Using [poetry](https://python-poetry.org/) install from inside the repo directory:
 
 ```bash
-poetry install
+pdm install
 ```
 
-This will set up a virtualenv which you can always activate with either `poetry shell` or run specific commands with `poetry run`. All instructions below that are meant to be run in the virtualenv will be prefaced with `(legion-cli)$ `
-
 #### IDE Setup
 
 **Sublime Text 3**
 
 ```bash
-curl -sSL https://gitlab.com/-/snippets/2066312/raw/master/poetry.sublime-project.py | poetry run python
+curl -sSL https://gitlab.com/-/snippets/2385805/raw/main/pdm.sublime-project.py | pdm run python > legion-cli.sublime-project
 ```
 
-#### Development
-
 ### Testing
 
 All testing should be done with `pytest` which is installed with the `dev` requirements.
 
 To run all the unit tests, execute the following from the repo directory:
 
 ```bash
-(legion-cli)$  pytest
+pdm run pytest
 ```
 
-This should produce a coverage report in `/path/to/dewey-api/htmlcov/`
+This should produce a coverage report in `/path/to/legion-cli/htmlcov/`
 
 While developing, you can use [`watchexec`](https://github.com/watchexec/watchexec) to monitor the file system for changes and re-run the tests:
 
 ```bash
-(legion-cli)$ watchexec -r -e py,yaml pytest
+watchexec -r -e py,yaml pdm run pytest
 ```
 
 To run a specific test file:
 
 ```bash
-(legion-cli)$ pytest tests/unit/test_cli.py
+pdm run pytest tests/unit/test_config.py
 ```
 
 To run a specific test:
 
 ```bash
-(legion-cli)$ pytest tests/unit/test_cli.py::test_cli_basics
+pdm run pytest tests/unit/test_config.py::test_config_loading
 ```
 
 For more information on testing, see the `pytest.ini` file as well as the [documentation](https://docs.pytest.org/en/stable/).
+
+#### Integration Testing
+
+For integration testing, this code uses [testcontainers-rabbitmq](https://testcontainers-python.readthedocs.io/en/latest/rabbitmq/README.html). In order to enable this, you will need to install docker, and ensure that your user has the ability to interact with the docker service:
+
+```bash
+sudo apt install docker
+sudo groupadd docker # may fail if the docker group already exists
+sudo usermod -aG docker $USER
+newgrp docker
+docker run hello-world # verify that everything is working well
+```
```

### Comparing `legion-cli-0.2.6/legion_cli/alerts_manager.py` & `legion-cli-0.2.7/legion_cli/alerts_manager.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/legion_cli/cli.py` & `legion-cli-0.2.7/legion_cli/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -30,24 +30,26 @@
     proc.terminate()
     proc.join(timeout=timeout)
     proc.kill()
     proc.join()
 
 
 class MessagePrinter:
+    @typechecked
     def __init__(
         self, msg_limit_received: Optional[Event] = None, num_msgs: Optional[int] = None
     ):
         self.msg_limit_received = msg_limit_received
         self.num_msgs = num_msgs
 
     @property
     def term_width(self) -> int:
         return get_terminal_size().columns
 
+    @typechecked
     def _priority_color(self, msg: Message) -> Optional[str]:
         if msg.contents["priority"] == 1:
             return "blue"
         if msg.contents["priority"] == 2:
             return "yellow"
         if msg.contents["priority"] == 3:
             return "red"
@@ -55,26 +57,28 @@
             return "magenta"
         return None
 
     @lru_cache
     def _label(self, msg: Message) -> str:
         return f"{Priority(msg.contents['priority']).name}: {msg.timestamp.format()}"
 
+    @typechecked
     def _header(self, msg: Message) -> str:
         width = self.term_width
         untrimmed_header = f"{'=' * ((width - 2 - len(self._label(msg))) // 2 + 1)} {self._label(msg)} {'=' * ((width - 2 - len(self._label(msg))) // 2)}"
         return untrimmed_header[:width]
 
+    @typechecked
     def _route(self, msg: Message) -> str:
         width = self.term_width
         untrimmed_route = f"{'-' * ((width - 2 - len(msg.routing_key)) // 2 + 1)} {msg.routing_key} {'-' * ((width - 2 - len(msg.routing_key)) // 2)}"
         return untrimmed_route[:width]
 
     @typechecked
-    def watch(self, msg: Message) -> None:
+    def print_msg(self, msg: Message) -> None:
         print(colored(self._header(msg), self._priority_color(msg)))
         print(colored(self._route(msg), self._priority_color(msg)))
         print(colored(pformat(msg.contents), self._priority_color(msg)))
         print(colored("=" * self.term_width, self._priority_color(msg)))
         if self.num_msgs is not None:  # pragma: no cover
             self.num_msgs -= 1
             if self.num_msgs <= 0 and self.msg_limit_received is not None:
@@ -87,28 +91,29 @@
     exchange_routes: Optional[Iterable[Tuple[str, str]]] = None,
     alert_exchanges: Optional[Iterable[str]] = None,
     done: Optional[Event] = None,
     config: Optional[RobotnikConfig] = None,
     num_msgs: Optional[int] = None,
 ):
     try:
-        watcher = MessagePrinter(done, num_msgs)
+        msg_printer = MessagePrinter(done, num_msgs)
         sub = Subscriber(config=config)
         if exchanges is not None:
             for exchange in exchanges:
                 sub.bind(exchange)
         if exchange_routes is not None:
             for exchange, binding in exchange_routes:
                 sub.bind(exchange, binding)
         if alert_exchanges is not None:
             for exchange in alert_exchanges:
                 sub.bind(exchange, "#.warning")
                 sub.bind(exchange, "#.error")
                 sub.bind(exchange, "#.critical")
-        sub.run(watcher.watch)
+        for msg in sub.consume():
+            msg_printer.print_msg(msg)
     except KeyboardInterrupt:
         pass
     except Exception:  # pylint: disable=W0703
         print_exc()
     finally:
         if done is not None:
             done.set()
```

### Comparing `legion-cli-0.2.6/legion_cli/log.py` & `legion-cli-0.2.7/legion_cli/log.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/legion_cli/tui/alerts_monitor.py` & `legion-cli-0.2.7/legion_cli/tui/alerts_monitor.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/legion_cli/tui/detail_list.py` & `legion-cli-0.2.7/legion_cli/tui/detail_list.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/legion_cli/tui/keyboard.py` & `legion-cli-0.2.7/legion_cli/tui/keyboard.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/pyproject.toml` & `legion-cli-0.2.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "legion-cli"
-version = "0.2.6"
+version = "0.2.7"
 description = "Commandline Utilities for the Legion Alerting and Monitoring System"
 authors = [
     { name = "Eugene Kovalev", email = "eugene@kovalev.systems" },
 ]
 dependencies = [
     "click>=8.0",
-    "legion-utils>=0.2.12",
+    "legion-utils>=0.2.14",
     "rich>=10.8.0",
     "termcolor>=1.1",
 ]
 requires-python = ">=3.8.3,<4.0"
 readme = "README.md"
 
 [project.license]
@@ -26,14 +26,17 @@
 dev = [
     "pytest>=7.3.0",
     "pytest-cov>=4.0.0",
     "pylint<3.0.0,>=2.12.2",
     "pytest-mock>=3.6.1",
     "mypy<1.0,>=0.930",
     "flake8<5.0.0,>=3.0.0",
+    "testcontainers[rabbitmq]>=3.7.1",
+    "robotnikmq @ file:///${PROJECT_ROOT}/../robotnikmq",
+    "legion-utils @ file:///${PROJECT_ROOT}/../legion-utils",
 ]
 
 [tool.pdm.scripts.publish-test]
 cmd = "twine upload -r testpypi dist/*"
 
 [tool.pdm.scripts.publish-prod]
 cmd = "twine upload -r pypi dist/*"
```

### Comparing `legion-cli-0.2.6/tests/integration/test_watch.py` & `legion-cli-0.2.7/tests/integration/test_watch.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,40 +1,50 @@
-from os.path import realpath
-from pathlib import Path
+# from os.path import realpath
+# from pathlib import Path
 
-from robotnikmq.config import RobotnikConfig, server_config
+# from robotnikmq.config import RobotnikConfig, server_config
 
-from tests.integration.utils import vagrant_test
+# from tests.integration.utils import vagrant_test
 
-from legion_cli.cli import _watch
+# from legion_cli.cli import _watch
 
-try:
-    from pytest_cov.embed import cleanup_on_sigterm
-except ImportError:
-    pass
-else:
-    cleanup_on_sigterm()
-
-HERE = Path(realpath(__file__)).parent
-CA_CERT = HERE / 'vagrant' / 'pki' / 'robotnik-ca.crt'
-USERNAME = 'legion'
-PASSWORD = 'hackme'
-VIRTUAL_HOST = '/legion'
-CERT = HERE / 'vagrant' / 'pki' / 'issued' / 'rabbitmq-vm' / 'rabbitmq-vm.crt'
-KEY = HERE / 'vagrant' / 'pki' / 'issued' / 'rabbitmq-vm' / 'rabbitmq-vm.key'
-PORT = 5671
-LOCALHOST = '127.0.0.1'
-META_QUEUE = 'skynet.legion'
-CONFIG = RobotnikConfig(tiers=[[server_config(LOCALHOST, PORT, USERNAME, PASSWORD,
-                                VIRTUAL_HOST, CA_CERT, CERT, KEY)]])
-
-
-# @vagrant_test
-# def test_basic_watch():
-#     print()
-#     _watch(['skynet.rabbitmq-vm.network'], msg_limit=2, config=CONFIG)
-
-
-# @vagrant_test
-# def test_big_message_watch():
-#     print()
-#     _watch(['skynet.rabbitmq-vm.system'], msg_limit=2, config=CONFIG)
+# try:
+#     from pytest_cov.embed import cleanup_on_sigterm
+# except ImportError:
+#     pass
+# else:
+#     cleanup_on_sigterm()
+
+# HERE = Path(realpath(__file__)).parent
+# CA_CERT = HERE / 'vagrant' / 'pki' / 'robotnik-ca.crt'
+# USERNAME = 'legion'
+# PASSWORD = 'hackme'
+# VIRTUAL_HOST = '/legion'
+# CERT = HERE / 'vagrant' / 'pki' / 'issued' / 'rabbitmq-vm' / 'rabbitmq-vm.crt'
+# KEY = HERE / 'vagrant' / 'pki' / 'issued' / 'rabbitmq-vm' / 'rabbitmq-vm.key'
+# PORT = 5671
+# LOCALHOST = '127.0.0.1'
+# META_QUEUE = 'skynet.legion'
+# CONFIG = RobotnikConfig(tiers=[[server_config(LOCALHOST, PORT, USERNAME, PASSWORD,
+#                                 VIRTUAL_HOST, CA_CERT, CERT, KEY)]])
+
+
+# # @vagrant_test
+# # def test_basic_watch():
+# #     print()
+# #     _watch(['skynet.rabbitmq-vm.network'], msg_limit=2, config=CONFIG)
+
+
+# # @vagrant_test
+# # def test_big_message_watch():
+# #     print()
+# #     _watch(['skynet.rabbitmq-vm.system'], msg_limit=2, config=CONFIG)
+
+# import pika
+from testcontainers.rabbitmq import RabbitMqContainer
+
+
+def test_basic_watch():
+    with RabbitMqContainer("rabbitmq:3.9.10") as rabbitmq:
+        print(rabbitmq.get_connection_params())
+        # connection = pika.BlockingConnection(rabbitmq.get_connection_params())
+        # # channel = connection.channel()
```

### Comparing `legion-cli-0.2.6/tests/unit/test_alerts_manager.py` & `legion-cli-0.2.7/tests/unit/test_alerts_manager.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/tests/unit/test_config.py` & `legion-cli-0.2.7/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `legion-cli-0.2.6/tests/unit/test_detail_list.py` & `legion-cli-0.2.7/tests/unit/test_detail_list.py`

 * *Files identical despite different names*

