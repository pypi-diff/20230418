# Comparing `tmp/espeak_phonemizer-1.2.0.tar.gz` & `tmp/espeak_phonemizer-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "espeak_phonemizer-1.2.0.tar", last modified: Sun Apr  9 16:31:19 2023, max compression
+gzip compressed data, was "espeak_phonemizer-1.3.0.tar", last modified: Tue Apr 18 03:37:37 2023, max compression
```

## Comparing `espeak_phonemizer-1.2.0.tar` & `espeak_phonemizer-1.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35147 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/LICENSE
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1712 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/README.md
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/espeak_phonemizer/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-04-09 16:25:07.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/VERSION
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     5456 2023-04-09 16:29:57.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3981 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/__main__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/espeak_phonemizer/py.typed
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/PKG-INFO
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      400 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/SOURCES.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/dependency_links.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/entry_points.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-04-09 16:31:19.000000 espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/top_level.txt
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)      113 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/setup.cfg
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1480 2022-03-18 20:12:33.000000 espeak_phonemizer-1.2.0/setup.py
-drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-09 16:31:19.497766 espeak_phonemizer-1.2.0/tests/
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.2.0/tests/__init__.py
--rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1995 2023-04-09 16:23:34.000000 espeak_phonemizer-1.2.0/tests/test_phonemizer.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)    35147 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/LICENSE
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1712 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/README.md
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/espeak_phonemizer/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        6 2023-04-18 03:36:43.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/VERSION
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     8182 2023-04-18 03:36:43.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3981 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/__main__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/espeak_phonemizer/py.typed
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     2275 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/PKG-INFO
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      400 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/SOURCES.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        1 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/dependency_links.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       71 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/entry_points.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)       24 2023-04-18 03:37:37.000000 espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/top_level.txt
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)      113 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/setup.cfg
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     1480 2022-03-18 20:12:33.000000 espeak_phonemizer-1.3.0/setup.py
+drwxr-xr-x   0 hansenm   (1000) hansenm   (1000)        0 2023-04-18 03:37:37.979704 espeak_phonemizer-1.3.0/tests/
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)        0 2021-10-11 19:22:13.000000 espeak_phonemizer-1.3.0/tests/__init__.py
+-rw-r--r--   0 hansenm   (1000) hansenm   (1000)     3085 2023-04-18 03:36:43.000000 espeak_phonemizer-1.3.0/tests/test_phonemizer.py
```

### Comparing `espeak_phonemizer-1.2.0/LICENSE` & `espeak_phonemizer-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.2.0/PKG-INFO` & `espeak_phonemizer-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espeak_phonemizer
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lightweight International Phonetic Alphabet (IPA) phonemizer that uses libespeak-ng
 Home-page: https://github.com/rhasspy/espeak-phonemizer
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `espeak_phonemizer-1.2.0/README.md` & `espeak_phonemizer-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.2.0/espeak_phonemizer/__main__.py` & `espeak_phonemizer-1.3.0/espeak_phonemizer/__main__.py`

 * *Files identical despite different names*

### Comparing `espeak_phonemizer-1.2.0/espeak_phonemizer.egg-info/PKG-INFO` & `espeak_phonemizer-1.3.0/espeak_phonemizer.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: espeak-phonemizer
-Version: 1.2.0
+Version: 1.3.0
 Summary: Lightweight International Phonetic Alphabet (IPA) phonemizer that uses libespeak-ng
 Home-page: https://github.com/rhasspy/espeak-phonemizer
 Author: Michael Hansen
 Author-email: mike@rhasspy.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `espeak_phonemizer-1.2.0/setup.py` & `espeak_phonemizer-1.3.0/setup.py`

 * *Files identical despite different names*

