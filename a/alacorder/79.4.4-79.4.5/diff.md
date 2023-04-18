# Comparing `tmp/alacorder-79.4.4.tar.gz` & `tmp/alacorder-79.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-79.4.4.tar", max compression
+gzip compressed data, was "alacorder-79.4.5.tar", max compression
```

## Comparing `alacorder-79.4.4.tar` & `alacorder-79.4.5.tar`

### file list

```diff
@@ -1,14 +1,5 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.4.4/LICENSE
--rw-r--r--   0        0        0     9974 2023-04-17 22:44:04.290109 alacorder-79.4.4/README.md
--rw-r--r--   0        0        0      682 2023-04-18 01:16:26.768476 alacorder-79.4.4/pyproject.toml
--rw-r--r--   0        0        0       72 2023-04-18 00:34:28.695299 alacorder-79.4.4/src/alacorder/.ipynb_checkpoints/Untitled-checkpoint.ipynb
--rw-r--r--   0        0        0        7 2023-03-29 02:30:55.845385 alacorder-79.4.4/src/alacorder/.python-version
--rw-r--r--   0        0        0     2129 2023-03-28 18:45:29.612372 alacorder-79.4.4/src/alacorder/__init__.py
--rw-r--r--   0        0        0   131800 2023-04-18 01:15:45.116930 alacorder-79.4.4/src/alacorder/__main__.py
--rw-r--r--   0        0        0   131800 2023-04-18 01:15:50.291900 alacorder-79.4.4/src/alacorder/alac.py
--rw-r--r--   0        0        0   123492 2023-04-18 01:16:10.865431 alacorder-79.4.4/src/alacorder/graphical.py
--rw-r--r--   0        0        0    53236 2023-03-30 00:46:11.281022 alacorder-79.4.4/src/alacorder/img/alac.icns
--rw-r--r--   0        0        0    99678 2023-04-17 22:01:20.160909 alacorder-79.4.4/src/alacorder/img/alac.ico
--rw-r--r--   0        0        0     8334 2023-03-23 21:38:13.000000 alacorder-79.4.4/src/alacorder/img/alac.png
--rw-r--r--   0        0        0      162 2023-04-17 22:02:29.686094 alacorder-79.4.4/src/alacorder/~$E 302 Portfolio.docx
--rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 alacorder-79.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-79.4.5/LICENSE
+-rw-r--r--   0        0        0     9974 2023-04-17 22:44:04.290109 alacorder-79.4.5/README.md
+-rw-r--r--   0        0        0   132623 2023-04-18 13:47:03.977909 alacorder-79.4.5/alacorder.py
+-rw-r--r--   0        0        0      682 2023-04-18 13:49:49.601984 alacorder-79.4.5/pyproject.toml
+-rw-r--r--   0        0        0    10865 1970-01-01 00:00:00.000000 alacorder-79.4.5/PKG-INFO
```

### Comparing `alacorder-79.4.4/LICENSE` & `alacorder-79.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.4/README.md` & `alacorder-79.4.5/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-79.4.4/pyproject.toml` & `alacorder-79.4.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "79.4.4"
+version = "79.4.5"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-79.4.4/src/alacorder/__main__.py` & `alacorder-79.4.5/alacorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """
  ┌─┐┌─┐┬─┐┌┬┐┬ ┬┌┬┐┌─┐┬ ┬┌┐┌┌┬┐┌─┐┬┌┐┌
  ├─┘├─┤├┬┘ │ └┬┘││││ ││ ││││ │ ├─┤││││
  ┴  ┴ ┴┴└─ ┴  ┴ ┴ ┴└─┘└─┘┘└┘ ┴ ┴ ┴┴┘└┘
  ALACORDER 79
 
- Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, click, selenium, click, tqdm, xlsxwriter, xlsx2csv
- (c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
+Dependencies: python 3.9+, polars, PyMuPDF, PySimpleGUI, click, selenium, click, tqdm, xlsxwriter, xlsx2csv
+(c) 2023 Sam Robson <sbrobson@crimson.ua.edu>
  
 """
 
 name = "ALACORDER"
-version = "79.4.4"
+version = "79.4.5"
 long_version = "partymountain"
 
 autoload_graphical_user_interface = False
 
 import click, fitz, os, sys, time, glob, inspect, math, re, warnings, xlsxwriter, threading, platform, selenium
 from tqdm.auto import tqdm
 import polars as pl
@@ -994,15 +994,25 @@
                 "attorneys",
                 "images",
             ],
             cf=cf,
         )
     if window:
         window.write_event_value("COMPLETE-TB", True)
-    return ca, ch, fs, settings, cas, wit, att, img
+    out = {
+    'cases': ca,
+    'charges': ch,
+    'fees': fs,
+    'settings': settings,
+    'case-action-summary': cas,
+    'witnesses': wit,
+    'attorneys': att,
+    'images': img
+    }
+    return out
 
 
 def cases(cf, window=None, debug=False):
     """
     Start cases table collection using configuration object `cf`.
     """
     df = read(cf, window)
@@ -1174,14 +1184,35 @@
     if window:
         window.write_event_value("COMPLETE-MA", True)
     return a
 
 
 #   #   #   #         CONFIGURATION & I/O        #   #   #   #
 
+def conf(inputs,
+    outputs=None,
+    count=0,
+    table="",
+    archive=False,
+    no_prompt=True,
+    debug=False,
+    overwrite=False,
+    no_write=False,
+    fetch=False,
+    cID="",
+    uID="",
+    pwd="",
+    qmax=0,
+    qskip=0,
+    append=False,
+    window=None,
+    force=False,
+    no_update=False,
+    now=False,):
+    return set(inputs=inputs, outputs=outputs, count=count, table=table, archive=archive, no_prompt=no_prompt, debug=debug, overwrite=overwrite, no_write=no_write, fetch=fetch, cID=cID, uID=uID, pwd=pwd, qmax=qmax, qskip=qskip, append=append, window=window, force=force, no_update=no_update, now=now)
 
 def set(
     inputs,
     outputs=None,
     count=0,
     table="",
     archive=False,
@@ -2617,21 +2648,22 @@
             .alias("SHORTCASENO"),
             pl.col("AllPagesText")
             .str.extract(r"(?:County: )(\d{2})")
             .alias("SHORTCOUNTY"),
             pl.col("AllPagesText")
             .str.replace_all(r"\n", "")
             .str.extract(r"(Settings.+Court Action)", group_index=1)
-            .str.replace_all(r"Settings   Date: Que: Time: Description:   Settings", "")
-            .str.replace_all(r"Settings   Settings Date: Que: Time: Description:", "")
-            .str.replace_all(
+            .str.replace(r"Settings   Date: Que: Time: Description:   Settings", "")
+            .str.replace(r"Settings   Settings Date: Que: Time: Description:", "")
+            .str.replace(
                 r"Disposition Charges   # Code Court Action Category Cite Court Action",
                 "",
             )
-            .str.replace_all(r"Court Action.+", "")
+            .str.replace(r"Parties Party 1 - Plaintiff","")
+            .str.replace(r"Court Action.+", "")
             .str.strip()
             .alias("Settings"),
         ]
     )
     settings = settings.select(
         [
             pl.concat_str(
```

### Comparing `alacorder-79.4.4/PKG-INFO` & `alacorder-79.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 79.4.4
+Version: 79.4.5
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

