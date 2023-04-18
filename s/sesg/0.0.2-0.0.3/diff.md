# Comparing `tmp/sesg-0.0.2.tar.gz` & `tmp/sesg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sesg-0.0.2.tar", max compression
+gzip compressed data, was "sesg-0.0.3.tar", max compression
```

## Comparing `sesg-0.0.2.tar` & `sesg-0.0.3.tar`

### file list

```diff
@@ -1,11 +1,14 @@
--rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.2/LICENSE
--rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.2/README.md
--rw-r--r--   0        0        0     3014 2023-04-17 21:18:26.339911 sesg-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.2/src/sesg/__init__.py
--rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.2/src/sesg/graph.py
--rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.2/src/sesg/metrics.py
--rw-r--r--   0        0        0    16870 2023-04-16 16:49:33.237266 sesg-0.0.2/src/sesg/scopus_client.py
--rw-r--r--   0        0        0    13843 2023-04-17 14:58:16.710757 sesg-0.0.2/src/sesg/search_string.py
--rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.2/src/sesg/snowballing.py
--rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.2/src/sesg/topic_extraction.py
--rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    35148 2023-04-17 17:41:20.988197 sesg-0.0.3/LICENSE
+-rw-r--r--   0        0        0      478 2023-04-17 17:33:48.160350 sesg-0.0.3/README.md
+-rw-r--r--   0        0        0     3014 2023-04-18 04:45:02.663654 sesg-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-04-17 15:18:13.051151 sesg-0.0.3/src/sesg/__init__.py
+-rw-r--r--   0        0        0     8127 2023-04-17 21:13:02.702530 sesg-0.0.3/src/sesg/graph.py
+-rw-r--r--   0        0        0     6744 2023-04-17 14:56:33.924330 sesg-0.0.3/src/sesg/metrics.py
+-rw-r--r--   0        0        0      173 2023-04-18 04:38:35.955358 sesg-0.0.3/src/sesg/scopus/__init__.py
+-rw-r--r--   0        0        0     7628 2023-04-18 04:43:47.784342 sesg-0.0.3/src/sesg/scopus/api.py
+-rw-r--r--   0        0        0     5914 2023-04-18 04:39:34.710767 sesg-0.0.3/src/sesg/scopus/client.py
+-rw-r--r--   0        0        0    16416 2023-04-18 03:04:34.582222 sesg-0.0.3/src/sesg/scopus_client.py
+-rw-r--r--   0        0        0    13843 2023-04-18 03:31:52.519891 sesg-0.0.3/src/sesg/search_string.py
+-rw-r--r--   0        0        0     7659 2023-04-17 15:00:57.692606 sesg-0.0.3/src/sesg/snowballing.py
+-rw-r--r--   0        0        0     5056 2023-04-16 16:49:33.237266 sesg-0.0.3/src/sesg/topic_extraction.py
+-rw-r--r--   0        0        0     1829 1970-01-01 00:00:00.000000 sesg-0.0.3/PKG-INFO
```

### Comparing `sesg-0.0.2/LICENSE` & `sesg-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sesg-0.0.2/pyproject.toml` & `sesg-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sesg"
-version = "0.0.2"
+version = "0.0.3"
 description = "SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string."
 authors = ["Demetrius Panovitch <demetrius.mp789@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
   {include = "sesg", from = "src"}
 ]
```

### Comparing `sesg-0.0.2/src/sesg/graph.py` & `sesg-0.0.3/src/sesg/graph.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.2/src/sesg/metrics.py` & `sesg-0.0.3/src/sesg/metrics.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.2/src/sesg/scopus_client.py` & `sesg-0.0.3/src/sesg/scopus_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -295,22 +295,14 @@
 
 
 class ScopusClient:
     """A Scopus API Client that redoes requests if it takes longer than a given timeout,
     and automatically rotates API keys once one of them expires.
     """  # noqa: E501
 
-    __slots__ = (
-        "__timeout",
-        "__api_keys",
-        "__timeout_attempts",
-        "__ResultsIterator",
-        "_private_current_api_key_index",
-    )
-
     __timeout: float
     __api_keys: List[str]
     __timeout_attempts: int
 
     _private_current_api_key_index: int
 
     @dataclass
@@ -338,25 +330,14 @@
     ) -> None:
         self.__timeout = timeout
         self.__api_keys = api_keys
         self.__timeout_attempts = timeout_attempts
         self._private_current_api_key_index = 0
 
         class ResultsIterator:
-            __slots__ = (
-                "timeout",
-                "api_keys",
-                "query",
-                "timeout_attempts",
-                "scopus_client",
-                "current_page",
-                "iterator",
-                "current_attempt",
-            )
-
             timeout: float
             api_keys: List[str]
             query: str
             timeout_attempts: int
             scopus_client: ScopusClient
 
             iterator: AsyncIterator[_ScopusSearchResults]
```

### Comparing `sesg-0.0.2/src/sesg/search_string.py` & `sesg-0.0.3/src/sesg/search_string.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.2/src/sesg/snowballing.py` & `sesg-0.0.3/src/sesg/snowballing.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.2/src/sesg/topic_extraction.py` & `sesg-0.0.3/src/sesg/topic_extraction.py`

 * *Files identical despite different names*

### Comparing `sesg-0.0.2/PKG-INFO` & `sesg-0.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sesg
-Version: 0.0.2
+Version: 0.0.3
 Summary: SeSG is a tool developed to help Systematic Literature Review researchers, specifically at the step of building a search string.
 License: GPL-3.0-only
 Author: Demetrius Panovitch
 Author-email: demetrius.mp789@gmail.com
 Requires-Python: >=3.10,<3.11
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

