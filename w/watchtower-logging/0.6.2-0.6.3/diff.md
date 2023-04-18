# Comparing `tmp/watchtower_logging-0.6.2.tar.gz` & `tmp/watchtower_logging-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "watchtower_logging-0.6.2.tar", last modified: Fri Jan 27 19:23:04 2023, max compression
+gzip compressed data, was "watchtower_logging-0.6.3.tar", last modified: Tue Apr 18 10:48:36 2023, max compression
```

## Comparing `watchtower_logging-0.6.2.tar` & `watchtower_logging-0.6.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-01-27 19:23:04.243900 watchtower_logging-0.6.2/
--rw-rw-rw-   0        0        0      265 2023-01-27 19:23:04.243900 watchtower_logging-0.6.2/PKG-INFO
--rw-rw-rw-   0        0        0     9544 2022-02-05 12:27:35.000000 watchtower_logging-0.6.2/README.md
--rw-rw-rw-   0        0        0       42 2023-01-27 19:23:04.247415 watchtower_logging-0.6.2/setup.cfg
--rw-rw-rw-   0        0        0      965 2021-03-24 14:34:42.000000 watchtower_logging-0.6.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:23:04.227845 watchtower_logging-0.6.2/watchtower_logging/
--rw-rw-rw-   0        0        0      301 2021-03-24 14:31:06.000000 watchtower_logging-0.6.2/watchtower_logging/__init__.py
--rw-rw-rw-   0        0        0      864 2022-08-16 10:20:17.000000 watchtower_logging-0.6.2/watchtower_logging/django.py
--rw-rw-rw-   0        0        0       39 2021-01-11 14:33:51.000000 watchtower_logging-0.6.2/watchtower_logging/exceptions.py
--rw-rw-rw-   0        0        0     1158 2021-06-07 12:10:05.000000 watchtower_logging-0.6.2/watchtower_logging/utils.py
--rw-rw-rw-   0        0        0       21 2023-01-25 20:02:04.000000 watchtower_logging-0.6.2/watchtower_logging/version.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:23:04.237218 watchtower_logging-0.6.2/watchtower_logging/watchtower_handler/
--rw-rw-rw-   0        0        0    13484 2023-01-27 19:20:36.000000 watchtower_logging-0.6.2/watchtower_logging/watchtower_handler/__init__.py
--rw-rw-rw-   0        0        0    10632 2023-01-25 19:36:41.000000 watchtower_logging-0.6.2/watchtower_logging/watchtower_logging.py
-drwxrwxrwx   0        0        0        0 2023-01-27 19:23:04.237218 watchtower_logging-0.6.2/watchtower_logging.egg-info/
--rw-rw-rw-   0        0        0      265 2023-01-27 19:23:03.000000 watchtower_logging-0.6.2/watchtower_logging.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      469 2023-01-27 19:23:03.000000 watchtower_logging-0.6.2/watchtower_logging.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-27 19:23:03.000000 watchtower_logging-0.6.2/watchtower_logging.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-01-27 19:23:03.000000 watchtower_logging-0.6.2/watchtower_logging.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-01-27 19:23:03.000000 watchtower_logging-0.6.2/watchtower_logging.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/
+-rw-rw-rw-   0        0        0      265 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0     9544 2022-02-05 12:27:35.000000 watchtower_logging-0.6.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/setup.cfg
+-rw-rw-rw-   0        0        0      965 2021-03-24 14:34:42.000000 watchtower_logging-0.6.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.017777 watchtower_logging-0.6.3/watchtower_logging/
+-rw-rw-rw-   0        0        0      301 2021-03-24 14:31:06.000000 watchtower_logging-0.6.3/watchtower_logging/__init__.py
+-rw-rw-rw-   0        0        0      864 2022-08-16 10:20:17.000000 watchtower_logging-0.6.3/watchtower_logging/django.py
+-rw-rw-rw-   0        0        0       39 2021-01-11 14:33:51.000000 watchtower_logging-0.6.3/watchtower_logging/exceptions.py
+-rw-rw-rw-   0        0        0     1158 2021-06-07 12:10:05.000000 watchtower_logging-0.6.3/watchtower_logging/utils.py
+-rw-rw-rw-   0        0        0       21 2023-04-18 10:47:14.000000 watchtower_logging-0.6.3/watchtower_logging/version.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/watchtower_logging/watchtower_handler/
+-rw-rw-rw-   0        0        0    14097 2023-04-18 10:45:17.000000 watchtower_logging-0.6.3/watchtower_logging/watchtower_handler/__init__.py
+-rw-rw-rw-   0        0        0    10632 2023-01-25 19:36:41.000000 watchtower_logging-0.6.3/watchtower_logging/watchtower_logging.py
+drwxrwxrwx   0        0        0        0 2023-04-18 10:48:36.033830 watchtower_logging-0.6.3/watchtower_logging.egg-info/
+-rw-rw-rw-   0        0        0      265 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      469 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-18 10:48:35.000000 watchtower_logging-0.6.3/watchtower_logging.egg-info/top_level.txt
```

### Comparing `watchtower_logging-0.6.2/README.md` & `watchtower_logging-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.2/setup.py` & `watchtower_logging-0.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.2/watchtower_logging/django.py` & `watchtower_logging-0.6.3/watchtower_logging/django.py`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.2/watchtower_logging/utils.py` & `watchtower_logging-0.6.3/watchtower_logging/utils.py`

 * *Files identical despite different names*

