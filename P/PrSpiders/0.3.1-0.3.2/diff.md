# Comparing `tmp/PrSpiders-0.3.1.tar.gz` & `tmp/PrSpiders-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.3.1.tar", last modified: Mon Apr 17 12:23:30 2023, max compression
+gzip compressed data, was "PrSpiders-0.3.2.tar", last modified: Tue Apr 18 02:50:26 2023, max compression
```

## Comparing `PrSpiders-0.3.1.tar` & `PrSpiders-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:30.123780 PrSpiders-0.3.1/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.1/LICENSE.txt
--rw-rw-rw-   0        0        0     4465 2023-04-17 12:23:30.120779 PrSpiders-0.3.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:29.854781 PrSpiders-0.3.1/PrSpider/
--rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.1/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.1/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11166 2023-04-17 02:59:19.000000 PrSpiders-0.3.1/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4196 2023-04-17 09:57:49.000000 PrSpiders-0.3.1/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.1/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:30.029776 PrSpiders-0.3.1/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4465 2023-04-17 12:23:29.000000 PrSpiders-0.3.1/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-04-17 12:23:29.000000 PrSpiders-0.3.1/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 12:23:29.000000 PrSpiders-0.3.1/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-17 12:23:29.000000 PrSpiders-0.3.1/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-17 12:23:29.000000 PrSpiders-0.3.1/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       38 2023-04-17 12:23:29.000000 PrSpiders-0.3.1/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3953 2023-04-12 08:30:03.000000 PrSpiders-0.3.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:30.069779 PrSpiders-0.3.1/pkg/
--rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.3.1/pkg/__init.py
--rw-rw-rw-   0        0        0        0 2023-04-17 12:21:36.000000 PrSpiders-0.3.1/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:30.083779 PrSpiders-0.3.1/pkg/prspider/
--rw-rw-rw-   0        0        0     1164 2023-04-17 12:23:25.000000 PrSpiders-0.3.1/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.1/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.1/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      492 2023-03-31 06:15:13.000000 PrSpiders-0.3.1/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:30.105776 PrSpiders-0.3.1/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.3.1/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8883 2023-03-22 07:44:13.000000 PrSpiders-0.3.1/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.3.1/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.1/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-17 12:23:30.124784 PrSpiders-0.3.1/setup.cfg
--rw-rw-rw-   0        0        0     1020 2023-04-17 12:23:25.000000 PrSpiders-0.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-17 12:23:30.117780 PrSpiders-0.3.1/table_parse/
--rw-rw-rw-   0        0        0   282891 2023-03-22 06:00:42.000000 PrSpiders-0.3.1/table_parse/T.py
--rw-rw-rw-   0        0        0        0 2023-03-22 06:03:34.000000 PrSpiders-0.3.1/table_parse/__init__.py
--rw-rw-rw-   0        0        0     3005 2023-03-22 08:01:31.000000 PrSpiders-0.3.1/table_parse/tb_parse.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.601161 PrSpiders-0.3.2/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.3.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-18 02:50:26.566156 PrSpiders-0.3.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 02:50:25.974155 PrSpiders-0.3.2/PrSpider/
+-rw-rw-rw-   0        0        0     9065 2023-04-10 14:06:53.000000 PrSpiders-0.3.2/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.3.2/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11166 2023-04-17 02:59:19.000000 PrSpiders-0.3.2/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4073 2023-04-18 02:20:24.000000 PrSpiders-0.3.2/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.3.2/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.189157 PrSpiders-0.3.2/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      474 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-18 02:50:23.000000 PrSpiders-0.3.2/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.3.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.276159 PrSpiders-0.3.2/pkg/
+-rw-rw-rw-   0        0        0        0 2023-03-31 05:23:03.000000 PrSpiders-0.3.2/pkg/__init.py
+-rw-rw-rw-   0        0        0        0 2023-04-17 12:21:36.000000 PrSpiders-0.3.2/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-18 02:50:26.504165 PrSpiders-0.3.2/pkg/prspider/
+-rw-rw-rw-   0        0        0     1166 2023-04-18 02:49:55.000000 PrSpiders-0.3.2/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.3.2/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.3.2/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.3.2/pkg/prspider/start.py
+-rw-rw-rw-   0        0        0       42 2023-04-18 02:50:26.602157 PrSpiders-0.3.2/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-18 02:49:58.000000 PrSpiders-0.3.2/setup.py
```

### Comparing `PrSpiders-0.3.1/LICENSE.txt` & `PrSpiders-0.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.1/PrSpider/PrSpiders.py` & `PrSpiders-0.3.2/PrSpider/PrSpiders.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.1/PrSpider/pxpath.py` & `PrSpiders-0.3.2/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.1/PrSpider/requestXpath.py` & `PrSpiders-0.3.2/PrSpider/requestXpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,33 +110,30 @@
         return self.response.status_code
 
     @property
     def headers(self):
         return self.response.headers
 
     @property
-    def get_len(self):
+    def len(self):
         return len(self.response.text)
 
     @property
     def tree(self):
         return Xpath(self.response.text)
 
     def xpath(self, xpath_str, **kwargs):
         return Xpath(self.response.text).xpath(xpath_str, **kwargs)
 
-    def xxpath(self, xpath_str, **kwargs):
-        return Xpath(self.response.text).xxpath(xpath_str, **kwargs)
-
     @property
     def ok(self):
         return self.response.ok
 
     @property
     def meta(self):
         return self.meta_
 
     def close(self):
         self.response.close()
 
     def __str__(self) -> str:
-        return f"<Request Code={self.code} Len={self.get_len}>"
+        return f"<Response Code={self.code} Len={self.len}>"
```

### Comparing `PrSpiders-0.3.1/PrSpider/useragent.py` & `PrSpiders-0.3.2/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.3.1/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.3.2/pkg/prspider/PrSpider_CMD.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # encoding:utf-8
 
-__version__ = "v.0.3.1"
+__version__ = "v.0.3.2"
 
 import argparse
 
 from .start import start_code
 
 
 def get_version():
-    return "1.0.0.0"
+    return __version__
 
 
 def main():
     # args = docopt(__doc__, version=__version__)
     # print(args)
 
     parse = argparse.ArgumentParser()  # 创建参数对象
```

### Comparing `PrSpiders-0.3.1/setup.py` & `PrSpiders-0.3.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
-__version__ = '0.3.1'
 
-with open("README.md", "r", encoding='utf-8') as fh:
+__version__ = "0.3.2"
+
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
     author="penr",
     author_email="1944542244@qq.com",
```

