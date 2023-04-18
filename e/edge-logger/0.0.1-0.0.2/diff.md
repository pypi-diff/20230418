# Comparing `tmp/edge_logger-0.0.1.tar.gz` & `tmp/edge_logger-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge_logger-0.0.1.tar", max compression
+gzip compressed data, was "edge_logger-0.0.2.tar", max compression
```

## Comparing `edge_logger-0.0.1.tar` & `edge_logger-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.1/LICENSE
--rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.1/edge_logger/__init__.py
--rw-r--r--   0        0        0     4964 2023-04-17 02:57:57.724043 edge_logger-0.0.1/edge_logger/edge_logger.py
--rw-r--r--   0        0        0      359 2023-04-16 20:05:25.473619 edge_logger-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 edge_logger-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-16 19:59:55.248252 edge_logger-0.0.2/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-17 03:01:06.502367 edge_logger-0.0.2/README.md
+-rw-r--r--   0        0        0        0 2023-04-16 20:07:03.564649 edge_logger-0.0.2/edge_logger/__init__.py
+-rw-r--r--   0        0        0     3804 2023-04-18 00:47:07.321721 edge_logger-0.0.2/edge_logger/edge_logger.py
+-rw-r--r--   0        0        0      359 2023-04-18 00:47:07.326978 edge_logger-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      438 1970-01-01 00:00:00.000000 edge_logger-0.0.2/PKG-INFO
```

### Comparing `edge_logger-0.0.1/LICENSE` & `edge_logger-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edge_logger-0.0.1/edge_logger/edge_logger.py` & `edge_logger-0.0.2/edge_logger/edge_logger.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,66 +1,36 @@
 import logging
 import json
 import sys
 from typing import Mapping, Any
 
 
 # https://github.com/tomoum/logzilla/blob/main/src/logzilla/logzilla.py#L145
-class ColorFormatter(logging.Formatter):
-    """Custom formatter for logging module"""
 
-    white = "\x1b[37;20m"
-    green = "\x1b[32;20m"
-    blue = "\x1b[34;20m"
-    cyan = "\x1b[36;20m"
-    yellow = "\x1b[33;20m"
-    red = "\x1b[31;20m"
-    bold_red = "\x1b[31;1m"
-    reset = "\x1b[0m"
+class JsonFormatter(logging.Formatter):
 
-    def __init__(self) -> None:
+    def __init__(self, indent=False):
         super().__init__()
-        self.formats = {
-            logging.DEBUG: self.cyan + "%(message)s" + self.reset,
-            logging.INFO: self.green + "%(message)s" + self.reset,
-            logging.WARNING: self.yellow + "%(message)s" + self.reset,
-            logging.ERROR: self.red + "%(message)s" + self.reset,
-            logging.CRITICAL: self.bold_red + "%(message)s" + self.reset,
-        }
-
-    def format(self, record):
-        log_data = {
-            'time': self.formatTime(record),
-            'level': record.levelname,
-            'name': record.name,
-            'message': record.getMessage(),
-            # 'line': record.lineno,
-        }
-        # If we added extra information, update log record
-        if record.__getattribute__("_extra"):
-            log_data.update(record.__getattribute__("_extra"))
-        log_fmt = self.formats.get(record.levelno)
-        record.msg = json.dumps(log_data)
-        formatter = logging.Formatter(log_fmt)
-        return formatter.format(record)
+        self._indent = indent
 
-
-class JsonFormatter(logging.Formatter):
     def format(self, record):
         log_data = {
             'time': self.formatTime(record),
             'level': record.levelname,
             'name': record.name,
             'message': record.getMessage(),
             # 'line': record.lineno,
         }
         # If we added extra information, update log record
         if record.__getattribute__("_extra"):
             log_data.update(record.__getattribute__("_extra"))
-        return json.dumps(log_data, indent=4)
+        if self._indent:
+            return json.dumps(log_data, indent=4)
+        else:
+            return json.dumps(log_data)
 
 
 class EdgeLogger(logging.Logger):
     """
     Subclass logging.Logger so we can extend makeRecord to add dynamic information on a per-log basis
     https://docs.python.org/3/library/logging.html#logging.Logger
     """
```

