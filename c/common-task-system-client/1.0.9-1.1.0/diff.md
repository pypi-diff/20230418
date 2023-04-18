# Comparing `tmp/common-task-system-client-1.0.9.tar.gz` & `tmp/common-task-system-client-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "common-task-system-client-1.0.9.tar", last modified: Tue Apr 18 05:11:28 2023, max compression
+gzip compressed data, was "common-task-system-client-1.1.0.tar", last modified: Tue Apr 18 05:45:45 2023, max compression
```

## Comparing `common-task-system-client-1.0.9.tar` & `common-task-system-client-1.1.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.270627 common-task-system-client-1.0.9/
--rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.0.9/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-18 05:11:28.270627 common-task-system-client-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.143511 common-task-system-client-1.0.9/common_task_system_client.egg-info/
--rw-rw-rw-   0        0        0      302 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-18 05:11:28.000000 common-task-system-client-1.0.9/common_task_system_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 05:11:28.271618 common-task-system-client-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      424 2023-04-18 05:09:54.000000 common-task-system-client-1.0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.156650 common-task-system-client-1.0.9/task_system_client/
--rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.0.9/task_system_client/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.170903 common-task-system-client-1.0.9/task_system_client/callback/
--rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.0.9/task_system_client/callback/__init__.py
--rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.0.9/task_system_client/callback/base.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.176903 common-task-system-client-1.0.9/task_system_client/callback/callbacks/
--rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.0.9/task_system_client/callback/callbacks/__init__.py
--rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.0.9/task_system_client/callback/callbacks/upload_log.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.190114 common-task-system-client-1.0.9/task_system_client/executor/
--rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.0.9/task_system_client/executor/__init__.py
--rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.0.9/task_system_client/executor/base.py
--rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.0.9/task_system_client/executor/executor.py
--rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.0.9/task_system_client/main.py
--rw-rw-rw-   0        0        0     1711 2023-03-17 05:50:08.000000 common-task-system-client-1.0.9/task_system_client/settings.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.210615 common-task-system-client-1.0.9/task_system_client/subscriber/
--rw-rw-rw-   0        0        0      514 2023-03-16 03:25:28.000000 common-task-system-client-1.0.9/task_system_client/subscriber/__init__.py
--rw-rw-rw-   0        0        0     2742 2023-03-23 03:55:16.000000 common-task-system-client-1.0.9/task_system_client/subscriber/base.py
--rw-rw-rw-   0        0        0     3578 2023-03-17 09:31:53.000000 common-task-system-client-1.0.9/task_system_client/subscriber/threaded.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.216267 common-task-system-client-1.0.9/task_system_client/task_center/
--rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.0.9/task_system_client/task_center/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.226101 common-task-system-client-1.0.9/task_system_client/task_center/dispatch/
--rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.0.9/task_system_client/task_center/dispatch/__init__.py
--rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.0.9/task_system_client/task_center/dispatch/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.248583 common-task-system-client-1.0.9/task_system_client/task_center/subscription/
--rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/__init__.py
--rw-rw-rw-   0        0        0      934 2023-03-23 02:33:23.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/base.py
--rw-rw-rw-   0        0        0     1283 2023-03-23 02:33:48.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/http.py
--rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/redis.py
--rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.0.9/task_system_client/task_center/subscription/sql.py
--rw-rw-rw-   0        0        0     2107 2023-04-18 05:09:27.000000 common-task-system-client-1.0.9/task_system_client/task_center/task.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:11:28.269624 common-task-system-client-1.0.9/task_system_client/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.0.9/task_system_client/utils/__init__.py
--rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.0.9/task_system_client/utils/class_loader.py
--rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.0.9/task_system_client/utils/db_utils.py
--rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.0.9/task_system_client/utils/module_loading.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.296633 common-task-system-client-1.1.0/
+-rw-rw-rw-   0        0        0     1085 2023-02-20 07:10:46.000000 common-task-system-client-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-18 05:45:45.296633 common-task-system-client-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       24 2023-02-20 07:10:46.000000 common-task-system-client-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.280985 common-task-system-client-1.1.0/common_task_system_client.egg-info/
+-rw-rw-rw-   0        0        0      302 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 05:45:45.000000 common-task-system-client-1.1.0/common_task_system_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-18 05:45:45.296633 common-task-system-client-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      424 2023-04-18 05:45:30.000000 common-task-system-client-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.282990 common-task-system-client-1.1.0/task_system_client/
+-rw-rw-rw-   0        0        0        0 2023-02-20 07:12:05.000000 common-task-system-client-1.1.0/task_system_client/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.285413 common-task-system-client-1.1.0/task_system_client/callback/
+-rw-rw-rw-   0        0        0       42 2023-03-17 05:21:49.000000 common-task-system-client-1.1.0/task_system_client/callback/__init__.py
+-rw-rw-rw-   0        0        0      490 2023-03-17 06:56:57.000000 common-task-system-client-1.1.0/task_system_client/callback/base.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.286670 common-task-system-client-1.1.0/task_system_client/callback/callbacks/
+-rw-rw-rw-   0        0        0        0 2023-03-17 03:52:57.000000 common-task-system-client-1.1.0/task_system_client/callback/callbacks/__init__.py
+-rw-rw-rw-   0        0        0      701 2023-03-23 01:18:51.000000 common-task-system-client-1.1.0/task_system_client/callback/callbacks/upload_log.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.287676 common-task-system-client-1.1.0/task_system_client/executor/
+-rw-rw-rw-   0        0        0      193 2023-03-14 03:27:53.000000 common-task-system-client-1.1.0/task_system_client/executor/__init__.py
+-rw-rw-rw-   0        0        0      390 2023-03-24 06:53:45.000000 common-task-system-client-1.1.0/task_system_client/executor/base.py
+-rw-rw-rw-   0        0        0     1913 2023-04-18 05:09:27.000000 common-task-system-client-1.1.0/task_system_client/executor/executor.py
+-rw-rw-rw-   0        0        0      382 2023-03-16 03:20:59.000000 common-task-system-client-1.1.0/task_system_client/main.py
+-rw-rw-rw-   0        0        0     1711 2023-03-17 05:50:08.000000 common-task-system-client-1.1.0/task_system_client/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.289689 common-task-system-client-1.1.0/task_system_client/subscriber/
+-rw-rw-rw-   0        0        0      514 2023-03-16 03:25:28.000000 common-task-system-client-1.1.0/task_system_client/subscriber/__init__.py
+-rw-rw-rw-   0        0        0     2777 2023-04-18 05:44:26.000000 common-task-system-client-1.1.0/task_system_client/subscriber/base.py
+-rw-rw-rw-   0        0        0     3578 2023-03-17 09:31:53.000000 common-task-system-client-1.1.0/task_system_client/subscriber/threaded.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.290688 common-task-system-client-1.1.0/task_system_client/task_center/
+-rw-rw-rw-   0        0        0      130 2023-02-22 05:09:58.000000 common-task-system-client-1.1.0/task_system_client/task_center/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.291685 common-task-system-client-1.1.0/task_system_client/task_center/dispatch/
+-rw-rw-rw-   0        0        0      286 2023-02-27 02:22:48.000000 common-task-system-client-1.1.0/task_system_client/task_center/dispatch/__init__.py
+-rw-rw-rw-   0        0        0      857 2023-03-17 09:28:16.000000 common-task-system-client-1.1.0/task_system_client/task_center/dispatch/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.293683 common-task-system-client-1.1.0/task_system_client/task_center/subscription/
+-rw-rw-rw-   0        0        0      487 2023-02-27 02:22:30.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/__init__.py
+-rw-rw-rw-   0        0        0      934 2023-03-23 02:33:23.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/base.py
+-rw-rw-rw-   0        0        0     1382 2023-04-18 05:41:46.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/http.py
+-rw-rw-rw-   0        0        0      547 2023-02-27 03:21:04.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/redis.py
+-rw-rw-rw-   0        0        0      655 2023-02-27 03:14:11.000000 common-task-system-client-1.1.0/task_system_client/task_center/subscription/sql.py
+-rw-rw-rw-   0        0        0     2107 2023-04-18 05:09:27.000000 common-task-system-client-1.1.0/task_system_client/task_center/task.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:45:45.295620 common-task-system-client-1.1.0/task_system_client/utils/
+-rw-rw-rw-   0        0        0        0 2023-02-20 09:58:14.000000 common-task-system-client-1.1.0/task_system_client/utils/__init__.py
+-rw-rw-rw-   0        0        0      428 2023-02-22 03:46:05.000000 common-task-system-client-1.1.0/task_system_client/utils/class_loader.py
+-rw-rw-rw-   0        0        0     2627 2023-02-27 01:52:51.000000 common-task-system-client-1.1.0/task_system_client/utils/db_utils.py
+-rw-rw-rw-   0        0        0     1068 2023-03-14 03:24:44.000000 common-task-system-client-1.1.0/task_system_client/utils/module_loading.py
```

### Comparing `common-task-system-client-1.0.9/LICENSE` & `common-task-system-client-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/common_task_system_client.egg-info/SOURCES.txt` & `common-task-system-client-1.1.0/common_task_system_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/callback/callbacks/upload_log.py` & `common-task-system-client-1.1.0/task_system_client/callback/callbacks/upload_log.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/executor/executor.py` & `common-task-system-client-1.1.0/task_system_client/executor/executor.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/settings.py` & `common-task-system-client-1.1.0/task_system_client/settings.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/subscriber/__init__.py` & `common-task-system-client-1.1.0/task_system_client/subscriber/__init__.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/subscriber/base.py` & `common-task-system-client-1.1.0/task_system_client/subscriber/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             time.sleep(0.1)
             try:
                 if not self.is_schedulable():
                     time.sleep(1)
                     continue
                 schedule = get_schedule(block)
                 if not schedule:
