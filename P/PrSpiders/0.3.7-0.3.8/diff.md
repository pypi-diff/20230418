# Comparing `tmp/PrSpiders-0.3.7.tar.gz` & `tmp/PrSpiders-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.3.7.tar", last modified: Tue Apr 18 06:27:02 2023, max compression
+gzip compressed data, was "PrSpiders-0.3.8.tar", last modified: Tue Apr 18 08:55:30 2023, max compression
```

## Comparing `PrSpiders-0.3.7.tar` & `PrSpiders-0.3.8.tar`

### file list

```diff
@@ -1,26 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:27:02.003039 PrSpiders-0.3.7/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.7/LICENSE.txt
--rw-rw-rw-   0        0        0     4583 2023-04-18 06:27:01.999040 PrSpiders-0.3.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.900040 PrSpiders-0.3.7/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.7/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.7/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.7/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4461 2023-04-18 06:26:14.000000 PrSpiders-0.3.7/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.7/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.950041 PrSpiders-0.3.7/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4583 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 06:27:01.000000 PrSpiders-0.3.7/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.958039 PrSpiders-0.3.7/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-18 06:26:26.000000 PrSpiders-0.3.7/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:27:01.992041 PrSpiders-0.3.7/pkg/prspider/
--rw-rw-rw-   0        0        0     1168 2023-04-18 06:21:44.000000 PrSpiders-0.3.7/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.7/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.7/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.7/pkg/prspider/start.py
--rw-rw-rw-   0        0        0       42 2023-04-18 06:27:02.010041 PrSpiders-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-18 06:26:31.000000 PrSpiders-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:55:30.556273 PrSpiders-0.3.8/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.8/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-18 08:55:30.537271 PrSpiders-0.3.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 08:55:26.471267 PrSpiders-0.3.8/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.8/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.8/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.8/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4461 2023-04-18 06:26:14.000000 PrSpiders-0.3.8/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.8/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:55:29.583283 PrSpiders-0.3.8/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-18 08:55:23.000000 PrSpiders-0.3.8/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-04-18 08:55:23.000000 PrSpiders-0.3.8/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 08:55:23.000000 PrSpiders-0.3.8/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 08:55:23.000000 PrSpiders-0.3.8/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-18 08:55:23.000000 PrSpiders-0.3.8/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-18 08:55:23.000000 PrSpiders-0.3.8/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 08:55:29.749287 PrSpiders-0.3.8/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-18 06:26:26.000000 PrSpiders-0.3.8/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:55:30.354270 PrSpiders-0.3.8/pkg/prspider/
+-rw-rw-rw-   0        0        0     1168 2023-04-18 06:21:44.000000 PrSpiders-0.3.8/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.8/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.8/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.8/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-04-18 08:55:30.517275 PrSpiders-0.3.8/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.3.8/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.3.8/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.3.8/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.8/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 08:55:30.557272 PrSpiders-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-18 08:55:19.000000 PrSpiders-0.3.8/setup.py
```

### Comparing `PrSpiders-0.3.7/LICENSE.txt` & `PrSpiders-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/PKG-INFO` & `PrSpiders-0.3.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.7
+Version: 0.3.8
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.7/PrSpider/PrSpiders.py` & `PrSpiders-0.3.8/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/PrSpider/pxpath.py` & `PrSpiders-0.3.8/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/PrSpider/requestXpath.py` & `PrSpiders-0.3.8/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/PrSpider/useragent.py` & `PrSpiders-0.3.8/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.3.8/PrSpiders.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.7
+Version: 0.3.8
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.7/README.md` & `PrSpiders-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.3.8/pkg/prspider/PrSpider_CMD.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.7/setup.py` & `PrSpiders-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.3.7"
+__version__ = "0.3.8"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

