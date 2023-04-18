# Comparing `tmp/windbg_copilot-1.0.2.tar.gz` & `tmp/windbg_copilot-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.2.tar", last modified: Tue Apr 18 05:47:49 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.3.tar", last modified: Tue Apr 18 05:52:11 2023, max compression
```

## Comparing `windbg_copilot-1.0.2.tar` & `windbg_copilot-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:47:49.479441 windbg_copilot-1.0.2/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-18 05:47:49.480443 windbg_copilot-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2023-04-18 05:46:31.000000 windbg_copilot-1.0.2/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-18 05:47:49.483449 windbg_copilot-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:47:49.443076 windbg_copilot-1.0.2/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.2/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-18 05:47:15.000000 windbg_copilot-1.0.2/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     7120 2023-04-18 05:03:54.000000 windbg_copilot-1.0.2/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:47:49.477440 windbg_copilot-1.0.2/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-18 05:47:49.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:47:48.000000 windbg_copilot-1.0.2/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:52:11.489809 windbg_copilot-1.0.3/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-18 05:52:11.490812 windbg_copilot-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-04-18 05:46:31.000000 windbg_copilot-1.0.3/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-18 05:52:11.497819 windbg_copilot-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:52:11.464817 windbg_copilot-1.0.3/windbg_copilot/
+-rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.3/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-18 05:52:01.000000 windbg_copilot-1.0.3/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7054 2023-04-18 05:51:13.000000 windbg_copilot-1.0.3/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:52:11.488812 windbg_copilot-1.0.3/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-18 05:52:11.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 05:52:10.000000 windbg_copilot-1.0.3/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.2/LICENSE.txt` & `windbg_copilot-1.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.2/PKG-INFO` & `windbg_copilot-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.2
+Version: 1.0.3
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

### Comparing `windbg_copilot-1.0.2/README.md` & `windbg_copilot-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.2/setup.cfg` & `windbg_copilot-1.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.2/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.3/windbg_copilot/windbg_copilot.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,16 @@
 
 print("Hello engineer, I am Windows Debugger Copilot, I'm here to assist you with any pain points you have while debugging. Whether you're a beginner or an experienced developer, debugging can be a challenging process. However, there are some techniques and best practices that can help make your debugging more efficient and effective.")
 speak("Hello engineer, I am Windows Debugger Copilot, I'm here to assist you with any pain points you have while debugging. Whether you're a beginner or an experienced developer, debugging can be a challenging process. However, there are some techniques and best practices that can help make your debugging more efficient and effective.")
 
 print("\nThis software is used for Windows Debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
 speak("\nThis software is used for Windows Debugging learning purpose, do NOT load any customer data, all input and output will be sent to OpenAI API.")
 
-print("\nFirst, Where is the memory dump? You may drag the dump file here.")
-speak("First, Where is the memory dump? You may drag the dump file here.")
+print("\nFirst, Where is the memory dump?")
+speak("First, Where is the memory dump?")
 
 dumpfile = input("Memory dump file location:")
 
 command = r'C:\Program Files (x86)\Windows Kits\10\Debuggers\x64\cdb.exe'
 arguments = [command]
 arguments.extend(['-y', "srv*C:\debug\symbols*https://msdl.microsoft.com/download/symbols"])  # Symbol path, may use sys.argv[1]
 # arguments.extend(['-i', sys.argv[2]])  # Image path
```

### Comparing `windbg_copilot-1.0.2/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.3/windbg_copilot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.2
+Version: 1.0.3
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
```

