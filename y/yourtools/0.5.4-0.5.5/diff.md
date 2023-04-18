# Comparing `tmp/yourtools-0.5.4.tar.gz` & `tmp/yourtools-0.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/yourtools-0.5.4.tar", last modified: Fri Apr 14 11:28:38 2023, max compression
+gzip compressed data, was "dist/yourtools-0.5.5.tar", last modified: Tue Apr 18 01:52:47 2023, max compression
```

## Comparing `yourtools-0.5.4.tar` & `yourtools-0.5.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 11:28:38.000000 yourtools-0.5.4/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools/
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools/db/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.4/yourtools/db/__init__.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.4/yourtools/db/dbutils.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.4/yourtools/db/hive.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.4/yourtools/db/mysql.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.4/yourtools/Azkaban.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      730 2023-04-14 11:27:27.000000 yourtools-0.5.4/yourtools/Time.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     6292 2023-04-14 11:05:56.000000 yourtools-0.5.4/yourtools/WeChat.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.4/yourtools/__init__.py
-drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools.egg-info/
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools.egg-info/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools.egg-info/SOURCES.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools.egg-info/dependency_links.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools.egg-info/requires.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-14 11:28:38.000000 yourtools-0.5.4/yourtools.egg-info/top_level.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.4/README.md
--rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.4/requirements.txt
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-14 10:46:10.000000 yourtools-0.5.4/setup.py
--rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-14 11:28:38.000000 yourtools-0.5.4/PKG-INFO
--rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-14 11:28:38.000000 yourtools-0.5.4/setup.cfg
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools/
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools/db/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      347 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/db/__init__.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      739 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/db/dbutils.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2122 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/db/hive.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2399 2023-04-13 10:15:47.000000 yourtools-0.5.5/yourtools/db/mysql.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     3842 2023-04-07 10:28:09.000000 yourtools-0.5.5/yourtools/Azkaban.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1025 2023-04-18 01:51:31.000000 yourtools-0.5.5/yourtools/Time.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     6292 2023-04-14 11:05:56.000000 yourtools-0.5.5/yourtools/WeChat.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      474 2023-04-14 10:42:59.000000 yourtools-0.5.5/yourtools/__init__.py
+drwxrwxr-x   0 zfang     (3307) zfang     (3307)        0 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      372 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/SOURCES.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)        1 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/dependency_links.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      190 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/requires.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       10 2023-04-18 01:52:47.000000 yourtools-0.5.5/yourtools.egg-info/top_level.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2232 2023-04-07 10:28:09.000000 yourtools-0.5.5/README.md
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)      189 2023-04-13 08:31:32.000000 yourtools-0.5.5/requirements.txt
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     1577 2023-04-14 10:46:10.000000 yourtools-0.5.5/setup.py
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)     2658 2023-04-18 01:52:47.000000 yourtools-0.5.5/PKG-INFO
+-rw-rw-r--   0 zfang     (3307) zfang     (3307)       38 2023-04-18 01:52:47.000000 yourtools-0.5.5/setup.cfg
```

### Comparing `yourtools-0.5.4/yourtools/db/dbutils.py` & `yourtools-0.5.5/yourtools/db/dbutils.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/yourtools/db/hive.py` & `yourtools-0.5.5/yourtools/db/hive.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/yourtools/db/mysql.py` & `yourtools-0.5.5/yourtools/db/mysql.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/yourtools/Azkaban.py` & `yourtools-0.5.5/yourtools/Azkaban.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/yourtools/Time.py` & `yourtools-0.5.5/yourtools/Time.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,21 +8,32 @@
 @filename   : Time.py
 @create time: 2023/4/13 3:35 PM
 @modify time: 2023/4/13 3:35 PM
 @describe   : 
 -------------------------------------------------
 """
 from time import strftime, localtime
+from datetime import datetime, timedelta
 
 
 class Time:
     def __init__(self):
         self.time_format = "%Y-%m-%d %H:%M:%S"
 
     def curr_time(self, time_format=None):
         if time_format:
             return strftime(time_format, localtime())
         else:
             return strftime(self.time_format, localtime())
 
     def curr_time_by_number(self):
-        return self.curr_time("%Y%m%d%H%M%S")
+        return self.curr_time("%Y%m%d%H%M%S")
+
+    def _today(self):
+        return datetime.today()
+
+    def today(self):
+        return self._today().strftime("%Y-%m-%d")
+
+    def yesterday(self):
+        yesterday = self._today() - timedelta(days=1)
+        return yesterday.strftime('%Y-%m-%d')
```

### Comparing `yourtools-0.5.4/yourtools/WeChat.py` & `yourtools-0.5.5/yourtools/WeChat.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/yourtools.egg-info/PKG-INFO` & `yourtools-0.5.5/yourtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `yourtools-0.5.4/README.md` & `yourtools-0.5.5/README.md`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/setup.py` & `yourtools-0.5.5/setup.py`

 * *Files identical despite different names*

### Comparing `yourtools-0.5.4/PKG-INFO` & `yourtools-0.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yourtools
-Version: 0.5.4
+Version: 0.5.5
 Summary: Python helper tools
 Home-page: https://pypi.org/project/yourtools/
 Author: zfang
 Author-email: founder517518@163.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

