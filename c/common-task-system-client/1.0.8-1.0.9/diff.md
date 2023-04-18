# Comparing `tmp/common-task-system-client-1.0.8.tar.gz` & `tmp/common-task-system-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-task-system-client-1.0.8.tar", last modified: Fri Mar 24 07:10:30 2023, max compression
+gzip compressed data, was "common-task-system-client-1.0.9.tar", last modified: Tue Apr 18 05:11:28 2023, max compression
```

## Comparing `common-task-system-client-1.0.8.tar` & `common-task-system-client-1.0.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:30.057035 common-task-system-client-1.0.8/
--rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      302 2023-03-24 07:10:30.056005 common-task-system-client-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:29.966671 common-task-system-client-1.0.8/common_task_system_client.egg-info/
--rw-rw-rw-   0        0        0      302 2023-03-24 07:10:29.000000 common-task-system-client-1.0.8/common_task_system_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-03-24 07:10:29.000000 common-task-system-client-1.0.8/common_task_system_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-24 07:10:29.000000 common-task-system-client-1.0.8/common_task_system_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-03-24 07:10:29.000000 common-task-system-client-1.0.8/common_task_system_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-24 07:10:29.000000 common-task-system-client-1.0.8/common_task_system_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-24 07:10:30.057035 common-task-system-client-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-03-24 07:10:10.000000 common-task-system-client-1.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:29.983670 common-task-system-client-1.0.8/task_system_client/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.0.8/task_system_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:29.987323 common-task-system-client-1.0.8/task_system_client/callback/
--rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.0.8/task_system_client/callback/__init__.py
--rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.0.8/task_system_client/callback/base.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:29.988323 common-task-system-client-1.0.8/task_system_client/callback/callbacks/
--rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.0.8/task_system_client/callback/callbacks/__init__.py
--rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.0.8/task_system_client/callback/callbacks/upload_log.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:29.997324 common-task-system-client-1.0.8/task_system_client/executor/
--rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.0.8/task_system_client/executor/__init__.py
--rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.0.8/task_system_client/executor/base.py
--rw-rw-rw-   0        0        0     1870 2023-03-23 02:02:50.000000 common-task-system-client-1.0.8/task_system_client/executor/executor.py
--rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.0.8/task_system_client/main.py
--rw-rw-rw-   0        0        0     1711 2023-03-17 05:50:08.000000 common-task-system-client-1.0.8/task_system_client/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:30.000810 common-task-system-client-1.0.8/task_system_client/subscriber/
--rw-rw-rw-   0        0        0      514 2023-03-16 03:25:28.000000 common-task-system-client-1.0.8/task_system_client/subscriber/__init__.py
--rw-rw-rw-   0        0        0     2742 2023-03-23 03:55:16.000000 common-task-system-client-1.0.8/task_system_client/subscriber/base.py
--rw-rw-rw-   0        0        0     3578 2023-03-17 09:31:53.000000 common-task-system-client-1.0.8/task_system_client/subscriber/threaded.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:30.002735 common-task-system-client-1.0.8/task_system_client/task_center/
--rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.0.8/task_system_client/task_center/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:30.015024 common-task-system-client-1.0.8/task_system_client/task_center/dispatch/
--rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.0.8/task_system_client/task_center/dispatch/__init__.py
--rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.0.8/task_system_client/task_center/dispatch/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:30.031924 common-task-system-client-1.0.8/task_system_client/task_center/subscription/
--rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.0.8/task_system_client/task_center/subscription/__init__.py
--rw-rw-rw-   0        0        0      934 2023-03-23 02:33:23.000000 common-task-system-client-1.0.8/task_system_client/task_center/subscription/base.py
--rw-rw-rw-   0        0        0     1283 2023-03-23 02:33:48.000000 common-task-system-client-1.0.8/task_system_client/task_center/subscription/http.py
--rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.0.8/task_system_client/task_center/subscription/redis.py
--rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.0.8/task_system_client/task_center/subscription/sql.py
--rw-rw-rw-   0        0        0     2057 2023-03-22 06:01:36.000000 common-task-system-client-1.0.8/task_system_client/task_center/task.py
-drwxrwxrwx   0        0        0        0 2023-03-24 07:10:30.055006 common-task-system-client-1.0.8/task_system_client/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.0.8/task_system_client/utils/__init__.py
--rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.0.8/task_system_client/utils/class_loader.py
--rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.0.8/task_system_client/utils/db_utils.py
--rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.0.8/task_system_client/utils/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.270627 common-task-system-client-1.0.9/
+-rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-18 05:11:28.270627 common-task-system-client-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.143511 common-task-system-client-1.0.9/common_task_system_client.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:11:28.271618 common-task-system-client-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-04-18 05:09:54.000000 common-task-system-client-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.156650 common-task-system-client-1.0.9/task_system_client/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.0.9/task_system_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.170903 common-task-system-client-1.0.9/task_system_client/callback/
+-rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.0.9/task_system_client/callback/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.0.9/task_system_client/callback/base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.176903 common-task-system-client-1.0.9/task_system_client/callback/callbacks/
+-rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.0.9/task_system_client/callback/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.0.9/task_system_client/callback/callbacks/upload_log.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.190114 common-task-system-client-1.0.9/task_system_client/executor/
+-rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.0.9/task_system_client/executor/__init__.py
+-rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.0.9/task_system_client/executor/base.py
+-rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.0.9/task_system_client/executor/executor.py
+-rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.0.9/task_system_client/main.py
+-rw-rw-rw-   0        0        0     1711 2023-03-17 05:50:08.000000 common-task-system-client-1.0.9/task_system_client/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.210615 common-task-system-client-1.0.9/task_system_client/subscriber/
+-rw-rw-rw-   0        0        0      514 2023-03-16 03:25:28.000000 common-task-system-client-1.0.9/task_system_client/subscriber/__init__.py
+-rw-rw-rw-   0        0        0     2742 2023-03-23 03:55:16.000000 common-task-system-client-1.0.9/task_system_client/subscriber/base.py
+-rw-rw-rw-   0        0        0     3578 2023-03-17 09:31:53.000000 common-task-system-client-1.0.9/task_system_client/subscriber/threaded.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.216267 common-task-system-client-1.0.9/task_system_client/task_center/
+-rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.0.9/task_system_client/task_center/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.226101 common-task-system-client-1.0.9/task_system_client/task_center/dispatch/
+-rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.0.9/task_system_client/task_center/dispatch/__init__.py
+-rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.0.9/task_system_client/task_center/dispatch/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.248583 common-task-system-client-1.0.9/task_system_client/task_center/subscription/
+-rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/__init__.py
+-rw-rw-rw-   0        0        0      934 2023-03-23 02:33:23.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/base.py
+-rw-rw-rw-   0        0        0     1283 2023-03-23 02:33:48.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/http.py
+-rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/redis.py
+-rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/sql.py
+-rw-rw-rw-   0        0        0     2107 2023-04-18 05:09:27.000000 common-task-system-client-1.0.9/task_system_client/task_center/task.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.269624 common-task-system-client-1.0.9/task_system_client/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.0.9/task_system_client/utils/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.0.9/task_system_client/utils/class_loader.py
+-rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.0.9/task_system_client/utils/db_utils.py
+-rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.0.9/task_system_client/utils/module_loading.py
```

### Comparing `common-task-system-client-1.0.8/LICENSE` & `common-task-system-client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/common_task_system_client.egg-info/SOURCES.txt` & `common-task-system-client-1.0.9/common_task_system_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/callback/callbacks/upload_log.py` & `common-task-system-client-1.0.9/task_system_client/callback/callbacks/upload_log.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/executor/executor.py` & `common-task-system-client-1.0.9/task_system_client/executor/executor.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,15 @@
         return time.time() - self.create_time > self.ttl
 
     def generate_log(self):
         return {
             "schedule": self.schedule.schedule_id,
             "status": self.execute_status.value,
             "result": self.result,
+            "queue": self.schedule.queue,
             "schedule_time": self.schedule.schedule_time.strftime('%Y-%m-%d %H:%M:%S'),
         }
 
     def run(self):
         raise NotImplementedError
 
     def on_success(self):
