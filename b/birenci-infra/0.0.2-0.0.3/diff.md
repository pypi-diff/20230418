# Comparing `tmp/birenci-infra-0.0.2.tar.gz` & `tmp/birenci-infra-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birenci-infra-0.0.2.tar", last modified: Tue Apr 18 03:47:26 2023, max compression
+gzip compressed data, was "birenci-infra-0.0.3.tar", last modified: Tue Apr 18 05:47:35 2023, max compression
```

## Comparing `birenci-infra-0.0.2.tar` & `birenci-infra-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1078 2023-04-18 03:41:13.000000 birenci-infra-0.0.2/LICENSE.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1975 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birenci-infra-0.0.2/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.302518 birenci-infra-0.0.2/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.302518 birenci-infra-0.0.2/birenci_infra.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1975 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      636 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 03:47:26.000000 birenci-infra-0.0.2/birenci_infra.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.302518 birenci-infra-0.0.2/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/handles/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/schemas/test_case.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/sdk/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:40:10.000000 birenci-infra-0.0.2/sdk/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      588 2023-04-18 03:47:24.000000 birenci-infra-0.0.2/setup.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:47:26.306518 birenci-infra-0.0.2/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.2/utils/xml_utils.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1078 2023-04-18 03:41:13.000000 birenci-infra-0.0.3/LICENSE.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1975 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birenci-infra-0.0.3/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/birenci_infra.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1975 2023-04-18 05:47:34.000000 birenci-infra-0.0.3/birenci_infra.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      636 2023-04-18 05:47:34.000000 birenci-infra-0.0.3/birenci_infra.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 05:47:34.000000 birenci-infra-0.0.3/birenci_infra.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 05:47:34.000000 birenci-infra-0.0.3/birenci_infra.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/handles/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/schemas/test_case.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/sdk/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:42:30.000000 birenci-infra-0.0.3/sdk/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      588 2023-04-18 05:44:43.000000 birenci-infra-0.0.3/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 05:47:35.015651 birenci-infra-0.0.3/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.3/utils/xml_utils.py
```

### Comparing `birenci-infra-0.0.2/LICENSE.txt` & `birenci-infra-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/PKG-INFO` & `birenci-infra-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birenci-infra
-Version: 0.0.2
+Version: 0.0.3
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birenci-infra-0.0.2/README.md` & `birenci-infra-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/apis/build.py` & `birenci-infra-0.0.3/apis/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/apis/client.py` & `birenci-infra-0.0.3/apis/client.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/apis/pdu.py` & `birenci-infra-0.0.3/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/apis/perf.py` & `birenci-infra-0.0.3/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/apis/pr.py` & `birenci-infra-0.0.3/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/birenci_infra.egg-info/PKG-INFO` & `birenci-infra-0.0.3/birenci_infra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birenci-infra
-Version: 0.0.2
+Version: 0.0.3
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birenci-infra-0.0.2/birenci_infra.egg-info/SOURCES.txt` & `birenci-infra-0.0.3/birenci_infra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/handles/build.py` & `birenci-infra-0.0.3/handles/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/handles/pdu.py` & `birenci-infra-0.0.3/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/handles/perf.py` & `birenci-infra-0.0.3/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/handles/pr.py` & `birenci-infra-0.0.3/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/schemas/pull_request.py` & `birenci-infra-0.0.3/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/setup.py` & `birenci-infra-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="birenci-infra", 
-    version="0.0.2",    
+    version="0.0.3",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
```

### Comparing `birenci-infra-0.0.2/utils/csv_utils.py` & `birenci-infra-0.0.3/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.2/utils/xml_utils.py` & `birenci-infra-0.0.3/utils/xml_utils.py`

 * *Files identical despite different names*

