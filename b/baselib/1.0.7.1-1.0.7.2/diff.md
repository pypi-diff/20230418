# Comparing `tmp/baselib-1.0.7.1.tar.gz` & `tmp/baselib-1.0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baselib-1.0.7.1.tar", last modified: Mon Apr 10 09:53:31 2023, max compression
+gzip compressed data, was "baselib-1.0.7.2.tar", last modified: Tue Apr 18 02:27:56 2023, max compression
```

## Comparing `baselib-1.0.7.1.tar` & `baselib-1.0.7.2.tar`

### file list

```diff
@@ -1,41 +1,43 @@
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.243776 baselib-1.0.7.1/
--rw-r--r--   0 linkerui   (501) staff       (20)     1684 2023-04-10 09:53:31.243323 baselib-1.0.7.1/PKG-INFO
--rw-r--r--   0 linkerui   (501) staff       (20)     1024 2023-04-10 02:10:09.000000 baselib-1.0.7.1/README.md
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.224850 baselib-1.0.7.1/baselib/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.229088 baselib-1.0.7.1/baselib/demo/
--rw-r--r--   0 linkerui   (501) staff       (20)       22 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/demo/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)       86 2023-04-10 04:09:02.000000 baselib-1.0.7.1/baselib/demo/demo.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.230873 baselib-1.0.7.1/baselib/json/
--rw-r--r--   0 linkerui   (501) staff       (20)       44 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/json/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1687 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/json/json_file.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.232337 baselib-1.0.7.1/baselib/log/
--rw-r--r--   0 linkerui   (501) staff       (20)       40 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/log/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2219 2023-04-10 02:11:14.000000 baselib-1.0.7.1/baselib/log/file.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.233337 baselib-1.0.7.1/baselib/py/
--rw-r--r--   0 linkerui   (501) staff       (20)      605 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/py/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.234861 baselib-1.0.7.1/baselib/qywx/
--rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/qywx/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)    13625 2023-04-10 09:39:56.000000 baselib-1.0.7.1/baselib/qywx/qywx.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.235685 baselib-1.0.7.1/baselib/request/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/request/__init__.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.241190 baselib-1.0.7.1/baselib/tests/
--rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/tests/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4989 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/tests/debug.py
--rw-r--r--   0 linkerui   (501) staff       (20)      126 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/tests/demo_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)     1838 2023-04-10 02:21:48.000000 baselib-1.0.7.1/baselib/tests/file_logger_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      494 2023-04-10 02:10:09.000000 baselib-1.0.7.1/baselib/tests/httplib_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)      849 2023-04-10 09:42:38.000000 baselib-1.0.7.1/baselib/tests/json_file_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)     2800 2023-04-10 04:07:37.000000 baselib-1.0.7.1/baselib/tests/period_test.py
--rw-r--r--   0 linkerui   (501) staff       (20)     3154 2023-04-10 02:10:09.000000 baselib-1.0.7.1/baselib/tests/qywx_test.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.242511 baselib-1.0.7.1/baselib/time/
--rw-r--r--   0 linkerui   (501) staff       (20)       39 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/time/__init__.py
--rw-r--r--   0 linkerui   (501) staff       (20)     4480 2023-04-04 11:38:24.000000 baselib-1.0.7.1/baselib/time/period.py
-drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-10 09:53:31.227054 baselib-1.0.7.1/baselib.egg-info/
--rw-r--r--   0 linkerui   (501) staff       (20)     1684 2023-04-10 09:53:31.000000 baselib-1.0.7.1/baselib.egg-info/PKG-INFO
--rw-r--r--   0 linkerui   (501) staff       (20)      706 2023-04-10 09:53:31.000000 baselib-1.0.7.1/baselib.egg-info/SOURCES.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-10 09:53:31.000000 baselib-1.0.7.1/baselib.egg-info/dependency_links.txt
--rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-01-31 07:20:51.000000 baselib-1.0.7.1/baselib.egg-info/not-zip-safe
--rw-r--r--   0 linkerui   (501) staff       (20)        8 2023-04-10 09:53:31.000000 baselib-1.0.7.1/baselib.egg-info/top_level.txt
--rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-10 09:53:31.243943 baselib-1.0.7.1/setup.cfg
--rw-r--r--   0 linkerui   (501) staff       (20)      636 2023-04-10 09:52:49.000000 baselib-1.0.7.1/setup.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.449592 baselib-1.0.7.2/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1684 2023-04-18 02:27:56.449250 baselib-1.0.7.2/PKG-INFO
+-rw-r--r--   0 linkerui   (501) staff       (20)     1024 2023-04-10 02:10:09.000000 baselib-1.0.7.2/README.md
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.430094 baselib-1.0.7.2/baselib/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.434297 baselib-1.0.7.2/baselib/demo/
+-rw-r--r--   0 linkerui   (501) staff       (20)       22 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/demo/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)       86 2023-04-10 04:09:02.000000 baselib-1.0.7.2/baselib/demo/demo.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.436006 baselib-1.0.7.2/baselib/json/
+-rw-r--r--   0 linkerui   (501) staff       (20)       44 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/json/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1687 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/json/json_file.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.437476 baselib-1.0.7.2/baselib/log/
+-rw-r--r--   0 linkerui   (501) staff       (20)       40 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/log/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2219 2023-04-10 02:11:14.000000 baselib-1.0.7.2/baselib/log/file.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.438371 baselib-1.0.7.2/baselib/os/
+-rw-r--r--   0 linkerui   (501) staff       (20)      758 2023-04-13 07:00:09.000000 baselib-1.0.7.2/baselib/os/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.438906 baselib-1.0.7.2/baselib/py/
+-rw-r--r--   0 linkerui   (501) staff       (20)      605 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/py/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.440271 baselib-1.0.7.2/baselib/qywx/
+-rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/qywx/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)    13625 2023-04-10 09:39:56.000000 baselib-1.0.7.2/baselib/qywx/qywx.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.441292 baselib-1.0.7.2/baselib/request/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/request/__init__.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.447051 baselib-1.0.7.2/baselib/tests/
+-rw-r--r--   0 linkerui   (501) staff       (20)        0 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/tests/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4989 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/tests/debug.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      126 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/tests/demo_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     1838 2023-04-10 02:21:48.000000 baselib-1.0.7.2/baselib/tests/file_logger_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      494 2023-04-10 02:10:09.000000 baselib-1.0.7.2/baselib/tests/httplib_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)      849 2023-04-10 09:42:38.000000 baselib-1.0.7.2/baselib/tests/json_file_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     2800 2023-04-10 04:07:37.000000 baselib-1.0.7.2/baselib/tests/period_test.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     3154 2023-04-10 02:10:09.000000 baselib-1.0.7.2/baselib/tests/qywx_test.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.448449 baselib-1.0.7.2/baselib/time/
+-rw-r--r--   0 linkerui   (501) staff       (20)       39 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/time/__init__.py
+-rw-r--r--   0 linkerui   (501) staff       (20)     4480 2023-04-04 11:38:24.000000 baselib-1.0.7.2/baselib/time/period.py
+drwxr-xr-x   0 linkerui   (501) staff       (20)        0 2023-04-18 02:27:56.432739 baselib-1.0.7.2/baselib.egg-info/
+-rw-r--r--   0 linkerui   (501) staff       (20)     1684 2023-04-18 02:27:56.000000 baselib-1.0.7.2/baselib.egg-info/PKG-INFO
+-rw-r--r--   0 linkerui   (501) staff       (20)      729 2023-04-18 02:27:56.000000 baselib-1.0.7.2/baselib.egg-info/SOURCES.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-04-18 02:27:56.000000 baselib-1.0.7.2/baselib.egg-info/dependency_links.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)        1 2023-01-31 07:20:51.000000 baselib-1.0.7.2/baselib.egg-info/not-zip-safe
+-rw-r--r--   0 linkerui   (501) staff       (20)        8 2023-04-18 02:27:56.000000 baselib-1.0.7.2/baselib.egg-info/top_level.txt
+-rw-r--r--   0 linkerui   (501) staff       (20)       38 2023-04-18 02:27:56.449705 baselib-1.0.7.2/setup.cfg
+-rw-r--r--   0 linkerui   (501) staff       (20)      830 2023-04-18 02:27:53.000000 baselib-1.0.7.2/setup.py
```

### Comparing `baselib-1.0.7.1/PKG-INFO` & `baselib-1.0.7.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselib
-Version: 1.0.7.1
+Version: 1.0.7.2
 Summary: base common lib for python
 Home-page: https://github.com/coreylam/base_common_lib
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Description: # base_common_lib
         常用的基础通用Lib集合
