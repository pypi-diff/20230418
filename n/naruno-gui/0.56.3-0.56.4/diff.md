# Comparing `tmp/naruno_gui-0.56.3.tar.gz` & `tmp/naruno_gui-0.56.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naruno_gui-0.56.3.tar", last modified: Fri Apr 14 12:52:04 2023, max compression
+gzip compressed data, was "naruno_gui-0.56.4.tar", last modified: Tue Apr 18 00:15:08 2023, max compression
```

## Comparing `naruno_gui-0.56.3.tar` & `naruno_gui-0.56.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.733431 naruno_gui-0.56.3/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 12:52:04.733431 naruno_gui-0.56.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 12:52:04.729431 naruno_gui-0.56.3/naruno_gui.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-14 12:52:04.000000 naruno_gui-0.56.3/naruno_gui.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-14 12:52:04.000000 naruno_gui-0.56.3/naruno_gui.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:52:04.000000 naruno_gui-0.56.3/naruno_gui.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:52:04.000000 naruno_gui-0.56.3/naruno_gui.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-14 12:52:04.000000 naruno_gui-0.56.3/naruno_gui.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 12:52:04.000000 naruno_gui-0.56.3/naruno_gui.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 12:52:04.733431 naruno_gui-0.56.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-14 12:51:50.000000 naruno_gui-0.56.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:15:08.612600 naruno_gui-0.56.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 00:15:08.612600 naruno_gui-0.56.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 00:15:08.612600 naruno_gui-0.56.4/naruno_gui.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-18 00:15:08.000000 naruno_gui-0.56.4/naruno_gui.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 00:15:08.000000 naruno_gui-0.56.4/naruno_gui.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:15:08.000000 naruno_gui-0.56.4/naruno_gui.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:15:08.000000 naruno_gui-0.56.4/naruno_gui.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-18 00:15:08.000000 naruno_gui-0.56.4/naruno_gui.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 00:15:08.000000 naruno_gui-0.56.4/naruno_gui.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 00:15:08.612600 naruno_gui-0.56.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-18 00:14:50.000000 naruno_gui-0.56.4/setup.py
```

### Comparing `naruno_gui-0.56.3/setup.py` & `naruno_gui-0.56.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at https://mozilla.org/MPL/2.0/.
 from setuptools import setup
 
 setup(
     name="naruno_gui",
-    version="0.56.3",
+    version="0.56.4",
     description="""This is GUI mode installer for Naruno""",
     url="https://docs.naruno.org/",
     author="Naruno Developers",
     author_email="onur.atakan.ulusoy@naruno.org",
     license="MPL-2.0",
     install_requires="""
 Kivy==2.1.0
```

