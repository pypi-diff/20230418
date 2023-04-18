# Comparing `tmp/jija-0.1.1.tar.gz` & `tmp/jija-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jija-0.1.1.tar", last modified: Sun Feb 26 06:58:24 2023, max compression
+gzip compressed data, was "jija-0.2.0.tar", last modified: Tue Apr 18 04:00:37 2023, max compression
```

## Comparing `jija-0.1.1.tar` & `jija-0.2.0.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.381451 jija-0.1.1/
--rw-r--r--   0 root         (0) root         (0)      181 2023-02-26 06:58:24.381451 jija-0.1.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.371451 jija-0.1.1/jija/
--rwxr-xr-x   0 root         (0) root         (0)      355 2023-01-23 14:07:37.000000 jija-0.1.1/jija/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     5461 2023-02-26 06:55:56.000000 jija-0.1.1/jija/app.py
--rwxr-xr-x   0 root         (0) root         (0)     4455 2023-01-23 14:10:41.000000 jija-0.1.1/jija/apps.py
--rwxr-xr-x   0 root         (0) root         (0)      460 2023-01-22 17:43:04.000000 jija-0.1.1/jija/collector.py
--rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.1.1/jija/command.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.371451 jija-0.1.1/jija/commands/
--rwxr-xr-x   0 root         (0) root         (0)      325 2022-11-05 14:37:03.000000 jija-0.1.1/jija/commands/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      226 2022-11-05 21:57:40.000000 jija-0.1.1/jija/commands/migrate.py
--rwxr-xr-x   0 root         (0) root         (0)     1195 2023-02-26 03:18:53.000000 jija-0.1.1/jija/commands/run.py
--rwxr-xr-x   0 root         (0) root         (0)      299 2023-02-26 05:34:17.000000 jija-0.1.1/jija/commands/runprocess.py
--rwxr-xr-x   0 root         (0) root         (0)       97 2022-11-05 14:37:03.000000 jija-0.1.1/jija/commands/test.py
--rwxr-xr-x   0 root         (0) root         (0)      223 2022-11-05 21:57:40.000000 jija-0.1.1/jija/commands/update.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.371451 jija-0.1.1/jija/config/
--rwxr-xr-x   0 root         (0) root         (0)      175 2023-01-23 14:16:07.000000 jija-0.1.1/jija/config/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.1.1/jija/config/base.py
--rwxr-xr-x   0 root         (0) root         (0)      597 2022-11-18 11:42:58.000000 jija-0.1.1/jija/config/database.py
--rwxr-xr-x   0 root         (0) root         (0)      382 2023-02-26 03:28:48.000000 jija-0.1.1/jija/config/docs.py
--rwxr-xr-x   0 root         (0) root         (0)      463 2022-11-18 11:42:58.000000 jija-0.1.1/jija/config/drivers.py
--rwxr-xr-x   0 root         (0) root         (0)      575 2023-01-22 17:43:04.000000 jija-0.1.1/jija/config/fields.py
--rwxr-xr-x   0 root         (0) root         (0)      262 2022-11-18 11:42:58.000000 jija-0.1.1/jija/config/network.py
--rwxr-xr-x   0 root         (0) root         (0)     1207 2022-11-18 11:42:58.000000 jija-0.1.1/jija/config/structute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.371451 jija-0.1.1/jija/contrib/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.371451 jija-0.1.1/jija/contrib/auth/
--rwxr-xr-x   0 root         (0) root         (0)      460 2022-11-19 22:00:09.000000 jija-0.1.1/jija/contrib/auth/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.381451 jija-0.1.1/jija/docs/
--rwxr-xr-x   0 root         (0) root         (0)       29 2023-01-22 17:43:04.000000 jija-0.1.1/jija/docs/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)     4563 2023-02-26 05:35:18.000000 jija-0.1.1/jija/docs/processor.py
--rwxr-xr-x   0 root         (0) root         (0)     1361 2023-02-26 03:58:21.000000 jija-0.1.1/jija/docs/setup.py
--rwxr-xr-x   0 root         (0) root         (0)      240 2023-01-22 17:43:04.000000 jija-0.1.1/jija/docs/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.381451 jija-0.1.1/jija/drivers/
--rwxr-xr-x   0 root         (0) root         (0)      105 2022-11-18 11:42:58.000000 jija-0.1.1/jija/drivers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)       22 2022-11-18 11:42:58.000000 jija-0.1.1/jija/drivers/base.py
--rwxr-xr-x   0 root         (0) root         (0)     1446 2022-11-19 22:00:09.000000 jija-0.1.1/jija/drivers/database.py
--rwxr-xr-x   0 root         (0) root         (0)       72 2022-11-18 11:42:58.000000 jija-0.1.1/jija/drivers/docs.py
--rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.1.1/jija/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.1.1/jija/middleware.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.381451 jija-0.1.1/jija/middlewares/
--rwxr-xr-x   0 root         (0) root         (0)       28 2022-11-05 14:37:03.000000 jija-0.1.1/jija/middlewares/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      966 2022-11-05 14:37:03.000000 jija-0.1.1/jija/middlewares/print_request.py
--rwxr-xr-x   0 root         (0) root         (0)     1664 2023-01-22 17:43:04.000000 jija-0.1.1/jija/reloader.py
--rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.1.1/jija/response.py
--rwxr-xr-x   0 root         (0) root         (0)     2067 2023-01-22 17:43:04.000000 jija-0.1.1/jija/router.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.381451 jija-0.1.1/jija/serializers/
--rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.1.1/jija/serializers/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.1.1/jija/serializers/exceptions.py
--rwxr-xr-x   0 root         (0) root         (0)     2902 2023-01-22 17:55:13.000000 jija-0.1.1/jija/serializers/fields.py
--rwxr-xr-x   0 root         (0) root         (0)     1331 2023-01-22 17:43:04.000000 jija-0.1.1/jija/serializers/serializer.py
--rwxr-xr-x   0 root         (0) root         (0)     2640 2023-01-22 17:43:04.000000 jija-0.1.1/jija/serializers/validators.py
--rwxr-xr-x   0 root         (0) root         (0)     3832 2023-01-22 17:43:04.000000 jija-0.1.1/jija/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-26 06:58:24.371451 jija-0.1.1/jija.egg-info/
--rw-r--r--   0 root         (0) root         (0)      181 2023-02-26 06:58:24.000000 jija-0.1.1/jija.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1093 2023-02-26 06:58:24.000000 jija-0.1.1/jija.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-26 06:58:24.000000 jija-0.1.1/jija.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-26 06:58:24.000000 jija-0.1.1/jija.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       83 2023-02-26 06:58:24.000000 jija-0.1.1/jija.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-26 06:58:24.000000 jija-0.1.1/jija.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-26 06:58:24.381451 jija-0.1.1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)      564 2023-02-26 06:58:04.000000 jija-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-18 04:00:37.714460 jija-0.2.0/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.704460 jija-0.2.0/jija/
+-rwxr-xr-x   0 root         (0) root         (0)      355 2023-01-23 14:07:37.000000 jija-0.2.0/jija/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     5461 2023-02-26 06:55:56.000000 jija-0.2.0/jija/app.py
+-rwxr-xr-x   0 root         (0) root         (0)     4455 2023-01-23 14:10:41.000000 jija-0.2.0/jija/apps.py
+-rwxr-xr-x   0 root         (0) root         (0)      460 2023-01-22 17:43:04.000000 jija-0.2.0/jija/collector.py
+-rwxr-xr-x   0 root         (0) root         (0)      456 2022-11-19 22:00:09.000000 jija-0.2.0/jija/command.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/commands/
+-rwxr-xr-x   0 root         (0) root         (0)      325 2022-11-05 14:37:03.000000 jija-0.2.0/jija/commands/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      226 2022-11-05 21:57:40.000000 jija-0.2.0/jija/commands/migrate.py
+-rwxr-xr-x   0 root         (0) root         (0)     1195 2023-02-26 03:18:53.000000 jija-0.2.0/jija/commands/run.py
+-rwxr-xr-x   0 root         (0) root         (0)      299 2023-02-26 05:34:17.000000 jija-0.2.0/jija/commands/runprocess.py
+-rwxr-xr-x   0 root         (0) root         (0)       97 2022-11-05 14:37:03.000000 jija-0.2.0/jija/commands/test.py
+-rwxr-xr-x   0 root         (0) root         (0)      223 2022-11-05 21:57:40.000000 jija-0.2.0/jija/commands/update.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/config/
+-rwxr-xr-x   0 root         (0) root         (0)      175 2023-01-23 14:16:07.000000 jija-0.2.0/jija/config/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     1162 2023-01-23 14:19:45.000000 jija-0.2.0/jija/config/base.py
+-rwxr-xr-x   0 root         (0) root         (0)      597 2022-11-18 11:42:58.000000 jija-0.2.0/jija/config/database.py
+-rwxr-xr-x   0 root         (0) root         (0)      382 2023-02-26 03:28:48.000000 jija-0.2.0/jija/config/docs.py
+-rwxr-xr-x   0 root         (0) root         (0)      463 2022-11-18 11:42:58.000000 jija-0.2.0/jija/config/drivers.py
+-rwxr-xr-x   0 root         (0) root         (0)      575 2023-01-22 17:43:04.000000 jija-0.2.0/jija/config/fields.py
+-rwxr-xr-x   0 root         (0) root         (0)      262 2022-11-18 11:42:58.000000 jija-0.2.0/jija/config/network.py
+-rwxr-xr-x   0 root         (0) root         (0)     1207 2022-11-18 11:42:58.000000 jija-0.2.0/jija/config/structute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.704460 jija-0.2.0/jija/contrib/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/contrib/auth/
+-rwxr-xr-x   0 root         (0) root         (0)      460 2022-11-19 22:00:09.000000 jija-0.2.0/jija/contrib/auth/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/docs/
+-rwxr-xr-x   0 root         (0) root         (0)       29 2023-01-22 17:43:04.000000 jija-0.2.0/jija/docs/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)     4563 2023-02-26 05:35:18.000000 jija-0.2.0/jija/docs/processor.py
+-rwxr-xr-x   0 root         (0) root         (0)     1361 2023-02-26 03:58:21.000000 jija-0.2.0/jija/docs/setup.py
+-rwxr-xr-x   0 root         (0) root         (0)      240 2023-01-22 17:43:04.000000 jija-0.2.0/jija/docs/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/drivers/
+-rwxr-xr-x   0 root         (0) root         (0)      105 2022-11-18 11:42:58.000000 jija-0.2.0/jija/drivers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)       22 2022-11-18 11:42:58.000000 jija-0.2.0/jija/drivers/base.py
+-rwxr-xr-x   0 root         (0) root         (0)     1446 2022-11-19 22:00:09.000000 jija-0.2.0/jija/drivers/database.py
+-rwxr-xr-x   0 root         (0) root         (0)       72 2022-11-18 11:42:58.000000 jija-0.2.0/jija/drivers/docs.py
+-rwxr-xr-x   0 root         (0) root         (0)      171 2023-01-22 17:43:04.000000 jija-0.2.0/jija/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)      270 2023-01-22 17:43:04.000000 jija-0.2.0/jija/middleware.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/middlewares/
+-rwxr-xr-x   0 root         (0) root         (0)       28 2022-11-05 14:37:03.000000 jija-0.2.0/jija/middlewares/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      966 2022-11-05 14:37:03.000000 jija-0.2.0/jija/middlewares/print_request.py
+-rwxr-xr-x   0 root         (0) root         (0)     1664 2023-01-22 17:43:04.000000 jija-0.2.0/jija/reloader.py
+-rwxr-xr-x   0 root         (0) root         (0)     1370 2023-01-22 17:43:04.000000 jija-0.2.0/jija/response.py
+-rwxr-xr-x   0 root         (0) root         (0)     2079 2023-04-18 00:55:04.000000 jija-0.2.0/jija/router.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.714460 jija-0.2.0/jija/serializers/
+-rwxr-xr-x   0 root         (0) root         (0)      138 2023-01-22 17:43:04.000000 jija-0.2.0/jija/serializers/__init__.py
+-rwxr-xr-x   0 root         (0) root         (0)      310 2023-01-22 17:43:04.000000 jija-0.2.0/jija/serializers/exceptions.py
+-rwxr-xr-x   0 root         (0) root         (0)     2902 2023-01-22 17:55:13.000000 jija-0.2.0/jija/serializers/fields.py
+-rwxr-xr-x   0 root         (0) root         (0)     1331 2023-01-22 17:43:04.000000 jija-0.2.0/jija/serializers/serializer.py
+-rwxr-xr-x   0 root         (0) root         (0)     2640 2023-01-22 17:43:04.000000 jija-0.2.0/jija/serializers/validators.py
+-rwxr-xr-x   0 root         (0) root         (0)     5937 2023-04-18 03:59:37.000000 jija-0.2.0/jija/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 04:00:37.704460 jija-0.2.0/jija.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      181 2023-04-18 04:00:37.000000 jija-0.2.0/jija.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-04-18 04:00:37.000000 jija-0.2.0/jija.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 04:00:37.000000 jija-0.2.0/jija.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 04:00:37.000000 jija-0.2.0/jija.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       83 2023-04-18 04:00:37.000000 jija-0.2.0/jija.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-04-18 04:00:37.000000 jija-0.2.0/jija.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 04:00:37.714460 jija-0.2.0/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)      564 2023-04-18 04:00:20.000000 jija-0.2.0/setup.py
```

### Comparing `jija-0.1.1/jija/app.py` & `jija-0.2.0/jija/app.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/apps.py` & `jija-0.2.0/jija/apps.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/commands/run.py` & `jija-0.2.0/jija/commands/run.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/config/base.py` & `jija-0.2.0/jija/config/base.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/config/database.py` & `jija-0.2.0/jija/config/database.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/config/fields.py` & `jija-0.2.0/jija/config/fields.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/config/structute.py` & `jija-0.2.0/jija/config/structute.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/docs/processor.py` & `jija-0.2.0/jija/docs/processor.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/docs/setup.py` & `jija-0.2.0/jija/docs/setup.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/drivers/database.py` & `jija-0.2.0/jija/drivers/database.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/middlewares/print_request.py` & `jija-0.2.0/jija/middlewares/print_request.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/reloader.py` & `jija-0.2.0/jija/reloader.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/response.py` & `jija-0.2.0/jija/response.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/router.py` & `jija-0.2.0/jija/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,17 @@
 
 class AbsEndpoint:
     def generate_routes(self, prefix=''):
         raise NotImplementedError()
 
 
 class Endpoint(AbsEndpoint):
-    def __init__(self, path, view: typing.Type[views.View]):
-        if not issubclass(view, views.View):
-            raise AttributeError(f'view must be a subclass of "jija.views.View", got {view}')
+    def __init__(self, path, view: typing.Type[views.ViewBase]):
+        if not issubclass(view, views.ViewBase):
+            raise AttributeError(f'view must be a subclass of "jija.views.ViewBase", got {view}')
 
         self.__path = path
         self.__view = view
 
     @property
     def path(self) -> str:
         return self.__path
```

### Comparing `jija-0.1.1/jija/serializers/fields.py` & `jija-0.2.0/jija/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/serializers/serializer.py` & `jija-0.2.0/jija/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija/serializers/validators.py` & `jija-0.2.0/jija/serializers/validators.py`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/jija.egg-info/SOURCES.txt` & `jija-0.2.0/jija.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jija-0.1.1/setup.py` & `jija-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='jija',
-    version='0.1.1',
+    version='0.2.0',
     description='',
     packages=[
         'jija',
         'jija.docs',
         'jija.serializers',
         'jija.commands',
         'jija.middlewares',
```

