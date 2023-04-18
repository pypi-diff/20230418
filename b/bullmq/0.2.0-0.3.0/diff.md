# Comparing `tmp/bullmq-0.2.0.tar.gz` & `tmp/bullmq-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.2.0.tar", last modified: Wed Mar 29 08:26:59 2023, max compression
+gzip compressed data, was "bullmq-0.3.0.tar", last modified: Tue Apr 18 08:58:58 2023, max compression
```

## Comparing `bullmq-0.2.0.tar` & `bullmq-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-03-29 08:26:59.207622 bullmq-0.2.0/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-03-29 08:26:59.207160 bullmq-0.2.0/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-03-29 08:17:29.000000 bullmq-0.2.0/README.md
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-03-29 08:26:59.185293 bullmq-0.2.0/bullmq/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      268 2023-02-16 14:21:48.000000 bullmq-0.2.0/bullmq/__init__.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-03-29 08:26:59.206478 bullmq-0.2.0/bullmq/commands/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/addJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/drain-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/getState-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/moveJobFromActiveToWait-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/pause-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/promote-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/reprocessJob-4.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/takeLock-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/updateData-1.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.2.0/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      199 2023-02-16 14:21:48.000000 bullmq-0.2.0/bullmq/error_code.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      595 2023-02-16 14:21:48.000000 bullmq-0.2.0/bullmq/event_emitter.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     2774 2023-02-16 14:21:48.000000 bullmq-0.2.0/bullmq/job.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     2914 2023-02-22 15:05:49.000000 bullmq-0.2.0/bullmq/queue.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      634 2023-02-16 14:21:48.000000 bullmq-0.2.0/bullmq/redis_connection.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     9614 2023-03-29 08:15:17.000000 bullmq-0.2.0/bullmq/scripts.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)      702 2023-02-16 14:21:48.000000 bullmq-0.2.0/bullmq/timer.py
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     6812 2023-03-29 08:06:55.000000 bullmq-0.2.0/bullmq/worker.py
-drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-03-29 08:26:59.186867 bullmq-0.2.0/bullmq.egg-info/
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-03-29 08:26:59.000000 bullmq-0.2.0/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1333 2023-03-29 08:26:59.000000 bullmq-0.2.0/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-03-29 08:26:59.000000 bullmq-0.2.0/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-03-29 08:26:59.000000 bullmq-0.2.0/bullmq.egg-info/requires.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-03-29 08:26:59.000000 bullmq-0.2.0/bullmq.egg-info/top_level.txt
--rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-03-29 08:26:59.207740 bullmq-0.2.0/setup.cfg
--rw-r--r--   0 manuelastudillo   (501) staff       (20)     1183 2023-03-29 08:26:42.000000 bullmq-0.2.0/setup.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.060057 bullmq-0.3.0/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-04-18 08:58:58.059681 bullmq-0.3.0/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      999 2023-03-29 08:17:29.000000 bullmq-0.3.0/README.md
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.036847 bullmq-0.3.0/bullmq/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      268 2023-02-16 14:21:48.000000 bullmq-0.3.0/bullmq/__init__.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.058868 bullmq-0.3.0/bullmq/commands/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     8245 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      810 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     9375 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5979 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/drain-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      501 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      809 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1748 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1313 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getState-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      934 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      897 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      424 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      543 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveJobFromActiveToWait-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    11863 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7013 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     4123 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    21423 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1315 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7844 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      522 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/pause-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1967 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/promote-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      292 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     7980 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      666 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      846 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/reprocessJob-4.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     3150 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1830 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      282 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/takeLock-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      246 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      420 2023-02-13 17:54:41.000000 bullmq-0.3.0/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      200 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/error_code.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      632 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/event_emitter.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5277 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/job.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     5285 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/queue.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      676 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/redis_connection.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)    10209 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/scripts.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)      699 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/timer.py
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     8492 2023-04-18 08:29:50.000000 bullmq-0.3.0/bullmq/worker.py
+drwxr-xr-x   0 manuelastudillo   (501) staff       (20)        0 2023-04-18 08:58:58.038537 bullmq-0.3.0/bullmq.egg-info/
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1651 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1333 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        1 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       14 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/requires.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)        7 2023-04-18 08:58:57.000000 bullmq-0.3.0/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)       38 2023-04-18 08:58:58.060205 bullmq-0.3.0/setup.cfg
+-rw-r--r--   0 manuelastudillo   (501) staff       (20)     1183 2023-04-18 08:57:31.000000 bullmq-0.3.0/setup.py
```

### Comparing `bullmq-0.2.0/PKG-INFO` & `bullmq-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.2.0
+Version: 0.3.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.2.0/README.md` & `bullmq-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/addJob-8.lua` & `bullmq-0.3.0/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/changeDelay-3.lua` & `bullmq-0.3.0/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.3.0/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/drain-4.lua` & `bullmq-0.3.0/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/getCounts-1.lua` & `bullmq-0.3.0/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/getRanges-1.lua` & `bullmq-0.3.0/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/getState-7.lua` & `bullmq-0.3.0/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/getStateV2-7.lua` & `bullmq-0.3.0/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/isFinished-3.lua` & `bullmq-0.3.0/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/moveJobFromActiveToWait-4.lua` & `bullmq-0.3.0/bullmq/commands/moveJobFromActiveToWait-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.3.0/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/moveToActive-9.lua` & `bullmq-0.3.0/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.3.0/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.3.0/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.3.0/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/obliterate-2.lua` & `bullmq-0.3.0/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/pause-4.lua` & `bullmq-0.3.0/bullmq/commands/pause-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/promote-6.lua` & `bullmq-0.3.0/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/removeJob-1.lua` & `bullmq-0.3.0/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.3.0/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/reprocessJob-4.lua` & `bullmq-0.3.0/bullmq/commands/reprocessJob-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/retryJob-8.lua` & `bullmq-0.3.0/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/commands/retryJobs-6.lua` & `bullmq-0.3.0/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/bullmq/event_emitter.py` & `bullmq-0.3.0/bullmq/event_emitter.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 
 
 class EventEmitter:
 
     def __init__(self):
         self._callbacks: Dict[str, callable] = {}
 
