# Comparing `tmp/np_queuey-0.1.2.tar.gz` & `tmp/np_queuey-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.1.2.tar", last modified: Sat Apr 15 22:58:32 2023, max compression
+gzip compressed data, was "np_queuey-0.1.3.tar", last modified: Tue Apr 18 15:31:47 2023, max compression
```

## Comparing `np_queuey-0.1.2.tar` & `np_queuey-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.2/README.md
--rw-r--r--   0        0        0     2365 2023-04-15 22:58:32.469679 np_queuey-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.2/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.2/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     8523 2023-04-15 22:58:13.363400 np_queuey-0.1.2/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.2/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6771 2023-04-15 00:21:38.677120 np_queuey-0.1.2/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.2/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0     3019 2023-04-13 23:41:51.924236 np_queuey-0.1.2/src/np_queuey/queues.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.2/src/np_queuey/tasks.py
--rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.2/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.2/tests/test_huey.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.3/README.md
+-rw-r--r--   0        0        0     2448 2023-04-18 15:31:47.068894 np_queuey-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.3/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.3/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     8730 2023-04-18 15:29:38.975821 np_queuey-0.1.3/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.3/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6771 2023-04-15 00:21:38.677120 np_queuey-0.1.3/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.3/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0     3019 2023-04-13 23:41:51.924236 np_queuey-0.1.3/src/np_queuey/queues.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.3/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.3/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.3/tests/test_huey.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.3/PKG-INFO
```

### Comparing `np_queuey-0.1.2/pyproject.toml` & `np_queuey-0.1.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.1.2"
+version = "0.1.3"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "np-config>=0.4.17",
@@ -79,18 +79,25 @@
     "pdm build",
     "pdm publish --no-build --repository https://test.pypi.org/simple",
 ]
 
 [tool.pdm.scripts.publish]
 composite = [
     "prebuild",
+    "bump",
     "pdm build",
     "pdm publish --no-build",
 ]
 
+[tool.pdm.scripts.pub]
+composite = [
+    "bump",
+    "pdm publish",
+]
+
 [tool.ruff]
 ignore-init-module-imports = true
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
     "--doctest-modules",
```

### Comparing `np_queuey-0.1.2/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.3/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,26 +8,27 @@
 import np_config
 import np_logging
 import np_session
 import np_tools
 
 import np_queuey
 from np_queuey.jobs import dynamicrouting_behavior_session_mtrain_upload as job
+import np_queuey.utils as utils
 
 logger = np_logging.getLogger()
 
-huey = np_queuey.HueyQueue(job.DB_PATH).huey
+huey = np_queuey.HueyQueue(utils.DEFAULT_HUEY_SQLITE_DB_PATH).huey
 
 UPLOAD_JSON_DIR_CONFIG_KEY = (
     'dynamicrouting_behavior_session_mtrain_upload_json_dir'
 )
 """Single leading fwd slash, for unix compatibility on hpc"""
 
 
-@huey.periodic_task(_huey.crontab(minute='*/30', strict=True))
+@huey.periodic_task(_huey.crontab(minute='*/10', strict=True))
 def upload_outstanding_sessions() -> None:
     sessions: list[
         tuple[str, str]
     ] = job.get_outstanding_behavior_sessions_for_processing()
     if not sessions:
         logger.info('No outstanding sessions to upload')
         return
@@ -81,14 +82,18 @@
         'Behavior session %r verified in mtrain', foraging_id_and_filename
     )
 
 
 def is_behavior_session_in_mtrain(
     foraging_id_and_filename: tuple[str, str]
 ) -> bool:
+    """
+    >>> is_behavior_session_in_mtrain(('e4d6666e-3c0d-4726-9dd8-afccd124e872', 'DynamicRouting1_660023_20230417_162846.hdf5'))
+    False
+    """
     _, filename = foraging_id_and_filename
     _, mouse_id, date, time = job.parse_filename(filename)
     mtrain = np_session.Mouse(mouse_id).mtrain
     return foraging_id_and_filename[0].replace('-', '') in [
         _['id'].replace('-', '') for _ in mtrain.all_behavior_sessions
     ]
```

### Comparing `np_queuey-0.1.2/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.3/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.2/src/np_queuey/queues.py` & `np_queuey-0.1.3/src/np_queuey/queues.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.2/tests/test_huey.py` & `np_queuey-0.1.3/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.2/PKG-INFO` & `np_queuey-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.1.2
+Version: 0.1.3
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

