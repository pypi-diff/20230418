# Comparing `tmp/jdDesktopEntryEdit-1.0.tar.gz` & `tmp/jdDesktopEntryEdit-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jdDesktopEntryEdit-1.0.tar", last modified: Sat Feb  4 12:22:09 2023, max compression
+gzip compressed data, was "jdDesktopEntryEdit-1.1.tar", last modified: Tue Apr 18 12:31:58 2023, max compression
```

## Comparing `jdDesktopEntryEdit-1.0.tar` & `jdDesktopEntryEdit-1.1.tar`

### file list

```diff
@@ -1,47 +1,51 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 12:22:09.309864 jdDesktopEntryEdit-1.0/
--rw-r--r--   0 root         (0) root         (0)     1931 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/BuildBackend.py
--rw-r--r--   0 root         (0) root         (0)    35080 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      197 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1267 2023-02-04 12:22:09.309864 jdDesktopEntryEdit-1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       76 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 12:22:09.305864 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/
--rw-r--r--   0 root         (0) root         (0)      575 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/AboutDialog.py
--rw-r--r--   0 root         (0) root         (0)     3045 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/AboutDialog.ui
--rw-r--r--   0 root         (0) root         (0)     4774 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/EditActionDialog.py
--rw-r--r--   0 root         (0) root         (0)     2139 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/EditActionDialog.ui
--rw-r--r--   0 root         (0) root         (0)     3792 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py
--rw-r--r--   0 root         (0) root         (0)     3182 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Environment.py
--rw-r--r--   0 root         (0) root         (0)     5475 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Functions.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Icon.svg
--rw-r--r--   0 root         (0) root         (0)     4105 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ListEditWidget.py
--rw-r--r--   0 root         (0) root         (0)    28868 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/MainWindow.py
--rw-r--r--   0 root         (0) root         (0)    20748 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/MainWindow.ui
--rw-r--r--   0 root         (0) root         (0)     4812 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ManageTemplatesWindow.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ManageTemplatesWindow.ui
--rw-r--r--   0 root         (0) root         (0)     2518 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/PreviewDialog.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/PreviewDialog.ui
--rw-r--r--   0 root         (0) root         (0)     1591 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Settings.py
--rw-r--r--   0 root         (0) root         (0)     3649 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/SettingsDialog.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/SettingsDialog.ui
--rw-r--r--   0 root         (0) root         (0)     4044 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/TranslateDialog.py
--rw-r--r--   0 root         (0) root         (0)     1649 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/TranslateDialog.ui
--rw-r--r--   0 root         (0) root         (0)      787 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ValidationDialog.py
--rw-r--r--   0 root         (0) root         (0)     2124 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ValidationDialog.ui
--rw-r--r--   0 root         (0) root         (0)      831 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/WelcomeDialog.py
--rw-r--r--   0 root         (0) root         (0)     3740 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/WelcomeDialog.ui
--rw-r--r--   0 root         (0) root         (0)     1862 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/__init__.py
--rw-r--r--   0 root         (0) root         (0)       26 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 12:22:09.305864 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/data/
--rw-r--r--   0 root         (0) root         (0)     1405 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/data/categories.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 12:22:09.305864 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/translations/
--rw-r--r--   0 root         (0) root         (0)    42280 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts
--rw-r--r--   0 root         (0) root         (0)        3 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/version.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-04 12:22:09.305864 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1267 2023-02-04 12:22:09.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1389 2023-02-04 12:22:09.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-04 12:22:09.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       59 2023-02-04 12:22:09.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-02-04 12:22:09.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2023-02-04 12:22:09.000000 jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1500 2023-02-04 12:21:28.000000 jdDesktopEntryEdit-1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-02-04 12:22:09.309864 jdDesktopEntryEdit-1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/
+-rw-r--r--   0 root         (0) root         (0)     2060 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/BuildBackend.py
+-rw-r--r--   0 root         (0) root         (0)    35080 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      197 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4119 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.257099 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/
+-rw-r--r--   0 root         (0) root         (0)     1596 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.py
+-rw-r--r--   0 root         (0) root         (0)     4427 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4774 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.py
+-rw-r--r--   0 root         (0) root         (0)     2139 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     3792 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py
+-rw-r--r--   0 root         (0) root         (0)     3182 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Environment.py
+-rw-r--r--   0 root         (0) root         (0)     5475 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Functions.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Icon.svg
+-rw-r--r--   0 root         (0) root         (0)      297 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Languages.py
+-rw-r--r--   0 root         (0) root         (0)     4105 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ListEditWidget.py
+-rw-r--r--   0 root         (0) root         (0)    29363 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.py
+-rw-r--r--   0 root         (0) root         (0)    21447 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     4812 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.ui
+-rw-r--r--   0 root         (0) root         (0)     2518 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     1591 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Settings.py
+-rw-r--r--   0 root         (0) root         (0)     3481 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     4044 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.ui
+-rw-r--r--   0 root         (0) root         (0)      787 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.ui
+-rw-r--r--   0 root         (0) root         (0)      831 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.py
+-rw-r--r--   0 root         (0) root         (0)     3740 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.ui
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       26 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/categories.txt
+-rw-r--r--   0 root         (0) root         (0)      111 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/changelog.html
+-rw-r--r--   0 root         (0) root         (0)       39 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/translators.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/
+-rw-r--r--   0 root         (0) root         (0)    43488 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts
+-rw-r--r--   0 root         (0) root         (0)    43020 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts
+-rw-r--r--   0 root         (0) root         (0)        3 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/version.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5309 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       59 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-04-18 12:31:58.000000 jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-04-18 12:31:18.000000 jdDesktopEntryEdit-1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 12:31:58.261098 jdDesktopEntryEdit-1.1/setup.cfg
```

### Comparing `jdDesktopEntryEdit-1.0/BuildBackend.py` & `jdDesktopEntryEdit-1.1/BuildBackend.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is used durring the build process
 from setuptools import build_meta as origin
 from typing import Optional
 import subprocess
 import tempfile
 import pathlib
 import shutil
