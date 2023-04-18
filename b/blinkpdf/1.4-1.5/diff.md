# Comparing `tmp/blinkpdf-1.4.tar.gz` & `tmp/blinkpdf-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blinkpdf-1.4.tar", last modified: Fri Apr 30 08:31:10 2021, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `blinkpdf-1.4.tar` & `blinkpdf-1.5.tar`

### file list

```diff
@@ -1,15 +1,7 @@
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-04-30 08:31:10.654461 blinkpdf-1.4/
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1324 2021-04-30 08:31:10.654461 blinkpdf-1.4/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      346 2021-02-19 16:48:26.000000 blinkpdf-1.4/README.md
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-04-30 08:31:10.654461 blinkpdf-1.4/blinkpdf/
--rw-r--r--   0 ntome     (1000) ntome     (1000)       20 2021-04-30 08:30:39.000000 blinkpdf-1.4/blinkpdf/__init__.py
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)     4273 2021-04-30 08:19:42.000000 blinkpdf-1.4/blinkpdf/__main__.py
-drwxr-xr-x   0 ntome     (1000) ntome     (1000)        0 2021-04-30 08:31:10.654461 blinkpdf-1.4/blinkpdf.egg-info/
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1324 2021-04-30 08:31:09.000000 blinkpdf-1.4/blinkpdf.egg-info/PKG-INFO
--rw-r--r--   0 ntome     (1000) ntome     (1000)      264 2021-04-30 08:31:09.000000 blinkpdf-1.4/blinkpdf.egg-info/SOURCES.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        1 2021-04-30 08:31:09.000000 blinkpdf-1.4/blinkpdf.egg-info/dependency_links.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       53 2021-04-30 08:31:09.000000 blinkpdf-1.4/blinkpdf.egg-info/entry_points.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)       20 2021-04-30 08:31:09.000000 blinkpdf-1.4/blinkpdf.egg-info/requires.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)        9 2021-04-30 08:31:09.000000 blinkpdf-1.4/blinkpdf.egg-info/top_level.txt
--rw-r--r--   0 ntome     (1000) ntome     (1000)     1010 2021-04-30 08:31:10.658461 blinkpdf-1.4/setup.cfg
--rwxr-xr-x   0 ntome     (1000) ntome     (1000)      138 2021-02-19 16:03:16.000000 blinkpdf-1.4/setup.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 blinkpdf-1.5/blinkpdf/__init__.py
+-rwxr-xr-x   0        0        0     4311 2020-02-02 00:00:00.000000 blinkpdf-1.5/blinkpdf/__main__.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 blinkpdf-1.5/.gitignore
+-rw-r--r--   0        0        0     1211 2020-02-02 00:00:00.000000 blinkpdf-1.5/LICENSE
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 blinkpdf-1.5/README.md
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 blinkpdf-1.5/pyproject.toml
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 blinkpdf-1.5/PKG-INFO
```

### Comparing `blinkpdf-1.4/PKG-INFO` & `blinkpdf-1.5/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: blinkpdf
-Version: 1.4
+Version: 1.5
 Summary: Blink-based webpage-to-pdf converter
-Home-page: https://gitlab.com/hydrargyrum/blinkpdf
-Author: Hg
-Author-email: dev@indigo.re
-Maintainer: Hg
-Maintainer-email: dev@indigo.re
-License: UNKNOWN
-Description: BlinkPDF is yet another webpage-to-pdf converter.
-        
-        It uses PyQt5 and QtWebEngine (with Blink engine) to do so.
-        
-        Pass an URL and an output filename, the page will be retrieved and converted
-        to PDF. Additionally, it can be given custom cookies and headers and also
-        some javascript code to execute (if needing to perform custom tweaks to
-        the page).
-        
-Platform: UNKNOWN
+Project-URL: Homepage, https://gitlab.com/hydrargyrum/blinkpdf
+Author-email: Hg <dev@indigo.re>
+License-Expression: Unlicense
+License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Environment :: No Input/Output (Daemon)
 Classifier: Intended Audience :: Developers
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: License :: Public Domain
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Utilities
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Printing
+Classifier: Topic :: Utilities
 Requires-Python: >=3.5
+Requires-Dist: pyqt5
+Requires-Dist: pyqtwebengine
+Description-Content-Type: text/markdown
+
+BlinkPDF is yet another webpage-to-pdf converter.
+
+It uses PyQt5 and QtWebEngine (with Blink engine) to do so.
+
+Pass an URL and an output filename, the page will be retrieved and converted
+to PDF. Additionally, it can be given custom cookies and headers and also
+some javascript code to execute (if needing to perform custom tweaks to
+the page).
```

### Comparing `blinkpdf-1.4/blinkpdf/__main__.py` & `blinkpdf-1.5/blinkpdf/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 #!/usr/bin/env python3
+# SPDX-License-Identifier: Unlicense
+
 # This is free and unencumbered software released into the public domain.
 # For more information, please refer to <http://unlicense.org/>
 # or LICENSE file
 
 from argparse import ArgumentParser
 from contextlib import contextmanager
 import os
```

