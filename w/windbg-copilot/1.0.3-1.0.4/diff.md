# Comparing `tmp/windbg_copilot-1.0.3.tar.gz` & `tmp/windbg_copilot-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.3.tar", last modified: Tue Apr 18 05:52:11 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.4.tar", last modified: Tue Apr 18 06:10:21 2023, max compression
```

## Comparing `windbg_copilot-1.0.3.tar` & `windbg_copilot-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:52:11.489809 windbg_copilot-1.0.3/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.3/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-18 05:52:11.490812 windbg_copilot-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2023-04-18 05:46:31.000000 windbg_copilot-1.0.3/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-18 05:52:11.497819 windbg_copilot-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:52:11.464817 windbg_copilot-1.0.3/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.3/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-18 05:52:01.000000 windbg_copilot-1.0.3/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     7054 2023-04-18 05:51:13.000000 windbg_copilot-1.0.3/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:52:11.488812 windbg_copilot-1.0.3/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-18 05:52:11.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 06:10:21.370214 windbg_copilot-1.0.4/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.4/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-18 06:10:21.371441 windbg_copilot-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-04-18 05:46:31.000000 windbg_copilot-1.0.4/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-18 06:10:21.373502 windbg_copilot-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:10:21.357218 windbg_copilot-1.0.4/windbg_copilot/
+-rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.4/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-18 06:09:24.000000 windbg_copilot-1.0.4/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7054 2023-04-18 05:57:42.000000 windbg_copilot-1.0.4/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:10:21.369216 windbg_copilot-1.0.4/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-18 06:10:20.000000 windbg_copilot-1.0.4/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-18 06:10:21.000000 windbg_copilot-1.0.4/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:10:20.000000 windbg_copilot-1.0.4/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-18 06:10:20.000000 windbg_copilot-1.0.4/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 06:10:20.000000 windbg_copilot-1.0.4/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.3/LICENSE.txt` & `windbg_copilot-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.3/PKG-INFO` & `windbg_copilot-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.3
+Version: 1.0.4
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

### Comparing `windbg_copilot-1.0.3/README.md` & `windbg_copilot-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.3/setup.cfg` & `windbg_copilot-1.0.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.3/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.4/windbg_copilot/windbg_copilot.py`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.3/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.4/windbg_copilot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.3
+Version: 1.0.4
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

