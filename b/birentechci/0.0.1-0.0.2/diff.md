# Comparing `tmp/birentechci-0.0.1.tar.gz` & `tmp/birentechci-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birentechci-0.0.1.tar", last modified: Tue Apr 18 08:23:48 2023, max compression
+gzip compressed data, was "birentechci-0.0.2.tar", last modified: Tue Apr 18 08:40:23 2023, max compression
```

## Comparing `birentechci-0.0.1.tar` & `birentechci-0.0.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 08:23:48.893905 birentechci-0.0.1/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.1/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/birentechci.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 08:23:48.000000 birentechci-0.0.1/birentechci.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      751 2023-04-18 08:23:48.000000 birentechci-0.0.1/birentechci.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 08:23:48.000000 birentechci-0.0.1/birentechci.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        4 2023-04-18 08:23:48.000000 birentechci-0.0.1/birentechci.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/sdk/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/sdk/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/sdk/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/sdk/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/sdk/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:23:48.893905 birentechci-0.0.1/sdk/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.1/sdk/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 08:23:48.893905 birentechci-0.0.1/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      683 2023-04-18 08:23:27.000000 birentechci-0.0.1/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 08:40:23.628498 birentechci-0.0.2/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.2/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/birentechci.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 08:40:23.000000 birentechci-0.0.2/birentechci.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      751 2023-04-18 08:40:23.000000 birentechci-0.0.2/birentechci.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 08:40:23.000000 birentechci-0.0.2/birentechci.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        4 2023-04-18 08:40:23.000000 birentechci-0.0.2/birentechci.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/sdk/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/sdk/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/sdk/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/sdk/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/run.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/sdk/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/test_hander_perf.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:40:23.628498 birentechci-0.0.2/sdk/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.2/sdk/utils/xml_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 08:40:23.628498 birentechci-0.0.2/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      683 2023-04-18 08:37:29.000000 birentechci-0.0.2/setup.py
```

### Comparing `birentechci-0.0.1/PKG-INFO` & `birentechci-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.1
+Version: 0.0.2
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birentechci-0.0.1/README.md` & `birentechci-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/birentechci.egg-info/PKG-INFO` & `birentechci-0.0.2/birentechci.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.1
+Version: 0.0.2
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birentechci-0.0.1/birentechci.egg-info/SOURCES.txt` & `birentechci-0.0.2/birentechci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/apis/build.py` & `birentechci-0.0.2/sdk/apis/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/apis/client.py` & `birentechci-0.0.2/sdk/apis/client.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/apis/pdu.py` & `birentechci-0.0.2/sdk/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/apis/perf.py` & `birentechci-0.0.2/sdk/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/apis/pr.py` & `birentechci-0.0.2/sdk/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/handles/build.py` & `birentechci-0.0.2/sdk/handles/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/handles/pdu.py` & `birentechci-0.0.2/sdk/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/handles/perf.py` & `birentechci-0.0.2/sdk/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/handles/pr.py` & `birentechci-0.0.2/sdk/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/run.py` & `birentechci-0.0.2/sdk/run.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/schemas/pull_request.py` & `birentechci-0.0.2/sdk/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/test_hander_perf.py` & `birentechci-0.0.2/sdk/test_hander_perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/utils/csv_utils.py` & `birentechci-0.0.2/sdk/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/sdk/utils/xml_utils.py` & `birentechci-0.0.2/sdk/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.1/setup.py` & `birentechci-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="birentechci", 
-    version="0.0.1",    
+    version="0.0.2",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
```

