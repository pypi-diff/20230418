# Comparing `tmp/cenao-0.8.0.tar.gz` & `tmp/cenao-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cenao-0.8.0.tar", last modified: Thu Apr  6 20:52:23 2023, max compression
+gzip compressed data, was "cenao-0.9.0.tar", last modified: Mon Apr 17 22:55:21 2023, max compression
```

## Comparing `cenao-0.8.0.tar` & `cenao-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:52:23.046271 cenao-0.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1071 2022-04-03 12:51:06.000000 cenao-0.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-06 20:52:23.046271 cenao-0.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       57 2022-04-03 12:51:06.000000 cenao-0.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)       85 2022-04-03 12:51:06.000000 cenao-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-06 20:52:23.046271 cenao-0.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1487 2023-01-31 14:58:38.000000 cenao-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:52:23.046271 cenao-0.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:52:23.046271 cenao-0.8.0/src/cenao/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 20:52:12.000000 cenao-0.8.0/src/cenao/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4520 2023-01-31 14:58:38.000000 cenao-0.8.0/src/cenao/app.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2023-01-23 19:46:22.000000 cenao-0.8.0/src/cenao/config.py
--rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-06 20:52:12.000000 cenao-0.8.0/src/cenao/errors.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2022-04-03 12:51:06.000000 cenao-0.8.0/src/cenao/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:52:23.046271 cenao-0.8.0/src/cenao/features/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 20:52:12.000000 cenao-0.8.0/src/cenao/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      480 2022-04-13 21:27:34.000000 cenao-0.8.0/src/cenao/features/health.py
--rw-rw-rw-   0 root         (0) root         (0)     4264 2022-04-03 12:51:06.000000 cenao-0.8.0/src/cenao/features/redis.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:52:23.046271 cenao-0.8.0/src/cenao/features/redis_storage/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-06 20:52:12.000000 cenao-0.8.0/src/cenao/features/redis_storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      341 2022-04-03 12:51:06.000000 cenao-0.8.0/src/cenao/features/redis_storage/app_feature.py
--rw-rw-rw-   0 root         (0) root         (0)       30 2022-04-03 12:51:06.000000 cenao-0.8.0/src/cenao/features/redis_storage/model.py
--rw-rw-rw-   0 root         (0) root         (0)     4750 2023-04-06 20:52:12.000000 cenao-0.8.0/src/cenao/features/s3.py
--rw-rw-rw-   0 root         (0) root         (0)     2533 2023-01-23 19:46:22.000000 cenao-0.8.0/src/cenao/features/web.py
--rw-rw-rw-   0 root         (0) root         (0)     1996 2023-01-23 19:46:22.000000 cenao-0.8.0/src/cenao/runner.py
--rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-06 20:52:17.000000 cenao-0.8.0/src/cenao/version.py
--rw-rw-rw-   0 root         (0) root         (0)     1953 2023-04-06 20:52:12.000000 cenao-0.8.0/src/cenao/view.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-06 20:52:23.046271 cenao-0.8.0/src/cenao.egg-info/
--rw-r--r--   0 root         (0) root         (0)      723 2023-04-06 20:52:23.000000 cenao-0.8.0/src/cenao.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      641 2023-04-06 20:52:23.000000 cenao-0.8.0/src/cenao.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-06 20:52:23.000000 cenao-0.8.0/src/cenao.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      178 2023-04-06 20:52:23.000000 cenao-0.8.0/src/cenao.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-04-06 20:52:23.000000 cenao-0.8.0/src/cenao.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:55:21.888428 cenao-0.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2022-04-03 12:51:06.000000 cenao-0.9.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-17 22:55:21.888428 cenao-0.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       57 2022-04-03 12:51:06.000000 cenao-0.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       85 2022-04-03 12:51:06.000000 cenao-0.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-17 22:55:21.888428 cenao-0.9.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1487 2023-01-31 14:58:38.000000 cenao-0.9.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:55:21.888428 cenao-0.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:55:21.888428 cenao-0.9.0/src/cenao/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:55:11.000000 cenao-0.9.0/src/cenao/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4653 2023-04-17 22:55:11.000000 cenao-0.9.0/src/cenao/app.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2023-01-23 19:46:22.000000 cenao-0.9.0/src/cenao/config.py
+-rw-rw-rw-   0 root         (0) root         (0)     1278 2023-04-06 20:52:12.000000 cenao-0.9.0/src/cenao/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2022-04-03 12:51:06.000000 cenao-0.9.0/src/cenao/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:55:21.888428 cenao-0.9.0/src/cenao/features/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:55:11.000000 cenao-0.9.0/src/cenao/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      480 2022-04-13 21:27:34.000000 cenao-0.9.0/src/cenao/features/health.py
+-rw-rw-rw-   0 root         (0) root         (0)     4264 2022-04-03 12:51:06.000000 cenao-0.9.0/src/cenao/features/redis.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:55:21.888428 cenao-0.9.0/src/cenao/features/redis_storage/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-17 22:55:11.000000 cenao-0.9.0/src/cenao/features/redis_storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      341 2022-04-03 12:51:06.000000 cenao-0.9.0/src/cenao/features/redis_storage/app_feature.py
+-rw-rw-rw-   0 root         (0) root         (0)       30 2022-04-03 12:51:06.000000 cenao-0.9.0/src/cenao/features/redis_storage/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4750 2023-04-06 20:52:12.000000 cenao-0.9.0/src/cenao/features/s3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3949 2023-04-17 22:55:11.000000 cenao-0.9.0/src/cenao/features/web.py
+-rw-rw-rw-   0 root         (0) root         (0)     1996 2023-01-23 19:46:22.000000 cenao-0.9.0/src/cenao/runner.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-04-17 22:55:16.000000 cenao-0.9.0/src/cenao/version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1953 2023-04-06 20:52:12.000000 cenao-0.9.0/src/cenao/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-17 22:55:21.888428 cenao-0.9.0/src/cenao.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      723 2023-04-17 22:55:21.000000 cenao-0.9.0/src/cenao.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      641 2023-04-17 22:55:21.000000 cenao-0.9.0/src/cenao.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-17 22:55:21.000000 cenao-0.9.0/src/cenao.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      178 2023-04-17 22:55:21.000000 cenao-0.9.0/src/cenao.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-04-17 22:55:21.000000 cenao-0.9.0/src/cenao.egg-info/top_level.txt
```

### Comparing `cenao-0.8.0/LICENSE` & `cenao-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/PKG-INFO` & `cenao-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cenao
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python framework for fast and async applications
 Home-page: https://gitlab.uwtech.org/uwtech/cenao
 Author: Roman Shishkin
 Author-email: spark@uwtech.org
 License: MIT
 Project-URL: Source, https://gitlab.uwtech.org/uwtech/cenao
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cenao-0.8.0/setup.py` & `cenao-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao/app.py` & `cenao-0.9.0/src/cenao/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,42 +118,43 @@
         while True:
             await asyncio.sleep(3600)
 
     def run(self):
         self.logger.info('Application started')
         features: List[AppFeature] = []
         ft: AppFeature
