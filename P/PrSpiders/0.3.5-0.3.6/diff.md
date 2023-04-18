# Comparing `tmp/PrSpiders-0.3.5.tar.gz` & `tmp/PrSpiders-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.3.5.tar", last modified: Tue Apr 18 06:15:12 2023, max compression
+gzip compressed data, was "PrSpiders-0.3.6.tar", last modified: Tue Apr 18 06:21:58 2023, max compression
```

## Comparing `PrSpiders-0.3.5.tar` & `PrSpiders-0.3.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:15:12.278829 PrSpiders-0.3.5/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.5/LICENSE.txt
--rw-rw-rw-   0        0        0     4583 2023-04-18 06:15:12.272829 PrSpiders-0.3.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-18 06:15:12.128828 PrSpiders-0.3.5/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.5/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.5/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.5/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4073 2023-04-18 02:20:24.000000 PrSpiders-0.3.5/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.5/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:15:12.191845 PrSpiders-0.3.5/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4583 2023-04-18 06:15:11.000000 PrSpiders-0.3.5/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-04-18 06:15:11.000000 PrSpiders-0.3.5/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:15:11.000000 PrSpiders-0.3.5/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-18 06:15:11.000000 PrSpiders-0.3.5/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-18 06:15:11.000000 PrSpiders-0.3.5/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-04-18 06:15:11.000000 PrSpiders-0.3.5/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.5/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 06:15:12.210830 PrSpiders-0.3.5/pkg/
--rw-rw-rw-   0        0        0       31 2023-04-18 06:14:34.000000 PrSpiders-0.3.5/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:15:12.264831 PrSpiders-0.3.5/pkg/prspider/
--rw-rw-rw-   0        0        0     1175 2023-04-18 06:11:20.000000 PrSpiders-0.3.5/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.5/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.5/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.5/pkg/prspider/start.py
--rw-rw-rw-   0        0        0       42 2023-04-18 06:15:12.283829 PrSpiders-0.3.5/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-18 06:15:03.000000 PrSpiders-0.3.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:21:58.066411 PrSpiders-0.3.6/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-18 06:21:58.064415 PrSpiders-0.3.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 06:21:57.858409 PrSpiders-0.3.6/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.6/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.6/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.3.6/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4073 2023-04-18 02:20:24.000000 PrSpiders-0.3.6/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.6/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:21:57.948411 PrSpiders-0.3.6/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      460 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 06:21:57.000000 PrSpiders-0.3.6/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.6/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 06:21:57.982412 PrSpiders-0.3.6/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-18 06:20:57.000000 PrSpiders-0.3.6/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:21:58.054412 PrSpiders-0.3.6/pkg/prspider/
+-rw-rw-rw-   0        0        0     1168 2023-04-18 06:21:44.000000 PrSpiders-0.3.6/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.6/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.6/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.6/pkg/prspider/start.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 06:21:58.066411 PrSpiders-0.3.6/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-18 06:21:04.000000 PrSpiders-0.3.6/setup.py
```

### Comparing `PrSpiders-0.3.5/LICENSE.txt` & `PrSpiders-0.3.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.5/PKG-INFO` & `PrSpiders-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.5
+Version: 0.3.6
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.5/PrSpider/PrSpiders.py` & `PrSpiders-0.3.6/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.5/PrSpider/pxpath.py` & `PrSpiders-0.3.6/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.5/PrSpider/requestXpath.py` & `PrSpiders-0.3.6/PrSpider/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.5/PrSpider/useragent.py` & `PrSpiders-0.3.6/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.5/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.3.6/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.3.5
+Version: 0.3.6
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.3.5/README.md` & `PrSpiders-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.5/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.3.6/pkg/prspider/PrSpider_CMD.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # encoding:utf-8
 
-from ..prspider import __version__
+from pkg import __version__
 import argparse
 
 from .start import start_code
 
 
 def get_version():
     return __version__
```

### Comparing `PrSpiders-0.3.5/setup.py` & `PrSpiders-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

