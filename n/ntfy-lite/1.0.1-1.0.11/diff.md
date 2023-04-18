# Comparing `tmp/ntfy_lite-1.0.1.tar.gz` & `tmp/ntfy_lite-1.0.11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ntfy_lite-1.0.1.tar", max compression
+gzip compressed data, was "ntfy_lite-1.0.11.tar", max compression
```

## Comparing `ntfy_lite-1.0.1.tar` & `ntfy_lite-1.0.11.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1552 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/LICENSE
--rw-r--r--   0        0        0      242 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/__init__.py
--rw-r--r--   0        0        0     2486 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/actions.py
--rw-r--r--   0        0        0      495 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/defaults.py
--rw-r--r--   0        0        0      407 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/error.py
--rw-r--r--   0        0        0     4653 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/handler.py
--rw-r--r--   0        0        0     4770 2023-01-11 12:55:20.699672 ntfy_lite-1.0.1/ntfy_lite/ntfy.py
--rw-r--r--   0        0        0      896 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/ntfy2logging.py
--rw-r--r--   0        0        0        0 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/py.typed
--rw-r--r--   0        0        0      510 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/utils.py
--rw-r--r--   0        0        0       93 2022-10-25 10:00:23.479164 ntfy_lite-1.0.1/ntfy_lite/version.py
--rw-r--r--   0        0        0      787 2023-01-11 12:55:39.463911 ntfy_lite-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1181 2023-01-11 12:56:05.032238 ntfy_lite-1.0.1/readme.md
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 ntfy_lite-1.0.1/setup.py
--rw-r--r--   0        0        0     2107 1970-01-01 00:00:00.000000 ntfy_lite-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1552 2023-04-18 13:18:09.708251 ntfy_lite-1.0.11/LICENSE
+-rw-r--r--   0        0        0     1445 2023-04-18 13:18:09.708251 ntfy_lite-1.0.11/README.md
+-rw-r--r--   0        0        0      275 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/__init__.py
+-rw-r--r--   0        0        0     3051 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/actions.py
+-rw-r--r--   0        0        0      703 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/defaults.py
+-rw-r--r--   0        0        0     3845 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/demo_logging.py
+-rw-r--r--   0        0        0     2189 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/demo_push.py
+-rw-r--r--   0        0        0      407 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/error.py
+-rw-r--r--   0        0        0     5311 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/handler.py
+-rw-r--r--   0        0        0     6692 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/ntfy.py
+-rw-r--r--   0        0        0     1185 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/ntfy2logging.py
+-rw-r--r--   0        0        0        0 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/py.typed
+-rw-r--r--   0        0        0      565 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/utils.py
+-rw-r--r--   0        0        0       76 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/ntfy_lite/version.py
+-rw-r--r--   0        0        0      946 2023-04-18 13:18:09.712251 ntfy_lite-1.0.11/pyproject.toml
+-rw-r--r--   0        0        0     2054 1970-01-01 00:00:00.000000 ntfy_lite-1.0.11/PKG-INFO
```

### Comparing `ntfy_lite-1.0.1/LICENSE` & `ntfy_lite-1.0.11/LICENSE`

 * *Files identical despite different names*

### Comparing `ntfy_lite-1.0.1/ntfy_lite/actions.py` & `ntfy_lite-1.0.11/ntfy_lite/actions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,32 @@
+""" Module defining the Action class as well as it subclasses:
+
+- ViewAction
+- HttpAction
+"""
+
 import typing
 from enum import Enum, auto
 from .utils import validate_url
 
 
 class Action:
     """
     Superclass for action buttons.
-    See: https://ntfy.sh/docs/publish/#action-buttons
+
+    See: [ntfy button action documentation](https://ntfy.sh/docs/publish/#action-buttons)
 
     Args:
       action: name of the action (e.g. 'view', 'http')
       label: description of the action
       url: where the action redirects
       clear: if true, the notification is deleted upon click
     """
 
     def __init__(self, action: str, label: str, url: str, clear: bool = False):
-
         validate_url("Action.url", url)
 
         self.action = action
         self.label = label
         self.url = url
         if clear:
             self.clear = "true"
@@ -34,16 +40,16 @@
             + [f"{attr}={value}" for attr, value in values.items() if value is not None]
         )
 
 
 class ViewAction(Action):
     """
     Class encapsulating the information of a view action.
-    See: https://ntfy.sh/docs/publish/#open-websiteapp
-    For arguments: see documentation of the Action superclass
+    See: [ntfy view action](https://ntfy.sh/docs/publish/#open-websiteapp)
+    For arguments: see documentation of the [ntfy_lite.actions.Action][] superclass
     """
 
     def __init__(self, label: str, url: str, clear: bool = False) -> None:
         super().__init__("view", label, url, clear)
 
     def __str__(self) -> str:
         _attrs = ("label", "url", "clear")