-        for ft in self.ft:
-            self.logger.info('Startup feature %s', ft.name)
-            self._task = self.loop.create_task(ft.on_startup())
-            try:
-                self.loop.run_until_complete(self._task)
-            except asyncio.CancelledError:
-                pass
-            except Exception as e:
-                self.logger.exception('Got exception while feature startup: %r', e, exc_info=e)
-                break
-            features.append(ft)
-
         try:
-            self._task = self.loop.create_task(self.do_sleep())
-            self.loop.run_until_complete(self._task)
-        except asyncio.CancelledError:
-            pass
+            for ft in self.ft:
+                self.logger.info('Startup feature %s', ft.name)
+                self._task = self.loop.create_task(ft.on_startup())
+                try:
+                    self.loop.run_until_complete(self._task)
+                except asyncio.CancelledError:
+                    pass
+                except Exception as e:
+                    self.logger.exception('Got exception while feature startup: %r', e, exc_info=e)
+                    raise
+                features.append(ft)
 
-        for ft in reversed(features):
-            self.logger.info('Shutdown feature %s', ft.name)
-            self._task = self.loop.create_task(ft.on_shutdown())
             try:
+                self._task = self.loop.create_task(self.do_sleep())
                 self.loop.run_until_complete(self._task)
             except asyncio.CancelledError:
                 pass
-            except Exception as e:
-                self.logger.exception('Got exception while feature shutdown: %r', e, exc_info=e)
-                break
+        finally:
+            for ft in reversed(features):
+                self.logger.info('Shutdown feature %s', ft.name)
+                self._task = self.loop.create_task(ft.on_shutdown())
+                try:
+                    self.loop.run_until_complete(self._task)
+                except asyncio.CancelledError:
+                    pass
+                except Exception as e:
+                    self.logger.exception('Got exception while feature shutdown: %r', e, exc_info=e)
+                    break
 
         self.logger.info('Application stopped')
 
     def shutdown(self):
         self.logger.info('Shutdown requested')
         if self._task:
             self._task.cancel()
```

### Comparing `cenao-0.8.0/src/cenao/config.py` & `cenao-0.9.0/src/cenao/config.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao/errors.py` & `cenao-0.9.0/src/cenao/errors.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao/features/redis.py` & `cenao-0.9.0/src/cenao/features/redis.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao/features/s3.py` & `cenao-0.9.0/src/cenao/features/s3.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao/runner.py` & `cenao-0.9.0/src/cenao/runner.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao/view.py` & `cenao-0.9.0/src/cenao/view.py`

 * *Files identical despite different names*

### Comparing `cenao-0.8.0/src/cenao.egg-info/PKG-INFO` & `cenao-0.9.0/src/cenao.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cenao
-Version: 0.8.0
+Version: 0.9.0
 Summary: Python framework for fast and async applications
 Home-page: https://gitlab.uwtech.org/uwtech/cenao
 Author: Roman Shishkin
 Author-email: spark@uwtech.org
 License: MIT
 Project-URL: Source, https://gitlab.uwtech.org/uwtech/cenao
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cenao-0.8.0/src/cenao.egg-info/SOURCES.txt` & `cenao-0.9.0/src/cenao.egg-info/SOURCES.txt`

 * *Files identical despite different names*