### Comparing `watchtower_logging-0.6.2/watchtower_logging/watchtower_handler/__init__.py` & `watchtower_logging-0.6.3/watchtower_logging/watchtower_handler/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -40,32 +40,48 @@
 
 
 class WatchTowerHandler(logging.Handler):
     """
     A logging handler to send events to a Watch Tower instance
     """
 
-    def __init__(self, beam_id, host=DEFAULT_HOST, use_fallback=True, fallback_host=None, token=None, debug=False, flush_interval=5.0,
-                 force_keep_ahead=False, protocol='https',
-                 queue_size=DEFAULT_QUEUE_SIZE,
-                 retry_backoff=2.0, retry_count=2, timeout=1.0, verify=True, version=__version__, dev=False):
+    def __init__(self,
+                 beam_id: str,
+                 token: (str, None) = None,
+                 host: str = DEFAULT_HOST,
+                 use_fallback: bool = True,
+                 fallback_host: (str, None) = None,
+                 dev: bool = False,
+                 debug: bool = False,
+                 flush_interval: float = 5.0,
+                 force_keep_ahead: bool = False,
+                 protocol: str = 'https',
+                 queue_size: int = DEFAULT_QUEUE_SIZE,
+                 retry_backoff: float = 2.0,
+                 retry_count: int = 2,
+                 timeout: float = 1.0,
+                 verify: bool = True,
+                 version: str = __version__):
         """
         Args:
-            host (str): The Watch Tower host (should include port if necessary)
-            fallback_host (str): The Watchtower fallback host, defaults to fallback.<host>
+            beam_id (str): The id of the Watchtower beam to send the events to
             token (str): Authentication token
+            host (str): The Watchtower host (should include port if necessary)
+            fallback_host (str): The Watchtower fallback host, defaults to fallback.<host>
+            dev (bool): Whether to send the dev flag with all event
             debug (bool): Whether to print debug console messages
-            flush_interval (float): How often to push events to Watch Tower in seconds
+            flush_interval (float): How often to push events to Watchtower in seconds
             force_keep_ahead (bool): Sleep instead of dropping logs when queue fills
             protocol (str): The web protocol to use
             queue_size (int): The max number of logs to queue, set to 0 for no max
             retry_backoff (float): The requests lib backoff factor
             retry_count (int): The number of times to retry a failed request
             timeout (float): The time to wait for a response from Watch Tower
             verify (bool): Whether to perform ssl certificate validation
+            version (str): Version string to specify the watchtower-logging library version
         """
 
         global instances
         instances.append(self)
         logging.Handler.__init__(self)
 
         self.beam_id = beam_id
@@ -88,29 +104,20 @@
         self.retry_count = retry_count
         self.retry_backoff = retry_backoff
         self.protocol = protocol or 'https'
         self.processing_payload = False
         self.version = version
         self.dev = dev
 
-        self.url = '{protocol}://{host}/api/beams/{beam_id}'.format(protocol=self.protocol,
-                                                                    host=self.host,
-                                                                    beam_id=self.beam_id)
-        self.fallback_url = '{protocol}://{host}/api/beams/{beam_id}'.format(protocol=self.protocol,
-                                                                             host=self.fallback_host,
-                                                                             beam_id=self.beam_id)
-
-
         # Keep ahead depends on queue size, so cannot be 0
         if self.force_keep_ahead and not self.max_queue_size:
             self.write_log('Cannot keep ahead of unbound queue, using default queue size')
             self.max_queue_size = DEFAULT_QUEUE_SIZE
 
         self.write_debug_log('Starting debug mode')
-
         self.write_debug_log('Preparing to override loggers')
 
         # prevent infinite recursion by silencing requests and urllib3 loggers
         logging.getLogger('requests').propagate = False
         logging.getLogger('urllib3').propagate = False
 
         # and do the same for ourselves
@@ -123,23 +130,33 @@
         if self.verify and self.protocol == 'http':
             self.write_debug_log('cannot use SSL Verify and unsecure connection')
 
         # Set up automatic retry with back-off
         self.write_debug_log('Preparing to create a Requests session')
         retry = Retry(total=self.retry_count,
                       backoff_factor=self.retry_backoff,
-                      method_whitelist=False,  # Retry for any HTTP verb
+                      allowed_methods=None,  # Retry for any HTTP verb
                       status_forcelist=[500, 502, 503, 504])
         self.session.mount(self.protocol + '://', HTTPAdapter(max_retries=retry))
 
         self.start_worker_thread()
 
         self.write_debug_log('Class initialize complete')
 
