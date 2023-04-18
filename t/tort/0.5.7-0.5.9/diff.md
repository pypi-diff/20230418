# Comparing `tmp/tort-0.5.7.tar.gz` & `tmp/tort-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tort-0.5.7.tar", last modified: Wed Mar 20 07:47:03 2019, max compression
+gzip compressed data, was "tort-0.5.9.tar", last modified: Tue Apr 18 09:47:35 2023, max compression
```

## Comparing `tort-0.5.7.tar` & `tort-0.5.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 belk       (501) staff       (20)        0 2019-03-20 07:47:03.000000 tort-0.5.7/
--rw-r--r--   0 belk       (501) staff       (20)     1457 2019-03-20 07:47:03.000000 tort-0.5.7/PKG-INFO
-drwxr-xr-x   0 belk       (501) staff       (20)        0 2019-03-20 07:47:03.000000 tort-0.5.7/tort.egg-info/
--rw-r--r--   0 belk       (501) staff       (20)     1457 2019-03-20 07:47:03.000000 tort-0.5.7/tort.egg-info/PKG-INFO
--rw-r--r--   0 belk       (501) staff       (20)      405 2019-03-20 07:47:03.000000 tort-0.5.7/tort.egg-info/SOURCES.txt
--rw-r--r--   0 belk       (501) staff       (20)       17 2019-03-20 07:47:03.000000 tort-0.5.7/tort.egg-info/requires.txt
--rw-r--r--   0 belk       (501) staff       (20)        5 2019-03-20 07:47:03.000000 tort-0.5.7/tort.egg-info/top_level.txt
--rw-r--r--   0 belk       (501) staff       (20)        1 2019-03-20 07:47:03.000000 tort-0.5.7/tort.egg-info/dependency_links.txt
--rw-r--r--   0 belk       (501) staff       (20)      895 2019-03-20 07:32:06.000000 tort-0.5.7/setup.py
--rw-r--r--   0 belk       (501) staff       (20)      124 2019-03-20 07:47:03.000000 tort-0.5.7/setup.cfg
-drwxr-xr-x   0 belk       (501) staff       (20)        0 2019-03-20 07:47:03.000000 tort-0.5.7/tort/
--rw-r--r--   0 belk       (501) staff       (20)       18 2019-03-20 07:32:30.000000 tort-0.5.7/tort/version.py
--rw-r--r--   0 belk       (501) staff       (20)     6791 2019-02-15 16:04:39.000000 tort-0.5.7/tort/handler.py
-drwxr-xr-x   0 belk       (501) staff       (20)        0 2019-03-20 07:47:03.000000 tort-0.5.7/tort/test/
--rw-r--r--   0 belk       (501) staff       (20)        0 2019-01-18 16:52:11.000000 tort-0.5.7/tort/test/__init__.py
--rw-r--r--   0 belk       (501) staff       (20)     1100 2019-01-29 10:04:49.000000 tort-0.5.7/tort/test/import_test.py
--rw-r--r--   0 belk       (501) staff       (20)     3729 2019-01-29 10:05:45.000000 tort-0.5.7/tort/test/runtests.py
-drwxr-xr-x   0 belk       (501) staff       (20)        0 2019-03-20 07:47:03.000000 tort-0.5.7/tort/util/
--rw-r--r--   0 belk       (501) staff       (20)     2088 2019-02-15 16:00:38.000000 tort-0.5.7/tort/util/request.py
--rw-r--r--   0 belk       (501) staff       (20)        0 2019-01-18 05:32:32.000000 tort-0.5.7/tort/util/__init__.py
--rw-r--r--   0 belk       (501) staff       (20)      775 2019-01-29 10:04:49.000000 tort-0.5.7/tort/util/xml_etree.py
--rw-r--r--   0 belk       (501) staff       (20)      812 2019-01-18 05:35:42.000000 tort-0.5.7/tort/util/parse.py
--rw-r--r--   0 belk       (501) staff       (20)       53 2019-01-17 16:36:43.000000 tort-0.5.7/tort/__init__.py
--rw-r--r--   0 belk       (501) staff       (20)     3409 2019-02-15 16:56:20.000000 tort-0.5.7/tort/logger.py
--rw-r--r--   0 belk       (501) staff       (20)      167 2019-01-18 16:59:47.000000 tort-0.5.7/tort/request_id.py
--rw-r--r--   0 belk       (501) staff       (20)      754 2019-01-29 10:09:33.000000 tort-0.5.7/README.rst
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2023-04-18 09:47:35.496368 tort-0.5.9/
+-rw-r--r--   0 glibin     (503) staff       (20)     1148 2023-04-18 09:47:35.496648 tort-0.5.9/PKG-INFO
+-rw-r--r--   0 glibin     (503) staff       (20)      739 2023-04-18 09:47:20.000000 tort-0.5.9/README.md
+-rw-r--r--   0 glibin     (503) staff       (20)       80 2023-04-18 09:47:35.497988 tort-0.5.9/setup.cfg
+-rw-r--r--   0 glibin     (503) staff       (20)      897 2023-04-18 09:46:54.000000 tort-0.5.9/setup.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2023-04-18 09:47:35.481022 tort-0.5.9/tort/
+-rw-r--r--   0 glibin     (503) staff       (20)       53 2023-04-18 09:38:43.000000 tort-0.5.9/tort/__init__.py
+-rw-r--r--   0 glibin     (503) staff       (20)     6791 2023-04-18 09:38:43.000000 tort-0.5.9/tort/handler.py
+-rw-r--r--   0 glibin     (503) staff       (20)     3409 2023-04-18 09:38:43.000000 tort-0.5.9/tort/logger.py
+-rw-r--r--   0 glibin     (503) staff       (20)      167 2023-04-18 09:38:43.000000 tort-0.5.9/tort/request_id.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2023-04-18 09:47:35.485228 tort-0.5.9/tort/test/
+-rw-r--r--   0 glibin     (503) staff       (20)        0 2023-04-18 09:38:43.000000 tort-0.5.9/tort/test/__init__.py
+-rw-r--r--   0 glibin     (503) staff       (20)     1100 2023-04-18 09:38:43.000000 tort-0.5.9/tort/test/import_test.py
+-rw-r--r--   0 glibin     (503) staff       (20)     3729 2023-04-18 09:38:43.000000 tort-0.5.9/tort/test/runtests.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2023-04-18 09:47:35.495441 tort-0.5.9/tort/util/
+-rw-r--r--   0 glibin     (503) staff       (20)        0 2023-04-18 09:38:43.000000 tort-0.5.9/tort/util/__init__.py
+-rw-r--r--   0 glibin     (503) staff       (20)      812 2023-04-18 09:38:43.000000 tort-0.5.9/tort/util/parse.py
+-rw-r--r--   0 glibin     (503) staff       (20)     2088 2023-04-18 09:38:43.000000 tort-0.5.9/tort/util/request.py
+-rw-r--r--   0 glibin     (503) staff       (20)      775 2023-04-18 09:38:43.000000 tort-0.5.9/tort/util/xml_etree.py
+-rw-r--r--   0 glibin     (503) staff       (20)       18 2023-04-18 09:44:05.000000 tort-0.5.9/tort/version.py
+drwxr-xr-x   0 glibin     (503) staff       (20)        0 2023-04-18 09:47:35.483186 tort-0.5.9/tort.egg-info/
+-rw-r--r--   0 glibin     (503) staff       (20)     1148 2023-04-18 09:47:35.000000 tort-0.5.9/tort.egg-info/PKG-INFO
+-rw-r--r--   0 glibin     (503) staff       (20)      404 2023-04-18 09:47:35.000000 tort-0.5.9/tort.egg-info/SOURCES.txt
+-rw-r--r--   0 glibin     (503) staff       (20)        1 2023-04-18 09:47:35.000000 tort-0.5.9/tort.egg-info/dependency_links.txt
+-rw-r--r--   0 glibin     (503) staff       (20)       15 2023-04-18 09:47:35.000000 tort-0.5.9/tort.egg-info/requires.txt
+-rw-r--r--   0 glibin     (503) staff       (20)        5 2023-04-18 09:47:35.000000 tort-0.5.9/tort.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `tort-0.5.7/tort/handler.py` & `tort-0.5.9/tort/handler.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/tort/test/import_test.py` & `tort-0.5.9/tort/test/import_test.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/tort/test/runtests.py` & `tort-0.5.9/tort/test/runtests.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/tort/util/request.py` & `tort-0.5.9/tort/util/request.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/tort/util/xml_etree.py` & `tort-0.5.9/tort/util/xml_etree.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/tort/util/parse.py` & `tort-0.5.9/tort/util/parse.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/tort/logger.py` & `tort-0.5.9/tort/logger.py`

 * *Files identical despite different names*

### Comparing `tort-0.5.7/README.rst` & `tort-0.5.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Use cases
 =========
 
 Add Request Id to all requests
 ------------------------------
 
-.. code-block:: python
+```
     import logging
     import tornado.ioloop
     import tornado.web
     from tort.logger import configure_logging
 
     class MainHandler(tornado.web.RequestHandler):
         def get(self):
@@ -28,7 +28,8 @@
             (r"/", MainHandler),
         ])
 
     if __name__ == "__main__":
         app = make_app()
         app.listen(8888)
         tornado.ioloop.IOLoop.current().start()
+```
```

