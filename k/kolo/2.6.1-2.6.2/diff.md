# Comparing `tmp/kolo-2.6.1.tar.gz` & `tmp/kolo-2.6.2.tar.gz`

## Comparing `kolo-2.6.1.tar` & `kolo-2.6.2.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.6.1/rust/Cargo.toml
--rw-rw-r--   0     1000     1001       54 2023-04-18 10:49:25.000000 kolo-2.6.1/rust/build.rs
--rw-rw-r--   0     1000     1001    35236 2023-04-18 10:49:25.000000 kolo-2.6.1/rust/src/lib.rs
--rw-rw-r--   0     1000     1001     2106 2023-04-18 10:49:25.000000 kolo-2.6.1/pyproject.toml
--rw-rw-r--   0     1000     1001    11199 2023-04-18 10:50:04.000000 kolo-2.6.1/rust/Cargo.lock
--rw-rw-r--   0     1000     1001     3681 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/serialize.py
--rw-rw-r--   0     1000     1001     3161 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/requests.py
--rw-rw-r--   0     1000     1001      348 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/kolo.py
--rw-rw-r--   0     1000     1001     1322 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/unittest.py
--rw-rw-r--   0     1000     1001     4355 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/exception.py
--rw-rw-r--   0     1000     1001     1457 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/pytest.py
--rw-rw-r--   0     1000     1001     4345 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/sql.py
--rw-rw-r--   0     1000     1001     2262 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/celery.py
--rw-rw-r--   0     1000     1001     3157 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/urllib.py
--rw-rw-r--   0     1000     1001     4055 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/django.py
--rw-rw-r--   0     1000     1001     1778 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/logging.py
--rw-rw-r--   0     1000     1001     5180 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/core.py
--rw-rw-r--   0     1000     1001      809 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/attrs.py
--rw-rw-r--   0     1000     1001     3707 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/urllib3.py
--rw-rw-r--   0     1000     1001      141 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/pypy.py
--rw-rw-r--   0     1000     1001        0 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/__init__.py
--rw-rw-r--   0     1000     1001     2921 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/filters/huey.py
--rw-rw-r--   0     1000     1001     2640 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/middleware.py
--rw-rw-r--   0     1000     1001      951 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/templates/django_request_test.py.j2
--rw-rw-r--   0     1000     1001    13710 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/profiler.py
--rw-rw-r--   0     1000     1001      169 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/version.py
--rw-rw-r--   0     1000     1001     3210 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/generate_tests.py
--rw-rw-r--   0     1000     1001     6765 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/__main__.py
--rw-rw-r--   0     1000     1001     3556 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/db.py
--rw-rw-r--   0     1000     1001      473 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/git.py
--rw-rw-r--   0     1000     1001      228 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/pytest_plugin.py
--rw-rw-r--   0     1000     1001      108 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/__init__.py
--rw-rw-r--   0     1000     1001     2881 2023-04-18 10:49:25.000000 kolo-2.6.1/src/kolo/config.py
--rw-rw-r--   0     1000     1001      228 2023-04-18 10:49:25.000000 kolo-2.6.1/README.md
--rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 kolo-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 kolo-2.6.2/rust/Cargo.toml
+-rw-rw-r--   0     1000     1001       54 2023-04-18 16:24:50.000000 kolo-2.6.2/rust/build.rs
+-rw-rw-r--   0     1000     1001    35236 2023-04-18 16:24:50.000000 kolo-2.6.2/rust/src/lib.rs
+-rw-rw-r--   0     1000     1001     2106 2023-04-18 16:24:50.000000 kolo-2.6.2/pyproject.toml
+-rw-rw-r--   0     1000     1001    11199 2023-04-18 16:25:15.000000 kolo-2.6.2/rust/Cargo.lock
+-rw-rw-r--   0     1000     1001     3681 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/serialize.py
+-rw-rw-r--   0     1000     1001     3400 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/requests.py
+-rw-rw-r--   0     1000     1001      348 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/kolo.py
+-rw-rw-r--   0     1000     1001     1322 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/unittest.py
+-rw-rw-r--   0     1000     1001     4355 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/exception.py
+-rw-rw-r--   0     1000     1001     1457 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/pytest.py
+-rw-rw-r--   0     1000     1001     4345 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/sql.py
+-rw-rw-r--   0     1000     1001     2262 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/celery.py
+-rw-rw-r--   0     1000     1001     3157 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/urllib.py
+-rw-rw-r--   0     1000     1001     4055 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/django.py
+-rw-rw-r--   0     1000     1001     1778 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/logging.py
+-rw-rw-r--   0     1000     1001     5180 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/core.py
+-rw-rw-r--   0     1000     1001      809 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/attrs.py
+-rw-rw-r--   0     1000     1001     3707 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/urllib3.py
+-rw-rw-r--   0     1000     1001      141 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/pypy.py
+-rw-rw-r--   0     1000     1001        0 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/__init__.py
+-rw-rw-r--   0     1000     1001     2921 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/filters/huey.py
+-rw-rw-r--   0     1000     1001     2640 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/middleware.py
+-rw-rw-r--   0     1000     1001      951 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/templates/django_request_test.py.j2
+-rw-rw-r--   0     1000     1001    13710 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/profiler.py
+-rw-rw-r--   0     1000     1001      169 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/version.py
+-rw-rw-r--   0     1000     1001     3210 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/generate_tests.py
+-rw-rw-r--   0     1000     1001     6765 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/__main__.py
+-rw-rw-r--   0     1000     1001     3556 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/db.py
+-rw-rw-r--   0     1000     1001      473 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/git.py
+-rw-rw-r--   0     1000     1001      228 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/pytest_plugin.py
+-rw-rw-r--   0     1000     1001      108 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/__init__.py
+-rw-rw-r--   0     1000     1001     2881 2023-04-18 16:24:50.000000 kolo-2.6.2/src/kolo/config.py
+-rw-rw-r--   0     1000     1001      228 2023-04-18 16:24:50.000000 kolo-2.6.2/README.md
+-rw-r--r--   0        0        0     2221 1970-01-01 00:00:00.000000 kolo-2.6.2/PKG-INFO
```

### Comparing `kolo-2.6.1/rust/Cargo.toml` & `kolo-2.6.2/rust/Cargo.toml`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/rust/src/lib.rs` & `kolo-2.6.2/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/pyproject.toml` & `kolo-2.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["maturin>=0.14,<0.15"]
 build-backend = "maturin"
 
 [project]
 name = "kolo"
-version = "2.6.1"
+version = "2.6.2"
 description = "See everything happening in your running Django app"
 readme = "README.md"
 authors = [
     {name = "Wilhelm Klopp", email = "team@kolo.app"},
     {name = "Lily Foote", email = "lily@kolo.app"},
 ]
 urls.Homepage = "https://kolo.app"
```