+import sys
 import os
 
 
 TRANSLATION_DIRS = [
     "jdDesktopEntryEdit/translations"
 ]
 
@@ -30,14 +31,18 @@
 
 prepare_metadata_for_build_wheel = origin.prepare_metadata_for_build_wheel
 get_requires_for_build_sdist = origin.get_requires_for_build_sdist
 build_sdist = origin.build_sdist
 
 
 def build_wheel(wheel_directory, config_settings=None, metadata_directory=None):
+    if get_lrelease_command() is None:
+        print("lrealease was not found", file=sys.stderr)
+        sys.exit(1)
+
     wheel_name =  origin.build_wheel(wheel_directory, config_settings=config_settings, metadata_directory=metadata_directory)
     wheel_path = os.path.join(wheel_directory, wheel_name)
     with tempfile.TemporaryDirectory() as tempdir:
         subprocess.run(["wheel", "unpack", "--dest", tempdir, wheel_path])
         current_dir = os.path.join(tempdir, os.listdir(tempdir)[0])
         build_translations(current_dir)
         try:
```

### Comparing `jdDesktopEntryEdit-1.0/LICENSE` & `jdDesktopEntryEdit-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/PKG-INFO` & `jdDesktopEntryEdit-1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,49 @@
-Metadata-Version: 2.1
-Name: jdDesktopEntryEdit
-Version: 1.0
-Summary: A graphical Program to create and edit Desktop Entries
-Author-email: JakobDev <jakobdev@gmx.de>
-License: GPL-3
-Project-URL: Source, https://codeberg.org/JakobDev/jdDesktopEntryEdit
-Project-URL: Issues, https://codeberg.org/JakobDev/jdDesktopEntryEdit/issues
-Project-URL: Donation, https://ko-fi.com/jakobdev
-Keywords: JakobDev,Linux,.desktop,freedesktop
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Environment :: Other Environment
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: POSIX :: BSD
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+[build-system]
+requires = ["setuptools"]
+build-backend = "BuildBackend"
+backend-path = ["."]
 
-# jdDesktopEntryEdit
+[project]
+name = "jdDesktopEntryEdit"
+description = "A graphical Program to create and edit Desktop Entries"
+readme = "README.md"
+requires-python = ">=3.10"
+keywords = ["JakobDev", "Linux", ".desktop", "freedesktop"]
+license = { text = "GPL-3" }
+authors = [
+    { name = "JakobDev", email = "jakobdev@gmx.de" }
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Environment :: Other Environment",
+    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
+    "Operating System :: POSIX",
+    "Operating System :: POSIX :: BSD",
+    "Operating System :: POSIX :: Linux",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: Implementation :: CPython"
+]
+dependencies = [
+  "PyQt6",
+  "desktop-entry-lib"
+]
+dynamic = ["version"]
 
-A graphical Program to create and edit Desktop Entries
+[project.urls]
+Source = "https://codeberg.org/JakobDev/jdDesktopEntryEdit"
+Issues = "https://codeberg.org/JakobDev/jdDesktopEntryEdit/issues"
+Donation = "https://ko-fi.com/jakobdev"
+
+[project.gui-scripts]
+jdDesktopEntryEdit = "jdDesktopEntryEdit:main"
+
+[tool.setuptools]
+packages = ["jdDesktopEntryEdit"]
+
+[tool.setuptools.dynamic]
+version = { file = "jdDesktopEntryEdit/version.txt" }
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/AboutDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.ui`

 * *Files 18% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/AboutDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/AboutDialog.ui`

