# Comparing `tmp/sesg-0.0.4.tar.gz` & `tmp/sesg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.4.tar", max compression
+gzip compressed data, was "sesg-0.0.5.tar", max compression
```

## Comparing `sesg-0.0.4.tar` & `sesg-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.4/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.4/README.md
--rw-r--r--   0        0        0     2779 2023-04-18 04:54:00.660082 sesg-0.0.4/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.4/src/sesg/__init__.py
--rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.4/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.4/src/sesg/metrics.py
--rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.4/src/sesg/scopus/__init__.py
--rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.4/src/sesg/scopus/api.py
--rw-r--r--   0        0        0     5914 2023-04-18 04:39:34.710767 sesg-0.0.4/src/sesg/scopus/client.py
--rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.4/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.4/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.4/src/sesg/snowballing.py
--rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.4/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.5/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.5/README.md
+-rw-r--r--   0        0        0     2779 2023-04-18 12:05:47.964047 sesg-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.5/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.5/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.5/src/sesg/metrics.py
+-rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.5/src/sesg/scopus/__init__.py
+-rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.5/src/sesg/scopus/api.py
+-rw-r--r--   0        0        0     6080 2023-04-18 12:05:40.816197 sesg-0.0.5/src/sesg/scopus/client.py
+-rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.5/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.5/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.5/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.5/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.5/PKG-INFO
```

### Comparing `sesg-0.0.4/LICENSE` & `sesg-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/pyproject.toml` & `sesg-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.4"
+version = "0.0.5"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
```

### Comparing `sesg-0.0.4/src/sesg/graph.py` & `sesg-0.0.5/src/sesg/graph.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/src/sesg/metrics.py` & `sesg-0.0.5/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/src/sesg/scopus/api.py` & `sesg-0.0.5/src/sesg/scopus/api.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/src/sesg/scopus/client.py` & `sesg-0.0.5/src/sesg/scopus/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,19 @@
         return self.__current_query
 
     @property
     def api_keys(self) -> List[str]:
         """The Scopus API keys for this client."""
         return self.__api_keys
 
+    @property
+    def current_timeout_retry(self) -> int:
+        """The current retry for the same timed out request"""
+        return self.__current_timeout_retry
+
     def __restart_iterator_with_current_state(self):
         return api.search(
             api_key=self.current_api_key,
             query=self.__current_query,
             timeout=self.__timeout,
             page=self.__current_page,
         )
```

### Comparing `sesg-0.0.4/src/sesg/scopus_client.py` & `sesg-0.0.5/src/sesg/scopus_client.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/src/sesg/search_string.py` & `sesg-0.0.5/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/src/sesg/snowballing.py` & `sesg-0.0.5/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/src/sesg/topic_extraction.py` & `sesg-0.0.5/src/sesg/topic_extraction.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.4/PKG-INFO` & `sesg-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.4
+Version: 0.0.5
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