-    def on(self, event_name, function):
-        self._callbacks[event_name] = self._callbacks.get(event_name, []) + [function]
+    def on(self, event_name: str, function):
+        self._callbacks[event_name] = self._callbacks.get(
+            event_name, []) + [function]
         return function
 
-    def emit(self, event_name, *args, **kwargs):
-        [function(*args, **kwargs) for function in self._callbacks.get(event_name, [])]
+    def emit(self, event_name: str, *args, **kwargs):
+        [function(*args, **kwargs)
+         for function in self._callbacks.get(event_name, [])]
 
-    def off(self, event_name, function):
+    def off(self, event_name: str, function):
         self._callbacks.get(event_name, []).remove(function)
```

### Comparing `bullmq-0.2.0/bullmq/redis_connection.py` & `bullmq-0.3.0/bullmq/redis_connection.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 import redis.asyncio as redis
 
-"""
-    RedisConnection class
-"""
+
 class RedisConnection:
-    def __init__(self, redisOpts = {}):
+    """
+    RedisConnection class
+    """
+
+    def __init__(self, redisOpts: dict = {}):
         host = redisOpts.get("host") or "localhost"
         port = redisOpts.get("port") or 6379
         db = redisOpts.get("db") or 0
         password = redisOpts.get("password") or None
-        
-        self.conn = redis.Redis(host=host, port=port, db=db, password=password, decode_responses=True)
-        
+
+        self.conn = redis.Redis(
+            host=host, port=port, db=db, password=password, decode_responses=True)
+
     def disconnect(self):
-        """ "Disconnect from Redis" """
+        """
+        Disconnect from Redis
+        """
         return self.conn.disconnect()
+
     def close(self):
-        """ "Close the connection" """
+        """
+        Close the connection
+        """
         return self.conn.close()
```

### Comparing `bullmq-0.2.0/bullmq/scripts.py` & `bullmq-0.3.0/bullmq/scripts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,226 +1,253 @@
 """
     This class is used to load and execute Lua scripts.
     It is a wrapper around the Redis client.
 """
-from typing import Any, Dict, List, Union
+from typing import Any
+from redis import Redis
+from bullmq.job import Job
+from bullmq.error_code import ErrorCode
+
 import time
 import json
 import msgpack
 import os
 
