# Comparing `tmp/searchkit-0.2.2.post1.tar.gz` & `tmp/searchkit-0.2.2.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "searchkit-0.2.2.post1.tar", last modified: Tue Apr 18 13:51:07 2023, max compression
+gzip compressed data, was "searchkit-0.2.2.post2.tar", last modified: Tue Apr 18 16:15:14 2023, max compression
```

## Comparing `searchkit-0.2.2.post1.tar` & `searchkit-0.2.2.post2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 13:51:07.523371 searchkit-0.2.2.post1/
--rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.2.post1/LICENSE
--rw-rw-r--   0 user1     (1000) user1     (1000)     3111 2023-04-18 13:51:07.523371 searchkit-0.2.2.post1/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.2.post1/README.md
--rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.2.post1/pyproject.toml
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 13:51:07.519371 searchkit-0.2.2.post1/searchkit/
--rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.2.post1/searchkit/__init__.py
--rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.2.post1/searchkit/constraints.py
--rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.2.post1/searchkit/log.py
--rwxrwxr-x   0 user1     (1000) user1     (1000)    44352 2023-04-18 13:42:32.000000 searchkit-0.2.2.post1/searchkit/search.py
--rw-rw-r--   0 user1     (1000) user1     (1000)     4743 2023-04-13 20:08:39.000000 searchkit-0.2.2.post1/searchkit/utils.py
-drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 13:51:07.523371 searchkit-0.2.2.post1/searchkit.egg-info/
--rw-rw-r--   0 user1     (1000) user1     (1000)     3111 2023-04-18 13:51:07.000000 searchkit-0.2.2.post1/searchkit.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-18 13:51:07.000000 searchkit-0.2.2.post1/searchkit.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-18 13:51:07.000000 searchkit-0.2.2.post1/searchkit.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-18 13:51:07.000000 searchkit-0.2.2.post1/searchkit.egg-info/requires.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-18 13:51:07.000000 searchkit-0.2.2.post1/searchkit.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-18 13:51:07.523371 searchkit-0.2.2.post1/setup.cfg
--rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.2.post1/setup.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/
+-rw-rw-r--   0 user1     (1000) user1     (1000)    11357 2023-01-10 10:19:33.000000 searchkit-0.2.2.post2/LICENSE
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3111 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)     2897 2023-04-12 11:04:01.000000 searchkit-0.2.2.post2/README.md
+-rw-rw-r--   0 user1     (1000) user1     (1000)      734 2023-04-17 12:11:23.000000 searchkit-0.2.2.post2/pyproject.toml
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/searchkit/
+-rw-rw-r--   0 user1     (1000) user1     (1000)      121 2023-04-18 13:47:52.000000 searchkit-0.2.2.post2/searchkit/__init__.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)    22833 2023-04-11 08:53:59.000000 searchkit-0.2.2.post2/searchkit/constraints.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)      277 2023-01-29 21:35:16.000000 searchkit-0.2.2.post2/searchkit/log.py
+-rwxrwxr-x   0 user1     (1000) user1     (1000)    44374 2023-04-18 16:13:04.000000 searchkit-0.2.2.post2/searchkit/search.py
+-rw-rw-r--   0 user1     (1000) user1     (1000)     4743 2023-04-13 20:08:39.000000 searchkit-0.2.2.post2/searchkit/utils.py
+drwxrwxr-x   0 user1     (1000) user1     (1000)        0 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/searchkit.egg-info/
+-rw-rw-r--   0 user1     (1000) user1     (1000)     3111 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1000) user1     (1000)      308 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)        1 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       57 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       10 2023-04-18 16:15:14.000000 searchkit-0.2.2.post2/searchkit.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1000) user1     (1000)       38 2023-04-18 16:15:14.192248 searchkit-0.2.2.post2/setup.cfg
+-rw-rw-r--   0 user1     (1000) user1     (1000)       54 2023-01-29 21:35:16.000000 searchkit-0.2.2.post2/setup.py
```

### Comparing `searchkit-0.2.2.post1/LICENSE` & `searchkit-0.2.2.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post1/PKG-INFO` & `searchkit-0.2.2.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.2.post1
+Version: 0.2.2.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

### Comparing `searchkit-0.2.2.post1/README.md` & `searchkit-0.2.2.post2/README.md`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post1/pyproject.toml` & `searchkit-0.2.2.post2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post1/searchkit/constraints.py` & `searchkit-0.2.2.post2/searchkit/constraints.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post1/searchkit/search.py` & `searchkit-0.2.2.post2/searchkit/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -226,15 +226,15 @@
         """
         @param index: index of this result
         @param value: value of this result
         @param field_info: ResultFieldInfo object
         """
         self.index = index
         self.value = value
-        if field_info:
+        if field_info and value is not None:
             self.name = field_info.index_to_name(index - 1)
             self.value = field_info.ensure_type(self.name, value)
         else:
             self.name = None
 
 
 class ResultFieldInfo(UserDict):
```

### Comparing `searchkit-0.2.2.post1/searchkit/utils.py` & `searchkit-0.2.2.post2/searchkit/utils.py`

 * *Files identical despite different names*

### Comparing `searchkit-0.2.2.post1/searchkit.egg-info/PKG-INFO` & `searchkit-0.2.2.post2/searchkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: searchkit
-Version: 0.2.2.post1
+Version: 0.2.2.post2
 Summary: Python library providing tools to search files in parallel.
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Searchkit
```

