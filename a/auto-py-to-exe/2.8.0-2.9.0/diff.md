# Comparing `tmp/auto-py-to-exe-2.8.0.tar.gz` & `tmp/auto-py-to-exe-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/auto-py-to-exe-2.8.0.tar", last modified: Mon Feb  8 10:05:32 2021, max compression
+gzip compressed data, was "dist/auto-py-to-exe-2.9.0.tar", last modified: Wed May  5 11:09:13 2021, max compression
```

## Comparing `auto-py-to-exe-2.8.0.tar` & `auto-py-to-exe-2.9.0.tar`

### file list

```diff
@@ -1,45 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       59 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6868 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2899 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      591 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2981 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (121)     5124 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/packaging.py
--rw-r--r--   0 runner    (1001) docker     (121)     4435 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/ui.py
--rw-r--r--   0 runner    (1001) docker     (121)     2801 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/
--rw-r--r--   0 runner    (1001) docker     (121)    48576 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/Nunito-Light.ttf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/css/
--rw-r--r--   0 runner    (1001) docker     (121)     2906 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/css/general.css
--rw-r--r--   0 runner    (1001) docker     (121)     4761 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/css/main.css
--rw-r--r--   0 runner    (1001) docker     (121)   167233 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/img/
--rw-r--r--   0 runner    (1001) docker     (121)      540 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/img/chevron-square-up.svg
--rw-r--r--   0 runner    (1001) docker     (121)      549 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/img/plus.svg
--rw-r--r--   0 runner    (1001) docker     (121)      444 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/img/remove.svg
--rw-r--r--   0 runner    (1001) docker     (121)    12231 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/index.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/configuration.js
--rw-r--r--   0 runner    (1001) docker     (121)     2526 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/constants.js
--rw-r--r--   0 runner    (1001) docker     (121)    12791 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/i18n.js
--rw-r--r--   0 runner    (1001) docker     (121)     1318 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/importExport.js
--rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/initialise.js
--rw-r--r--   0 runner    (1001) docker     (121)    16207 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/interface.js
--rw-r--r--   0 runner    (1001) docker     (121)      723 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/messages.js
--rw-r--r--   0 runner    (1001) docker     (121)     2630 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/packaging.js
--rw-r--r--   0 runner    (1001) docker     (121)     9754 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/staticEvents.js
--rw-r--r--   0 runner    (1001) docker     (121)      773 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/utils.js
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8593 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1101 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      106 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       29 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-08 10:05:32.000000 auto-py-to-exe-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2021-02-08 10:05:14.000000 auto-py-to-exe-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:13.000000 auto-py-to-exe-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8589 2021-05-05 11:09:13.000000 auto-py-to-exe-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     6864 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2899 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      591 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4842 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5124 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/packaging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4435 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/ui.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2801 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1200 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/
+-rw-r--r--   0 runner    (1001) docker     (121)    48576 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/Nunito-Light.ttf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:13.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/css/
+-rw-r--r--   0 runner    (1001) docker     (121)     2967 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/css/general.css
+-rw-r--r--   0 runner    (1001) docker     (121)     4778 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/css/main.css
+-rw-r--r--   0 runner    (1001) docker     (121)     1043 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/css/modal.css
+-rw-r--r--   0 runner    (1001) docker     (121)   167233 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:13.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/img/
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/img/chevron-square-up.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      549 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/img/plus.svg
+-rw-r--r--   0 runner    (1001) docker     (121)      444 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/img/remove.svg
+-rw-r--r--   0 runner    (1001) docker     (121)    12434 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/index.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:13.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/
+-rw-r--r--   0 runner    (1001) docker     (121)     2778 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/configuration.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2526 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/constants.js
+-rw-r--r--   0 runner    (1001) docker     (121)    13395 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/i18n.js
+-rw-r--r--   0 runner    (1001) docker     (121)     1811 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/importExport.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3398 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/initialise.js
+-rw-r--r--   0 runner    (1001) docker     (121)    16207 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/interface.js
+-rw-r--r--   0 runner    (1001) docker     (121)      723 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/messages.js
+-rw-r--r--   0 runner    (1001) docker     (121)     3426 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/modal.js
+-rw-r--r--   0 runner    (1001) docker     (121)     2630 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/packaging.js
+-rw-r--r--   0 runner    (1001) docker     (121)     9754 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/staticEvents.js
+-rw-r--r--   0 runner    (1001) docker     (121)      991 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/utils.js
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8589 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      106 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-05-05 11:09:12.000000 auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-05 11:09:13.000000 auto-py-to-exe-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1386 2021-05-05 11:08:51.000000 auto-py-to-exe-2.9.0/setup.py
```

### Comparing `auto-py-to-exe-2.8.0/LICENSE` & `auto-py-to-exe-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/PKG-INFO` & `auto-py-to-exe-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-py-to-exe
-Version: 2.8.0
+Version: 2.9.0
 Summary: Converts .py to .exe using a simple graphical interface.
 Home-page: https://github.com/brentvollebregt/auto-py-to-exe
 Author: Brent Vollebregt
 Author-email: brent@nitratine.net
 License: MIT
 Description: <h1 align="center">Auto PY to EXE</h1>
         <p align="center">A .py to .exe converter using a simple graphical interface and <a href="https://www.pyinstaller.org/">PyInstaller</a> in Python.</p>
