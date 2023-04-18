# Comparing `tmp/birentechci-0.0.3.tar.gz` & `tmp/birentechci-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birentechci-0.0.3.tar", last modified: Tue Apr 18 08:47:06 2023, max compression
+gzip compressed data, was "birentechci-0.0.4.tar", last modified: Tue Apr 18 09:18:33 2023, max compression
```

## Comparing `birentechci-0.0.3.tar` & `birentechci-0.0.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 08:47:06.848725 birentechci-0.0.3/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.3/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/birentechci.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 08:47:06.000000 birentechci-0.0.3/birentechci.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      779 2023-04-18 08:47:06.000000 birentechci-0.0.3/birentechci.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 08:47:06.000000 birentechci-0.0.3/birentechci.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-04-18 08:47:06.000000 birentechci-0.0.3/birentechci.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/brci/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/brci/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/brci/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/brci/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/brci/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 08:47:06.848725 birentechci-0.0.3/brci/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.3/brci/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 08:47:06.848725 birentechci-0.0.3/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      683 2023-04-18 08:46:46.000000 birentechci-0.0.3/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 09:18:33.400900 birentechci-0.0.4/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.4/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/birentechci.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 09:18:33.000000 birentechci-0.0.4/birentechci.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      792 2023-04-18 09:18:33.000000 birentechci-0.0.4/birentechci.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 09:18:33.000000 birentechci-0.0.4/birentechci.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-04-18 09:18:33.000000 birentechci-0.0.4/birentechci.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/brci/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/brci/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/brci/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/brci/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3308 2023-04-18 09:17:37.000000 birentechci-0.0.4/brci/main.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/run.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/brci/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/test_hander_perf.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 09:18:33.400900 birentechci-0.0.4/brci/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.4/brci/utils/xml_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 09:18:33.400900 birentechci-0.0.4/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      681 2023-04-18 09:17:56.000000 birentechci-0.0.4/setup.py
```

### Comparing `birentechci-0.0.3/PKG-INFO` & `birentechci-0.0.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.3
+Version: 0.0.4
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birentechci-0.0.3/README.md` & `birentechci-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/birentechci.egg-info/PKG-INFO` & `birentechci-0.0.4/birentechci.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.3
+Version: 0.0.4
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birentechci-0.0.3/birentechci.egg-info/SOURCES.txt` & `birentechci-0.0.4/birentechci.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 setup.py
 birentechci.egg-info/PKG-INFO
 birentechci.egg-info/SOURCES.txt
 birentechci.egg-info/dependency_links.txt
 birentechci.egg-info/top_level.txt
 brci/__init__.py
+brci/main.py
 brci/run.py
 brci/test_hander_perf.py
 brci/apis/__init__.py
 brci/apis/build.py
 brci/apis/client.py
 brci/apis/pdu.py
 brci/apis/perf.py
```

### Comparing `birentechci-0.0.3/brci/apis/build.py` & `birentechci-0.0.4/brci/apis/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/apis/client.py` & `birentechci-0.0.4/brci/apis/client.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/apis/pdu.py` & `birentechci-0.0.4/brci/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/apis/perf.py` & `birentechci-0.0.4/brci/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/apis/pr.py` & `birentechci-0.0.4/brci/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/handles/build.py` & `birentechci-0.0.4/brci/handles/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/handles/pdu.py` & `birentechci-0.0.4/brci/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/handles/perf.py` & `birentechci-0.0.4/brci/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/handles/pr.py` & `birentechci-0.0.4/brci/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/run.py` & `birentechci-0.0.4/brci/run.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/schemas/pull_request.py` & `birentechci-0.0.4/brci/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/test_hander_perf.py` & `birentechci-0.0.4/brci/test_hander_perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/utils/csv_utils.py` & `birentechci-0.0.4/brci/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/brci/utils/xml_utils.py` & `birentechci-0.0.4/brci/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.3/setup.py` & `birentechci-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools 
  
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
  
 setuptools.setup(
     name="birentechci", 
-    version="0.0.3",    
+    version="0.0.4",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
 
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    python_requires='>=3.6',   
+    python_requires='>=3.6', 
 )
```