-from redis import Redis
-
-from bullmq.job import Job
-from bullmq.error_code import ErrorCode
 
 basePath = os.path.dirname(os.path.realpath(__file__))
 
+
 class Scripts:
 
-    def __init__(self, prefix: str, queueName: str, redisClient):
+    def __init__(self, prefix: str, queueName: str, redisClient: Redis):
         self.prefix = prefix
         self.queueName = queueName
         self.keys = {}
         self.redisClient = redisClient
         self.commands = {
             "addJob": redisClient.register_script(self.getScript("addJob-8.lua")),
+            "getCounts": redisClient.register_script(self.getScript("getCounts-1.lua")),
             "obliterate": redisClient.register_script(self.getScript("obliterate-2.lua")),
             "pause": redisClient.register_script(self.getScript("pause-4.lua")),
             "moveToActive": redisClient.register_script(self.getScript("moveToActive-9.lua")),
             "moveToFinished": redisClient.register_script(self.getScript("moveToFinished-12.lua")),
             "extendLock": redisClient.register_script(self.getScript("extendLock-2.lua")),
             "moveStalledJobsToWait": redisClient.register_script(self.getScript("moveStalledJobsToWait-8.lua")),
             "retryJobs": redisClient.register_script(self.getScript("retryJobs-6.lua")),
         }
 
         # loop all the names and add them to the keys object
-        names = ["", "active", "wait", "paused", "completed", "failed", "delayed", "stalled", "limiter", "priority", "id", "stalled-check", "meta", "events"]
+        names = ["", "active", "wait", "paused", "completed", "failed", "delayed",
+                 "stalled", "limiter", "priority", "id", "stalled-check", "meta", "events"]
         for name in names:
             self.keys[name] = self.toKey(name)
-    
-    def toKey(self, name):
-        return self.prefix + ":" + self.queueName + ":" + name
-
-    def getScript(self, name):
-        "Get a script by name"
-        file = open(basePath + "/commands/" + name, "r")
+
+    def toKey(self, name: str):
+        return f"{self.prefix}:{self.queueName}:{name}"
+
+    def getScript(self, name: str):
+        """
+        Get a script by name
+        """
+        file = open(f"{basePath}/commands/{name}", "r")
         data = file.read()
         file.close()
         return data
 
-    def getKeys(self, keys: list):
+    def getKeys(self, keys: list[str]):
         def mapKey(key):
             return self.keys[key]
         return list(map(mapKey, keys))
 
     def addJob(self, job: Job):
-        "Add an item to the queue"
-
-        packedArgs = msgpack.packb([self.keys[""], job.id or "", job.name, job.timestamp], use_bin_type=True)
+        """
+        Add an item to the queue
+        """
+        packedArgs = msgpack.packb(
+            [self.keys[""], job.id or "", job.name, job.timestamp], use_bin_type=True)
         #  We are still lacking some arguments here:
         #  ARGV[1] msgpacked arguments array
         #         [1]  key prefix,
         #         [2]  custom id (will not generate one automatically)
         #         [3]  name
         #         [4]  timestamp
         #         [5]  parentKey?
         #         [6]  waitChildrenKey key.
         #         [7]  parent dependencies key.
         #         [8]  parent? {id, queueKey}
         #         [9]  repeat job key
-        
+
         jsonData = json.dumps(job.data, separators=(',', ':'))
         packedOpts = msgpack.packb(job.opts)
-        
-        keys = self.getKeys(['wait', 'paused', 'meta', 'id', 'delayed', 'priority', 'completed', 'events'])
-      
+
+        keys = self.getKeys(['wait', 'paused', 'meta', 'id',
+                            'delayed', 'priority', 'completed', 'events'])
+
         return self.commands["addJob"](keys=keys, args=[packedArgs, jsonData, packedOpts])
-    
-    def pause(self, pause: bool = True):
-        "Pause or resume a queue"
 
+    def getCounts(self, types):
+        keys = self.getKeys([''])
+        transformed_types = list(map(lambda type: 'wait' if type == 'waiting' else type, types))
+
+        return self.commands["getCounts"](keys=keys, args=transformed_types)
+
+    def pause(self, pause: bool = True):
+        """
+        Pause or resume a queue
+        """
         src = "wait" if pause else "paused"
         dst = "paused" if pause else "wait"
