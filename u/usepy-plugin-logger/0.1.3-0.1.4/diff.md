# Comparing `tmp/usepy_plugin_logger-0.1.3.tar.gz` & `tmp/usepy_plugin_logger-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "usepy_plugin_logger-0.1.3.tar", max compression
+gzip compressed data, was "usepy_plugin_logger-0.1.4.tar", max compression
```

## Comparing `usepy_plugin_logger-0.1.3.tar` & `usepy_plugin_logger-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     1634 2023-03-23 13:14:54.089494 usepy_plugin_logger-0.1.3/README.md
--rw-r--r--   0        0        0      443 2023-03-23 13:16:03.032023 usepy_plugin_logger-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      266 2023-03-23 13:14:54.090097 usepy_plugin_logger-0.1.3/src/usepy_logger/__init__.py
--rw-r--r--   0        0        0     2042 2023-03-23 13:14:54.090266 usepy_plugin_logger-0.1.3/src/usepy_logger/formatters.py
--rw-r--r--   0        0        0     1176 2023-03-23 13:14:54.090421 usepy_plugin_logger-0.1.3/src/usepy_logger/handlers.py
--rw-r--r--   0        0        0     2791 2023-03-23 13:14:54.090587 usepy_plugin_logger-0.1.3/src/usepy_logger/intercept.py
--rw-r--r--   0        0        0     1814 2023-03-23 13:14:54.090754 usepy_plugin_logger-0.1.3/src/usepy_logger/logger.py
--rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 usepy_plugin_logger-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1634 2023-03-16 05:21:59.499727 usepy_plugin_logger-0.1.4/README.md
+-rw-r--r--   0        0        0      443 2023-04-18 05:54:08.855988 usepy_plugin_logger-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      266 2023-03-16 05:22:21.156519 usepy_plugin_logger-0.1.4/src/usepy_logger/__init__.py
+-rw-r--r--   0        0        0     2042 2023-02-28 14:41:08.787739 usepy_plugin_logger-0.1.4/src/usepy_logger/formatters.py
+-rw-r--r--   0        0        0     1176 2023-03-18 11:44:20.698249 usepy_plugin_logger-0.1.4/src/usepy_logger/handlers.py
+-rw-r--r--   0        0        0     2791 2023-03-10 14:10:02.480477 usepy_plugin_logger-0.1.4/src/usepy_logger/intercept.py
+-rw-r--r--   0        0        0     2087 2023-04-18 05:53:23.372461 usepy_plugin_logger-0.1.4/src/usepy_logger/logger.py
+-rw-r--r--   0        0        0     2406 1970-01-01 00:00:00.000000 usepy_plugin_logger-0.1.4/setup.py
+-rw-r--r--   0        0        0     2168 1970-01-01 00:00:00.000000 usepy_plugin_logger-0.1.4/PKG-INFO
```

### Comparing `usepy_plugin_logger-0.1.3/README.md` & `usepy_plugin_logger-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `usepy_plugin_logger-0.1.3/src/usepy_logger/formatters.py` & `usepy_plugin_logger-0.1.4/src/usepy_logger/formatters.py`

 * *Files identical despite different names*

### Comparing `usepy_plugin_logger-0.1.3/src/usepy_logger/handlers.py` & `usepy_plugin_logger-0.1.4/src/usepy_logger/handlers.py`

 * *Files identical despite different names*

### Comparing `usepy_plugin_logger-0.1.3/src/usepy_logger/intercept.py` & `usepy_plugin_logger-0.1.4/src/usepy_logger/intercept.py`

 * *Files identical despite different names*

### Comparing `usepy_plugin_logger-0.1.3/PKG-INFO` & `usepy_plugin_logger-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: usepy-plugin-logger
-Version: 0.1.3
+Version: 0.1.4
 Summary: 一个全局拦截日志并转为loguru日志的插件
 Author: nowanti
 Author-email: believel.y@qq.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: usepy-plugin-logger Version: 0.1.3 Summary:
+Metadata-Version: 2.1 Name: usepy-plugin-logger Version: 0.1.4 Summary:
 ä¸ä¸ªå¨å±æ¦æªæ¥å¿å¹¶è½¬ä¸ºloguruæ¥å¿çæä»¶ Author: nowanti Author-
 email: believel.y@qq.com Requires-Python: >=3.8,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: loguru (>=0.6.0,<0.7.0) Description-Content-Type: text/markdown
 ### ä¸ä¸ªå¨å±æ¦æªæ¥å¿å¹¶è½¬ä¸ºloguruæ¥å¿çæä»¶ [Package_version]
```

