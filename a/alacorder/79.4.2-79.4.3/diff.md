# Comparing `tmp/alacorder-79.4.2.tar.gz` & `tmp/alacorder-79.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.4.2.tar", max compression
+gzip compressed data, was "alacorder-79.4.3.tar", max compression
```

## Comparing `alacorder-79.4.2.tar` & `alacorder-79.4.3.tar`

### file list

```diff
@@ -1,15 +1,14 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.4.2/LICENSE
--rw-r--r--   0        0        0     9974 2023-04-17 22:44:04.290109 alacorder-79.4.2/README.md
--rw-r--r--   0        0        0      682 2023-04-18 01:08:56.617913 alacorder-79.4.2/pyproject.toml
--rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.4.2/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.4.2/src/alacorder/.python-version
--rw-r--r--   0        0        0     5509 2023-04-18 00:53:37.301612 alacorder-79.4.2/src/alacorder/Untitled.ipynb
--rw-r--r--   0        0        0     2129 2023-03-28 18:45:29.612372 alacorder-79.4.2/src/alacorder/__init__.py
--rw-r--r--   0        0        0   131800 2023-04-18 00:59:59.107035 alacorder-79.4.2/src/alacorder/__main__.py
--rw-r--r--   0        0        0   131800 2023-04-18 00:59:59.107035 alacorder-79.4.2/src/alacorder/alac.py
--rw-r--r--   0        0        0   123499 2023-04-18 01:01:08.347561 alacorder-79.4.2/src/alacorder/graphical.py
--rw-r--r--   0        0        0    53236 2023-03-30 00:46:11.281022 alacorder-79.4.2/src/alacorder/img/alac.icns
--rw-r--r--   0        0        0    99678 2023-04-17 22:01:20.160909 alacorder-79.4.2/src/alacorder/img/alac.ico
--rw-r--r--   0        0        0     8334 2023-03-23 21:38:13.000000 alacorder-79.4.2/src/alacorder/img/alac.png
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.4.2/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 alacorder-79.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.4.3/LICENSE
+-rw-r--r--   0        0        0     9974 2023-04-17 22:44:04.290109 alacorder-79.4.3/README.md
+-rw-r--r--   0        0        0      682 2023-04-18 01:13:58.410187 alacorder-79.4.3/pyproject.toml
+-rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.4.3/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
+-rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.4.3/src/alacorder/.python-version
+-rw-r--r--   0        0        0     2129 2023-03-28 18:45:29.612372 alacorder-79.4.3/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   131800 2023-04-18 01:13:36.618609 alacorder-79.4.3/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   131800 2023-04-18 01:13:40.471267 alacorder-79.4.3/src/alacorder/alac.py
+-rw-r--r--   0        0        0   123499 2023-04-18 01:13:47.812484 alacorder-79.4.3/src/alacorder/graphical.py
+-rw-r--r--   0        0        0    53236 2023-03-30 00:46:11.281022 alacorder-79.4.3/src/alacorder/img/alac.icns
+-rw-r--r--   0        0        0    99678 2023-04-17 22:01:20.160909 alacorder-79.4.3/src/alacorder/img/alac.ico
+-rw-r--r--   0        0        0     8334 2023-03-23 21:38:13.000000 alacorder-79.4.3/src/alacorder/img/alac.png
+-rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.4.3/src/alacorder/~$E 302 Portfolio.docx
+-rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 alacorder-79.4.3/PKG-INFO
```

### Comparing `alacorder-79.4.2/LICENSE` & `alacorder-79.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.2/README.md` & `alacorder-79.4.3/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.2/pyproject.toml` & `alacorder-79.4.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.4.2"
+version = "79.4.3"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.4.2/src/alacorder/__init__.py` & `alacorder-79.4.3/src/alacorder/__init__.py`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.2/src/alacorder/__main__.py` & `alacorder-79.4.3/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
  Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, click, selenium, click, tqdm, xlsxwriter, xlsx2csv
  (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.2"
+version = "79.4.3"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
```

### Comparing `alacorder-79.4.2/src/alacorder/alac.py` & `alacorder-79.4.3/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
  Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, click, selenium, click, tqdm, xlsxwriter, xlsx2csv
  (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.2"
+version = "79.4.3"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
```

### Comparing `alacorder-79.4.2/src/alacorder/graphical.py` & `alacorder-79.4.3/src/alacorder/graphical.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
  Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, selenium, click, tqdm, xlsxwriter, xlsx2csv
  (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.2"
+version = "79.4.3"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = True
 
 import fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
```

### Comparing `alacorder-79.4.2/src/alacorder/img/alac.icns` & `alacorder-79.4.3/src/alacorder/img/alac.icns`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.2/src/alacorder/img/alac.ico` & `alacorder-79.4.3/src/alacorder/img/alac.ico`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.2/src/alacorder/img/alac.png` & `alacorder-79.4.3/src/alacorder/img/alac.png`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.2/PKG-INFO` & `alacorder-79.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.4.2
+Version: 79.4.3
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