-
         keys = self.getKeys([src, dst, 'meta', 'events'])
         return self.commands["pause"](keys, args=["paused" if pause else "resumed"])
-    
+
     async def obliterate(self, count: int, force: bool = False):
-        "Remove a queue completely"
+        """
+        Remove a queue completely
+        """
         keys = self.getKeys(['meta', ''])
         result = await self.commands["obliterate"](keys, args=[count, force or ""])
         if (result < 0):
             if (result == -1):
                 raise Exception("Cannot obliterate non-paused queue")
             if (result == -2):
                 raise Exception("Cannot obliterate queue with active jobs")
         return result
 
-    async def retryJobs(self, state: str = "failed", count: int = 1000, timestamp: int = round(time.time()*1000)):
-        "Remove a queue completely"
-        keys = self.getKeys(['', 'events', state, 'wait', 'paused', 'meta'])
-        result = await self.commands["retryJobs"](keys, args=[count, timestamp, state])
+    async def retryJobs(self, state: str, count: int, timestamp: int):
+        """
+        Remove a queue completely
+        """
+        current_state = state or 'failed'
+        keys = self.getKeys(['', 'events', current_state, 'wait', 'paused', 'meta'])
+        result = await self.commands["retryJobs"](keys=keys, args=[count or 1000, timestamp or round(time.time()*1000), current_state])
         return result
 
     async def moveToActive(self, token: str, opts: dict, jobId: str = "") -> list[Any]:
-        "Add an item to the queue"
-
+        """
+        Add an item to the queue
+        """
         timestamp = round(time.time() * 1000)
-
         lockDuration = opts.get("lockDuration", 0)
         limiter = opts.get("limiter", None)
-      
-        keys = self.getKeys(['wait', 'active', 'priority', 'events', 'stalled', 'limiter', 'delayed', 'paused', 'meta'])
-        packedOpts = msgpack.packb({"token": token, "lockDuration": lockDuration, "limiter": limiter }, use_bin_type=True)
+
+        keys = self.getKeys(['wait', 'active', 'priority', 'events',
+                            'stalled', 'limiter', 'delayed', 'paused', 'meta'])
+        packedOpts = msgpack.packb(
+            {"token": token, "lockDuration": lockDuration, "limiter": limiter}, use_bin_type=True)
         args = [self.keys[''], timestamp, jobId or "", packedOpts]
-      
+
         result = await self.commands["moveToActive"](keys=keys, args=args)
 
         # Todo: up to 4 results in tuple (only 2 now)
         return raw2NextJobData(result)
 
-
-    def moveToCompleted(self, job: Job, val: Any, removeOnComplete, token: str, opts: dict, fetchNext = True):
+    def moveToCompleted(self, job: Job, val: Any, removeOnComplete, token: str, opts: dict, fetchNext=True):
         return self.moveToFinished(job, val, "returnvalue", removeOnComplete, "completed", token, opts, fetchNext)
 
-    def moveToFailed(self, job: Job, failedReason: str, removeOnFailed, token: str, opts: dict, fetchNext = True):
+    def moveToFailed(self, job: Job, failedReason: str, removeOnFailed, token: str, opts: dict, fetchNext=True):
         return self.moveToFinished(job, failedReason, "failedReason", removeOnFailed, "failed", token, opts, fetchNext)
 
-    async def moveToFinished(self, job: Job, val: Any, propVal: str, shouldRemove, target, token: str, opts: dict, fetchNext = True ) -> list[Any] | None:
+    async def moveToFinished(self, job: Job, val: Any, propVal: str, shouldRemove, target, token: str, opts: dict, fetchNext=True) -> list[Any] | None:
         timestamp = round(time.time() * 1000)
-        metricsKey = self.toKey('metrics:' + target);
+        metricsKey = self.toKey('metrics:' + target)
 
-        keys = self.getKeys(['wait', 'active', 'priority', 'events', 'stalled', 'limiter', 'delayed', 'paused', target])
+        keys = self.getKeys(['wait', 'active', 'priority', 'events',
+                            'stalled', 'limiter', 'delayed', 'paused', target])
         keys.append(self.toKey(job.id))
         keys.append(self.keys['meta'])
         keys.append(metricsKey)
 
