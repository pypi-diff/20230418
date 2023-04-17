# Comparing `tmp/arfindata-0.1.2.tar.gz` & `tmp/arfindata-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\arfindata-0.1.2.tar", last modified: Mon Apr 17 23:02:40 2023, max compression
+gzip compressed data, was "dist\arfindata-0.1.3.tar", last modified: Mon Apr 17 23:21:34 2023, max compression
```

## Comparing `arfindata-0.1.2.tar` & `arfindata-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 23:02:40.914668 arfindata-0.1.2/
--rw-rw-rw-   0        0        0     1088 2023-04-17 19:43:26.000000 arfindata-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0      332 2023-04-17 23:02:40.914668 arfindata-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     3842 2023-04-17 22:09:45.000000 arfindata-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-17 23:02:40.914668 arfindata-0.1.2/arfindata/
--rw-rw-rw-   0        0        0     3241 2023-04-17 21:21:22.000000 arfindata-0.1.2/arfindata/ARdata.py
--rw-rw-rw-   0        0        0       98 2023-04-17 19:35:47.000000 arfindata-0.1.2/arfindata/__init__.py
--rw-rw-rw-   0        0        0     4140 2023-04-17 19:58:46.000000 arfindata-0.1.2/arfindata/sh.py
--rw-rw-rw-   0        0        0     5036 2023-04-17 20:00:18.000000 arfindata-0.1.2/arfindata/sz.py
-drwxrwxrwx   0        0        0        0 2023-04-17 23:02:40.914668 arfindata-0.1.2/arfindata.egg-info/
--rw-rw-rw-   0        0        0      332 2023-04-17 23:02:40.000000 arfindata-0.1.2/arfindata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      268 2023-04-17 23:02:40.000000 arfindata-0.1.2/arfindata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 23:02:40.000000 arfindata-0.1.2/arfindata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-17 23:02:40.000000 arfindata-0.1.2/arfindata.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-17 23:02:40.000000 arfindata-0.1.2/arfindata.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-17 23:02:40.914668 arfindata-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      838 2023-04-17 23:01:02.000000 arfindata-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:21:34.341949 arfindata-0.1.3/
+-rw-rw-rw-   0        0        0     1088 2023-04-17 19:43:26.000000 arfindata-0.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0      332 2023-04-17 23:21:34.340951 arfindata-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3842 2023-04-17 22:09:45.000000 arfindata-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-17 23:21:34.325578 arfindata-0.1.3/arfindata/
+-rw-rw-rw-   0        0        0     3241 2023-04-17 21:21:22.000000 arfindata-0.1.3/arfindata/ARdata.py
+-rw-rw-rw-   0        0        0       98 2023-04-17 19:35:47.000000 arfindata-0.1.3/arfindata/__init__.py
+-rw-rw-rw-   0        0        0     4200 2023-04-17 23:19:24.000000 arfindata-0.1.3/arfindata/sh.py
+-rw-rw-rw-   0        0        0     5096 2023-04-17 23:19:25.000000 arfindata-0.1.3/arfindata/sz.py
+drwxrwxrwx   0        0        0        0 2023-04-17 23:21:34.338957 arfindata-0.1.3/arfindata.egg-info/
+-rw-rw-rw-   0        0        0      332 2023-04-17 23:21:33.000000 arfindata-0.1.3/arfindata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      268 2023-04-17 23:21:34.000000 arfindata-0.1.3/arfindata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-17 23:21:33.000000 arfindata-0.1.3/arfindata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-04-17 23:21:33.000000 arfindata-0.1.3/arfindata.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-17 23:21:33.000000 arfindata-0.1.3/arfindata.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-17 23:21:34.341949 arfindata-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      838 2023-04-17 23:19:34.000000 arfindata-0.1.3/setup.py
```

### Comparing `arfindata-0.1.2/LICENSE.txt` & `arfindata-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.2/README.md` & `arfindata-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.2/arfindata/ARdata.py` & `arfindata-0.1.3/arfindata/ARdata.py`

 * *Files identical despite different names*

### Comparing `arfindata-0.1.2/arfindata/sh.py` & `arfindata-0.1.3/arfindata/sh.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 
 
 import pandas as pd
 import re
 import time
 import os
 from selenium.webdriver.common.by import By
+from selenium import webdriver
 
-
+browser = webdriver.Chrome()
 
 def select_sh(data): #筛选沪市股票代码
     sh=['6','900']
     lst = [ x for x in data for startcode in sh if x[:3].startswith(startcode)==True ]
     df = pd.DataFrame(lst,columns=['code'])
     return df
```

### Comparing `arfindata-0.1.2/arfindata/sz.py` & `arfindata-0.1.3/arfindata/sz.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,17 @@
 import pandas as pd
 import re
 import time
 import os
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.common.action_chains import ActionChains
+from selenium import webdriver
 
-
+browser = webdriver.Chrome()
 
 def select_sz(data): #筛选深市股票代码
      sz=['200','300','301','00','080']   #深市股票代码A股是以000开头；深市B股代码是以200开头；中小板股票以002开头；
                                          #深市创业板的股票是以300、301开头(比如第一只创业板股票特锐德)。
                                          #另外新股申购代码以00开头、配股代码以080开头。
      lst = [ x for x in data for startcode in sz if x[:3].startswith(startcode)==True ]
      df = pd.DataFrame(lst,columns=['code'])
```

### Comparing `arfindata-0.1.2/setup.py` & `arfindata-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'arfindata'
 DESCRIPTION = "Python package for the aquisition and pre-treatment of China's listed companies' annual reports"
 URL = 'https://github.com/napstablook04/ARfindata'
 EMAIL = 'linkfr@163.com'    # 你的邮箱
 AUTHOR = 'linkfr'     # 你的名字
 REQUIRES_PYTHON = '>=3.6.0' # 项目支持的python版本
-VERSION = '0.1.2'           # 项目版本号
+VERSION = '0.1.3'           # 项目版本号
 REQUIRED = ['pandas','selenium','fitz','pdfplumber','requests']
 
 setup(
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
     author=AUTHOR,
```