+                    time.sleep(1)
                     continue
                 executor = dispatch(schedule)
                 if not self.is_executable(executor):
                     continue
                 try:
                     self.run_executor(executor)
                 except Exception as e:
```

### Comparing `common-task-system-client-1.0.9/task_system_client/subscriber/threaded.py` & `common-task-system-client-1.1.0/task_system_client/subscriber/threaded.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/task_center/dispatch/dispatcher.py` & `common-task-system-client-1.1.0/task_system_client/task_center/dispatch/dispatcher.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/task_center/subscription/base.py` & `common-task-system-client-1.1.0/task_system_client/task_center/subscription/base.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/task_center/subscription/http.py` & `common-task-system-client-1.1.0/task_system_client/task_center/subscription/http.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,16 +23,17 @@
             response = requests.get(self.subscription_url)
             if response.status_code == 200:
                 return TaskSchedule(response.json())
             elif response.status_code == 204:
                 stdout.write('[%s]no more schedule now, wait 1 second...\r' % time.strftime('%Y-%m-%d %H:%M:%S'))
                 stdout.flush()
             else:
+                # 有可能存在500情况是被nginx代理的，所以输出response.text不会错
                 stdout.write('[%s]get schedule error, status code: %s\n' % (
-                    time.strftime('%Y-%m-%d %H:%M:%S'), response.json()))
+                    time.strftime('%Y-%m-%d %H:%M:%S'), response.text))
                 stdout.flush()
         except Exception as e:
             logger.exception(e)
         if block:
             time.sleep(1)
             return self.get(block=block)
         return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `common-task-system-client-1.0.9/task_system_client/task_center/subscription/redis.py` & `common-task-system-client-1.1.0/task_system_client/task_center/subscription/redis.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/task_center/subscription/sql.py` & `common-task-system-client-1.1.0/task_system_client/task_center/subscription/sql.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/task_center/task.py` & `common-task-system-client-1.1.0/task_system_client/task_center/task.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/utils/db_utils.py` & `common-task-system-client-1.1.0/task_system_client/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `common-task-system-client-1.0.9/task_system_client/utils/module_loading.py` & `common-task-system-client-1.1.0/task_system_client/utils/module_loading.py`

 * *Files identical despite different names*

