# Comparing `tmp/structlog-sentry-2.0.0b2.tar.gz` & `tmp/structlog_sentry-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "structlog-sentry-2.0.0b2.tar", max compression
+gzip compressed data, was "structlog_sentry-2.0.1.tar", max compression
```

## Comparing `structlog-sentry-2.0.0b2.tar` & `structlog_sentry-2.0.1.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0       20 2022-08-22 08:35:42.729340 structlog-sentry-2.0.0b2/.coveragerc
--rw-r--r--   0        0        0      618 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1065 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/LICENSE
--rw-r--r--   0        0        0     5903 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/README.md
--rw-r--r--   0        0        0     1211 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/pyproject.toml
--rw-r--r--   0        0        0     6801 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/structlog_sentry/__init__.py
--rw-r--r--   0        0        0        0 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/structlog_sentry/py.typed
--rw-r--r--   0        0        0      581 2022-08-22 08:35:42.733340 structlog-sentry-2.0.0b2/tox.ini
--rw-r--r--   0        0        0     6780 2022-08-22 08:35:59.040636 structlog-sentry-2.0.0b2/setup.py
--rw-r--r--   0        0        0     6882 2022-08-22 08:35:59.041004 structlog-sentry-2.0.0b2/PKG-INFO
+-rw-r--r--   0        0        0       20 2023-04-18 12:56:42.797586 structlog_sentry-2.0.1/.coveragerc
+-rw-r--r--   0        0        0      618 2023-04-18 12:56:42.797586 structlog_sentry-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1065 2023-04-18 12:56:42.797586 structlog_sentry-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5876 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/README.md
+-rw-r--r--   0        0        0     1225 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     7312 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/structlog_sentry/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/structlog_sentry/py.typed
+-rw-r--r--   0        0        0      581 2023-04-18 12:56:42.801586 structlog_sentry-2.0.1/tox.ini
+-rw-r--r--   0        0        0     7178 1970-01-01 00:00:00.000000 structlog_sentry-2.0.1/PKG-INFO
```

### Comparing `structlog-sentry-2.0.0b2/.pre-commit-config.yaml` & `structlog_sentry-2.0.1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 repos:
   - repo: https://github.com/psf/black
-    rev: 22.6.0
+    rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
 
-  - repo: https://gitlab.com/pycqa/flake8
-    rev: 5.0.4
+  - repo: https://github.com/pycqa/flake8
+    rev: 6.0.0
     hooks:
       - id: flake8
         language_version: python3
 
   - repo: https://github.com/pycqa/isort
-    rev: 5.10.1
+    rev: 5.12.0
     hooks:
       - id: isort
         # extra dependencies for config in pyproject.toml
         additional_dependencies: [".[pyproject]"]
 
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.3.0
+    rev: v4.4.0
     hooks:
       - id: trailing-whitespace
       - id: end-of-file-fixer
       - id: debug-statements
```

### Comparing `structlog-sentry-2.0.0b2/LICENSE` & `structlog_sentry-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `structlog-sentry-2.0.0b2/README.md` & `structlog_sentry-2.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -42,27 +42,26 @@
 ```
 
 Do not forget to add the `structlog.stdlib.add_log_level` and optionally the
 `structlog.stdlib.add_logger_name` processors before `SentryProcessor`. The
 `SentryProcessor` class takes the following arguments:
 
 - `level` Events of this or higher levels will be reported as Sentry
-  breadcrumbs. Dfault is :obj:`logging.INFO`.
+  breadcrumbs. Dfault is `logging.INFO`.
 - `event_level` Events of this or higher levels will be reported to Sentry
-  as events. Default is :obj:`logging.WARNING`.
+  as events. Default is `logging.WARNING`.
 - `active` A flag to make this processor enabled/disabled.
-- `as_context` Send `event_dict` as extra info to Sentry.
-  Default is :obj:`True`.
+- `as_context` Send `event_dict` as extra info to Sentry. Default is `True`.
 - `tag_keys` A list of keys. If any if these keys appear in `event_dict`,
   the key and its corresponding value in `event_dict` will be used as Sentry
   event tags. use `"__all__"` to report all key/value pairs of event as tags.
 - `ignore_loggers` A list of logger names to ignore any events from.
 - `verbose` Report the action taken by the logger in the `event_dict`.