-        def getKeepJobs(shouldRemove):
-            if shouldRemove == True:
-                return { "count": 0 }
-            
+        def getKeepJobs(shouldRemove: bool | dict | int | None):
             if type(shouldRemove) == int:
-                return { "count": shouldRemove }
+                return {"count": shouldRemove}
 
             if type(shouldRemove) == dict:
                 return shouldRemove
 
-            if shouldRemove == False or shouldRemove == None:
-                return { "count": -1 }
+            if shouldRemove:
+                return {"count": 0}
 
-        def getMetricsSize(opts):
+            if not shouldRemove or shouldRemove is None:
+                return {"count": -1}
+
+        def getMetricsSize(opts: dict):
             metrics = opts.get("metrics")
-            if metrics != None:
+            if metrics is not None:
                 return metrics.get("maxDataPoints", "")
             return ""
 
-        def getFailParentOnFailure(job):
+        def getFailParentOnFailure(job: Job):
             opts = job.opts
-            if opts != None:
+            if opts is not None:
                 return opts.get("failParentOnFailure", False)
 
         keepJobs = getKeepJobs(shouldRemove)
 
         packedOpts = msgpack.packb({
             "token": token,
             "keepJobs": keepJobs,
             "limiter": opts.get("limiter"),
             "lockDuration": opts.get("lockDuration"),
             "attempts": job.attempts,
             "attemptsMade": job.attemptsMade,
             "maxMetricsSize": getMetricsSize(opts),
             "fpof": getFailParentOnFailure(job),
         }, use_bin_type=True)
-         
-        args = [job.id, timestamp, propVal, val or "", target, "", fetchNext and "fetch" or "" , self.keys[''], packedOpts]
+
+        args = [job.id, timestamp, propVal, val or "", target, "",
+                fetchNext and "fetch" or "", self.keys[''], packedOpts]
         result = await self.commands["moveToFinished"](keys=keys, args=args)
 
-        if result != None:
+        if result is not None:
             if result < 0:
-                raise finishedErrors(result, job.id, 'finished', 'active');
+                raise finishedErrors(result, job.id, 'finished', 'active')
             else:
                 # I do not like this as it is using a sideeffect
                 job.finishedOn = timestamp
             return raw2NextJobData(result)
         return None
 
     def extendLock(self, jobId: str, token: str, duration: int, client: Redis = None):
         keys = [self.toKey(jobId) + ":lock", self.keys['stalled']]
         args = [token, duration, jobId]
         return self.commands["extendLock"](keys, args, client)
 
     def moveStalledJobsToWait(self, maxStalledCount: int, stalledInterval: int):
-        keys = self.getKeys(['stalled', 'wait', 'active', 'failed', 'stalled-check', 'meta', 'paused', 'events'])
-        args = [maxStalledCount, self.keys[''], round(time.time() * 1000), stalledInterval]
+        keys = self.getKeys(['stalled', 'wait', 'active', 'failed',
+                            'stalled-check', 'meta', 'paused', 'events'])
+        args = [maxStalledCount, self.keys[''], round(
+            time.time() * 1000), stalledInterval]
         return self.commands["moveStalledJobsToWait"](keys, args)
 
+
 def finishedErrors(code: int, jobId: str, command: str, state: str) -> TypeError:
     if code == ErrorCode.JobNotExist.value:
-        return TypeError("Missing key for job " + jobId + "." + command)
+        return TypeError(f"Missing key for job {jobId}.{command}")
     elif code == ErrorCode.JobLockNotExist.value:
-        return TypeError("Missing lock for job " + jobId + "." + command)
+        return TypeError(f"Missing lock for job {jobId}.{command}")
     elif code == ErrorCode.JobNotInState.value:
-        return TypeError("Job " + jobId + " is not in the state" + state + "." + command)
+        return TypeError(f"Job {jobId} is not in the state {state}.{command}")
     elif code == ErrorCode.JobPendingDependencies.value:
-        return TypeError("Job " + jobId + " has pending dependencies. " + command)
+        return TypeError(f"Job {jobId} has pending dependencies.{command}")
     elif code == ErrorCode.ParentJobNotExist.value:
-        return TypeError("Missing key for parent job " + jobId + "." + command)
+        return TypeError(f"Missing key for parent job {jobId}.{command}")
     elif code == ErrorCode.JobLockMismatch.value:
-        return TypeError("Lock mismatch for job " + jobId + ". Cmd "+ command + " from " + state)
+        return TypeError(f"Lock mismatch for job {jobId}. Cmd {command} from {state}")
     else:
-        return TypeError("Unknown code " + str(code) + " error for " + jobId + "." + command)
+        return TypeError(f"Unknown code {str(code)} error for {jobId}.{command}")
+
 
 def raw2NextJobData(raw: list[Any]) -> list[Any] | None:
     if raw:
         # TODO: return all the raw datas (up to 4)
         if raw[0]:
             return (array2obj(raw[0]), raw[1])
         else:
             return (None, raw[1])
     return None
 
-def array2obj(arr: [str]) -> {str: str}:
+
+def array2obj(arr: list[str]) -> dict[str, str]:
     obj = {}
     for i in range(0, len(arr), 2):
         obj[arr[i]] = arr[i + 1]
     return obj
```

### Comparing `bullmq-0.2.0/bullmq/timer.py` & `bullmq-0.3.0/bullmq/timer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import asyncio
 
 # Credits: https://stackoverflow.com/questions/45419723/python-timer-with-asyncio-coroutine
+
+
 class Timer:
-    def __init__(self, interval, callback, *args, **kwargs):
+    def __init__(self, interval: int, callback, *args, **kwargs):
         self.interval = interval
-        self.args       = args
-        self.kwargs     = kwargs
+        self.args = args
+        self.kwargs = kwargs
         self.callback = callback
         self._ok = True
         self._task = asyncio.ensure_future(self._job())
 
     async def _job(self):
         try:
             while self._ok:
```

### Comparing `bullmq-0.2.0/bullmq/worker.py` & `bullmq-0.3.0/bullmq/worker.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,130 +1,186 @@
-from typing import Callable
+from typing import Callable, TypedDict, Any, List
 from uuid import uuid4
-import asyncio
-import traceback
-import time
-
-from redis import Redis
-
 from bullmq.scripts import Scripts
 from bullmq.redis_connection import RedisConnection
 from bullmq.event_emitter import EventEmitter
 from bullmq.job import Job
 from bullmq.timer import Timer
 
+import asyncio
+import traceback
+import time
+
+
+class WorkerOptions(TypedDict, total=False):
+    autorun: bool
+    """
+    Condition to start processor at instance creation
+
+    @default true
+    """
+
+    concurrency: int
+    """
+    Amount of jobs that a single worker is allowed to work on
+    in parallel.
+
+    @default 1
+    @see https://docs.bullmq.io/guide/workers/concurrency
+    """
+
+    maxStalledCount: int
+    """
+    Amount of times a job can be recovered from a stalled state
+    to the `wait` state. If this is exceeded, the job is moved
+    to `failed`.
+
+    @default 1
+    """
+
+    stalledInterval: int
+    """
+    Number of milliseconds between stallness checks.
+
+    @default 30000
+    """
+
+    lockDuration: int
+    """
+    Duration of the lock for the job in milliseconds. The lock represents that
+    a worker is processing the job. If the lock is lost, the job will be eventually
+    be picked up by the stalled checker and move back to wait so that another worker
+    can process it again.
+
+    @default 30000
+    """
+
+    prefix: str
+    """
+    Prefix for all queue keys.
+    """
+
+    connection: dict[str, Any]
+    """
+    Options for connecting to a Redis instance.
+    """
+
+
 class Worker(EventEmitter):
-    def __init__(self, name: str, processor: Callable[[Job, str], asyncio.Future], opts = {}):
-        super().__init__()  
+    def __init__(self, name: str, processor: Callable[[Job, str], asyncio.Future], opts: WorkerOptions = {}):
+        super().__init__()
         self.name = name
         self.processor = processor
         self.opts = {
             "concurrency": opts.get("concurrency", 1),
             "lockDuration": opts.get("lockDuration", 30000),
             "maxStalledCount": opts.get("maxStalledCount", 1),
             "stalledInterval": opts.get("stalledInterval", 30000),
         }