@@ -17,15 +17,15 @@
             <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/v/auto-py-to-exe.svg" alt="PyPI Version"></a>
             <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/pyversions/auto-py-to-exe.svg" alt="PyPI Supported Versions"></a>
             <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/l/auto-py-to-exe.svg" alt="License"></a>
             <a href="https://pepy.tech/project/auto-py-to-exe"><img src="https://static.pepy.tech/badge/auto-py-to-exe/month" alt="Downloads Per Month"></a>
             <a href="https://pyinstaller.readthedocs.io/en/stable/requirements.html"><img src="https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-lightgrey" alt="Supported Platforms"></a>
         </p>
         
-        ### 阅读中文版的README ，点击 [这里](./README-Chinese.md)
+        阅读中文版的README ，点击 [这里](./README-Chinese.md)
         
         ## Getting Started
         
         ### Prerequisites
          - Python : 3.5-3.9
         
         *To have the interface displayed in the images, you will need chrome. If chrome is not installed or --no-chrome is supplied, the default browser will be used.*
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: auto-py-to-exe Version: 2.8.0 Summary: Converts .py
+Metadata-Version: 2.1 Name: auto-py-to-exe Version: 2.9.0 Summary: Converts .py
 to .exe using a simple graphical interface. Home-page: https://github.com/
 brentvollebregt/auto-py-to-exe Author: Brent Vollebregt Author-email:
 brent@nitratine.net License: MIT Description:
                          ****** Auto PY to EXE ******
  A .py to .exe converter using a simple graphical interface and PyInstaller in
                                     Python.
                                [Empty interface]
    [PyPI_Version] [PyPI_Supported_Versions] [License] [Downloads_Per_Month]
                              [Supported_Platforms]
