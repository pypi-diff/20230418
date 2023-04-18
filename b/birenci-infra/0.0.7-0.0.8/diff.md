# Comparing `tmp/birenci-infra-0.0.7.tar.gz` & `tmp/birenci-infra-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birenci-infra-0.0.7.tar", last modified: Tue Apr 18 07:10:58 2023, max compression
+gzip compressed data, was "birenci-infra-0.0.8.tar", last modified: Tue Apr 18 07:54:51 2023, max compression
```

## Comparing `birenci-infra-0.0.7.tar` & `birenci-infra-0.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birenci-infra-0.0.7/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.764624 birenci-infra-0.0.7/birenci_infra.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1949 2023-04-18 07:10:58.000000 birenci-infra-0.0.7/birenci_infra.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      759 2023-04-18 07:10:58.000000 birenci-infra-0.0.7/birenci_infra.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 07:10:58.000000 birenci-infra-0.0.7/birenci_infra.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        4 2023-04-18 07:10:58.000000 birenci-infra-0.0.7/birenci_infra.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.764624 birenci-infra-0.0.7/sdk/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.764624 birenci-infra-0.0.7/sdk/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/sdk/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/sdk/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/sdk/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/sdk/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.7/sdk/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 07:10:58.768625 birenci-infra-0.0.7/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      588 2023-04-18 07:10:52.000000 birenci-infra-0.0.7/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.012013 birenci-infra-0.0.8/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2047 2023-04-18 07:54:51.012013 birenci-infra-0.0.8/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birenci-infra-0.0.8/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/birenci_infra.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2047 2023-04-18 07:54:50.000000 birenci-infra-0.0.8/birenci_infra.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      759 2023-04-18 07:54:50.000000 birenci-infra-0.0.8/birenci_infra.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 07:54:50.000000 birenci-infra-0.0.8/birenci_infra.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        4 2023-04-18 07:54:50.000000 birenci-infra-0.0.8/birenci_infra.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/sdk/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/sdk/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/sdk/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/sdk/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/run.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/sdk/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/test_hander_perf.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 07:54:51.008012 birenci-infra-0.0.8/sdk/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birenci-infra-0.0.8/sdk/utils/xml_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 07:54:51.012013 birenci-infra-0.0.8/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      685 2023-04-18 07:54:41.000000 birenci-infra-0.0.8/setup.py
```

### Comparing `birenci-infra-0.0.7/PKG-INFO` & `birenci-infra-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: birenci-infra
-Version: 0.0.7
+Version: 0.0.8
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # 介绍
 ```
 默认会读取 以下 jenkins的环境变量
 export JOB_NAME="test/test"
```

### Comparing `birenci-infra-0.0.7/README.md` & `birenci-infra-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/birenci_infra.egg-info/PKG-INFO` & `birenci-infra-0.0.8/birenci_infra.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: birenci-infra
-Version: 0.0.7
+Version: 0.0.8
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # 介绍
 ```
 默认会读取 以下 jenkins的环境变量
 export JOB_NAME="test/test"
```

### Comparing `birenci-infra-0.0.7/birenci_infra.egg-info/SOURCES.txt` & `birenci-infra-0.0.8/birenci_infra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/apis/build.py` & `birenci-infra-0.0.8/sdk/apis/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/apis/client.py` & `birenci-infra-0.0.8/sdk/apis/client.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/apis/pdu.py` & `birenci-infra-0.0.8/sdk/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/apis/perf.py` & `birenci-infra-0.0.8/sdk/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/apis/pr.py` & `birenci-infra-0.0.8/sdk/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/handles/build.py` & `birenci-infra-0.0.8/sdk/handles/build.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/handles/pdu.py` & `birenci-infra-0.0.8/sdk/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/handles/perf.py` & `birenci-infra-0.0.8/sdk/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/handles/pr.py` & `birenci-infra-0.0.8/sdk/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/run.py` & `birenci-infra-0.0.8/sdk/run.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/schemas/pull_request.py` & `birenci-infra-0.0.8/sdk/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/test_hander_perf.py` & `birenci-infra-0.0.8/sdk/test_hander_perf.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/utils/csv_utils.py` & `birenci-infra-0.0.8/sdk/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/sdk/utils/xml_utils.py` & `birenci-infra-0.0.8/sdk/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birenci-infra-0.0.7/setup.py` & `birenci-infra-0.0.8/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="birenci-infra", 
-    version="0.0.7",    
+    version="0.0.8",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
+
     classifiers=[
         "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',   
 )
```

