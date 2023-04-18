# Comparing `tmp/python-send-logs-to-0.1.0b0.tar.gz` & `tmp/python-send-logs-to-0.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-send-logs-to-0.1.0b0.tar", last modified: Mon Jan  9 12:06:21 2023, max compression
+gzip compressed data, was "python-send-logs-to-0.2.0b0.tar", last modified: Tue Apr 18 10:51:00 2023, max compression
```

## Comparing `python-send-logs-to-0.1.0b0.tar` & `python-send-logs-to-0.2.0b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-01-09 12:06:21.520683 python-send-logs-to-0.1.0b0/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-01-09 11:43:11.000000 python-send-logs-to-0.1.0b0/LICENSE
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2191 2023-01-09 12:06:21.520683 python-send-logs-to-0.1.0b0/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1417 2023-01-09 11:59:08.000000 python-send-logs-to-0.1.0b0/README.md
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-01-09 12:06:21.520683 python-send-logs-to-0.1.0b0/log_to/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       27 2023-01-09 11:57:48.000000 python-send-logs-to-0.1.0b0/log_to/__init__.py
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5565 2023-01-09 11:16:45.000000 python-send-logs-to-0.1.0b0/log_to/redis.py
-drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-01-09 12:06:21.520683 python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2191 2023-01-09 12:06:21.000000 python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/PKG-INFO
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      275 2023-01-09 12:06:21.000000 python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/SOURCES.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-01-09 12:06:21.000000 python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/dependency_links.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        6 2023-01-09 12:06:21.000000 python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/requires.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        7 2023-01-09 12:06:21.000000 python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/top_level.txt
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-01-09 12:06:21.520683 python-send-logs-to-0.1.0b0/setup.cfg
--rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1700 2023-01-09 12:00:21.000000 python-send-logs-to-0.1.0b0/setup.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1072 2023-01-09 11:43:11.000000 python-send-logs-to-0.2.0b0/LICENSE
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2191 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1417 2023-01-09 11:59:08.000000 python-send-logs-to-0.2.0b0/README.md
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/log_to/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       27 2023-04-18 10:46:22.000000 python-send-logs-to-0.2.0b0/log_to/__init__.py
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     5706 2023-04-18 10:47:06.000000 python-send-logs-to-0.2.0b0/log_to/redis.py
+drwxrwxr-x   0 lenovo    (1000) lenovo    (1000)        0 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     2191 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/PKG-INFO
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)      275 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/SOURCES.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        1 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/dependency_links.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        6 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/requires.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)        7 2023-04-18 10:51:00.000000 python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/top_level.txt
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)       38 2023-04-18 10:51:00.894938 python-send-logs-to-0.2.0b0/setup.cfg
+-rw-rw-r--   0 lenovo    (1000) lenovo    (1000)     1700 2023-01-09 12:00:21.000000 python-send-logs-to-0.2.0b0/setup.py
```

### Comparing `python-send-logs-to-0.1.0b0/LICENSE` & `python-send-logs-to-0.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-send-logs-to-0.1.0b0/PKG-INFO` & `python-send-logs-to-0.2.0b0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-send-logs-to
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: A Python logging handler that sends logs to Redis; later to be a collection of logging handlers.
 Home-page: https://github.com/armandtvz/python-send-logs-to
 Author: Armandt van Zyl
 Author-email: armandtvz@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `python-send-logs-to-0.1.0b0/README.md` & `python-send-logs-to-0.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `python-send-logs-to-0.1.0b0/log_to/redis.py` & `python-send-logs-to-0.2.0b0/log_to/redis.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,14 +66,18 @@
         self.password = password
         self.db = db
         self.charset = charset
         self.cap = cap
         self.attach_date_to_key = attach_date_to_key
         self.redis = self.get_connection()
         self.expire_after = expire_after
+        self.formatter = logging.Formatter(
+            fmt='[{asctime}] {name} | {levelname} | {message}',
+            style='{',
+        )
 
         # Do checks for expire_after value
         if self.expire_after:
             if isinstance(self.expire_after, timedelta):
                 if self.expire_after.total_seconds() <= 10:
                     raise ValueError(
                         'expire_after timedelta object must have a delta '
```

### Comparing `python-send-logs-to-0.1.0b0/python_send_logs_to.egg-info/PKG-INFO` & `python-send-logs-to-0.2.0b0/python_send_logs_to.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-send-logs-to
-Version: 0.1.0b0
+Version: 0.2.0b0
 Summary: A Python logging handler that sends logs to Redis; later to be a collection of logging handlers.
 Home-page: https://github.com/armandtvz/python-send-logs-to
 Author: Armandt van Zyl
 Author-email: armandtvz@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `python-send-logs-to-0.1.0b0/setup.py` & `python-send-logs-to-0.2.0b0/setup.py`

 * *Files identical despite different names*