```

### Comparing `baselib-1.0.7.1/README.md` & `baselib-1.0.7.2/README.md`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/json/json_file.py` & `baselib-1.0.7.2/baselib/json/json_file.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/log/file.py` & `baselib-1.0.7.2/baselib/log/file.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/py/__init__.py` & `baselib-1.0.7.2/baselib/py/__init__.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/qywx/qywx.py` & `baselib-1.0.7.2/baselib/qywx/qywx.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/tests/debug.py` & `baselib-1.0.7.2/baselib/tests/debug.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/tests/file_logger_test.py` & `baselib-1.0.7.2/baselib/tests/file_logger_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/tests/json_file_test.py` & `baselib-1.0.7.2/baselib/tests/json_file_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/tests/period_test.py` & `baselib-1.0.7.2/baselib/tests/period_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/tests/qywx_test.py` & `baselib-1.0.7.2/baselib/tests/qywx_test.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib/time/period.py` & `baselib-1.0.7.2/baselib/time/period.py`

 * *Files identical despite different names*

### Comparing `baselib-1.0.7.1/baselib.egg-info/PKG-INFO` & `baselib-1.0.7.2/baselib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baselib
-Version: 1.0.7.1
+Version: 1.0.7.2
 Summary: base common lib for python
 Home-page: https://github.com/coreylam/base_common_lib
 Author: coreylam
 Author-email: coreylam@163.com
 License: GPL
 Description: # base_common_lib
         常用的基础通用Lib集合
```

### Comparing `baselib-1.0.7.1/baselib.egg-info/SOURCES.txt` & `baselib-1.0.7.2/baselib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 baselib.egg-info/top_level.txt
 baselib/demo/__init__.py
 baselib/demo/demo.py
 baselib/json/__init__.py
 baselib/json/json_file.py
 baselib/log/__init__.py
 baselib/log/file.py
+baselib/os/__init__.py
 baselib/py/__init__.py
 baselib/qywx/__init__.py
 baselib/qywx/qywx.py
 baselib/request/__init__.py
 baselib/tests/__init__.py
 baselib/tests/debug.py
 baselib/tests/demo_test.py
```

