# Comparing `tmp/mingdaoyun_sdk-0.0.6.tar.gz` & `tmp/mingdaoyun_sdk-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mingdaoyun_sdk-0.0.6.tar", last modified: Fri Apr 14 07:07:29 2023, max compression
+gzip compressed data, was "mingdaoyun_sdk-0.0.7.tar", last modified: Tue Apr 18 06:39:47 2023, max compression
```

## Comparing `mingdaoyun_sdk-0.0.6.tar` & `mingdaoyun_sdk-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:07:29.509810 mingdaoyun_sdk-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 07:07:29.509810 mingdaoyun_sdk-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-14 07:07:15.000000 mingdaoyun_sdk-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:07:29.509810 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-14 07:07:15.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/MingdaoOrg.py
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-14 07:07:15.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/MingdaoYun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 07:07:15.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-14 07:07:15.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 07:07:29.509810 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-14 07:07:29.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-14 07:07:29.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 07:07:29.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 07:07:29.000000 mingdaoyun_sdk-0.0.6/mingdaoyun_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 07:07:29.509810 mingdaoyun_sdk-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-14 07:07:15.000000 mingdaoyun_sdk-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:47.495808 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoOrg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8612 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoYun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-18 06:39:47.000000 mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:39:47.499807 mingdaoyun_sdk-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-04-18 06:39:36.000000 mingdaoyun_sdk-0.0.7/setup.py
```

### Comparing `mingdaoyun_sdk-0.0.6/PKG-INFO` & `mingdaoyun_sdk-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun_sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/MingdaoOrg.py` & `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoOrg.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/MingdaoYun.py` & `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/MingdaoYun.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,29 +27,31 @@
     GET_RELATIONS_URL = "/api/v2/open/worksheet/getRowRelations"
     ADD_URL = "/api/v2/open/worksheet/addRow"
     BATCH_ADD_URL = "/api/v2/open/worksheet/addRows"
     DELETE_URL = "/api/v2/open/worksheet/deleteRow"
     EDIT_URL = "/api/v2/open/worksheet/editRow"
     BATCH_EDIT_URL = "/api/v2/open/worksheet/editRows"
 
-    def __init__(self, appKey: str, sign: str, host: str):
+    def __init__(self, appKey: str, sign: str, host: str, cert_path: str = None):
         """
         初始化mingdaoyun方法
         :param appKey: {string} appKey
         :param sign:{string} sign
         :param host :{string} host
         :return:  Mingdaoyun 实体类
         """
         self.appKey = appKey
         self.sign = sign
         self.host = host
         self.params = {}
         self.filters = []
         self.worksheetId = ""
         self.view = ""
+        if cert_path is not None:
+            http.verify = cert_path
         return
 
     def table(self, table: str):
         """
         设置当前的worksheet
         :param table: 表名
         :return: 自身
```

### Comparing `mingdaoyun_sdk-0.0.6/mingdaoyun_sdk/common.py` & `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk/common.py`

 * *Files identical despite different names*

### Comparing `mingdaoyun_sdk-0.0.6/mingdaoyun_sdk.egg-info/PKG-INFO` & `mingdaoyun_sdk-0.0.7/mingdaoyun_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mingdaoyun-sdk
-Version: 0.0.6
+Version: 0.0.7
 Summary: 针对mingdaoyun的API封装的Python-SDK包
 Home-page: https://github.com/ghostlitao/mingdaoyun-python-sdk
 Author: Todd
 Author-email: ghostlitao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `mingdaoyun_sdk-0.0.6/setup.py` & `mingdaoyun_sdk-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="mingdaoyun_sdk",
     # 版本号, 版本号规范：https://www.python.org/dev/peps/pep-0440/
-    version="0.0.6",
+    version="0.0.7",
     # 作者名
     author="Todd",
     # 作者邮箱
     author_email="ghostlitao@gmail.com",
     # 包的简介描述
     description="针对mingdaoyun的API封装的Python-SDK包",
     # 包的详细介绍(一般通过加载README.md)
```

