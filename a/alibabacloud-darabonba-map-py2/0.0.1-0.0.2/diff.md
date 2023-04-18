# Comparing `tmp/alibabacloud_darabonba_map_py2-0.0.1.tar.gz` & `tmp/alibabacloud_darabonba_map_py2-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_darabonba_map_py2-0.0.1.tar", last modified: Sat Dec  4 03:41:24 2021, max compression
+gzip compressed data, was "dist/alibabacloud_darabonba_map_py2-0.0.2.tar", last modified: Tue Apr 18 12:10:17 2023, max compression
```

## Comparing `alibabacloud_darabonba_map_py2-0.0.1.tar` & `alibabacloud_darabonba_map_py2-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/
--rw-r--r--   0 root         (0) root         (0)     1027 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map/
--rw-r--r--   0 root         (0) root         (0)       22 2021-12-04 03:41:23.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map/__init__.py
--rw-r--r--   0 root         (0) root         (0)      418 2021-12-04 03:41:23.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map_py2.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1027 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map_py2.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      300 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map_py2.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map_py2.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map_py2.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2021-12-04 03:41:24.000000 alibabacloud_darabonba_map_py2-0.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2697 2021-12-04 03:41:23.000000 alibabacloud_darabonba_map_py2-0.0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map/
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-18 12:10:16.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-04-18 12:10:16.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map_py2.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1027 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map_py2.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      300 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map_py2.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map_py2.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map_py2.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:10:17.000000 alibabacloud_darabonba_map_py2-0.0.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2697 2023-04-18 12:10:16.000000 alibabacloud_darabonba_map_py2-0.0.2/setup.py
```

### Comparing `alibabacloud_darabonba_map_py2-0.0.1/PKG-INFO` & `alibabacloud_darabonba_map_py2-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_darabonba_map_py2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alibaba Cloud Darabonba Map SDK Library for Python2
 Home-page: https://github.com/aliyun/darabonba-map
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,darabonba,map,py2
```

### Comparing `alibabacloud_darabonba_map_py2-0.0.1/alibabacloud_darabonba_map_py2.egg-info/PKG-INFO` & `alibabacloud_darabonba_map_py2-0.0.2/alibabacloud_darabonba_map_py2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-darabonba-map-py2
-Version: 0.0.1
+Version: 0.0.2
 Summary: Alibaba Cloud Darabonba Map SDK Library for Python2
 Home-page: https://github.com/aliyun/darabonba-map
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: UNKNOWN
 Keywords: alibabacloud,darabonba,map,py2
```

### Comparing `alibabacloud_darabonba_map_py2-0.0.1/setup.py` & `alibabacloud_darabonba_map_py2-0.0.2/setup.py`

 * *Files identical despite different names*