-  Default is :obj:`False`.
-- `hub` Optionally specify :obj:`sentry_sdk.Hub`.
+  Default is `False`.
+- `hub` Optionally specify `sentry_sdk.Hub`.
 
 Now events are automatically captured by Sentry with `log.error()`:
 
 ```python
 try:
     1/0
 except ZeroDivisionError:
```

### Comparing `structlog-sentry-2.0.0b2/pyproject.toml` & `structlog_sentry-2.0.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "structlog-sentry"
-version = "2.0.0b2"
+version = "2.0.1"
 description = "Sentry integration for structlog"
 authors = ["Kiwi.com platform <platform@kiwi.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/kiwicom/structlog-sentry"
 homepage = "https://github.com/kiwicom/structlog-sentry"
 
@@ -21,18 +21,19 @@
     "Programming Language :: Python :: 3.10",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 include = ["*.md", "*.toml", "*.txt", "*.yml", "*.yaml", ".coveragerc", "tox.ini", "structlog_sentry/py.typed"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
+packaging = "*"
 sentry-sdk = "*"
 structlog = "*"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.1.2"
+pytest = "^7.1.3"
 pytest-cov = "^3.0.0"
 pytest-mock = "^3.8.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `structlog-sentry-2.0.0b2/structlog_sentry/__init__.py` & `structlog_sentry-2.0.1/structlog_sentry/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 from __future__ import annotations
 
 import logging
 import sys
 from fnmatch import fnmatch
 from typing import Any, Iterable, Optional
 
-from sentry_sdk import Hub
+from packaging import version
+
+from sentry_sdk import VERSION, Hub
 from sentry_sdk.integrations.logging import _IGNORED_LOGGERS
 from sentry_sdk.utils import capture_internal_exceptions, event_from_exception
 from structlog.types import EventDict, ExcInfo, WrappedLogger
 
+_IS_OLD_VERSION = version.parse(VERSION) < version.parse("1.17.0")
+
 
 def _figure_out_exc_info(v: Any) -> ExcInfo:
     """
     Depending on the Python version will try to do the smartest thing possible
     to transform *v* into an ``exc_info`` tuple.
     """
     if isinstance(v, BaseException):
@@ -103,15 +107,25 @@
 
         :param event_dict: structlog event_dict
         """
         exc_info = _figure_out_exc_info(event_dict.get("exc_info", None))
         has_exc_info = exc_info and exc_info != (None, None, None)
 
         if has_exc_info:
-            event, hint = event_from_exception(exc_info)
+            options = self._get_hub().client.options
+            include_local_variables = options.get(
+                "include_local_variables", options.get("with_locals")
+            )
+            key = "with_locals" if _IS_OLD_VERSION else "include_local_variables"
+            event, hint = event_from_exception(
+                exc_info,
+                client_options={
+                    key: include_local_variables,
+                },
+            )
         else:
             event, hint = {}, {}
 
         event["message"] = event_dict.get("event")
         event["level"] = event_dict.get("level")
         if "logger" in event_dict:
             event["logger"] = event_dict["logger"]
```

### Comparing `structlog-sentry-2.0.0b2/tox.ini` & `structlog_sentry-2.0.1/tox.ini`

 * *Files identical despite different names*

### Comparing `structlog-sentry-2.0.0b2/setup.py` & `structlog_sentry-2.0.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,225 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: structlog-sentry
+Version: 2.0.1
+Summary: Sentry integration for structlog
+Home-page: https://github.com/kiwicom/structlog-sentry
+License: MIT
+Author: Kiwi.com platform
+Author-email: platform@kiwi.com
+Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: packaging
+Requires-Dist: sentry-sdk
+Requires-Dist: structlog
+Project-URL: Repository, https://github.com/kiwicom/structlog-sentry
+Description-Content-Type: text/markdown
+
+# structlog-sentry
+
+| What          | Where                                         |
+| ------------- | --------------------------------------------- |
+| Documentation | <https://github.com/kiwicom/structlog-sentry> |
+| Maintainer    | @kiwicom/platform                             |
+
+Based on <https://gist.github.com/hynek/a1f3f92d57071ebc5b91>
+
+## Installation
+
+Install the package with [pip](https://pip.pypa.io/):
+
+```
+pip install structlog-sentry
+```
+
+## Usage
+
+This module is intended to be used with `structlog` like this:
+
+```python
+import sentry_sdk
+import structlog
+from structlog_sentry import SentryProcessor
+
+
+sentry_sdk.init()  # pass dsn in argument or via SENTRY_DSN env variable
+
+structlog.configure(
+    processors=[
+        structlog.stdlib.add_logger_name,  # optional, but before SentryProcessor()
+        structlog.stdlib.add_log_level,  # required before SentryProcessor()
+        SentryProcessor(event_level=logging.ERROR),
+    ],
+    logger_factory=...,
+    wrapper_class=...,
+)
+
+
+log = structlog.get_logger()
+```
+
+Do not forget to add the `structlog.stdlib.add_log_level` and optionally the
+`structlog.stdlib.add_logger_name` processors before `SentryProcessor`. The
+`SentryProcessor` class takes the following arguments:
+
+- `level` Events of this or higher levels will be reported as Sentry
+  breadcrumbs. Dfault is `logging.INFO`.
+- `event_level` Events of this or higher levels will be reported to Sentry
+  as events. Default is `logging.WARNING`.
+- `active` A flag to make this processor enabled/disabled.
+- `as_context` Send `event_dict` as extra info to Sentry. Default is `True`.
+- `tag_keys` A list of keys. If any if these keys appear in `event_dict`,
+  the key and its corresponding value in `event_dict` will be used as Sentry
+  event tags. use `"__all__"` to report all key/value pairs of event as tags.
+- `ignore_loggers` A list of logger names to ignore any events from.
+- `verbose` Report the action taken by the logger in the `event_dict`.
+  Default is `False`.
+- `hub` Optionally specify `sentry_sdk.Hub`.
+
+Now events are automatically captured by Sentry with `log.error()`:
+
+```python
+try:
+    1/0
+except ZeroDivisionError:
+    log.error("zero divsiion")
+
+try:
+    resp = requests.get(f"https://api.example.com/users/{user_id}/")
+    resp.raise_for_status()
+except RequestException:
+    log.error("request error", user_id=user_id)
+```
+
+This won't automatically collect `sys.exc_info()` along with the message, if you want
+to enable this behavior, just pass `exc_info=True`.
+
+When you want to use structlog's built-in
+[`format_exc_info`](http://www.structlog.org/en/stable/api.html#structlog.processors.format_exc_info)
+processor, make that the `SentryProcessor` comes *before* `format_exc_info`!
+Otherwise, the `SentryProcessor` won't have an `exc_info` to work with, because
+it's removed from the event by `format_exc_info`.
+
+Logging calls with no `sys.exc_info()` are also automatically captured by Sentry
+either as breadcrumbs (if configured by the `level` argument) or as events:
+
+```python
+log.info("info message", scope="accounts")
+log.warning("warning message", scope="invoices")
+log.error("error message", scope="products")
+```
+
+If you do not want to forward a specific logs into Sentry, you can pass the
+`sentry_skip=True` optional argument to logger methods, like this:
+
+```python
+log.error("error message", sentry_skip=True)
+```
+
+### Sentry Tags
+
+You can set some or all of key/value pairs of structlog `event_dict` as sentry `tags`:
+
+```python
+structlog.configure(
+    processors=[
+        structlog.stdlib.add_logger_name,
+        structlog.stdlib.add_log_level,
+        SentryProcessor(level=logging.ERROR, tag_keys=["city", "timezone"]),
+    ],...
+)
+
+log.error("error message", city="Tehran", timezone="UTC+3:30", movie_title="Some title")
+```
+
+this will report the error and the sentry event will have **city** and **timezone** tags.
+If you want to have all event data as tags, create the `SentryProcessor` with `tag_keys="__all__"`.
+
+```python
+structlog.configure(
+    processors=[
+        structlog.stdlib.add_logger_name,
+        structlog.stdlib.add_log_level,
+        SentryProcessor(level=logging.ERROR, tag_keys="__all__"),
+    ],...
+)
+```
+
+### Skip Context
+
+By default `SentryProcessor` will send `event_dict` key/value pairs as contextual info to sentry.
+Sometimes you may want to skip this, specially when sending the `event_dict` as sentry tags:
+
+```python
+structlog.configure(
+    processors=[
+        structlog.stdlib.add_logger_name,
+        structlog.stdlib.add_log_level,
+        SentryProcessor(level=logging.ERROR, as_context=False, tag_keys="__all__"),
+    ],...
+)
+```
+
+### Ignore specific loggers
+
+If you want to ignore specific loggers from being processed by the `SentryProcessor` just pass
+a list of loggers when instantiating the processor:
+
+```python
+structlog.configure(
+    processors=[
+        structlog.stdlib.add_logger_name,
+        structlog.stdlib.add_log_level,
+        SentryProcessor(level=logging.ERROR, ignore_loggers=["some.logger"]),
+    ],...
+)
+```
+
+### Logging as JSON
+
+If you want to configure `structlog` to format the output as **JSON** (maybe for
+[elk-stack](https://www.elastic.co/elk-stack)) you have to disable standard logging
+integration in Sentry SDK by passing the `LoggingIntegration(event_level=None, level=None)`
+instance to `sentry_sdk.init` method. This prevents duplication of an event reported to sentry:
+
+```python
+from sentry_sdk.integrations.logging import LoggingIntegration
+
+
+INTEGRATIONS = [
+    # ... other integrations
+    LoggingIntegration(event_level=None, level=None),
+]
+
+sentry_sdk.init(integrations=INTEGRATIONS)
+```
+
+This integration tells `sentry_sdk` to *ignore* standard logging and captures the events manually.
+
+## Testing
+
+To run all tests:
+
+```
+tox
+```
 
-packages = \
-['structlog_sentry']
+## Contributing
 
-package_data = \
-{'': ['*']}
+Create a merge request and tag @kiwicom/platform  for review.
 
-install_requires = \
-['sentry-sdk', 'structlog']
-
-setup_kwargs = {
-    'name': 'structlog-sentry',
-    'version': '2.0.0b2',
-    'description': 'Sentry integration for structlog',
-    'long_description': '# structlog-sentry\n\n| What          | Where                                         |\n| ------------- | --------------------------------------------- |\n| Documentation | <https://github.com/kiwicom/structlog-sentry> |\n| Maintainer    | @kiwicom/platform                             |\n\nBased on <https://gist.github.com/hynek/a1f3f92d57071ebc5b91>\n\n## Installation\n\nInstall the package with [pip](https://pip.pypa.io/):\n\n```\npip install structlog-sentry\n```\n\n## Usage\n\nThis module is intended to be used with `structlog` like this:\n\n```python\nimport sentry_sdk\nimport structlog\nfrom structlog_sentry import SentryProcessor\n\n\nsentry_sdk.init()  # pass dsn in argument or via SENTRY_DSN env variable\n\nstructlog.configure(\n    processors=[\n        structlog.stdlib.add_logger_name,  # optional, but before SentryProcessor()\n        structlog.stdlib.add_log_level,  # required before SentryProcessor()\n        SentryProcessor(event_level=logging.ERROR),\n    ],\n    logger_factory=...,\n    wrapper_class=...,\n)\n\n\nlog = structlog.get_logger()\n```\n\nDo not forget to add the `structlog.stdlib.add_log_level` and optionally the\n`structlog.stdlib.add_logger_name` processors before `SentryProcessor`. The\n`SentryProcessor` class takes the following arguments:\n\n- `level` Events of this or higher levels will be reported as Sentry\n  breadcrumbs. Dfault is :obj:`logging.INFO`.\n- `event_level` Events of this or higher levels will be reported to Sentry\n  as events. Default is :obj:`logging.WARNING`.\n- `active` A flag to make this processor enabled/disabled.\n- `as_context` Send `event_dict` as extra info to Sentry.\n  Default is :obj:`True`.\n- `tag_keys` A list of keys. If any if these keys appear in `event_dict`,\n  the key and its corresponding value in `event_dict` will be used as Sentry\n  event tags. use `"__all__"` to report all key/value pairs of event as tags.\n- `ignore_loggers` A list of logger names to ignore any events from.\n- `verbose` Report the action taken by the logger in the `event_dict`.\n  Default is :obj:`False`.\n- `hub` Optionally specify :obj:`sentry_sdk.Hub`.\n\nNow events are automatically captured by Sentry with `log.error()`:\n\n```python\ntry:\n    1/0\nexcept ZeroDivisionError:\n    log.error("zero divsiion")\n\ntry:\n    resp = requests.get(f"https://api.example.com/users/{user_id}/")\n    resp.raise_for_status()\nexcept RequestException:\n    log.error("request error", user_id=user_id)\n```\n\nThis won\'t automatically collect `sys.exc_info()` along with the message, if you want\nto enable this behavior, just pass `exc_info=True`.\n\nWhen you want to use structlog\'s built-in\n[`format_exc_info`](http://www.structlog.org/en/stable/api.html#structlog.processors.format_exc_info)\nprocessor, make that the `SentryProcessor` comes *before* `format_exc_info`!\nOtherwise, the `SentryProcessor` won\'t have an `exc_info` to work with, because\nit\'s removed from the event by `format_exc_info`.\n\nLogging calls with no `sys.exc_info()` are also automatically captured by Sentry\neither as breadcrumbs (if configured by the `level` argument) or as events:\n\n```python\nlog.info("info message", scope="accounts")\nlog.warning("warning message", scope="invoices")\nlog.error("error message", scope="products")\n```\n\nIf you do not want to forward a specific logs into Sentry, you can pass the\n`sentry_skip=True` optional argument to logger methods, like this:\n\n```python\nlog.error("error message", sentry_skip=True)\n```\n\n### Sentry Tags\n\nYou can set some or all of key/value pairs of structlog `event_dict` as sentry `tags`:\n\n```python\nstructlog.configure(\n    processors=[\n        structlog.stdlib.add_logger_name,\n        structlog.stdlib.add_log_level,\n        SentryProcessor(level=logging.ERROR, tag_keys=["city", "timezone"]),\n    ],...\n)\n\nlog.error("error message", city="Tehran", timezone="UTC+3:30", movie_title="Some title")\n```\n\nthis will report the error and the sentry event will have **city** and **timezone** tags.\nIf you want to have all event data as tags, create the `SentryProcessor` with `tag_keys="__all__"`.\n\n```python\nstructlog.configure(\n    processors=[\n        structlog.stdlib.add_logger_name,\n        structlog.stdlib.add_log_level,\n        SentryProcessor(level=logging.ERROR, tag_keys="__all__"),\n    ],...\n)\n```\n\n### Skip Context\n\nBy default `SentryProcessor` will send `event_dict` key/value pairs as contextual info to sentry.\nSometimes you may want to skip this, specially when sending the `event_dict` as sentry tags:\n\n```python\nstructlog.configure(\n    processors=[\n        structlog.stdlib.add_logger_name,\n        structlog.stdlib.add_log_level,\n        SentryProcessor(level=logging.ERROR, as_context=False, tag_keys="__all__"),\n    ],...\n)\n```\n\n### Ignore specific loggers\n\nIf you want to ignore specific loggers from being processed by the `SentryProcessor` just pass\na list of loggers when instantiating the processor:\n\n```python\nstructlog.configure(\n    processors=[\n        structlog.stdlib.add_logger_name,\n        structlog.stdlib.add_log_level,\n        SentryProcessor(level=logging.ERROR, ignore_loggers=["some.logger"]),\n    ],...\n)\n```\n\n### Logging as JSON\n\nIf you want to configure `structlog` to format the output as **JSON** (maybe for\n[elk-stack](https://www.elastic.co/elk-stack)) you have to disable standard logging\nintegration in Sentry SDK by passing the `LoggingIntegration(event_level=None, level=None)`\ninstance to `sentry_sdk.init` method. This prevents duplication of an event reported to sentry:\n\n```python\nfrom sentry_sdk.integrations.logging import LoggingIntegration\n\n\nINTEGRATIONS = [\n    # ... other integrations\n    LoggingIntegration(event_level=None, level=None),\n]\n\nsentry_sdk.init(integrations=INTEGRATIONS)\n```\n\nThis integration tells `sentry_sdk` to *ignore* standard logging and captures the events manually.\n\n## Testing\n\nTo run all tests:\n\n```\ntox\n```\n\n## Contributing\n\nCreate a merge request and tag @kiwicom/platform  for review.\n',
-    'author': 'Kiwi.com platform',
-    'author_email': 'platform@kiwi.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/kiwicom/structlog-sentry',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