```diff
@@ -3,15 +3,15 @@
   <class>AboutDialog</class>
   <widget class="QDialog" name="AboutDialog">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
         <width>400</width>
-        <height>300</height>
+        <height>312</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>About</string>
     </property>
     <layout class="QVBoxLayout" name="verticalLayout">
       <item>
@@ -35,80 +35,121 @@
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
         <widget class="QLabel" name="version_label">
           <property name="text">
-            <string notr="true">jdDesktopEntryEdit {version}</string>
+            <string notr="true">jdDesktopEntryEdit {{version}}</string>
           </property>
           <property name="alignment">
             <set>Qt::AlignCenter</set>
           </property>
         </widget>
       </item>
       <item>
-        <widget class="QLabel" name="label">
-          <property name="text">
-            <string>A graphical Program to create and edit Desktop Entries</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
+        <widget class="QTabWidget" name="tab_widget">
+          <property name="currentIndex">
+            <number>0</number>
+          </property>
+          <widget class="QWidget" name="tab">
+            <attribute name="title">
+              <string>About</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_2">
+              <item>
+                <widget class="QLabel" name="label">
+                  <property name="text">
+                    <string>A graphical Program to create and edit Desktop Entries</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QLabel" name="label_5">
+                  <property name="text">
+                    <string>The Icon was created by &lt;a href=&quot;https://icon-icons.com/icon/preferences-desktop-theme/93638&quot;&gt;Papirus Development Team&lt;/a&gt;</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QLabel" name="label_2">
+                  <property name="text">
+                    <string>This Program is licensed under GPL 3</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QLabel" name="label_3">
+                  <property name="text">
+                    <string notr="true">Copyright © 2023 JakobDev</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
+          <widget class="QWidget" name="tab_2">
+            <attribute name="title">
+              <string>Translators</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_3">
+              <item>
+                <widget class="QLabel" name="label_4">
+                  <property name="text">
+                    <string>The following people translated jdDesktopEntryEdit:</string>
+                  </property>
+                  <property name="alignment">
+                    <set>Qt::AlignCenter</set>
+                  </property>
+                  <property name="wordWrap">
+                    <bool>true</bool>
+                  </property>
+                </widget>
+              </item>
+              <item>
+                <widget class="QTextEdit" name="translators_edit">
+                  <property name="readOnly">
+                    <bool>true</bool>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
+          <widget class="QWidget" name="tab_3">
+            <attribute name="title">
+              <string>Changelog</string>
+            </attribute>
+            <layout class="QVBoxLayout" name="verticalLayout_4">
+              <item>
+                <widget class="QTextEdit" name="changelog_edit">
+                  <property name="readOnly">
+                    <bool>true</bool>
+                  </property>
+                </widget>
+              </item>
+            </layout>
+          </widget>
         </widget>
       </item>
       <item>
-        <widget class="QLabel" name="label_4">
+        <widget class="QPushButton" name="close_button">
           <property name="text">
-            <string>The Icon was created by &lt;a href=&quot;https://icon-icons.com/icon/preferences-desktop-theme/93638&quot;&gt;Papirus Development Team&lt;/a&gt;</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-          <property name="openExternalLinks">
-            <bool>true</bool>
+            <string>Close</string>
           </property>
         </widget>
       </item>
-      <item>
-        <widget class="QLabel" name="label_2">
-          <property name="text">
-            <string>This Program is licensed under GPL 3</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <widget class="QLabel" name="label_3">
-          <property name="text">
-            <string notr="true">Copyright © 2023 JakobDev</string>
-          </property>
-          <property name="alignment">
-            <set>Qt::AlignCenter</set>
-          </property>
-        </widget>
-      </item>
-      <item>
-        <layout class="QHBoxLayout" name="horizontalLayout">
-          <item>
-            <widget class="QPushButton" name="view_source_button">
-              <property name="text">
-                <string>View source</string>
-              </property>
-            </widget>
-          </item>
-          <item>
-            <widget class="QPushButton" name="close_button">
-              <property name="text">
-                <string>Close</string>
-              </property>
-            </widget>
-          </item>
-        </layout>
-      </item>
     </layout>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/EditActionDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/EditActionDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditActionDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/EditKeywordsTranslationDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Environment.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Environment.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Functions.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Functions.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Icon.svg` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Icon.svg`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ListEditWidget.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ListEditWidget.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/MainWindow.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,18 @@
         self.manage_templates_action.triggered.connect(self._manage_templates_window.open_dialog)
 
         self.validate_action.triggered.connect(self._validation_dialog.open_dialog)
         self.preview_action.triggered.connect(lambda: self._preview_dialog.open_preview(self.get_desktop_entry().get_text()))
 
         self.welcome_dialog_action.triggered.connect(self._welcome_dialog.open_dialog)
         self.specification_action.triggered.connect(lambda: webbrowser.open("https://specifications.freedesktop.org/desktop-entry-spec/desktop-entry-spec-latest.html"))
+        self.view_source_action.triggered.connect(lambda: webbrowser.open("https://codeberg.org/JakobDev/jdDesktopEntryEdit"))
+        self.report_bug_action.triggered.connect(lambda: webbrowser.open("https://codeberg.org/JakobDev/jdDesktopEntryEdit/issues"))
+        self.translate_action.triggered.connect(lambda: webbrowser.open("https://translate.codeberg.org/projects/jdDesktopEntryEdit"))
+        self.donate_action.triggered.connect(lambda: webbrowser.open("https://ko-fi.com/jakobdev"))
         self.about_action.triggered.connect(self._about_dialog.exec)
         self.about_qt_action.triggered.connect(QApplication.instance().aboutQt)
 
         self.translate_name_button.clicked.connect(lambda: self._env.translate_dialog.open_dialog("Name"))
         self.translate_generic_name_button.clicked.connect(lambda: self._env.translate_dialog.open_dialog("GenericName"))
         self.translate_comment_button.clicked.connect(lambda: self._env.translate_dialog.open_dialog("Comment"))
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/MainWindow.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.ui`

 * *Files 2% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/MainWindow.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/MainWindow.ui`

```diff
@@ -496,15 +496,15 @@
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
           <width>800</width>
-          <height>30</height>
+          <height>21</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuFile">
         <property name="title">
           <string>File</string>
         </property>
         <widget class="QMenu" name="recent_files_menu">
@@ -548,14 +548,19 @@
       <widget class="QMenu" name="menu">
         <property name="title">
           <string notr="true">?</string>
         </property>
         <addaction name="welcome_dialog_action"/>
         <addaction name="specification_action"/>
         <addaction name="separator"/>
+        <addaction name="view_source_action"/>
+        <addaction name="report_bug_action"/>
+        <addaction name="translate_action"/>
+        <addaction name="donate_action"/>
+        <addaction name="separator"/>
         <addaction name="about_action"/>
         <addaction name="about_qt_action"/>
       </widget>
       <addaction name="menuFile"/>
       <addaction name="menuSettings"/>
       <addaction name="menuTools"/>
       <addaction name="menu"/>
@@ -637,11 +642,31 @@
       </property>
     </action>
     <action name="welcome_dialog_action">
       <property name="text">
         <string>Show Welcome Dialog</string>
       </property>
     </action>
