# Comparing `tmp/serverless-sdk-0.4.1.tar.gz` & `tmp/serverless-sdk-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-0e7qlg8t/serverless-sdk-0.4.1.tar", last modified: Mon Apr 17 18:17:38 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-g14pvzlv/serverless-sdk-0.4.2.tar", last modified: Tue Apr 18 16:44:19 2023, max compression
```

## Comparing `serverless-sdk-0.4.1.tar` & `serverless-sdk-0.4.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     5283 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/sls_sdk/lib/warning_captured_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-17 18:17:38.000000 serverless-sdk-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    11489 2023-04-17 18:17:16.000000 serverless-sdk-0.4.1/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8136 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/sls_sdk/lib/warning_captured_event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 16:44:19.000000 serverless-sdk-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12051 2023-04-18 16:43:55.000000 serverless-sdk-0.4.2/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.1/PKG-INFO` & `serverless-sdk-0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.1/README.md` & `serverless-sdk-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/pyproject.toml` & `serverless-sdk-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 requires = [
     "setuptools>=65.6.3",
     "wheel>=0.38.4",
 ]
 
 [project]
 name = "serverless-sdk"
-version = "0.4.1"
+version = "0.4.2"
 description = "Serverless SDK for Python"
 readme = "README.md"
 authors = [{ name = "serverlessinc" }]
 requires-python = ">=3.7"
 dependencies = [
     "backports.cached-property", # included in Python >=3.8
     "blinker>=1.5",
```

### Comparing `serverless-sdk-0.4.1/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.2/serverless_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.1
+Version: 0.4.2
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
 Requires-Python: >=3.7
```

### Comparing `serverless-sdk-0.4.1/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.2/serverless_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/__init__.py` & `serverless-sdk-0.4.2/sls_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/exceptions.py` & `serverless-sdk-0.4.2/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.2/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/emitter.py` & `serverless-sdk-0.4.2/sls_sdk/lib/emitter.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/error.py` & `serverless-sdk-0.4.2/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.2/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/flask.py`

 * *Files 9% similar despite different names*

```diff
@@ -76,14 +76,19 @@
         except Exception as ex:
             report_error(ex)
 
     def _handle_request_started(self, sender, **extra):
         if not self._flask.request.endpoint:
             return
         try:
+            if self._flask.request.path:
+                del serverlessSdk.trace_spans.root.tags["aws.lambda.http_router.path"]
+                serverlessSdk.trace_spans.root.tags[
+                    "aws.lambda.http_router.path"
+                ] = self._flask.request.path
             span_name = ".".join(
                 [
                     "flask",
                     "route",
                     self.sanitize_span_name(self._flask.request.method),
                     self.sanitize_span_name(self._flask.request.endpoint),
                 ]
```

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/http.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.2/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/name.py` & `serverless-sdk-0.4.2/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.2/sls_sdk/lib/stack_trace_string.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.2/sls_sdk/lib/tags.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,14 +46,19 @@
 
     def set(self, key: str, value: ValidTags):
         try:
             self._set(key, value)
         except Exception as ex:
             report_error(ex)
 
+    def __delitem__(self, key: str):
+        with self._lock:
+            if key in self:
+                super().__delitem__(key)
+
     def __setitem__(self, key: str, value: ValidTags):
         self.set(key, value)
 
     def _update(
         self, mapping: Mapping[str, ValidTags], prefix: Optional[str] = None
     ) -> None:
         _prefix = ""
```

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.2/sls_sdk/lib/trace.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.2/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.2/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/tests/test_sdk.py` & `serverless-sdk-0.4.2/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.1/tests/test_thread_safety.py` & `serverless-sdk-0.4.2/tests/test_thread_safety.py`

 * *Files 9% similar despite different names*

```diff
@@ -285,14 +285,30 @@
         futures = [executor.submit(_set_tag_and_sleep, i) for i in range(parallelism)]
         for future in concurrent.futures.as_completed(futures):
             assert future.exception() is None
 
     # then
     assert len(sdk._custom_tags) == parallelism * scale
 
+    # given
+    def _del_tag_and_sleep(thread_index):
+        sleep(0.05)
+        for i in range(scale):
+            unique_value = thread_index * scale * 10 + i
+            del sdk._custom_tags[f"tag{unique_value}"]
+
+    # when
+    with concurrent.futures.ThreadPoolExecutor(max_workers=parallelism) as executor:
+        futures = [executor.submit(_del_tag_and_sleep, i) for i in range(parallelism)]
+        for future in concurrent.futures.as_completed(futures):
+            assert future.exception() is None
+
+    # then
+    assert len(sdk._custom_tags) == 0
+
 
 @pytest.mark.parametrize(
     "request_body,response_body",
     [
         (SMALL_REQUEST_PAYLOAD, SMALL_RESPONSE_PAYLOAD),
     ],
 )
```

