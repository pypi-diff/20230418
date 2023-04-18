# Comparing `tmp/birentechci-0.0.6.tar.gz` & `tmp/birentechci-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birentechci-0.0.6.tar", last modified: Tue Apr 18 10:00:33 2023, max compression
+gzip compressed data, was "birentechci-0.0.7.tar", last modified: Tue Apr 18 10:25:31 2023, max compression
```

## Comparing `birentechci-0.0.6.tar` & `birentechci-0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.471228 birentechci-0.0.6/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 10:00:33.471228 birentechci-0.0.6/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.6/README.md
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.467228 birentechci-0.0.6/birentechci.egg-info/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 10:00:33.000000 birentechci-0.0.6/birentechci.egg-info/PKG-INFO
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      826 2023-04-18 10:00:33.000000 birentechci-0.0.6/birentechci.egg-info/SOURCES.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 10:00:33.000000 birentechci-0.0.6/birentechci.egg-info/dependency_links.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       68 2023-04-18 10:00:33.000000 birentechci-0.0.6/birentechci.egg-info/requires.txt
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-04-18 10:00:33.000000 birentechci-0.0.6/birentechci.egg-info/top_level.txt
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.467228 birentechci-0.0.6/brci/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       14 2023-04-18 10:00:00.000000 birentechci-0.0.6/brci/__init__.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.467228 birentechci-0.0.6/brci/apis/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/apis/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/apis/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/apis/client.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/apis/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/apis/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/apis/pr.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.467228 birentechci-0.0.6/brci/config/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/config/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/config/develop.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/config/prod.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.467228 birentechci-0.0.6/brci/handles/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/handles/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/handles/build.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/handles/pdu.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/handles/perf.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/handles/pr.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3308 2023-04-18 09:17:37.000000 birentechci-0.0.6/brci/main.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/run.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.471228 birentechci-0.0.6/brci/schemas/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/schemas/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/schemas/jenkins.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/schemas/pull_request.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/schemas/pull_request_job.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/schemas/test_case.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/test_hander_perf.py
-drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:00:33.471228 birentechci-0.0.6/brci/utils/
--rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/utils/__init__.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/utils/csv_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/utils/file_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/utils/json_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/utils/pd_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.6/brci/utils/xml_utils.py
--rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 10:00:33.471228 birentechci-0.0.6/setup.cfg
--rw-rw-r--   0 e00928    (1001) e00928    (1001)     1148 2023-04-18 10:00:27.000000 birentechci-0.0.6/setup.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 10:25:31.171842 birentechci-0.0.7/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1609 2023-04-18 03:36:01.000000 birentechci-0.0.7/README.md
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/birentechci.egg-info/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     2045 2023-04-18 10:25:31.000000 birentechci-0.0.7/birentechci.egg-info/PKG-INFO
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      826 2023-04-18 10:25:31.000000 birentechci-0.0.7/birentechci.egg-info/SOURCES.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        1 2023-04-18 10:25:31.000000 birentechci-0.0.7/birentechci.egg-info/dependency_links.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       68 2023-04-18 10:25:31.000000 birentechci-0.0.7/birentechci.egg-info/requires.txt
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        5 2023-04-18 10:25:31.000000 birentechci-0.0.7/birentechci.egg-info/top_level.txt
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/brci/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:17:20.000000 birentechci-0.0.7/brci/__init__.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/brci/apis/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/apis/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1530 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/apis/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1631 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/apis/client.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     4188 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/apis/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1932 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/apis/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1291 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/apis/pr.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/brci/config/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      378 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/config/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      175 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/config/develop.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      176 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/config/prod.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/brci/handles/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       11 2023-04-18 10:18:01.000000 birentechci-0.0.7/brci/handles/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3694 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/handles/build.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3429 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/handles/pdu.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     7944 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/handles/perf.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1502 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/handles/pr.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3309 2023-04-18 10:22:03.000000 birentechci-0.0.7/brci/main.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     3697 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/run.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/brci/schemas/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/schemas/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      499 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/schemas/jenkins.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      619 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/schemas/pull_request.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      144 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/schemas/pull_request_job.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       94 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/schemas/test_case.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      540 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/test_hander_perf.py
+drwxrwxr-x   0 e00928    (1001) e00928    (1001)        0 2023-04-18 10:25:31.171842 birentechci-0.0.7/brci/utils/
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)        0 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/utils/__init__.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1292 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/utils/csv_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      369 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/utils/file_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      269 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/utils/json_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       83 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/utils/pd_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)      533 2023-04-18 03:37:21.000000 birentechci-0.0.7/brci/utils/xml_utils.py
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)       38 2023-04-18 10:25:31.171842 birentechci-0.0.7/setup.cfg
+-rw-rw-r--   0 e00928    (1001) e00928    (1001)     1148 2023-04-18 10:25:27.000000 birentechci-0.0.7/setup.py
```

### Comparing `birentechci-0.0.6/PKG-INFO` & `birentechci-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.6
+Version: 0.0.7
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birentechci-0.0.6/README.md` & `birentechci-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/birentechci.egg-info/PKG-INFO` & `birentechci-0.0.7/birentechci.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birentechci
-Version: 0.0.6
+Version: 0.0.7
 Summary: biren ci sdk
 Home-page: https://gitlab.birentech.com/software/br_ci_db
 Author: br_infra
 Author-email: br_infra@birentech.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `birentechci-0.0.6/birentechci.egg-info/SOURCES.txt` & `birentechci-0.0.7/birentechci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/apis/build.py` & `birentechci-0.0.7/brci/apis/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/apis/client.py` & `birentechci-0.0.7/brci/apis/client.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/apis/pdu.py` & `birentechci-0.0.7/brci/apis/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/apis/perf.py` & `birentechci-0.0.7/brci/apis/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/apis/pr.py` & `birentechci-0.0.7/brci/apis/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/handles/build.py` & `birentechci-0.0.7/brci/handles/build.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/handles/pdu.py` & `birentechci-0.0.7/brci/handles/pdu.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/handles/perf.py` & `birentechci-0.0.7/brci/handles/perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/handles/pr.py` & `birentechci-0.0.7/brci/handles/pr.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/main.py` & `birentechci-0.0.7/brci/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import io
 import sys
 
-from handles import build, pdu, perf, pr
+from .handles import build, pdu, perf, pr
 
 sys.stdout = sys.__stdout__ = io.TextIOWrapper(
     sys.stdout.detach(), encoding="utf-8", line_buffering=True
 )
 sys.stderr = sys.__stderr__ = io.TextIOWrapper(
     sys.stderr.detach(), encoding="utf-8", line_buffering=True
 )
```

### Comparing `birentechci-0.0.6/brci/run.py` & `birentechci-0.0.7/brci/run.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/schemas/pull_request.py` & `birentechci-0.0.7/brci/schemas/pull_request.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/test_hander_perf.py` & `birentechci-0.0.7/brci/test_hander_perf.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/utils/csv_utils.py` & `birentechci-0.0.7/brci/utils/csv_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/brci/utils/xml_utils.py` & `birentechci-0.0.7/brci/utils/xml_utils.py`

 * *Files identical despite different names*

### Comparing `birentechci-0.0.6/setup.py` & `birentechci-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         else:
             requires.append(pkg)
     return requires
 
 
 setuptools.setup(
     name="birentechci", 
-    version="0.0.6",    
+    version="0.0.7",    
     author="br_infra",    
     author_email="br_infra@birentech.com",    
     description="biren ci sdk",
     long_description=long_description,    
     long_description_content_type="text/markdown",
     url="https://gitlab.birentech.com/software/br_ci_db",    
     packages=setuptools.find_packages(),
```