-### éè¯»ä¸­æççREADME ï¼ç¹å» [è¿é](./README-Chinese.md) ## Getting
+éè¯»ä¸­æççREADME ï¼ç¹å» [è¿é](./README-Chinese.md) ## Getting
 Started ### Prerequisites - Python : 3.5-3.9 *To have the interface displayed
 in the images, you will need chrome. If chrome is not installed or --no-chrome
 is supplied, the default browser will be used.* > As of [PyInstaller 4.0]
 (https://github.com/pyinstaller/pyinstaller/releases/tag/v4.0), Python 2.7 is
 no longer supported. Read "[Python 2.7 Support](#python-27-support)" below for
 steps on how to use this tool with Python 2.7. ### Installation and Usage ####
 Installing Via [PyPI](https://pypi.org/project/auto-py-to-exe/) You can install
```

### Comparing `auto-py-to-exe-2.8.0/README.md` & `auto-py-to-exe-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/v/auto-py-to-exe.svg" alt="PyPI Version"></a>
     <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/pyversions/auto-py-to-exe.svg" alt="PyPI Supported Versions"></a>
     <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/l/auto-py-to-exe.svg" alt="License"></a>
     <a href="https://pepy.tech/project/auto-py-to-exe"><img src="https://static.pepy.tech/badge/auto-py-to-exe/month" alt="Downloads Per Month"></a>
     <a href="https://pyinstaller.readthedocs.io/en/stable/requirements.html"><img src="https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-lightgrey" alt="Supported Platforms"></a>
 </p>
 
-### 阅读中文版的README ，点击 [这里](./README-Chinese.md)
+阅读中文版的README ，点击 [这里](./README-Chinese.md)
 
 ## Getting Started
 
 ### Prerequisites
  - Python : 3.5-3.9
 
 *To have the interface displayed in the images, you will need chrome. If chrome is not installed or --no-chrome is supplied, the default browser will be used.*
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                          ****** Auto PY to EXE ******
  A .py to .exe converter using a simple graphical interface and PyInstaller in
                                     Python.
                                [Empty interface]
    [PyPI_Version] [PyPI_Supported_Versions] [License] [Downloads_Per_Month]
                              [Supported_Platforms]
-### éè¯»ä¸­æççREADME ï¼ç¹å» [è¿é](./README-Chinese.md) ## Getting
+éè¯»ä¸­æççREADME ï¼ç¹å» [è¿é](./README-Chinese.md) ## Getting
 Started ### Prerequisites - Python : 3.5-3.9 *To have the interface displayed
 in the images, you will need chrome. If chrome is not installed or --no-chrome
 is supplied, the default browser will be used.* > As of [PyInstaller 4.0]
 (https://github.com/pyinstaller/pyinstaller/releases/tag/v4.0), Python 2.7 is
 no longer supported. Read "[Python 2.7 Support](#python-27-support)" below for
 steps on how to use this tool with Python 2.7. ### Installation and Usage ####
 Installing Via [PyPI](https://pypi.org/project/auto-py-to-exe/) You can install
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/__main__.py` & `auto-py-to-exe-2.9.0/auto_py_to_exe/__main__.py`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/config.py` & `auto-py-to-exe-2.9.0/auto_py_to_exe/config.py`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/packaging.py` & `auto-py-to-exe-2.9.0/auto_py_to_exe/packaging.py`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/ui.py` & `auto-py-to-exe-2.9.0/auto_py_to_exe/ui.py`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/utils.py` & `auto-py-to-exe-2.9.0/auto_py_to_exe/utils.py`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/validation.py` & `auto-py-to-exe-2.9.0/auto_py_to_exe/validation.py`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/Nunito-Light.ttf` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/Nunito-Light.ttf`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/css/general.css` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/css/general.css`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
     --error: red;
     --unselected: lightgrey;
     --disabled: #808080;
 
     --title: #666666;
     --warning-background: #fff3cd;
     --warning-border: #a0987c;
+
+    --border-radius: 4px;
 }
 
 body {
     background-color: var(--background);
     font-family: 'Nunito', Helvetica, Arial, sans-serif;
     font-weight: 100;
     margin: 0 18px 10px 18px;
@@ -55,28 +57,28 @@
     font-size: 13px;
 }
 
 /* Generic inputs */
 
 button, input, select {
     border: 1px solid var(--primary);
-    border-radius: 4px;
+    border-radius: var(--border-radius);
     padding: 4px;
 
     font-family: 'Nunito', Helvetica, Arial, sans-serif;
     font-weight: 100;
 }
 
 input:focus {
     outline: none; /* Don't show outline so you can see the colour change */
 }
 
 button {
     cursor: pointer;
-    border-radius: 4px;
+    border-radius: var(--border-radius);
     background: transparent;
     padding: 3px 8px;
     transition: border 0.3s, background 0.3s;
     border-style: solid;
     border-width: 2px;
 }
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/css/main.css` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/css/main.css`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 #warnings {
     font-size: 13px;
 }
 
 #warnings > div {
     background: var(--warning-background);
     border: 1px solid var(--warning-border);
-    border-radius: 4px;
+    border-radius: var(--border-radius);
     margin: 10px 0;
     padding: 8px;
 }
 
 #warnings > div > p {
     margin: 0;
 }
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/favicon.ico` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/img/chevron-square-up.svg` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/img/chevron-square-up.svg`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/img/plus.svg` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/img/plus.svg`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/index.html` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -29,19 +29,21 @@
         <script type="text/javascript" src="/js/constants.js"></script>
         <script type="text/javascript" src="/js/i18n.js"></script>
         <script type="text/javascript" src="/js/initialise.js"></script>
         <script type="text/javascript" src="/js/configuration.js"></script>
         <script type="text/javascript" src="/js/staticEvents.js"></script>
         <script type="text/javascript" src="/js/interface.js"></script>
         <script type="text/javascript" src="/js/utils.js"></script>