+    <action name="view_source_action">
+      <property name="text">
+        <string>View Source</string>
+      </property>
+    </action>
+    <action name="report_bug_action">
+      <property name="text">
+        <string>Report Bug</string>
+      </property>
+    </action>
+    <action name="translate_action">
+      <property name="text">
+        <string>Translate</string>
+      </property>
+    </action>
+    <action name="donate_action">
+      <property name="text">
+        <string>Donate</string>
+      </property>
+    </action>
   </widget>
   <resources/>
   <connections/>
 </ui>
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ManageTemplatesWindow.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ManageTemplatesWindow.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ManageTemplatesWindow.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/PreviewDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/PreviewDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/PreviewDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/Settings.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/Settings.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/SettingsDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,32 @@
 from .Functions import select_combo_box_data
+from .Languages import get_language_names
 from PyQt6.QtCore import QCoreApplication
 from PyQt6.QtWidgets import QDialog
 from typing import TYPE_CHECKING
 from PyQt6 import uic
 import os
 
 
 if TYPE_CHECKING:
     from .Environment import Environment
     from .MainWindow import MainWindow
 
 
-
-def get_language_names() -> dict[str, str]:
-    return {
-        "en": QCoreApplication.translate("Language", "English"),
-        "de": QCoreApplication.translate("Language", "German")
-    }
-
-
 class SettingsDialog(QDialog):
     def __init__(self, env: "Environment", main_window: "MainWindow"):
         super().__init__()
         uic.loadUi(os.path.join(os.path.dirname(__file__), "SettingsDialog.ui"), self)
 
         self._env = env
         self._main_window = main_window
 
         language_names = get_language_names()
         self.language_box.addItem(QCoreApplication.translate("SettingsDialog", "System language"), "default")
-        self.language_box.addItem("Englisch", language_names.get("en", "en"))
+        self.language_box.addItem(language_names["en"], "en")
         translations_found = False
         for i in os.listdir(os.path.join(env.program_dir, "translations")):
             if i.endswith(".qm"):
                 language = i.removeprefix("jdDesktopEntryEdit_").removesuffix(".qm")
                 self.language_box.addItem(language_names.get(language, language), language)
                 translations_found = True
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/SettingsDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/SettingsDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/TranslateDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/TranslateDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/TranslateDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ValidationDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/ValidationDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/ValidationDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/WelcomeDialog.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.py`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/WelcomeDialog.ui` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/WelcomeDialog.ui`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/__init__.py` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,29 +12,31 @@
     parser.add_argument("file", nargs="?", help="The path to a file")
     args = parser.parse_known_args()[0]
 
     app = QApplication(sys.argv)
 
     env = Environment()
 
-    app.setDesktopFileName("com.gitlab.JakobDev.jdDesktopEntryEdit.desktop")
+    app.setDesktopFileName("page.codeberg.JakobDev.jdDesktopEntryEdit.desktop")
     app.setApplicationName("jdDesktopEntryEdit")
     app.setWindowIcon(env.icon)
 
     app_translator = QTranslator()
     qt_translator = QTranslator()
     app_trans_dir = os.path.join(env.program_dir, "translations")
     qt_trans_dir = QLibraryInfo.path(QLibraryInfo.LibraryPath.TranslationsPath)
     language = env.settings.get("language")
     if language == "default":
         system_language = QLocale.system().name()
         app_translator.load(os.path.join(app_trans_dir, "jdDesktopEntryEdit_" + system_language.split("_")[0] + ".qm"))
         app_translator.load(os.path.join(app_trans_dir, "jdDesktopEntryEdit_" + system_language + ".qm"))
         qt_translator.load(os.path.join(qt_trans_dir, "qt_" + system_language.split("_")[0] + ".qm"))
         qt_translator.load(os.path.join(qt_trans_dir, "qt_" + system_language + ".qm"))
+    elif language == "en":
+        pass
     else:
         app_translator.load(os.path.join(app_trans_dir, "jdDesktopEntryEdit_" + language + ".qm"))
         qt_translator.load(os.path.join(qt_trans_dir, "qt_" + language.split("_")[0] + ".qm"))
         qt_translator.load(os.path.join(qt_trans_dir, "qt_" + language + ".qm"))
     app.installTranslator(app_translator)
     app.installTranslator(qt_translator)
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/data/categories.txt` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/data/categories.txt`

 * *Files identical despite different names*

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts`

 * *Files 0% similar despite different names*

#### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts`

