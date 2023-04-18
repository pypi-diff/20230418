# Comparing `tmp/np_queuey-0.1.6.tar.gz` & `tmp/np_queuey-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "np_queuey-0.1.6.tar", last modified: Tue Apr 18 16:51:21 2023, max compression
+gzip compressed data, was "np_queuey-0.1.7.tar", last modified: Tue Apr 18 17:04:57 2023, max compression
```

## Comparing `np_queuey-0.1.6.tar` & `np_queuey-0.1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.6/README.md
--rw-r--r--   0        0        0     2448 2023-04-18 16:51:21.577675 np_queuey-0.1.6/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.6/src/np_queuey/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.6/src/np_queuey/hueys/__init__.py
--rw-r--r--   0        0        0     8732 2023-04-18 16:02:58.142537 np_queuey-0.1.6/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.6/src/np_queuey/jobs/__init__.py
--rw-r--r--   0        0        0     6844 2023-04-18 16:06:53.861920 np_queuey-0.1.6/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
--rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.6/src/np_queuey/jobs/run_small_jobs.py
--rw-r--r--   0        0        0     3136 2023-04-18 16:51:07.922149 np_queuey-0.1.6/src/np_queuey/queues.py
--rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.6/src/np_queuey/tasks.py
--rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.6/src/np_queuey/utils.py
--rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.6/tests/test_huey.py
--rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-04-13 16:35:48.733260 np_queuey-0.1.7/README.md
+-rw-r--r--   0        0        0     2448 2023-04-18 17:04:57.425135 np_queuey-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0       73 2023-04-13 23:41:50.797573 np_queuey-0.1.7/src/np_queuey/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.7/src/np_queuey/hueys/__init__.py
+-rw-r--r--   0        0        0     8732 2023-04-18 16:02:58.142537 np_queuey-0.1.7/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0        0 2023-04-13 22:30:49.775239 np_queuey-0.1.7/src/np_queuey/jobs/__init__.py
+-rw-r--r--   0        0        0     6844 2023-04-18 16:06:53.861920 np_queuey-0.1.7/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py
+-rw-r--r--   0        0        0      262 2023-04-15 22:53:44.311082 np_queuey-0.1.7/src/np_queuey/jobs/run_small_jobs.py
+-rw-r--r--   0        0        0     3177 2023-04-18 17:04:45.613009 np_queuey-0.1.7/src/np_queuey/queues.py
+-rw-r--r--   0        0        0       51 2023-04-13 23:41:50.828823 np_queuey-0.1.7/src/np_queuey/tasks.py
+-rw-r--r--   0        0        0      140 2023-04-15 00:21:38.620120 np_queuey-0.1.7/src/np_queuey/utils.py
+-rw-r--r--   0        0        0      593 2023-04-13 20:34:38.147095 np_queuey-0.1.7/tests/test_huey.py
+-rw-r--r--   0        0        0     1668 1970-01-01 00:00:00.000000 np_queuey-0.1.7/PKG-INFO
```

### Comparing `np_queuey-0.1.6/pyproject.toml` & `np_queuey-0.1.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "np_queuey"
-version = "0.1.6"
+version = "0.1.7"
 description = "Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows."
 authors = [
     { name = "Ben Hardcastle", email = "ben.hardcastle@alleninstitute.org" },
 ]
 dependencies = [
     "huey>=2.4.5",
     "np-config>=0.4.17",
```

### Comparing `np_queuey-0.1.6/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.7/src/np_queuey/hueys/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.6/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py` & `np_queuey-0.1.7/src/np_queuey/jobs/dynamicrouting_behavior_session_mtrain_upload.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.6/src/np_queuey/queues.py` & `np_queuey-0.1.7/src/np_queuey/queues.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,17 +33,17 @@
     """`huey` object for submitting tasks"""
 
     db_path: str
     """Path to the sqlite database for `huey`"""
 
     def __init__(self, sqlite_db_path: Optional[str] = None, **kwargs) -> None:
         self.db_path = sqlite_db_path or utils.DEFAULT_HUEY_SQLITE_DB_PATH
-        kwargs.setdefault('journal_mode', 'truncate')
-        kwargs.setdefault('fsync', True)
-        self.huey = huey.SqliteHuey(filename=self.db_path, **kwargs)
+        # kwargs.setdefault('journal_mode', 'truncate')
+        # kwargs.setdefault('fsync', True)
+        self.huey = huey.SqliteHuey(filename=self.db_path, journal_mode='truncate', fsync=True, **kwargs)
         for task in (
             _ for _ in dir(tasks) if isinstance(getattr(tasks, _), Callable)
         ):
             self.add_task(task)
 
     def add_task(self, task: str) -> None:
         setattr(self, task, self.huey.task()(getattr(tasks, task)))
```

### Comparing `np_queuey-0.1.6/tests/test_huey.py` & `np_queuey-0.1.7/tests/test_huey.py`

 * *Files identical despite different names*

### Comparing `np_queuey-0.1.6/PKG-INFO` & `np_queuey-0.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: np-queuey
-Version: 0.1.6
+Version: 0.1.7
 Summary: Tools for submitting and processing jobs through a message queue for Mindscope Neuropixels workflows.
 Author-Email: Ben Hardcastle <ben.hardcastle@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