+        <script type="text/javascript" src="/js/modal.js"></script>
         <script type="text/javascript" src="/js/messages.js"></script>
         <script type="text/javascript" src="/js/packaging.js"></script>
         <script type="text/javascript" src="/js/importExport.js"></script>
         <link rel="stylesheet" href="/css/general.css">
         <link rel="stylesheet" href="/css/main.css">
+        <link rel="stylesheet" href="/css/modal.css">
     </head>
 
     <body>
         <div class="mid">
             <div id="header">
                 <div class="title">
                     <a href="https://github.com/brentvollebregt/auto-py-to-exe" target="_blank"><img src="/favicon.ico" /></a>
@@ -226,9 +228,10 @@
                     Convert .py to .exe
                 </button>
                 <button id="open-output-folder-button" data-i18n="ui.button.openOutputFolder">
                     Open Output Folder
                 </button>
             </div>
         </div>
+        <div id="modal-area" class="modal-coverage modal-coverage-hidden"></div>
     </body>
 </html>
```

#### html2text {}

```diff
@@ -1,9 +1,10 @@
 
 
+
 [/favicon.ico]
 ******_Auto_Py_to_Exe_******
 
 ***** Script Location *****
 [                    ] Browse
 ***** Onefile (--onedir / --onefile) *****
  One Directory   One File
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/configuration.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/configuration.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -61,8 +61,12 @@
     const entryScript = entryScriptConfig === undefined ? "" : entryScriptConfig.value;
 
     return `pyinstaller ${optionsAndValues.join(' ')} ${getNonPyinstallerConfiguration().manualArguments} "${entryScript}"`;
 };
 
 const updateCurrentCommandDisplay = () => {
     document.querySelector('#current-command textarea').value = getCurrentCommand();
-};
+};
+
+const isCommandDefault = () => {
+    return getCurrentCommand() === 'pyinstaller --noconfirm --onedir --console  ""';
+}
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/constants.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/constants.js`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/i18n.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/i18n.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -236,14 +236,32 @@
                 en: 'Converting...',
                 zh: '转换中······'
             },
             clearOutput: {
                 en: 'Clear Output',
                 zh: '清除输出f'
             },
+        },
+        modal: {
+            configModalTitle: {
+                en: 'Override current configuration?',
+                zh: '覆盖当前配置？'
+            },
+            configModalDescription: {
+                en: 'All previously inserted values will be erased.',
+                zh: '所有先前插入的值将被删除。'
+            },
+            configModalConfirmButton: {
+                en: 'Confirm',
+                zh: '确认'
+            },
+            configModalCancelButton: {
+                en: 'Cancel',
+                zh: '取消'
+            }
         }
     },
     // Things like alerts
     nonDom: {
         alert: {
             noScriptsLocationProvided: {
                 en: 'You have not provided your scripts location.\nPlease enter this at the top of the page.',
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/initialise.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/initialise.js`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/interface.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/interface.js`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/messages.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/messages.js`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/packaging.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/packaging.js`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe/web/js/staticEvents.js` & `auto-py-to-exe-2.9.0/auto_py_to_exe/web/js/staticEvents.js`

 * *Files identical despite different names*

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/PKG-INFO` & `auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-py-to-exe
-Version: 2.8.0
+Version: 2.9.0
 Summary: Converts .py to .exe using a simple graphical interface.
 Home-page: https://github.com/brentvollebregt/auto-py-to-exe
 Author: Brent Vollebregt
 Author-email: brent@nitratine.net
 License: MIT
 Description: <h1 align="center">Auto PY to EXE</h1>
         <p align="center">A .py to .exe converter using a simple graphical interface and <a href="https://www.pyinstaller.org/">PyInstaller</a> in Python.</p>