@@ -53,22 +59,36 @@
 class HttpMethod(Enum):
     """
     List of methods supported by instances
     of HttpAction.
     """
 
     GET = auto()
+    """ GET http method """
+
     POST = auto()
+    """ POST http method """
+
     PUT = auto()
+    """ PUT http method """
 
 
 class HttpAction(Action):
     """
     Class encapsulating the information of a view action.
-    See: https://ntfy.sh/docs/publish/#send-http-request
+    See: [ntfy http action](https://ntfy.sh/docs/publish/#send-http-request)
+
+    Args:
+      label: arbitrary string
+      url: url to which the request should be sent
+      clear: if the ntfy notification should be cleared after the request succeeds
+      method: GET, POST or PUT
+      headers: HTTP headers to be passed in the request
+      body: HTTP body
+
     """
 
     def __init__(
         self,
         label: str,
         url: str,
         clear: bool = False,
```

### Comparing `ntfy_lite-1.0.1/ntfy_lite/handler.py` & `ntfy_lite-1.0.11/ntfy_lite/handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,43 @@
+"""
+Module defining the NtfyHandler class.
+
+The NtfyHandler is a logging handler, i.e. an handler suitable for the
+[python logging package](https://docs.python.org/3/library/logging.html)
+
+``` python
+# Basic usage
+
+import logging
+import ntfy_lite as ntfy
+
+ntfy_handler = ntfy.NtfyHandler("my_topic")
+
+logging.basicConfig(
+        level=logging.INFO,
+        format="[%(levelname)s] %(asctime)s | %(name)s |  %(message)s",
+        datefmt="%d-%b-%y %H:%M:%S",
+        handlers=(ntfy_handler,),
+)
+```
+
+
+"""
+
 import logging
 import typing
 from pathlib import Path
 from .ntfy2logging import LoggingLevel, Priority, level2priority
 from .defaults import level2tags
 from .ntfy import DryRun, push
 
 
 class NtfyHandler(logging.Handler):
-    """Logging Handler that push ntfy notifications.
+    """Subclass of [logging.Handler](https://docs.python.org/3/library/logging.html#handler-objects)
+    that pushes ntfy notifications.
 
     The notification title will be the record name, and the
     notification message will be either the record message or a
     file attachment (depending on the level2filepath argument).
     """
 
     def __init__(
@@ -75,14 +101,17 @@
             return True
         if record.msg == previous_message:
             return False
         self._last_messages[record.name] = record.msg
         return True
 
     def emit(self, record: logging.LogRecord) -> None:
+        """
+        Push the record as an ntfy message.
+        """
         if self._last_messages and not self._is_new_record(record):
             return
         try:
             filepath = self._level2filepath[record.levelno]
             message = None
         except KeyError:
             filepath = None
```

### Comparing `ntfy_lite-1.0.1/ntfy_lite/ntfy.py` & `ntfy_lite-1.0.11/ntfy_lite/ntfy.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+"""
+Module defining the push method, which send a message or the content of a file to an NTFY channel.
+"""
+
 import typing
 import requests
 from pathlib import Path
 from enum import Enum, auto
 from .ntfy2logging import Priority
 from .actions import Action
 from .utils import validate_url
@@ -17,15 +21,14 @@
     returns either the message string or the opened file, and ensure the file is closed
     (if data is a file).
     """
 
     def __init__(
         self, message: typing.Optional[str], filepath: typing.Optional[Path]
     ) -> None:
-
         # checking the user is at least pushing a message
         # or a file attachment
         if not any((message, filepath)):
             raise ValueError(
                 "must push either a message or a filepath"
                 " (no message nor filepath argument specified)"
             )
@@ -57,14 +60,26 @@
 
     def __exit__(self, _, __, ___) -> None:
         if not isinstance(self._data, str):
             self._data.close()
 
 
 class DryRun(Enum):
+    """
+    An optional value of DryRun may be passed as an argument to the [ntfy_lite.ntfy.push][] function.
+
+    - If 'off' is passed (default), then the [ntfy_lite.ntfy.push][] function will publish to ntfy.
+
+    - If 'on' is passed, then the [ntfy_lite.ntfy.push][] function will *not* publish to ntfy.
+
+    - If 'error' is passed, then the [ntfy_lite.ntfy.push][] function will raise an [ntfy_lite.error.NtfyError].
+
+    This is meant for testing.
+    """
+
     on = auto()
     off = auto()
     error = auto()
 
 
 def push(
     topic: str,
@@ -80,26 +95,53 @@
     actions: typing.Union[Action, typing.Sequence[Action]] = [],
     at: typing.Optional[str] = None,
     url: typing.Optional[str] = "https://ntfy.sh",
     dry_run: DryRun = DryRun.off,
 ) -> None:
     """
     Pushes a notification.
-    For documentation of all arguments, visit:
-    https://ntfy.sh/docs/publish/
+
+    ```python
+    # basic usage
+    import ntfy_lite as ntfy
+
+    ntfy.push(
+        "my topic", priority=ntfy.Priority.DEFAULT, message="my message"
+    )
+    ```
+
+    For more documentation of all arguments, visit:
+    [https://ntfy.sh/docs/publish/](https://ntfy.sh/docs/publish/)
+
+    Args:
+      topic: the ntfy topic on which to publish
+      title: the title of the notification
+      message: the message. It is optional and if None, then a filepath argument must be provided instead.
+      priority: the priority of the notification
+      tags (i.e. emojis): either a string (a single tag) or a list of string (several tags). see [supported emojis](https://docs.ntfy.sh)
+      click: URL link to be included in the notification
+      email: address to which the notification should also be sent
+      filepath: path to the file to be sent as attachement.
+        It is optional and if None, then a message argument must be provided instead.
+      icon: URL to an icon to include in the notification
+      actions: An action is either a [ntfy_lite.actions.ViewAction][]
+        (i.e. a link to a website) or a [ntfy_lite.actions.HttpAction][]
+        (i.e. sending of a HTTP GET, POST or PUT request to a website)
+      at: to be used for delayed notification, see [scheduled delivery](https://ntfy.sh/docs/publish/#scheduled-delivery)
+      url: ntfy server
+      dry_run: for testing purposes, see [ntfy_lite.ntfy.DryRun][]
     """
 
     # the message manager:
     # - checks that either message or filepath is not None
     # - if filepath is not None, data is a file to the path
     # - else data is the UTF-8 conversion of message
     # This context manager makes sure that data get closed
     # (if a file)
     with _DataManager(message, filepath) as data:
-
         # checking that arguments that are expected to be
         # urls are urls
         urls = {"click": click, "attach": attach, "icon": icon}
         for attr, value in urls.items():
             # throw value error if not None
             # and not a url
             validate_url(attr, value)
```

### Comparing `ntfy_lite-1.0.1/ntfy_lite/ntfy2logging.py` & `ntfy_lite-1.0.11/ntfy_lite/ntfy2logging.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,52 @@
+"""
+Module defining:
+
+- LoggingLevel: typing union of all logging levels
+- Priority: enumeration over ntfy priority levels
+- level2priority: default mapping between logging levels and ntfy priority levels
+"""
+
 from enum import Enum
 import typing
 import logging
 
 LoggingLevel = typing.Literal[  # type: ignore
     logging.DEBUG,  # type: ignore
     logging.INFO,
     logging.NOTSET,
     logging.WARNING,
     logging.ERROR,
     logging.CRITICAL,
 ]
 """
 Union of all logging levels (DEBUG, INFO, NOTSET,
-WARNING, ERROR and CRITICLA)
+WARNING, ERROR and CRITICAL)
 """
 
 
 class Priority(Enum):
     """
     Enumeration of supported ntfy priority levels
     """
 
     MAX = "5"
+    """MAX"""
+
     HIGH = "4"
+    """HIGH"""
+
     DEFAULT = "3"
+    """DEFAULT"""
+
     LOW = "2"
+    """LOW"""
+
     MIN = "1"
+    """MIN"""
 
 
 level2priority: typing.Dict[LoggingLevel, Priority] = {
     logging.CRITICAL: Priority.MAX,
     logging.ERROR: Priority.HIGH,
     logging.WARNING: Priority.HIGH,
     logging.INFO: Priority.DEFAULT,
```

### Comparing `ntfy_lite-1.0.1/readme.md` & `ntfy_lite-1.0.11/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ![unit tests](https://github.com/MPI-IS/ntfy_lite/actions/workflows/tests.yaml/badge.svg)
 ![mypy](https://github.com/MPI-IS/ntfy_lite/actions/workflows/python_mypy.yml/badge.svg)
+[![documentation](https://github.com/MPI-IS/ntfy_lite/actions/workflows/mkdocs.yaml/badge.svg)](https://mpi-is.github.io/ntfy_lite/)
+[![PyPI](https://github.com/MPI-IS/ntfy_lite/actions/workflows/pypi_publish.yml/badge.svg)](https://pypi.org/project/ntfy-lite/)
+
+
 
 # NTFY LITE
 
 **ntfy_lite** is a minimalistic python API for sending [ntfy](https://ntfy.sh) notifications.
 
 It comes with a **Handler** for the [logging package](https://docs.python.org/3/library/logging.html).
```

### Comparing `ntfy_lite-1.0.1/setup.py` & `ntfy_lite-1.0.11/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,67 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: ntfy-lite
+Version: 1.0.11
+Summary: minimalistic python API for sending ntfy notifications
+License: BSD-3-Clause
+Author: Vincent Berenz
+Author-email: vberenz@tuebingen.mpg.de
+Requires-Python: >3.8.1,<4
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: validators (>=0.20.0,<0.21.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['ntfy_lite']
+![unit tests](https://github.com/MPI-IS/ntfy_lite/actions/workflows/tests.yaml/badge.svg)
+![mypy](https://github.com/MPI-IS/ntfy_lite/actions/workflows/python_mypy.yml/badge.svg)
+[![documentation](https://github.com/MPI-IS/ntfy_lite/actions/workflows/mkdocs.yaml/badge.svg)](https://mpi-is.github.io/ntfy_lite/)
+[![PyPI](https://github.com/MPI-IS/ntfy_lite/actions/workflows/pypi_publish.yml/badge.svg)](https://pypi.org/project/ntfy-lite/)
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['pytest>=7.1.3,<8.0.0',
- 'requests>=2.28.1,<3.0.0',
- 'types-requests>=2.28.11.2,<3.0.0.0',
- 'validators>=0.20.0,<0.21.0']
-
-setup_kwargs = {
-    'name': 'ntfy-lite',
-    'version': '1.0.1',
-    'description': 'minimalistic python API for sending ntfy notifications',
-    'long_description': '![unit tests](https://github.com/MPI-IS/ntfy_lite/actions/workflows/tests.yaml/badge.svg)\n![mypy](https://github.com/MPI-IS/ntfy_lite/actions/workflows/python_mypy.yml/badge.svg)\n\n# NTFY LITE\n\n**ntfy_lite** is a minimalistic python API for sending [ntfy](https://ntfy.sh) notifications.\n\nIt comes with a **Handler** for the [logging package](https://docs.python.org/3/library/logging.html).\n\n\n## Installation\n\nfrom source:\n\n```bash\ngit clone https://github.com/MPI-IS/ntfy_lite.git\ncd ntfy_lite\npip install .\n```\n\nfrom pypi:\n```bash\npip install ntfy_lite\n```\n\n## Usage\n\nThe two following examples cover the full API.\nYou may also find the code in the demos folder of the sources.\n\n### pushing notifications\nhttps://github.com/MPI-IS/ntfy_lite/blob/da5750eed1ed58eacf4ff1bb1498586b41242f70/demos/ntfy_push.py#L1-L73\n\n### logging handler\n\nhttps://github.com/MPI-IS/ntfy_lite/blob/52fc7f008fdac3f735d39dd01064a0aa5b751e00/demos/ntfy_logging.py#L1-L146\n\n## Limitation\n\nNo check regarding ntfy [limitations](https://ntfy.sh/docs/publish/#limitations) is performed before notifications are sent.\n\n## Copyright\n\n© 2020, Max Planck Society - Max Planck Institute for Intelligent Systems\n\n',
-    'author': 'Vincent Berenz',
-    'author_email': 'vberenz@tuebingen.mpg.de',
-    'maintainer': 'Vincent Berenz',
-    'maintainer_email': 'vberenz@tuebingen.mpg.de',
-    'url': 'https://github.com/MPI-IS/ntfy_lite',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4',
-}
+
+# NTFY LITE
+
+**ntfy_lite** is a minimalistic python API for sending [ntfy](https://ntfy.sh) notifications.
+
+It comes with a **Handler** for the [logging package](https://docs.python.org/3/library/logging.html).
+
+
+## Installation
+
+from source:
+
+```bash
+git clone https://github.com/MPI-IS/ntfy_lite.git
+cd ntfy_lite
+pip install .
+```
+
+from pypi:
+```bash
+pip install ntfy_lite
+```
+
+## Usage
+
+The two following examples cover the full API.
+You may also find the code in the demos folder of the sources.
+
+### pushing notifications
+https://github.com/MPI-IS/ntfy_lite/blob/da5750eed1ed58eacf4ff1bb1498586b41242f70/demos/ntfy_push.py#L1-L73
+
+### logging handler
+
+https://github.com/MPI-IS/ntfy_lite/blob/52fc7f008fdac3f735d39dd01064a0aa5b751e00/demos/ntfy_logging.py#L1-L146
+
+## Limitation
+
+No check regarding ntfy [limitations](https://ntfy.sh/docs/publish/#limitations) is performed before notifications are sent.
+
+## Copyright
+
+© 2020, Max Planck Society - Max Planck Institute for Intelligent Systems
 
 
-setup(**setup_kwargs)
```

