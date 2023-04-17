# Comparing `tmp/taskiq-0.4.0.tar.gz` & `tmp/taskiq-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskiq-0.4.0.tar", max compression
+gzip compressed data, was "taskiq-0.4.1.tar", max compression
```

## Comparing `taskiq-0.4.0.tar` & `taskiq-0.4.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1075 2023-04-09 23:15:51.392623 taskiq-0.4.0/LICENSE
--rw-r--r--   0        0        0     1875 2023-04-09 23:15:51.392623 taskiq-0.4.0/README.md
--rw-r--r--   0        0        0     2888 2023-04-09 23:15:51.396623 taskiq-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1587 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/__init__.py
--rw-r--r--   0        0        0     2077 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/__main__.py
--rw-r--r--   0        0        0      194 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/__init__.py
--rw-r--r--   0        0        0     9488 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/broker.py
--rw-r--r--   0        0        0      323 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/cmd.py
--rw-r--r--   0        0        0      629 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/formatter.py
--rw-r--r--   0        0        0     2997 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/middleware.py
--rw-r--r--   0        0        0     1375 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/result_backend.py
--rw-r--r--   0        0        0     1084 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/abc/schedule_source.py
--rw-r--r--   0        0        0       34 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/__init__.py
--rw-r--r--   0        0        0     5874 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/inmemory_broker.py
--rw-r--r--   0        0        0     2154 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/shared_broker.py
--rw-r--r--   0        0        0     2514 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/brokers/zmq_broker.py
--rw-r--r--   0        0        0       31 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/__init__.py
--rw-r--r--   0        0        0      197 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/common_args.py
--rw-r--r--   0        0        0       37 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/__init__.py
--rw-r--r--   0        0        0     1990 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/args.py
--rw-r--r--   0        0        0      651 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/cmd.py
--rw-r--r--   0        0        0     3911 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/scheduler/run.py
--rw-r--r--   0        0        0     2550 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/utils.py
--rw-r--r--   0        0        0     1516 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/watcher.py
--rw-r--r--   0        0        0       43 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/__init__.py
--rw-r--r--   0        0        0     4286 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/args.py
--rw-r--r--   0        0        0      628 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/cmd.py
--rw-r--r--   0        0        0     1742 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/log_collector.py
--rw-r--r--   0        0        0     7498 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/process_manager.py
--rw-r--r--   0        0        0     5192 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/cli/worker/run.py
--rw-r--r--   0        0        0      468 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/context.py
--rw-r--r--   0        0        0     2929 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/decor.py
--rw-r--r--   0        0        0      510 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/events.py
--rw-r--r--   0        0        0      778 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/exceptions.py
--rw-r--r--   0        0        0       25 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/formatters/__init__.py
--rw-r--r--   0        0        0      844 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/formatters/json_formatter.py
--rw-r--r--   0        0        0     1887 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/funcs.py
--rw-r--r--   0        0        0     5552 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/kicker.py
--rw-r--r--   0        0        0      507 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/message.py
--rw-r--r--   0        0        0       26 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/middlewares/__init__.py
--rw-r--r--   0        0        0     4317 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/middlewares/prometheus_middleware.py
--rw-r--r--   0        0        0     2005 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/middlewares/retry_middleware.py
--rw-r--r--   0        0        0        0 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/py.typed
--rw-r--r--   0        0        0      113 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/receiver/__init__.py
--rw-r--r--   0        0        0     2795 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/receiver/params_parser.py
--rw-r--r--   0        0        0     9641 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/receiver/receiver.py
--rw-r--r--   0        0        0      476 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/result.py
--rw-r--r--   0        0        0       35 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/result_backends/__init__.py
--rw-r--r--   0        0        0     1351 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/result_backends/dummy.py
--rw-r--r--   0        0        0      146 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/schedule_sources/__init__.py
--rw-r--r--   0        0        0     1519 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/schedule_sources/label_based.py
--rw-r--r--   0        0        0      264 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/scheduler/__init__.py
--rw-r--r--   0        0        0     1056 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/scheduler/merge_functions.py
--rw-r--r--   0        0        0     1717 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/scheduler/scheduler.py
--rw-r--r--   0        0        0     1071 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/state.py
--rw-r--r--   0        0        0     4139 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/task.py
--rw-r--r--   0        0        0      874 2023-04-09 23:15:51.396623 taskiq-0.4.0/taskiq/utils.py
--rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 taskiq-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-04-17 22:32:14.530082 taskiq-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1875 2023-04-17 22:32:14.530082 taskiq-0.4.1/README.md
+-rw-r--r--   0        0        0     2888 2023-04-17 22:32:14.534082 taskiq-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1587 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/__init__.py
+-rw-r--r--   0        0        0     2077 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/__main__.py
+-rw-r--r--   0        0        0      194 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/__init__.py
+-rw-r--r--   0        0        0     9488 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/broker.py
+-rw-r--r--   0        0        0      323 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/cmd.py
+-rw-r--r--   0        0        0      629 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/formatter.py
+-rw-r--r--   0        0        0     2997 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/middleware.py
+-rw-r--r--   0        0        0     1375 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/result_backend.py
+-rw-r--r--   0        0        0     1084 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/abc/schedule_source.py
+-rw-r--r--   0        0        0       34 2023-04-17 22:32:14.534082 taskiq-0.4.1/taskiq/brokers/__init__.py
+-rw-r--r--   0        0        0     5874 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/brokers/inmemory_broker.py
+-rw-r--r--   0        0        0     2154 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/brokers/shared_broker.py
+-rw-r--r--   0        0        0     2514 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/brokers/zmq_broker.py
+-rw-r--r--   0        0        0       31 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/__init__.py
+-rw-r--r--   0        0        0      197 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/common_args.py
+-rw-r--r--   0        0        0       37 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/__init__.py
+-rw-r--r--   0        0        0     1990 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/args.py
+-rw-r--r--   0        0        0      651 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/cmd.py
+-rw-r--r--   0        0        0     3911 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/scheduler/run.py
+-rw-r--r--   0        0        0     2550 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/utils.py
+-rw-r--r--   0        0        0     1516 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/watcher.py
+-rw-r--r--   0        0        0       43 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/__init__.py
+-rw-r--r--   0        0        0     4286 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/args.py
+-rw-r--r--   0        0        0      628 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/cmd.py
+-rw-r--r--   0        0        0     1742 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/log_collector.py
+-rw-r--r--   0        0        0     7498 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/process_manager.py
+-rw-r--r--   0        0        0     5375 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/cli/worker/run.py
+-rw-r--r--   0        0        0      468 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/context.py
+-rw-r--r--   0        0        0     2929 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/decor.py
+-rw-r--r--   0        0        0      510 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/events.py
+-rw-r--r--   0        0        0      778 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/exceptions.py
+-rw-r--r--   0        0        0       25 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/formatters/__init__.py
+-rw-r--r--   0        0        0      844 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/formatters/json_formatter.py
+-rw-r--r--   0        0        0     1887 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/funcs.py
+-rw-r--r--   0        0        0     5552 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/kicker.py
+-rw-r--r--   0        0        0      507 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/message.py
+-rw-r--r--   0        0        0       26 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/middlewares/__init__.py
+-rw-r--r--   0        0        0     4315 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/middlewares/prometheus_middleware.py
+-rw-r--r--   0        0        0     2005 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/middlewares/retry_middleware.py
+-rw-r--r--   0        0        0        0 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/py.typed
+-rw-r--r--   0        0        0      113 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/receiver/__init__.py
+-rw-r--r--   0        0        0     2795 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/receiver/params_parser.py
+-rw-r--r--   0        0        0     9641 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/receiver/receiver.py
+-rw-r--r--   0        0        0      476 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/result.py
+-rw-r--r--   0        0        0       35 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/result_backends/__init__.py
+-rw-r--r--   0        0        0     1351 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/result_backends/dummy.py
+-rw-r--r--   0        0        0      146 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/schedule_sources/__init__.py
+-rw-r--r--   0        0        0     1519 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/schedule_sources/label_based.py
+-rw-r--r--   0        0        0      264 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/scheduler/__init__.py
+-rw-r--r--   0        0        0     1056 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/scheduler/merge_functions.py
+-rw-r--r--   0        0        0     1717 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/scheduler/scheduler.py
+-rw-r--r--   0        0        0     1071 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/state.py
+-rw-r--r--   0        0        0     4139 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/task.py
+-rw-r--r--   0        0        0      874 2023-04-17 22:32:14.538082 taskiq-0.4.1/taskiq/utils.py
+-rw-r--r--   0        0        0     3873 1970-01-01 00:00:00.000000 taskiq-0.4.1/PKG-INFO
```

### Comparing `taskiq-0.4.0/LICENSE` & `taskiq-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/README.md` & `taskiq-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/pyproject.toml` & `taskiq-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "taskiq"
-version = "0.4.0"
+version = "0.4.1"
 description = "Distributed task queue with full async support"
 authors = ["Pavel Kirilin <win10@list.ru>"]
 maintainers = ["Pavel Kirilin <win10@list.ru>"]
 readme = "README.md"
 repository = "https://github.com/taskiq-python/taskiq"
 homepage = "https://taskiq-python.github.io/"
 documentation = "https://taskiq-python.github.io/"
