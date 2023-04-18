# Comparing `tmp/strangeworks_vqe-0.1.1.tar.gz` & `tmp/strangeworks_vqe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strangeworks_vqe-0.1.1.tar", max compression
+gzip compressed data, was "strangeworks_vqe-0.1.2.tar", max compression
```

## Comparing `strangeworks_vqe-0.1.1.tar` & `strangeworks_vqe-0.1.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       19 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/README.md
--rw-r--r--   0        0        0      659 2023-04-18 10:47:24.411928 strangeworks_vqe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    11197 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/strangeworks_vqe/sdk.py
--rw-r--r--   0        0        0      691 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/strangeworks_vqe/serializer.py
--rw-r--r--   0        0        0     5677 2023-04-18 10:47:10.919855 strangeworks_vqe-0.1.1/strangeworks_vqe/utils.py
--rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       19 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/README.md
+-rw-r--r--   0        0        0      659 2023-04-18 13:22:04.374911 strangeworks_vqe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    11128 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/strangeworks_vqe/sdk.py
+-rw-r--r--   0        0        0      691 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/strangeworks_vqe/serializer.py
+-rw-r--r--   0        0        0     5677 2023-04-18 13:21:49.502083 strangeworks_vqe-0.1.2/strangeworks_vqe/utils.py
+-rw-r--r--   0        0        0      673 1970-01-01 00:00:00.000000 strangeworks_vqe-0.1.2/PKG-INFO
```

### Comparing `strangeworks_vqe-0.1.1/pyproject.toml` & `strangeworks_vqe-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "strangeworks-vqe"
-version = "0.1.1"
+version = "0.1.2"
 description = "Extension to strangeworks sdk to allow user to run qaoa service"
 authors = ["SFlann <stuart@strangeworks.com>"]
 readme = "README.md"
 packages = [{include = "strangeworks_vqe"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `strangeworks_vqe-0.1.1/strangeworks_vqe/sdk.py` & `strangeworks_vqe-0.1.2/strangeworks_vqe/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,16 +222,14 @@
         if result_url:
             result_file = strangeworks.download_job_files([result_url])[0]
         else:
             result = strangeworks.execute(
                 self.rsc, {"payload": {"job_slug": job_slug}}, "result"
             )
 
-            result = serializer.pickle_deserializer(result, "json")
-
             if result.strip().upper() == "COMPLETED":
                 result_url = strangeworks.execute(
                     self.rsc, {"payload": {"job_slug": job_slug}}, "get_results_url"
                 )
                 if result_url:
                     result_file = strangeworks.download_job_files([result_url])[0]
                 else:
```

### Comparing `strangeworks_vqe-0.1.1/strangeworks_vqe/serializer.py` & `strangeworks_vqe-0.1.2/strangeworks_vqe/serializer.py`

 * *Files identical despite different names*

### Comparing `strangeworks_vqe-0.1.1/strangeworks_vqe/utils.py` & `strangeworks_vqe-0.1.2/strangeworks_vqe/utils.py`

 * *Files identical despite different names*

### Comparing `strangeworks_vqe-0.1.1/PKG-INFO` & `strangeworks_vqe-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strangeworks-vqe
-Version: 0.1.1
+Version: 0.1.2
 Summary: Extension to strangeworks sdk to allow user to run qaoa service
 Author: SFlann
 Author-email: stuart@strangeworks.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