-
-        redisOpts = opts.get("connection") or {}
-
-        self.redisConnection = RedisConnection(redisOpts)
+        redis_opts = opts.get("connection", {})
+        self.redisConnection = RedisConnection(redis_opts)
+        self.blockingRedisConnection = RedisConnection(redis_opts)
         self.client = self.redisConnection.conn
-
-        self.blockingRedisConnection = RedisConnection(redisOpts)
         self.bclient = self.blockingRedisConnection.conn
-    
-        self.scripts = Scripts(opts.get("prefix") or "bull", name, self.client)
-
+        self.scripts = Scripts(opts.get("prefix", "bull"), name, self.client)
         self.closing = False
         self.forceClosing = False
         self.closed = False
         self.running = False
         self.processing = set()
         self.jobs = set()
 
         if opts.get("autorun", True):
             asyncio.ensure_future(self.run())
 
     async def run(self):
         if self.running:
             raise Exception("Worker is already running")
 
-        self.timer = Timer((self.opts.get("lockDuration") / 2) / 1000, self.extendLocks)
-        self.stalledCheckTimer = Timer(self.opts.get("stalledInterval") / 1000, self.runStalledJobsCheck)
+        self.timer = Timer(
+            (self.opts.get("lockDuration") / 2) / 1000, self.extendLocks)
+        self.stalledCheckTimer = Timer(self.opts.get(
+            "stalledInterval") / 1000, self.runStalledJobsCheck)
         self.running = True
-        job = None
+        jobs = []
 
         token = uuid4().hex
+
         while not self.closed:
-            # if not job and len(self.processing) < self.opts.get("concurrency") and not self.closing:
-            #     waitingJob = asyncio.ensure_future(self.getNextJob(token))
-            #     self.processing.add(waitingJob)
-
-            if job:
-                processingJob = asyncio.ensure_future(self.processJob(job, token))
-                self.processing.add(processingJob)
-
-            if len(self.processing) < self.opts.get("concurrency") and not self.closing:
-                waitingJob = asyncio.ensure_future(self.getNextJob(token))
-                self.processing.add(waitingJob)
+            if len(jobs) == 0 and len(self.processing) < self.opts.get("concurrency") and not self.closing:
+                waiting_job = asyncio.ensure_future(self.getNextJob(token))
+                self.processing.add(waiting_job)
+
+            if len(jobs) > 0:
+                jobs_to_process = [self.processJob(job, token) for job in jobs]
+                processing_jobs = [asyncio.ensure_future(
+                    j) for j in jobs_to_process]
+                self.processing.update(processing_jobs)
 
             try:
-                job, pending = await getFirstCompleted(self.processing)
+                jobs, pending = await getCompleted(self.processing)
+
                 self.processing = pending
 
-                if job == None or len(self.processing) == 0 and self.closing:
+                if (len(jobs) == 0 or len(self.processing) == 0) and self.closing:
                     # We are done processing so we can close the queue
                     break
 
             except Exception as e:
                 # This should never happen or we will have an endless loop
                 print("ERROR:", e)
                 traceback.print_exc()
                 return
 
         self.running = False
         self.timer.stop()
         self.stalledCheckTimer.stop()
 
     async def getNextJob(self, token: str):
+        """
+        Returns a promise that resolves to the next job in queue.
+        @param token: worker token to be assigned to retrieved job
+        @returns a Job or undefined if no job was available in the queue.
+        """
         # First try to move a job from the waiting list to the active list
         result = await self.scripts.moveToActive(token, self.opts)
         job = None
-        jobId = None
-        delayUntil = None
+        job_id = None
+        delay_until = None
         if result:
-            job, jobId = result
+            job, job_id = result
 
         # If there are no jobs in the waiting list we keep waiting with BRPOPLPUSH
-        if job == None:
-            timeout = min(delayUntil - int(time.time() * 1000) if delayUntil else 5000, 5000) / 1000
-            jobId = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
-            if jobId:
-                job, jobId = await self.scripts.moveToActive(token, self.opts, jobId)
+        if job is None:
+            timeout = min(delay_until - int(time.time() * 1000)
+                          if delay_until else 5000, 5000) / 1000
+            job_id = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
+            if job_id:
+                job, job_id = await self.scripts.moveToActive(token, self.opts, job_id)
 