```

### Comparing `common-task-system-client-1.0.8/task_system_client/settings.py` & `common-task-system-client-1.0.9/task_system_client/settings.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/subscriber/__init__.py` & `common-task-system-client-1.0.9/task_system_client/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/subscriber/base.py` & `common-task-system-client-1.0.9/task_system_client/subscriber/base.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/subscriber/threaded.py` & `common-task-system-client-1.0.9/task_system_client/subscriber/threaded.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/task_center/dispatch/dispatcher.py` & `common-task-system-client-1.0.9/task_system_client/task_center/dispatch/dispatcher.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/task_center/subscription/base.py` & `common-task-system-client-1.0.9/task_system_client/task_center/subscription/base.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/task_center/subscription/http.py` & `common-task-system-client-1.0.9/task_system_client/task_center/subscription/http.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/task_center/subscription/redis.py` & `common-task-system-client-1.0.9/task_system_client/task_center/subscription/redis.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/task_center/subscription/sql.py` & `common-task-system-client-1.0.9/task_system_client/task_center/subscription/sql.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/task_center/task.py` & `common-task-system-client-1.0.9/task_system_client/task_center/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 class TaskSchedule:
 
     def __init__(self, schedule):
         self.schedule_id = schedule['id']
         self.schedule_time = datetime.strptime(schedule['schedule_time'], '%Y-%m-%d %H:%M:%S')
         self.callback = schedule['callback']
         self.task = Task(schedule['task'])
+        self.queue = schedule.get('queue', None)
         self.config = schedule.get('config') or {}
 
     def __str__(self):
         return 'TaskSchedule(id=%s, time=%s, task=%s)' % (
             self.schedule_id, self.schedule_time, self.task
         )
```

### Comparing `common-task-system-client-1.0.8/task_system_client/utils/db_utils.py` & `common-task-system-client-1.0.9/task_system_client/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.8/task_system_client/utils/module_loading.py` & `common-task-system-client-1.0.9/task_system_client/utils/module_loading.py`

 * *Files identical despite different names*