-    def emit(self, record):
+    def build_endpoint(self,
+                       host: str):
+
+        return '{protocol}://{host}/api/beams/{beam_id}'.format(
+            protocol=self.protocol,
+            host=host,
+            beam_id=self.beam_id)
+
+    def emit(self,
+             record):
+
         self.write_debug_log("emit() called")
 
         try:
             record = self.format_record(record)
         except Exception as e:
             self.write_log('Exception in WatchTower logging handler: %s' % str(e))
             self.write_log(traceback.format_exc())
@@ -159,44 +176,53 @@
         # Put log message into queue; worker thread will pick up
         if not self.max_queue_size or len(self.queue) < self.max_queue_size:
             self.queue.append(record)
         else:
             self.write_log('Log queue full; log data will be dropped.')
 
     def close(self):
+
         self.shutdown()
         logging.Handler.close(self)
 
     #
     # helper methods
     #
 
     def start_worker_thread(self):
+
         # Start a worker thread responsible for sending logs
         if self.flush_interval > 0:
             self.write_debug_log('Preparing to spin off first worker thread Timer')
             self.timer = Timer(self.flush_interval, self._wt_worker)
             self.timer.daemon = True  # Auto-kill thread if main process exits
             self.timer.start()
 
-    def write_log(self, log_message):
+    def write_log(self,
+                  log_message: str):
+
         print('[WatchTowerHandler] ' + log_message)
 
-    def write_debug_log(self, log_message):
+    def write_debug_log(self,
+                        log_message: str):
+
         if self.debug:
             print('[WatchTowerHandler DEBUG] ' + log_message)
 
-    def format_record(self, record):
+    def format_record(self,
+                      record):
 
         self.write_debug_log('format_record() called')
         record.dev = self.dev
         return self.format(record)
 
 
-    def _wt_worker(self, payload=None):
+    def _wt_worker(self,
+                   payload: (str, None) = None):
+
         self.write_debug_log("_wt_worker() called")
         if self.flush_interval > 0:
             # Stop the timer. Happens automatically if this is called
             # via the timer, does not if invoked by force_flush()
             self.timer.cancel()
             self.processing_payload = True
             queue_is_empty = self.empty_queue()
@@ -278,17 +304,19 @@
                     timer_interval = self.alt_flush_interval
 
                 self.write_debug_log("Resetting timer thread")
                 self.timer = Timer(timer_interval, self._wt_worker)
                 self.timer.daemon = True  # Auto-kill thread if main process exits
                 self.timer.start()
                 self.write_debug_log("Timer thread scheduled")
+
         self.processing_payload = False
 
     def empty_queue(self):
+
         if len(self.queue) == 0:
             self.write_debug_log("Queue was empty")
             return True
 
         self.write_debug_log("Recursing through queue")
         if self.SIGTERM:
             self.log_payload += ','.join(self.queue)
@@ -301,19 +329,21 @@
             self.log_payload += ','.join(self.queue[:count])
             del self.queue[:count]
         self.write_debug_log("Queue task completed")
 
         return len(self.queue) > 0
 
     def force_flush(self):
+
         self.write_debug_log("Force flush requested")
         self._wt_worker()
         self.wait_until_empty()  # guarantees queue is emptied
 
     def shutdown(self):
+
         self.write_debug_log("Immediate shutdown requested")
 
         # Only initiate shutdown once
         if self.SIGTERM:
             return
 
         self.write_debug_log("Setting instance SIGTERM=True")
@@ -324,19 +354,32 @@
 
         self.write_debug_log("Starting up the final run of the worker thread before shutdown")
         # Send the remaining items that might be sitting in queue.
         self._wt_worker()
         self.wait_until_empty()  # guarantees queue is emptied before exit
 
     def wait_until_empty(self):
+
         self.write_debug_log("Waiting until queue empty")
         while len(self.queue) > 0 or self.processing_payload:
             self.write_debug_log("Current queue size: " + str(len(self.queue)))
             time.sleep(self.alt_flush_interval)
 
     @property
     def alt_flush_interval(self):
+
         return min(1.0, self.flush_interval / 2)
 
     @property
     def user_agent(self):
-        return 'watchtower-logging-python/{version}'.format(version=self.version)
+
+        return 'watchtower-logging-python/{version}'.format(version=self.version)
+
+    @property
+    def url(self):
+
+        return self.build_endpoint(host=self.host)
+
+    @property
+    def fallback_url(self):
+
+        return self.build_endpoint(host=self.fallback_host)
```

### Comparing `watchtower_logging-0.6.2/watchtower_logging/watchtower_logging.py` & `watchtower_logging-0.6.3/watchtower_logging/watchtower_logging.py`

 * *Files identical despite different names*