```

### Comparing `taskiq-0.4.0/taskiq/__init__.py` & `taskiq-0.4.1/taskiq/__init__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/__main__.py` & `taskiq-0.4.1/taskiq/__main__.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/abc/broker.py` & `taskiq-0.4.1/taskiq/abc/broker.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         :return: nothing.
         """
 
     @overload
     def task(
         self,
         task_name: Callable[_FuncParams, _ReturnType],
-        **lavels: Any,
+        **labels: Any,
     ) -> AsyncTaskiqDecoratedTask[_FuncParams, _ReturnType]:  # pragma: no cover
         ...
 
     @overload
     def task(
         self,
         task_name: Optional[str] = None,
```

### Comparing `taskiq-0.4.0/taskiq/abc/formatter.py` & `taskiq-0.4.1/taskiq/abc/formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/abc/middleware.py` & `taskiq-0.4.1/taskiq/abc/middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/abc/result_backend.py` & `taskiq-0.4.1/taskiq/abc/result_backend.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/abc/schedule_source.py` & `taskiq-0.4.1/taskiq/abc/schedule_source.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/brokers/inmemory_broker.py` & `taskiq-0.4.1/taskiq/brokers/inmemory_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/brokers/shared_broker.py` & `taskiq-0.4.1/taskiq/brokers/shared_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/brokers/zmq_broker.py` & `taskiq-0.4.1/taskiq/brokers/zmq_broker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/scheduler/args.py` & `taskiq-0.4.1/taskiq/cli/scheduler/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/scheduler/cmd.py` & `taskiq-0.4.1/taskiq/cli/scheduler/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/scheduler/run.py` & `taskiq-0.4.1/taskiq/cli/scheduler/run.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/utils.py` & `taskiq-0.4.1/taskiq/cli/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/watcher.py` & `taskiq-0.4.1/taskiq/cli/watcher.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/worker/args.py` & `taskiq-0.4.1/taskiq/cli/worker/args.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/worker/cmd.py` & `taskiq-0.4.1/taskiq/cli/worker/cmd.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/worker/log_collector.py` & `taskiq-0.4.1/taskiq/cli/worker/log_collector.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/worker/process_manager.py` & `taskiq-0.4.1/taskiq/cli/worker/process_manager.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/cli/worker/run.py` & `taskiq-0.4.1/taskiq/cli/worker/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,27 +124,31 @@
     """
     This function starts worker processes.
 
     It just creates multiple child processes
     and joins them all.
 
     :param args: CLI arguments.
