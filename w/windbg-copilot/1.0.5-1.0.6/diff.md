# Comparing `tmp/windbg_copilot-1.0.5.tar.gz` & `tmp/windbg_copilot-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.5.tar", last modified: Tue Apr 18 06:16:31 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.6.tar", last modified: Tue Apr 18 06:20:00 2023, max compression
```

## Comparing `windbg_copilot-1.0.5.tar` & `windbg_copilot-1.0.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 06:16:31.324285 windbg_copilot-1.0.5/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2947 2023-04-18 06:16:31.324285 windbg_copilot-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2113 2023-04-18 05:46:31.000000 windbg_copilot-1.0.5/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0      918 2023-04-18 06:16:31.326275 windbg_copilot-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:16:31.291611 windbg_copilot-1.0.5/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.5/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-18 06:16:00.000000 windbg_copilot-1.0.5/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     6699 2023-04-18 06:15:43.000000 windbg_copilot-1.0.5/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-18 06:16:31.322275 windbg_copilot-1.0.5/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2947 2023-04-18 06:16:30.000000 windbg_copilot-1.0.5/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-18 06:16:31.000000 windbg_copilot-1.0.5/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 06:16:30.000000 windbg_copilot-1.0.5/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 06:16:30.000000 windbg_copilot-1.0.5/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 06:16:30.000000 windbg_copilot-1.0.5/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 06:20:00.621506 windbg_copilot-1.0.6/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     2947 2023-04-18 06:20:00.622470 windbg_copilot-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2113 2023-04-18 06:19:04.000000 windbg_copilot-1.0.6/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-18 06:20:00.624421 windbg_copilot-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:20:00.582300 windbg_copilot-1.0.6/windbg_copilot/
+-rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.6/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-18 06:19:11.000000 windbg_copilot-1.0.6/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     6699 2023-04-18 06:15:43.000000 windbg_copilot-1.0.6/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 06:20:00.619424 windbg_copilot-1.0.6/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2947 2023-04-18 06:19:59.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-18 06:20:00.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 06:19:59.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-18 06:20:00.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 06:20:00.000000 windbg_copilot-1.0.6/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.5/LICENSE.txt` & `windbg_copilot-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.5/PKG-INFO` & `windbg_copilot-1.0.6/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.5
+Version: 1.0.6
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
@@ -35,15 +35,15 @@
 
 Installation
 
         Open a command prompt or terminal window, install the Windbg Copilot packages using pip:
 
         pip install pyttsx3==2.90
         pip install openai
-        pip install windbg_copilot
+        pip install windbg-copilot
 
         The packages will be downloaded and installed automatically.
 
 Usage
 
         Open command line and run python:
 
@@ -62,15 +62,15 @@
 Uninstallation
 
         Open a command prompt or terminal window.
         Use pip to uninstall the Windbg Copilot package:
 
         pip uninstall pyttsx3
         pip uninstall openai
-        pip uninstall windbg_copilot
+        pip uninstall windbg-copilot
 
         The packages will be uninstalled automatically.
 
 Conclusion
 
 Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. With its simple installation process and intuitive API, Windbg Copilot is an essential tool for anyone working on complex Windows debugging.
```

### Comparing `windbg_copilot-1.0.5/README.md` & `windbg_copilot-1.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Installation
 
         Open a command prompt or terminal window, install the Windbg Copilot packages using pip:
 
         pip install pyttsx3==2.90
         pip install openai
-        pip install windbg_copilot
+        pip install windbg-copilot
 
         The packages will be downloaded and installed automatically.
 
 Usage
 
         Open command line and run python:
 
@@ -38,14 +38,14 @@
 Uninstallation
 
         Open a command prompt or terminal window.
         Use pip to uninstall the Windbg Copilot package:
 
         pip uninstall pyttsx3
         pip uninstall openai
-        pip uninstall windbg_copilot
+        pip uninstall windbg-copilot
 
         The packages will be uninstalled automatically.
 
 Conclusion
 
 Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. With its simple installation process and intuitive API, Windbg Copilot is an essential tool for anyone working on complex Windows debugging.
```

### Comparing `windbg_copilot-1.0.5/setup.cfg` & `windbg_copilot-1.0.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.5/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.6/windbg_copilot/windbg_copilot.py`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.5/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.6/windbg_copilot.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.5
+Version: 1.0.6
 Summary: "windbg copilot"
 Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
@@ -35,15 +35,15 @@
 
 Installation
 
         Open a command prompt or terminal window, install the Windbg Copilot packages using pip:
 
         pip install pyttsx3==2.90
         pip install openai
-        pip install windbg_copilot
+        pip install windbg-copilot
 
         The packages will be downloaded and installed automatically.
 
 Usage
 
         Open command line and run python:
 
@@ -62,15 +62,15 @@
 Uninstallation
 
         Open a command prompt or terminal window.
         Use pip to uninstall the Windbg Copilot package:
 
         pip uninstall pyttsx3
         pip uninstall openai
-        pip uninstall windbg_copilot
+        pip uninstall windbg-copilot
 
         The packages will be uninstalled automatically.
 
 Conclusion
 
 Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. With its simple installation process and intuitive API, Windbg Copilot is an essential tool for anyone working on complex Windows debugging.
```