### Comparing `kolo-2.6.1/rust/Cargo.lock` & `kolo-2.6.2/rust/Cargo.lock`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/serialize.py` & `kolo-2.6.2/src/kolo/serialize.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/requests.py` & `kolo-2.6.2/src/kolo/filters/requests.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,20 @@
         method_and_full_url: str
         subtype: Literal["requests"]
         timestamp: float | str
         type: Literal["outbound_http_request"]
         url: str
 
     class ApiResponse(TypedDict):
-        body: str
+        body: str | None
         frame_id: str
-        headers: Dict[str, str]
+        headers: Dict[str, str] | None
         method: str
         method_and_full_url: str
-        status_code: int
+        status_code: int | None
         subtype: Literal["requests"]
         timestamp: float | str
         type: Literal["outbound_http_response"]
         url: str
 
 
 class ApiRequestFilter:
@@ -86,20 +86,29 @@
 
         response = arg
         if TYPE_CHECKING:
             from requests.models import Response
 
             assert isinstance(response, Response)
 
+        if response is None:
+            body = None
+            headers = None
+            status_code = None
+        else:
+            body = response.text
+            headers = dict(response.headers)
+            status_code = response.status_code
+
         api_response: ApiResponse = {
-            "body": response.text,
+            "body": body,
             "frame_id": self._frame_ids[id(frame)],
-            "headers": dict(response.headers),
+            "headers": headers,
             "method": request.method,
             "method_and_full_url": method_and_url,
-            "status_code": response.status_code,
+            "status_code": status_code,
             "subtype": "requests",
             "timestamp": timestamp,
             "type": "outbound_http_response",
             "url": request.url,
         }
         return api_response
```

### Comparing `kolo-2.6.1/src/kolo/filters/unittest.py` & `kolo-2.6.2/src/kolo/filters/unittest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/exception.py` & `kolo-2.6.2/src/kolo/filters/exception.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/pytest.py` & `kolo-2.6.2/src/kolo/filters/pytest.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/sql.py` & `kolo-2.6.2/src/kolo/filters/sql.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/celery.py` & `kolo-2.6.2/src/kolo/filters/celery.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/urllib.py` & `kolo-2.6.2/src/kolo/filters/urllib.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/django.py` & `kolo-2.6.2/src/kolo/filters/django.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/logging.py` & `kolo-2.6.2/src/kolo/filters/logging.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/core.py` & `kolo-2.6.2/src/kolo/filters/core.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/attrs.py` & `kolo-2.6.2/src/kolo/filters/attrs.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/urllib3.py` & `kolo-2.6.2/src/kolo/filters/urllib3.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/filters/huey.py` & `kolo-2.6.2/src/kolo/filters/huey.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/middleware.py` & `kolo-2.6.2/src/kolo/middleware.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/templates/django_request_test.py.j2` & `kolo-2.6.2/src/kolo/templates/django_request_test.py.j2`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/profiler.py` & `kolo-2.6.2/src/kolo/profiler.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/generate_tests.py` & `kolo-2.6.2/src/kolo/generate_tests.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/__main__.py` & `kolo-2.6.2/src/kolo/__main__.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/db.py` & `kolo-2.6.2/src/kolo/db.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/src/kolo/config.py` & `kolo-2.6.2/src/kolo/config.py`

 * *Files identical despite different names*

### Comparing `kolo-2.6.1/PKG-INFO` & `kolo-2.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kolo
-Version: 2.6.1
+Version: 2.6.2
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
@@ -35,17 +35,17 @@
 Requires-Dist: jinja2>=3.0.0; extra == 'test_generation'
 Provides-Extra: test_generation
 Summary: See everything happening in your running Django app
 Author-email: Wilhelm Klopp <team@kolo.app>, Lily Foote <lily@kolo.app>
 License: © Kolo
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: Changelog, https://docs.kolo.app/en/latest/python-changelog.html
 Project-URL: Repository, https://github.com/kolofordjango/kolo
 Project-URL: Homepage, https://kolo.app
+Project-URL: Changelog, https://docs.kolo.app/en/latest/python-changelog.html
 
 # Kolo
 
 See everything happening in your running Django app
 
 More information: https://kolo.app
```