+
+    :raises ValueError: if reload flag is used, but dependencies are not installed.
     """
     logging.basicConfig(
         level=logging.getLevelName(args.log_level),
         format="[%(asctime)s][%(name)s][%(levelname)-7s][%(processName)s] %(message)s",
     )
     logging.getLogger("watchdog.observers.inotify_buffer").setLevel(level=logging.INFO)
     logger.info("Starting %s worker processes.", args.workers)
 
     observer = None
-    if Observer is not None:
-        observer = Observer()
 
-    if observer is not None and args.reload:
+    if args.reload and Observer is None:
+        raise ValueError("To use '--reload' flag, please install 'taskiq[reload]'.")
+
+    if Observer is not None and args.reload:
+        observer = Observer()
         observer.start()
         args.workers = 1
         logging.warning(
             "Reload on chage enabled. Number of worker processes set to 1.",
         )
 
     manager = ProcessManager(args=args, observer=observer, worker_function=start_listen)
```

### Comparing `taskiq-0.4.0/taskiq/decor.py` & `taskiq-0.4.1/taskiq/decor.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/exceptions.py` & `taskiq-0.4.1/taskiq/exceptions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/formatters/json_formatter.py` & `taskiq-0.4.1/taskiq/formatters/json_formatter.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/funcs.py` & `taskiq-0.4.1/taskiq/funcs.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/kicker.py` & `taskiq-0.4.1/taskiq/kicker.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/middlewares/prometheus_middleware.py` & `taskiq-0.4.1/taskiq/middlewares/prometheus_middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -53,19 +53,18 @@
 
         try:
             from prometheus_client import (  # noqa: WPS433
                 Counter,
                 Histogram,
                 start_http_server,
             )
-        except ImportError:
-            logger.warn(
-                "Cannot initialize metrics. Please install 'taskiq[metrics]' extra.",
-            )
-            raise
+        except ImportError as exc:
+            raise ImportError(
+                "Cannot initialize metrics. Please install 'taskiq[metrics]'.",
+            ) from exc
 
         self.found_errors = Counter(
             "found_errors",
             "Number of found errors",
             ["task_name"],
         )
         self.received_tasks = Counter(
```

### Comparing `taskiq-0.4.0/taskiq/middlewares/retry_middleware.py` & `taskiq-0.4.1/taskiq/middlewares/retry_middleware.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/receiver/params_parser.py` & `taskiq-0.4.1/taskiq/receiver/params_parser.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/receiver/receiver.py` & `taskiq-0.4.1/taskiq/receiver/receiver.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/result_backends/dummy.py` & `taskiq-0.4.1/taskiq/result_backends/dummy.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/schedule_sources/label_based.py` & `taskiq-0.4.1/taskiq/schedule_sources/label_based.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/scheduler/merge_functions.py` & `taskiq-0.4.1/taskiq/scheduler/merge_functions.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/scheduler/scheduler.py` & `taskiq-0.4.1/taskiq/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/state.py` & `taskiq-0.4.1/taskiq/state.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/task.py` & `taskiq-0.4.1/taskiq/task.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/taskiq/utils.py` & `taskiq-0.4.1/taskiq/utils.py`

 * *Files identical despite different names*

### Comparing `taskiq-0.4.0/PKG-INFO` & `taskiq-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskiq
-Version: 0.4.0
+Version: 0.4.1
 Summary: Distributed task queue with full async support
 Home-page: https://taskiq-python.github.io/
 License: LICENSE
 Keywords: taskiq,tasks,distributed,async
 Author: Pavel Kirilin
 Author-email: win10@list.ru
 Maintainer: Pavel Kirilin
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: taskiq Version: 0.4.0 Summary: Distributed task
+Metadata-Version: 2.1 Name: taskiq Version: 0.4.1 Summary: Distributed task
 queue with full async support Home-page: https://taskiq-python.github.io/
 License: LICENSE Keywords: taskiq,tasks,distributed,async Author: Pavel Kirilin
 Author-email: win10@list.ru Maintainer: Pavel Kirilin Maintainer-email:
 win10@list.ru Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 3 -
 Alpha Classifier: Intended Audience :: Developers Classifier: License :: Other/
 Proprietary License Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python Classifier: Programming Language :: Python :: 3
```