-        if job and jobId:
-            return Job.fromJSON(self.client, job, jobId)
+        if job and job_id:
+            return Job.fromJSON(self.client, job, job_id)
 
     async def processJob(self, job: Job, token: str):
         try:
             self.jobs.add((job, token))
             result = await self.processor(job, token)
             if not self.forceClosing:
-                await self.scripts.moveToCompleted(job, result, job.opts.get("removeOnComplete", True), token, self.opts, fetchNext=not self.closing)
+                await self.scripts.moveToCompleted(job, result, job.opts.get("removeOnComplete", False), token, self.opts, fetchNext=not self.closing)
             self.emit("completed", job, result)
         except Exception as err:
             try:
                 print("Error processing job", err)
                 stacktrace = traceback.format_exc()
 
                 if not self.forceClosing:
                     await self.scripts.moveToFailed(job, str(err), job.opts.get("removeOnFail", False), token, self.opts, fetchNext=not self.closing)
 
                 # TODO: Store the stacktrace in the job
-                
+
                 self.emit("failed", job, err)
             except Exception as err:
                 print("Error moving job to failed", err)
                 self.emit("error", err, job)
         finally:
             self.jobs.remove((job, token))
 
@@ -136,44 +192,56 @@
                 await self.scripts.extendLock(job.id, token, self.opts.get("lockDuration"), multi)
             result = await multi.execute()
 
             # result includes an object with locks that may not have been renewed.
             # We should emit an error for each of those jobs.
             #    for jobId, err in result.items():
             #    self.emit("error", "could not renew lock for job " + jobId)
-            
+
         except Exception as e:
             print("Error renewing locks", e)
             traceback.print_exc()
 
     async def runStalledJobsCheck(self):
         try:
             failed, stalled = await self.scripts.moveStalledJobsToWait(self.opts.get("maxStalledCount"), self.opts.get("stalledInterval"))
             for jobId in failed:
-                self.emit("failed", jobId, "job stalled more than allowable limit")
+                self.emit("failed", jobId,
+                          "job stalled more than allowable limit")
             for jobId in stalled:
                 self.emit("stalled", jobId)
 
         except Exception as e:
             print("Error checking stalled jobs", e)
             self.emit('error', e)
 
     async def close(self, force: bool = False):
-        """ "Close the worker" """
+        """
+        Close the worker
+        """
         if force:
             self.forceClosing = True
 
         self.closing = True
 
         await self.blockingRedisConnection.close()
         await self.redisConnection.close()
 
-async def getFirstCompleted( taskSet: set):
-    jobSet, pending = await asyncio.wait(taskSet, return_when=asyncio.FIRST_COMPLETED)
-    for jobTask in jobSet:
-        try: 
-            job = jobTask.result()
-            return (job, pending)
-        except Exception as e:
-            print("ERROR:", e)
-            traceback.print_exc()
-            return (None, pending)
+
+async def getCompleted(task_set: set) -> tuple[list[Job], list]:
+    job_set, pending = await asyncio.wait(task_set, return_when=asyncio.FIRST_COMPLETED)
+    jobs = [extract_result(job_task) for job_task in job_set]
+    # we filter `None` out to remove:
+    # a) an empty 'completed jobs' list; and
+    # b) a failed extract_result
+    jobs = list(filter(lambda j: j is not None, jobs))
+    return jobs, pending
+
+
+def extract_result(job_task):
+    try:
+        return job_task.result()
+    except Exception as e:
+        # lets use a simple-but-effective error handling:
+        # print error message and ignore the job
+        print("ERROR:", e)
+        traceback.print_exc()
```

### Comparing `bullmq-0.2.0/bullmq.egg-info/PKG-INFO` & `bullmq-0.3.0/bullmq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.2.0
+Version: 0.3.0
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.2.0/bullmq.egg-info/SOURCES.txt` & `bullmq-0.3.0/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.2.0/setup.py` & `bullmq-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # Get the long description from the README file
 with open(path.join(".", 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='bullmq',
-    version='0.2.0',    
+    version='0.3.0',    
     description='BullMQ for Python',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://bullmq.io',
     author='Taskforce.sh Inc.',
     author_email='manast@taskforce.sh',
     license='MIT',
```