```diff
@@ -1,36 +1,47 @@
 <?xml version="1.0" encoding="utf-8"?>
 <!DOCTYPE TS>
 <TS version="2.1" language="de">
   <context>
     <name>AboutDialog</name>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
+      <location filename="../AboutDialog.ui" line="0"/>
       <source>About</source>
       <translation>Über</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
       <source>A graphical Program to create and edit Desktop Entries</source>
       <translation>Ein grafisches Programm zum erstellen und bearbeiten von Desktopeinträgen</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
       <source>The Icon was created by &lt;a href=&quot;https://icon-icons.com/icon/preferences-desktop-theme/93638&quot;&gt;Papirus Development Team&lt;/a&gt;</source>
-      <translation>Das Icon wurde vom &lt;a href=&quot;https://icon-icons.com/icon/preferences-desktop-theme/93638&quot;&gt;Papirus Development Team&lt;/a&gt; erstellt</translation>
+      <translation>Das icon wurde vom &lt;a href=&quot;https://icon-icons.com/icon/preferences-desktop-theme/93638&quot;&gt;Papirus Development Team&lt;/a&gt; erstellt</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
       <source>This Program is licensed under GPL 3</source>
       <translation>Dieses Programm ist unter der GPL 3 lizenziert</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
-      <source>View source</source>
-      <translation>Quelltext anzeigen</translation>
+      <source>Translators</source>
+      <translation>Übersetzer</translation>
+    </message>
+    <message>
+      <location filename="../AboutDialog.ui" line="0"/>
+      <source>The following people translated jdDesktopEntryEdit:</source>
+      <translation>Die folgenden Personen haben jdDesktopEntryEdit übersetzt:</translation>
+    </message>
+    <message>
+      <location filename="../AboutDialog.ui" line="0"/>
+      <source>Changelog</source>
+      <translation>Änderungsprotokoll</translation>
     </message>
     <message>
       <location filename="../AboutDialog.ui" line="0"/>
       <source>Close</source>
       <translation>Schließen</translation>
     </message>
   </context>
@@ -118,15 +129,15 @@
       <location filename="../EditKeywordsTranslationDialog.py" line="49"/>
       <source>You have to enter a Language</source>
       <translation>Du musst eine Sprache angeben</translation>
     </message>
     <message>
       <location filename="../EditKeywordsTranslationDialog.py" line="54"/>
       <source>Language exists</source>
-      <translation>Sprcahe existiert</translation>
+      <translation>Sprache existiert</translation>
     </message>
     <message>
       <location filename="../EditKeywordsTranslationDialog.py" line="54"/>
       <source>This Language already exists</source>
       <translation>Diese Sprache existiert bereits</translation>
     </message>
     <message>
@@ -197,23 +208,28 @@
       <source>Could not get data from the URL</source>
       <translation>Von der angegebenen URL können keine Daten erhalten werden</translation>
     </message>
   </context>
   <context>
     <name>Language</name>
     <message>
-      <location filename="../SettingsDialog.py" line="17"/>
+      <location filename="../Languages.py" line="6"/>
       <source>English</source>
       <translation>Englisch</translation>
     </message>
     <message>
-      <location filename="../SettingsDialog.py" line="18"/>
+      <location filename="../Languages.py" line="7"/>
       <source>German</source>
       <translation>Deutsch</translation>
     </message>
+    <message>
+      <location filename="../Languages.py" line="8"/>
+      <source>Dutch</source>
+      <translation>Niederländisch</translation>
+    </message>
   </context>
   <context>
     <name>ListEditWidget</name>
     <message>
       <location filename="../ListEditWidget.py" line="22"/>
       <source>Add</source>
       <translation>Hinzufügen</translation>
@@ -260,14 +276,216 @@
       <source>Please edit the Item</source>
       <translation>Bitte bearbeite das item</translation>
     </message>
   </context>
   <context>
     <name>MainWindow</name>
     <message>
+      <location filename="../MainWindow.py" line="44"/>
+      <source>A list of MimeTypes that this Application can open</source>
+      <translation>Eine Liste der MimeTypen, die das programm öffnen kann</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="45"/>
+      <source>The untranslated Keywords</source>
+      <translation>Du unübersetzten Schlüsselwörter</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="46"/>
+      <source>A list of interfaces that this application implements. If you don't know what this means, you probably won't need it.</source>
+      <translation>Eine Liste der Interfaces, die dieses programm implementiert. Wenn du nicht weisst wass es bedeutet, brauchst du es wahrscheinlich nicht.</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="47"/>
+      <source>If set, the Application is only visble when using this Desktop Environments</source>
+      <translation>Wenn gesetzt, wird der Desktopeintrag nur in diesen Desktopumgebungen angezeigt</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="48"/>
+      <source>The Application is not visble when using this Desktop Environments</source>
+      <translation>Dieser Desktopeintrag ist in diesen Desktopumgebungen nicht sichtbar</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="138"/>
+      <source>Unsaved changes</source>
+      <translation>Ungespeicherte Änderungen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="138"/>
+      <source>You have unsaved changes. Do you want to save now?</source>
+      <translation>Du hast ungespeicherte Änderungen. Möchtest du jetzt speichern?</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="148"/>
+      <source>Untitled</source>
+      <translation>Unbenannt</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="161"/>
+      <source>Error</source>
+      <translation>Fehler</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="176"/>
+      <source>No templates found</source>
+      <translation>Keine Vorlagen gefunden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="199"/>
+      <source>No recent files</source>
+      <translation>Keine zuletzt göffneten Dateien</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="212"/>
+      <source>Clear</source>
+      <translation>Löschen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="265"/>
+      <location filename="../MainWindow.py" line="238"/>
+      <source>Desktop Entries</source>
+      <translation>Desktopeinträge</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="265"/>
+      <location filename="../MainWindow.py" line="238"/>
+      <source>All Files</source>
+      <translation>Alle Dateien</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="251"/>
+      <source>Open URL</source>
+      <translation>URL öffnen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="251"/>
+      <source>Please enter the URL to the Desktop Entry</source>
+      <translation>Bitte gib die URL zum Desktopeintrag ein</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="281"/>
+      <source>Add a Categorie</source>
+      <translation>Kategorie hinzufügen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="281"/>
+      <source>Please select a Categorie from the list below</source>
+      <translation>Bitte wähle die Kategorie aus der Liste aus</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="285"/>
+      <source>Categorie already added</source>
+      <translation>Kategorie bereits vorhanden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="285"/>
+      <source>You can't add the same Categorie twice</source>
+      <translation>Du kannst nicht die gleiche Kategorie zweimal hinzufügen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="327"/>
+      <source>Delete Keywords translation</source>
+      <translation>Schlüsselwörterübersetzung löschen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="327"/>
+      <source>Are you really want to delete {{language}}?</source>
+      <translation>Bist du sicher, dass du {{language}} löschen willst?</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="344"/>
+      <source>Add Action</source>
+      <translation>Aktion hinzufügen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="344"/>
+      <source>Please enter the identifier for the new Action</source>
+      <translation>Bitte gib den Bezeichner für die neue Aktion ein</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="350"/>
+      <source>Invalid Identifier</source>
+      <translation>Ungültiger Bezeichner</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="350"/>
+      <source>This Identifier is not valid</source>
+      <translation>Dieser Bezeichner ist ungültig</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="354"/>
+      <source>Identifier exists</source>
+      <translation>Bezeichner existiert</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="354"/>
+      <source>This Identifier already exists</source>
+      <translation>Dieser Bezeichner existiert bereits</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="378"/>
+      <source>Delete Action</source>
+      <translation>Aktion löschen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="378"/>
+      <source>Are you really want to delete {{identifier}}?</source>
+      <translation>Bist du sicher, dass du {{identifier}} löschen möchtest?</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.py" line="403"/>
+      <source>Remove</source>
+      <translation>Entfernen</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="422"/>
+      <source>Invalid Key</source>
+      <translation>Ungültiger Schlüssel</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="422"/>
+      <source>{{key}} is not a valid custom Key</source>
+      <translation>{{key}} ist kein gültiger Schlüssel</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="426"/>
+      <source>Everything valid</source>
+      <translation>Alles gültig</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="426"/>
+      <source>No issues found</source>
+      <translation>Es wurden keine Probleme gefunden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="439"/>
+      <source>File not found</source>
+      <translation>Datei nicht gefunden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="439"/>
+      <source>{{path}} was not found</source>
+      <translation>{{path}} konnte nicht gefunden werden</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="468"/>
+      <location filename="../MainWindow.py" line="443"/>
+      <source>Error loading Desktop Entry</source>
+      <translation>Fehler beim Laden des Desktopeintrags</translation>
+    </message>
+    <message>
+      <location filename="../MainWindow.py" line="468"/>
+      <location filename="../MainWindow.py" line="443"/>
+      <source>This Desktop Entry couldn't be loaded. Make sure, it is in the right format.</source>
+      <translation>Dieser Desktopeintrag konnte nicht geladen werden. Stelle sicher, dass er das richtige Format hat.</translation>
+    </message>
+    <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>General</source>
       <translation>Allgemein</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Type:</source>
@@ -293,14 +511,15 @@
       <source>Name:</source>
       <translation>Name:</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
+      <location filename="../MainWindow.ui" line="0"/>
       <source>Translate</source>
       <translation>Übersetzen</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>GenericName:</source>
       <translation>GenricName:</translation>
@@ -385,22 +604,14 @@
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Add</source>
       <translation>Hinzufügen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="399"/>
-      <location filename="../MainWindow.ui" line="0"/>
-      <location filename="../MainWindow.ui" line="0"/>
-      <location filename="../MainWindow.ui" line="0"/>
-      <source>Remove</source>
-      <translation>Entfernen</translation>
-    </message>
-    <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>MimeType</source>
       <translation>MimeType</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Keywords</source>
@@ -415,15 +626,15 @@
       <location filename="../MainWindow.ui" line="0"/>
       <source>Translated</source>
       <translation>Übersetzt</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>A List of Languages in which are the Keywords translated</source>
-      <translation>Eine Lsite aller Sprachen, in die die Schlüsselwörter übersetzt sind</translation>
+      <translation>Eine Liste aller Sprachen, in die die Schlüsselwörter übersetzt sind</translation>
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Edit</source>
       <translation>Bearbeiten</translation>
     </message>
@@ -565,236 +776,32 @@
     </message>
     <message>
       <location filename="../MainWindow.ui" line="0"/>
       <source>Show Welcome Dialog</source>
       <translation>Willkommensdialog anzeigen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="44"/>
-      <source>A list of MimeTypes that this Application can open</source>
-      <translation>Eine Liste der MimeTypen, die das programm öffnen kann</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="45"/>
-      <source>The untranslated Keywords</source>
-      <translation>Du unübersetzten Schlüsselwörter</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="46"/>
-      <source>A list of interfaces that this application implements. If you don't know what this means, you probably won't need it.</source>
-      <translation>Eine Liste der Interfaces, die dieses programm implementiert. Wenn du nicht weisst wass es bedeutet, brauchst du es wahrscheinlich nicht.</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="47"/>
-      <source>If set, the Application is only visble when using this Desktop Environments</source>
-      <translation>Wenn gesetzt, wird der Desktopeintrag nur in diesen Desktopumgebungen angezeigt</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="48"/>
-      <source>The Application is not visble when using this Desktop Environments</source>
-      <translation>Dieser Desktopeintrag ist in diesen Desktopumgebungen nicht sichtbar</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="134"/>
-      <source>Unsaved changes</source>
-      <translation>Ungespeicherte Änderungen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="134"/>
-      <source>You have unsaved changes. Do you want to save now?</source>
-      <translation>Du hast ungespeicherte Änderungen. Möchtest du jetzt speichern?</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="144"/>
-      <source>Untitled</source>
-      <translation>Unbenannt</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="157"/>
-      <source>Error</source>
-      <translation>Fehler</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="172"/>
-      <source>No templates found</source>
-      <translation>Keine Vorlagen gefunden</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="195"/>
-      <source>No recent files</source>
-      <translation>Keine zuletzt göffneten Dateien</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="208"/>
-      <source>Clear</source>
-      <translation>Löschen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="261"/>
-      <location filename="../MainWindow.py" line="234"/>
-      <source>Desktop Entries</source>
-      <translation>Desktopeinträge</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="261"/>
-      <location filename="../MainWindow.py" line="234"/>
-      <source>All Files</source>
-      <translation>Alle Dateien</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="247"/>
-      <source>Open URL</source>
-      <translation>URL öffnen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="247"/>
-      <source>Please enter the URL to the Desktop Entry</source>
-      <translation>Bitte gib die URL zum Desktopeintrag ein</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="277"/>
-      <source>Add a Categorie</source>
-      <translation>Kategorie hinzufügen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="277"/>
-      <source>Please select a Categorie from the list below</source>
-      <translation>Bitte wähle die Kategorie aus der Liste aus</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="281"/>
-      <source>Categorie already added</source>
-      <translation>Kategorie bereits vorhanden</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="281"/>
-      <source>You can't add the same Categorie twice</source>
-      <translation>Du kannst nicht die gleiche Kategorie zweimal hinzufügen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="323"/>
-      <source>Delete Keywords translation</source>
-      <translation>Schlüsselwörterübersetzung löschen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="323"/>
-      <source>Are you really want to delete {{language}}?</source>
-      <translation>Bist du sicher, dass du {{language}} löschen willst?</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="340"/>
-      <source>Add Action</source>
-      <translation>Aktion hinzufügen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="340"/>
-      <source>Please enter the identifier for the new Action</source>
-      <translation>Bitte gib den Bezeichner für die neue Aktion ein</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="346"/>
-      <source>Invalid Identifier</source>
-      <translation>Ungültiger Bezeichner</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="346"/>
-      <source>This Identifier is not valid</source>
-      <translation>Dieser Bezeichner ist ungültig</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="350"/>
-      <source>Identifier exists</source>
-      <translation>Bezeichner existiert</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="350"/>
-      <source>This Identifier already exists</source>
-      <translation>Dieser Bezeichner existiert bereits</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="374"/>
-      <source>Delete Action</source>
-      <translation>Aktion löschen</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="374"/>
-      <source>Are you really want to delete {{identifier}}?</source>
-      <translation>Bist du sicher, dass du {{identifier}} löschen möchtest?</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="418"/>
-      <source>Invalid Key</source>
-      <translation>Ungültiger Schlüssel</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="418"/>
-      <source>{{key}} is not a valid custom Key</source>
-      <translation>{{key}} ist kein gültiger Schlüssel</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="422"/>
-      <source>Everything valid</source>
-      <translation>Alles gültig</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="422"/>
-      <source>No issues found</source>
-      <translation>Es wurden keine Probleme gefunden</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="435"/>
-      <source>File not found</source>
-      <translation>Datei nicht gefunden</translation>
-    </message>
-    <message>
-      <location filename="../MainWindow.py" line="435"/>
-      <source>{{path}} was not found</source>
-      <translation>{{path}} konnte nicht gefunden werden</translation>
+      <location filename="../MainWindow.ui" line="0"/>
+      <source>View Source</source>
+      <translation>Quelltext anzeigen</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="464"/>
-      <location filename="../MainWindow.py" line="439"/>
-      <source>Error loading Desktop Entry</source>
-      <translation>Fehler beim Laden des Desktopeintrags</translation>
+      <location filename="../MainWindow.ui" line="0"/>
+      <source>Report Bug</source>
+      <translation>Fehler melden</translation>
     </message>
     <message>
-      <location filename="../MainWindow.py" line="464"/>
-      <location filename="../MainWindow.py" line="439"/>
-      <source>This Desktop Entry couldn't be loaded. Make sure, it is in the right format.</source>
-      <translation>Dieser Desktopeintrag konnte nicht geladen werden. Stelle sicher, dass er das richtige Format hat.</translation>
+      <location filename="../MainWindow.ui" line="0"/>
+      <source>Donate</source>
+      <translation>Spenden</translation>
     </message>
   </context>
   <context>
     <name>ManageTemplatesWindow</name>
     <message>
-      <location filename="../ManageTemplatesWindow.ui" line="0"/>
-      <source>Manage templates</source>
-      <translation>Vorlagen verwalten</translation>
-    </message>
-    <message>
-      <location filename="../ManageTemplatesWindow.ui" line="0"/>
-      <source>Save</source>
-      <translation>Speichern</translation>
-    </message>
-    <message>
-      <location filename="../ManageTemplatesWindow.ui" line="0"/>
-      <source>Rename</source>
-      <translation>Umbennen</translation>
-    </message>
-    <message>
-      <location filename="../ManageTemplatesWindow.ui" line="0"/>
-      <source>Delete</source>
-      <translation>Löschen</translation>
-    </message>
-    <message>
-      <location filename="../ManageTemplatesWindow.ui" line="0"/>
-      <source>Close</source>
-      <translation>Schließen</translation>
-    </message>
-    <message>
       <location filename="../ManageTemplatesWindow.py" line="67"/>
       <location filename="../ManageTemplatesWindow.py" line="46"/>
       <source>Enter name</source>
       <translation>Namen eingeben</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.py" line="46"/>
@@ -840,14 +847,39 @@
       <translation>Bist du sicher, dass du {{name}} löschen möchtest?</translation>
     </message>
     <message>
       <location filename="../ManageTemplatesWindow.py" line="99"/>
       <source>A error occurred while deleting</source>
       <translation>Während des Löschens ist ein Fehler aufgetreten</translation>
     </message>
+    <message>
+      <location filename="../ManageTemplatesWindow.ui" line="0"/>
+      <source>Manage templates</source>
+      <translation>Vorlagen verwalten</translation>
+    </message>
+    <message>
+      <location filename="../ManageTemplatesWindow.ui" line="0"/>
+      <source>Save</source>
+      <translation>Speichern</translation>
+    </message>
+    <message>
+      <location filename="../ManageTemplatesWindow.ui" line="0"/>
+      <source>Rename</source>
+      <translation>Umbennen</translation>
+    </message>
+    <message>
+      <location filename="../ManageTemplatesWindow.ui" line="0"/>
+      <source>Delete</source>
+      <translation>Löschen</translation>
+    </message>
+    <message>
+      <location filename="../ManageTemplatesWindow.ui" line="0"/>
+      <source>Close</source>
+      <translation>Schließen</translation>
+    </message>
   </context>
   <context>
     <name>PreviewDialog</name>
     <message>
       <location filename="../PreviewDialog.ui" line="0"/>
       <source>Preview</source>
       <translation>Vorschau</translation>
@@ -867,14 +899,34 @@
       <source>Close</source>
       <translation>Schließen</translation>
     </message>
   </context>
   <context>
     <name>SettingsDialog</name>
     <message>
+      <location filename="../SettingsDialog.py" line="24"/>
+      <source>System language</source>
+      <translation>Systemsprache</translation>
+    </message>
+    <message>
+      <location filename="../SettingsDialog.py" line="36"/>
+      <source>Nothing</source>
+      <translation>Nichts</translation>
+    </message>
+    <message>
+      <location filename="../SettingsDialog.py" line="37"/>
+      <source>Filename</source>
+      <translation>Dateiname</translation>
+    </message>
+    <message>
+      <location filename="../SettingsDialog.py" line="38"/>
+      <source>Path</source>
+      <translation>Pfad</translation>
+    </message>
+    <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Settings</source>
       <translation>Einstellungen</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Language:</source>
@@ -921,34 +973,14 @@
       <translation>OK</translation>
     </message>
     <message>
       <location filename="../SettingsDialog.ui" line="0"/>
       <source>Cancel</source>
       <translation>Abbrechen</translation>
     </message>
-    <message>
-      <location filename="../SettingsDialog.py" line="31"/>
-      <source>System language</source>
-      <translation>Systemsprache</translation>
-    </message>
-    <message>
-      <location filename="../SettingsDialog.py" line="43"/>
-      <source>Nothing</source>
-      <translation>Nichts</translation>
-    </message>
-    <message>
-      <location filename="../SettingsDialog.py" line="44"/>
-      <source>Filename</source>
-      <translation>Dateiname</translation>
-    </message>
-    <message>
-      <location filename="../SettingsDialog.py" line="45"/>
-      <source>Path</source>
-      <translation>Pfad</translation>
-    </message>
   </context>
   <context>
     <name>TranslateDialog</name>
     <message>
       <location filename="../TranslateDialog.ui" line="0"/>
       <location filename="../TranslateDialog.py" line="38"/>
       <source>Remove</source>
@@ -1004,28 +1036,28 @@
       <source>Cancel</source>
       <translation>Entfernen</translation>
     </message>
   </context>
   <context>
     <name>ValidationDialog</name>
     <message>
+      <location filename="../ValidationDialog.py" line="23"/>
+      <source>desktop-file-validate was not found</source>
+      <translation>desktop-file-validate wurde nicht gefunden</translation>
+    </message>
+    <message>
       <location filename="../ValidationDialog.ui" line="0"/>
       <source>Validate</source>
       <translation>Validieren</translation>
     </message>
     <message>
       <location filename="../ValidationDialog.ui" line="0"/>
       <source>The Box below shows the output of desktop-file-validate</source>
       <translation>In der Box unten ist die Ausgabe von desktop-file-validate zu sehen</translation>
     </message>
-    <message>
-      <location filename="../ValidationDialog.py" line="23"/>
-      <source>desktop-file-validate was not found</source>
-      <translation>desktop-file-validate wurde nicht gefunden</translation>
-    </message>
   </context>
   <context>
     <name>WelcomeDialog</name>
     <message>
       <location filename="../WelcomeDialog.ui" line="0"/>
       <source>Welcome</source>
       <translation>Willkommen</translation>
```

