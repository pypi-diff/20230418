# Comparing `tmp/afscgap-0.0.8.tar.gz` & `tmp/afscgap-0.0.9.tar.gz`

## Comparing `afscgap-0.0.8.tar` & `afscgap-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-0.0.8/.gitattributes
--rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-0.0.8/CONDUCT.md
--rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-0.0.8/CONTRIBUTING.md
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-0.0.8/gruntfile.js
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-0.0.8/install_browser.sh
--rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-0.0.8/package-lock.json
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-0.0.8/package.json
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-0.0.8/setup.cfg
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/README.md
--rw-r--r--   0        0        0    58952 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/__init__.py
--rw-r--r--   0        0        0    42875 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/client.py
--rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/convert.py
--rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/cursor.py
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/http.py
--rw-r--r--   0        0        0    36994 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/inference.py
--rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/model.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/py.typed
--rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/query_util.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-0.0.8/afscgap/typesdef.py
--rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/README.md
--rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/architecture.drawio
--rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/library.png
--rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/paper.bib
--rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/paper.md
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/preview_paper.sh
--rw-r--r--   0        0        0   176314 2020-02-02 00:00:00.000000 afscgap-0.0.8/inst/viz.png
--rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 afscgap-0.0.8/.gitignore
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-0.0.8/LICENSE.md
--rw-r--r--   0        0        0    43240 2020-02-02 00:00:00.000000 afscgap-0.0.8/README.md
--rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 afscgap-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    44624 2020-02-02 00:00:00.000000 afscgap-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 afscgap-0.0.9/.gitattributes
+-rw-r--r--   0        0        0     2780 2020-02-02 00:00:00.000000 afscgap-0.0.9/CONDUCT.md
+-rw-r--r--   0        0        0     7583 2020-02-02 00:00:00.000000 afscgap-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 afscgap-0.0.9/gruntfile.js
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 afscgap-0.0.9/install_browser.sh
+-rw-r--r--   0        0        0   178220 2020-02-02 00:00:00.000000 afscgap-0.0.9/package-lock.json
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 afscgap-0.0.9/package.json
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 afscgap-0.0.9/setup.cfg
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/README.md
+-rw-r--r--   0        0        0    58952 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/__init__.py
+-rw-r--r--   0        0        0    42895 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/client.py
+-rw-r--r--   0        0        0     9440 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/convert.py
+-rw-r--r--   0        0        0     5132 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/cursor.py
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/http_util.py
+-rw-r--r--   0        0        0    37009 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/inference.py
+-rw-r--r--   0        0        0    37762 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/model.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/py.typed
+-rw-r--r--   0        0        0     2914 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/query_util.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 afscgap-0.0.9/afscgap/typesdef.py
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/README.md
+-rw-r--r--   0        0        0    13278 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/architecture.drawio
+-rw-r--r--   0        0        0    87762 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/library.png
+-rw-r--r--   0        0        0     5648 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/paper.bib
+-rw-r--r--   0        0        0     7867 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/paper.md
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/preview_paper.sh
+-rw-r--r--   0        0        0   176314 2020-02-02 00:00:00.000000 afscgap-0.0.9/inst/viz.png
+-rw-r--r--   0        0        0      240 2020-02-02 00:00:00.000000 afscgap-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 afscgap-0.0.9/LICENSE.md
+-rw-r--r--   0        0        0    43240 2020-02-02 00:00:00.000000 afscgap-0.0.9/README.md
+-rw-r--r--   0        0        0     1401 2020-02-02 00:00:00.000000 afscgap-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0    44624 2020-02-02 00:00:00.000000 afscgap-0.0.9/PKG-INFO
```

### Comparing `afscgap-0.0.8/CONDUCT.md` & `afscgap-0.0.9/CONDUCT.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/CONTRIBUTING.md` & `afscgap-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/gruntfile.js` & `afscgap-0.0.9/gruntfile.js`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/package-lock.json` & `afscgap-0.0.9/package-lock.json`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/__init__.py` & `afscgap-0.0.9/afscgap/__init__.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/client.py` & `afscgap-0.0.9/afscgap/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import copy
 import json
 import queue
 import typing
 
 import afscgap.convert
 import afscgap.cursor
-import afscgap.http
+import afscgap.http_util
 import afscgap.model
 import afscgap.query_util
 
 from afscgap.typesdef import OPT_FLOAT
 from afscgap.typesdef import OPT_INT
 from afscgap.typesdef import OPT_REQUESTOR
 from afscgap.typesdef import OPT_STR
@@ -122,15 +122,15 @@
         self._queue: queue.Queue[afscgap.model.Record] = queue.Queue()
         self._invalid_queue: queue.Queue[dict] = queue.Queue()
         self._done = False
 
         if requestor:
             self._request_strategy = requestor
         else:
