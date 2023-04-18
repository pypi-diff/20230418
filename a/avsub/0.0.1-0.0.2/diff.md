# Comparing `tmp/avsub-0.0.1.tar.gz` & `tmp/avsub-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avsub-0.0.1.tar", last modified: Thu Apr 13 18:29:32 2023, max compression
+gzip compressed data, was "avsub-0.0.2.tar", last modified: Tue Apr 18 01:12:21 2023, max compression
```

## Comparing `avsub-0.0.1.tar` & `avsub-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 18:29:32.254614 avsub-0.0.1/
--rw-rw-rw-   0        0        0    35823 2023-04-09 03:51:55.000000 avsub-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      797 2023-04-13 18:29:32.254614 avsub-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-13 18:29:32.254614 avsub-0.0.1/avsub/
--rw-rw-rw-   0        0        0      110 2023-04-13 02:09:57.000000 avsub-0.0.1/avsub/__init__.py
--rw-rw-rw-   0        0        0     3884 2023-04-13 18:23:25.000000 avsub-0.0.1/avsub/__main__.py
--rw-rw-rw-   0        0        0       81 2023-04-13 02:36:54.000000 avsub-0.0.1/avsub/__version__.py
--rw-rw-rw-   0        0        0      433 2023-04-13 17:23:33.000000 avsub-0.0.1/avsub/actions.py
--rw-rw-rw-   0        0        0     5722 2023-04-13 17:19:23.000000 avsub-0.0.1/avsub/cli.py
--rw-rw-rw-   0        0        0      609 2023-04-13 01:02:10.000000 avsub-0.0.1/avsub/consts.py
--rw-rw-rw-   0        0        0     3559 2023-04-13 17:48:03.000000 avsub-0.0.1/avsub/ffmpeg.py
--rw-rw-rw-   0        0        0      211 2023-04-11 12:57:13.000000 avsub-0.0.1/avsub/globs.py
--rw-rw-rw-   0        0        0     1680 2023-04-13 00:17:21.000000 avsub-0.0.1/avsub/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-13 18:29:32.254614 avsub-0.0.1/avsub.egg-info/
--rw-rw-rw-   0        0        0      797 2023-04-13 18:29:32.000000 avsub-0.0.1/avsub.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2023-04-13 18:29:32.000000 avsub-0.0.1/avsub.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 18:29:32.000000 avsub-0.0.1/avsub.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2023-04-13 18:29:32.000000 avsub-0.0.1/avsub.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-04-13 18:29:31.000000 avsub-0.0.1/avsub.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2023-04-13 18:29:32.000000 avsub-0.0.1/avsub.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1037 2023-04-13 02:22:05.000000 avsub-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-13 18:29:32.254614 avsub-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-18 01:12:21.700789 avsub-0.0.2/
+-rw-rw-rw-   0        0        0    35823 2023-04-09 03:51:55.000000 avsub-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      797 2023-04-18 01:12:21.700789 avsub-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-18 01:12:21.681568 avsub-0.0.2/avsub/
+-rw-rw-rw-   0        0        0      110 2023-04-13 02:09:57.000000 avsub-0.0.2/avsub/__init__.py
+-rw-rw-rw-   0        0        0     3850 2023-04-18 01:06:44.000000 avsub-0.0.2/avsub/__main__.py
+-rw-rw-rw-   0        0        0       81 2023-04-18 01:06:08.000000 avsub-0.0.2/avsub/__version__.py
+-rw-rw-rw-   0        0        0      433 2023-04-13 17:23:33.000000 avsub-0.0.2/avsub/actions.py
+-rw-rw-rw-   0        0        0     5722 2023-04-13 17:19:23.000000 avsub-0.0.2/avsub/cli.py
+-rw-rw-rw-   0        0        0      609 2023-04-13 01:02:10.000000 avsub-0.0.2/avsub/consts.py
+-rw-rw-rw-   0        0        0     3559 2023-04-13 17:48:03.000000 avsub-0.0.2/avsub/ffmpeg.py
+-rw-rw-rw-   0        0        0      211 2023-04-11 12:57:13.000000 avsub-0.0.2/avsub/globs.py
+-rw-rw-rw-   0        0        0     1680 2023-04-13 00:17:21.000000 avsub-0.0.2/avsub/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-18 01:12:21.700789 avsub-0.0.2/avsub.egg-info/
+-rw-rw-rw-   0        0        0      797 2023-04-18 01:12:21.000000 avsub-0.0.2/avsub.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2023-04-18 01:12:21.000000 avsub-0.0.2/avsub.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 01:12:21.000000 avsub-0.0.2/avsub.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-04-18 01:12:21.000000 avsub-0.0.2/avsub.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-04-18 01:12:21.000000 avsub-0.0.2/avsub.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-18 01:12:21.000000 avsub-0.0.2/avsub.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1037 2023-04-13 02:22:05.000000 avsub-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-04-18 01:12:21.700789 avsub-0.0.2/setup.cfg
```

### Comparing `avsub-0.0.1/LICENSE` & `avsub-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `avsub-0.0.1/PKG-INFO` & `avsub-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avsub
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simplified command-line interface for FFmpeg
 Author: Serhat Çelik
 License: GPLv3
 Keywords: avsub,audio,video,subtitle,ffmpeg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `avsub-0.0.1/avsub/__main__.py` & `avsub-0.0.2/avsub/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,16 +16,14 @@
 from avsub.ffmpeg import FFmpeg
 from avsub.globs import completed, controller, corrupted, untouched
 from avsub.utils import exit_if_not, separate, splitext
 
 
 def start() -> tuple[int | None, bool]:
     """Start the program."""
-    sys.excepthook = stop_hard
-
     opts = parser.parse_args()
 
     signal.signal(signal.SIGINT, stop)
 
     ff = FFmpeg()
 
     ff.build(opts)  # Start creating the FFmpeg command
```

### Comparing `avsub-0.0.1/avsub/cli.py` & `avsub-0.0.2/avsub/cli.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.1/avsub/consts.py` & `avsub-0.0.2/avsub/consts.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.1/avsub/ffmpeg.py` & `avsub-0.0.2/avsub/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.1/avsub/utils.py` & `avsub-0.0.2/avsub/utils.py`

 * *Files identical despite different names*

### Comparing `avsub-0.0.1/avsub.egg-info/PKG-INFO` & `avsub-0.0.2/avsub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avsub
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simplified command-line interface for FFmpeg
 Author: Serhat Çelik
 License: GPLv3
 Keywords: avsub,audio,video,subtitle,ffmpeg
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: End Users/Desktop
```

### Comparing `avsub-0.0.1/pyproject.toml` & `avsub-0.0.2/pyproject.toml`

 * *Files identical despite different names*