### Comparing `jdDesktopEntryEdit-1.0/jdDesktopEntryEdit.egg-info/SOURCES.txt` & `jdDesktopEntryEdit-1.1/jdDesktopEntryEdit.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 jdDesktopEntryEdit/AboutDialog.ui
 jdDesktopEntryEdit/EditActionDialog.py
 jdDesktopEntryEdit/EditActionDialog.ui
 jdDesktopEntryEdit/EditKeywordsTranslationDialog.py
 jdDesktopEntryEdit/Environment.py
 jdDesktopEntryEdit/Functions.py
 jdDesktopEntryEdit/Icon.svg
+jdDesktopEntryEdit/Languages.py
 jdDesktopEntryEdit/ListEditWidget.py
 jdDesktopEntryEdit/MainWindow.py
 jdDesktopEntryEdit/MainWindow.ui
 jdDesktopEntryEdit/ManageTemplatesWindow.py
 jdDesktopEntryEdit/ManageTemplatesWindow.ui
 jdDesktopEntryEdit/PreviewDialog.py
 jdDesktopEntryEdit/PreviewDialog.ui
@@ -33,8 +34,11 @@
 jdDesktopEntryEdit.egg-info/PKG-INFO
 jdDesktopEntryEdit.egg-info/SOURCES.txt
 jdDesktopEntryEdit.egg-info/dependency_links.txt
 jdDesktopEntryEdit.egg-info/entry_points.txt
 jdDesktopEntryEdit.egg-info/requires.txt
 jdDesktopEntryEdit.egg-info/top_level.txt
 jdDesktopEntryEdit/data/categories.txt
-jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts
+jdDesktopEntryEdit/data/changelog.html
+jdDesktopEntryEdit/data/translators.json
+jdDesktopEntryEdit/translations/jdDesktopEntryEdit_de.ts
+jdDesktopEntryEdit/translations/jdDesktopEntryEdit_nl.ts
```