-            self._request_strategy = afscgap.http.build_requestor()
+            self._request_strategy = afscgap.http_util.build_requestor()
 
         self._next_url = self.get_page_url()
 
     def get_base_url(self) -> str:
         """Get the URL at which the first page of query results can be found.
 
         Returns:
@@ -212,15 +212,15 @@
         Returns:
             Results from the page which, regardless of ignore_invalid, may
             contain a mixture of complete and incomplete records.
         """
         url = self.get_page_url(offset, limit)
 
         result = self._request_strategy(url)
-        afscgap.http.check_result(result)
+        afscgap.http_util.check_result(result)
 
         result_parsed = result.json()
         items_raw = result_parsed['items']
 
         parsed_maybe = map(try_parse, items_raw)
         parsed_with_none = map(lambda x: x.get_parsed(), parsed_maybe)
 
@@ -289,15 +289,15 @@
         into the waiting queues and updating the next url / done internal
         state in the process.
         """
         if self._done:
             return
 
         result = self._request_strategy(self._next_url)
-        afscgap.http.check_result(result)
+        afscgap.http_util.check_result(result)
 
         result_parsed = result.json()
 
         items_raw = result_parsed['items']
 
         items_parsed = map(try_parse, items_raw)
```

### Comparing `afscgap-0.0.8/afscgap/convert.py` & `afscgap-0.0.9/afscgap/convert.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/cursor.py` & `afscgap-0.0.9/afscgap/cursor.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/http.py` & `afscgap-0.0.9/afscgap/http_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/inference.py` & `afscgap-0.0.9/afscgap/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import itertools
 import queue
 import typing
 
 import afscgap.convert
 import afscgap.client
 import afscgap.cursor
-import afscgap.http
+import afscgap.http_util
 import afscgap.model
 import afscgap.query_util
 
 from afscgap.typesdef import OPT_FLOAT
 from afscgap.typesdef import OPT_INT
 from afscgap.typesdef import OPT_REQUESTOR
 from afscgap.typesdef import OPT_STR
@@ -157,18 +157,18 @@
     """
     if hauls_url is None:
         hauls_url = DEFAULT_HAULS_URL
 
     params_checker = build_params_checker(params)
 
     if requestor is None:
-        requestor = afscgap.http.build_requestor()
+        requestor = afscgap.http_util.build_requestor()
 
     response = requestor(hauls_url)
-    afscgap.http.check_result(response)
+    afscgap.http_util.check_result(response)
 
     response.encoding = 'utf-8'
     response_io = io.StringIO(response.text, newline='')
 
     response_rows = csv.DictReader(response_io)
     response_hauls = map(parse_haul, response_rows)
     response_hauls_filtered = filter(params_checker, response_hauls)
```

### Comparing `afscgap-0.0.8/afscgap/model.py` & `afscgap-0.0.9/afscgap/model.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/query_util.py` & `afscgap-0.0.9/afscgap/query_util.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/afscgap/typesdef.py` & `afscgap-0.0.9/afscgap/typesdef.py`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/inst/README.md` & `afscgap-0.0.9/inst/README.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/inst/architecture.drawio` & `afscgap-0.0.9/inst/architecture.drawio`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/inst/library.png` & `afscgap-0.0.9/inst/library.png`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/inst/paper.bib` & `afscgap-0.0.9/inst/paper.bib`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/inst/paper.md` & `afscgap-0.0.9/inst/paper.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/inst/viz.png` & `afscgap-0.0.9/inst/viz.png`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/LICENSE.md` & `afscgap-0.0.9/LICENSE.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/README.md` & `afscgap-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `afscgap-0.0.8/pyproject.toml` & `afscgap-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "afscgap"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="A Samuel Pottinger", email="sam.pottinger@berkeley.edu" },
 ]
 description = "Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `afscgap-0.0.8/PKG-INFO` & `afscgap-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afscgap
-Version: 0.0.8
+Version: 0.0.9
 Summary: Tools for interacting with the public bottom trawl surveys data from the NOAA AFSC GAP.
 Project-URL: Homepage, https://pyafscgap.org
 Project-URL: Documentation, https://pyafscgap.org/devdocs/afscgap.html
 Project-URL: Source, https://github.com/SchmidtDSE/afscgap
 Project-URL: Issue Tracker, https://github.com/SchmidtDSE/afscgap/issues
 Project-URL: Changelog, https://github.com/SchmidtDSE/afscgap#version-history
 Author-email: A Samuel Pottinger <sam.pottinger@berkeley.edu>
```

