# Comparing `tmp/windbg_copilot-1.0.1.tar.gz` & `tmp/windbg_copilot-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.1.tar", last modified: Tue Apr 18 05:30:45 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.2.tar", last modified: Tue Apr 18 05:47:49 2023, max compression
```

## Comparing `windbg_copilot-1.0.1.tar` & `windbg_copilot-1.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:30:45.686265 windbg_copilot-1.0.1/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2958 2023-04-18 05:30:45.686265 windbg_copilot-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2124 2023-04-18 05:25:59.000000 windbg_copilot-1.0.1/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-18 05:30:45.688254 windbg_copilot-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:30:45.664251 windbg_copilot-1.0.1/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.1/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-18 05:30:28.000000 windbg_copilot-1.0.1/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     7120 2023-04-18 05:03:54.000000 windbg_copilot-1.0.1/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:30:45.685252 windbg_copilot-1.0.1/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2958 2023-04-18 05:30:44.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-18 05:30:45.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:30:44.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 05:30:45.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:30:45.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:47:49.479441 windbg_copilot-1.0.2/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-18 05:47:49.480443 windbg_copilot-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-04-18 05:46:31.000000 windbg_copilot-1.0.2/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-18 05:47:49.483449 windbg_copilot-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:47:49.443076 windbg_copilot-1.0.2/windbg_copilot/
+-rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.2/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-18 05:47:15.000000 windbg_copilot-1.0.2/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7120 2023-04-18 05:03:54.000000 windbg_copilot-1.0.2/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:47:49.477440 windbg_copilot-1.0.2/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-18 05:47:49.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.1/LICENSE.txt` & `windbg_copilot-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.1/PKG-INFO` & `windbg_copilot-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.1
+Version: 1.0.2
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
@@ -41,17 +41,17 @@
         pip install openai
         pip install windbg_copilot
 
         The packages will be downloaded and installed automatically.
 
 Usage
 
-        Open command line and run windbg_copilot:
+        Open command line and run python:
 
-        python windbg_copilot.py
+        import windbg_copilot
 
         Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
                 !chat <you may ask anything related to debugging>
                 !ask <ask any question for the above output>
                 !explain: explain the last output
                 !suggest: suggest how to do next
```

### Comparing `windbg_copilot-1.0.1/README.md` & `windbg_copilot-1.0.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,17 @@
         pip install openai
         pip install windbg_copilot
 
         The packages will be downloaded and installed automatically.
 
 Usage
 
-        Open command line and run windbg_copilot:
+        Open command line and run python:
 
-        python windbg_copilot.py
+        import windbg_copilot
 
         Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
                 !chat <you may ask anything related to debugging>
                 !ask <ask any question for the above output>
                 !explain: explain the last output
                 !suggest: suggest how to do next
```

### Comparing `windbg_copilot-1.0.1/setup.cfg` & `windbg_copilot-1.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.1/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.2/windbg_copilot/windbg_copilot.py`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.1/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.2/windbg_copilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.1
+Version: 1.0.2
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
@@ -41,17 +41,17 @@
         pip install openai
         pip install windbg_copilot
 
         The packages will be downloaded and installed automatically.
 
 Usage
 
-        Open command line and run windbg_copilot:
+        Open command line and run python:
 
-        python windbg_copilot.py
+        import windbg_copilot
 
         Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
                 !chat <you may ask anything related to debugging>
                 !ask <ask any question for the above output>
                 !explain: explain the last output
                 !suggest: suggest how to do next
```