@@ -17,15 +17,15 @@
             <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/v/auto-py-to-exe.svg" alt="PyPI Version"></a>
             <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/pyversions/auto-py-to-exe.svg" alt="PyPI Supported Versions"></a>
             <a href="https://pypi.org/project/auto-py-to-exe/"><img src="https://img.shields.io/pypi/l/auto-py-to-exe.svg" alt="License"></a>
             <a href="https://pepy.tech/project/auto-py-to-exe"><img src="https://static.pepy.tech/badge/auto-py-to-exe/month" alt="Downloads Per Month"></a>
             <a href="https://pyinstaller.readthedocs.io/en/stable/requirements.html"><img src="https://img.shields.io/badge/platform-windows%20%7C%20linux%20%7C%20macos-lightgrey" alt="Supported Platforms"></a>
         </p>
         
-        ### 阅读中文版的README ，点击 [这里](./README-Chinese.md)
+        阅读中文版的README ，点击 [这里](./README-Chinese.md)
         
         ## Getting Started
         
         ### Prerequisites
          - Python : 3.5-3.9
         
         *To have the interface displayed in the images, you will need chrome. If chrome is not installed or --no-chrome is supplied, the default browser will be used.*
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: auto-py-to-exe Version: 2.8.0 Summary: Converts .py
+Metadata-Version: 2.1 Name: auto-py-to-exe Version: 2.9.0 Summary: Converts .py
 to .exe using a simple graphical interface. Home-page: https://github.com/
 brentvollebregt/auto-py-to-exe Author: Brent Vollebregt Author-email:
 brent@nitratine.net License: MIT Description:
                          ****** Auto PY to EXE ******
  A .py to .exe converter using a simple graphical interface and PyInstaller in
                                     Python.
                                [Empty interface]
    [PyPI_Version] [PyPI_Supported_Versions] [License] [Downloads_Per_Month]
                              [Supported_Platforms]
-### éè¯»ä¸­æççREADME ï¼ç¹å» [è¿é](./README-Chinese.md) ## Getting
+éè¯»ä¸­æççREADME ï¼ç¹å» [è¿é](./README-Chinese.md) ## Getting
 Started ### Prerequisites - Python : 3.5-3.9 *To have the interface displayed
 in the images, you will need chrome. If chrome is not installed or --no-chrome
 is supplied, the default browser will be used.* > As of [PyInstaller 4.0]
 (https://github.com/pyinstaller/pyinstaller/releases/tag/v4.0), Python 2.7 is
 no longer supported. Read "[Python 2.7 Support](#python-27-support)" below for
 steps on how to use this tool with Python 2.7. ### Installation and Usage ####
 Installing Via [PyPI](https://pypi.org/project/auto-py-to-exe/) You can install
```

### Comparing `auto-py-to-exe-2.8.0/auto_py_to_exe.egg-info/SOURCES.txt` & `auto-py-to-exe-2.9.0/auto_py_to_exe.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,20 +17,22 @@
 auto_py_to_exe.egg-info/requires.txt
 auto_py_to_exe.egg-info/top_level.txt
 auto_py_to_exe/web/Nunito-Light.ttf
 auto_py_to_exe/web/favicon.ico
 auto_py_to_exe/web/index.html
 auto_py_to_exe/web/css/general.css
 auto_py_to_exe/web/css/main.css
+auto_py_to_exe/web/css/modal.css
 auto_py_to_exe/web/img/chevron-square-up.svg
 auto_py_to_exe/web/img/plus.svg
 auto_py_to_exe/web/img/remove.svg
 auto_py_to_exe/web/js/configuration.js
 auto_py_to_exe/web/js/constants.js
 auto_py_to_exe/web/js/i18n.js
 auto_py_to_exe/web/js/importExport.js
 auto_py_to_exe/web/js/initialise.js
 auto_py_to_exe/web/js/interface.js
 auto_py_to_exe/web/js/messages.js
+auto_py_to_exe/web/js/modal.js
 auto_py_to_exe/web/js/packaging.js
 auto_py_to_exe/web/js/staticEvents.js
 auto_py_to_exe/web/js/utils.js
```

### Comparing `auto-py-to-exe-2.8.0/setup.py` & `auto-py-to-exe-2.9.0/setup.py`

 * *Files identical despite different names*

