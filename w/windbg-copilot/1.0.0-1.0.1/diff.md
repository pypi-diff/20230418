# Comparing `tmp/windbg_copilot-1.0.0.tar.gz` & `tmp/windbg_copilot-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "windbg_copilot-1.0.0.tar", last modified: Tue Apr 18 05:04:51 2023, max compression
+gzip compressed data, was "windbg_copilot-1.0.1.tar", last modified: Tue Apr 18 05:30:45 2023, max compression
```

## Comparing `windbg_copilot-1.0.0.tar` & `windbg_copilot-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 05:04:51.679770 windbg_copilot-1.0.0/
--rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.0/LICENSE.txt
--rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2907 2023-04-18 05:04:51.679770 windbg_copilot-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2080 2023-04-18 04:48:24.000000 windbg_copilot-1.0.0/README.md
--rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      911 2023-04-18 05:04:51.687770 windbg_copilot-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:04:51.647910 windbg_copilot-1.0.0/windbg_copilot/
--rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.0/windbg_copilot/__init__.py
--rw-rw-rw-   0        0        0       35 2023-04-07 21:28:41.000000 windbg_copilot-1.0.0/windbg_copilot/version.py
--rw-rw-rw-   0        0        0     7120 2023-04-18 05:03:54.000000 windbg_copilot-1.0.0/windbg_copilot/windbg_copilot.py
-drwxrwxrwx   0        0        0        0 2023-04-18 05:04:51.677870 windbg_copilot-1.0.0/windbg_copilot.egg-info/
--rw-rw-rw-   0        0        0     2907 2023-04-18 05:04:50.000000 windbg_copilot-1.0.0/windbg_copilot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      342 2023-04-18 05:04:51.000000 windbg_copilot-1.0.0/windbg_copilot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 05:04:50.000000 windbg_copilot-1.0.0/windbg_copilot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       29 2023-04-18 05:04:51.000000 windbg_copilot-1.0.0/windbg_copilot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-04-18 05:04:51.000000 windbg_copilot-1.0.0/windbg_copilot.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-18 05:30:45.686265 windbg_copilot-1.0.1/
+-rw-rw-rw-   0        0        0     1211 2023-04-18 04:47:10.000000 windbg_copilot-1.0.1/LICENSE.txt
+-rw-rw-rw-   0        0        0        0 2023-04-07 21:28:41.000000 windbg_copilot-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2958 2023-04-18 05:30:45.686265 windbg_copilot-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2124 2023-04-18 05:25:59.000000 windbg_copilot-1.0.1/README.md
+-rw-rw-rw-   0        0        0       78 2023-04-07 21:28:41.000000 windbg_copilot-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      918 2023-04-18 05:30:45.688254 windbg_copilot-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      110 2023-04-18 04:56:40.000000 windbg_copilot-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:30:45.664251 windbg_copilot-1.0.1/windbg_copilot/
+-rw-rw-rw-   0        0        0       91 2023-04-07 21:28:41.000000 windbg_copilot-1.0.1/windbg_copilot/__init__.py
+-rw-rw-rw-   0        0        0       35 2023-04-18 05:30:28.000000 windbg_copilot-1.0.1/windbg_copilot/version.py
+-rw-rw-rw-   0        0        0     7120 2023-04-18 05:03:54.000000 windbg_copilot-1.0.1/windbg_copilot/windbg_copilot.py
+drwxrwxrwx   0        0        0        0 2023-04-18 05:30:45.685252 windbg_copilot-1.0.1/windbg_copilot.egg-info/
+-rw-rw-rw-   0        0        0     2958 2023-04-18 05:30:44.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      342 2023-04-18 05:30:45.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-18 05:30:44.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-18 05:30:45.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-04-18 05:30:45.000000 windbg_copilot-1.0.1/windbg_copilot.egg-info/top_level.txt
```

### Comparing `windbg_copilot-1.0.0/LICENSE.txt` & `windbg_copilot-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.0/PKG-INFO` & `windbg_copilot-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: windbg_copilot
-Version: 1.0.0
+Version: 1.0.1
 Summary: "windbg copilot"
-Home-page: https://github.com/suannai231/ChatGPT
+Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,59 +18,59 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-README for Running Windbg Copilot Python Code
+README for Windbg Copilot
 
-Windbg Copilot Python Code is a package that allows you to use the machine learning capabilities of Windbg Copilot directly in your Python code. This readme file provides instructions for running Windbg Copilot Python Code on your local machine.
+Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. This readme file provides instructions for running Windbg Copilot on your local machine.
 
 Prerequisites
 
-A Windows machine running Windows 11
-Add environmet variable OPENAI_API_KEY with your openai api key
-The Windows Debugger (Windbg) installed on your machine C:\Program Files (x86)\Windows Kits\10\Debuggers\x64
-Python 3.9 or later installed on your machine
-An Internet connection for downloading and installing the package
+        A Windows machine running Windows 11, add environmet variable OPENAI_API_KEY with your openai api key.
+        The Windows Debugger (Windbg) installed on your machine C:\Program Files (x86)\Windows Kits\10\Debuggers\x64.
+        Python 3.9 or later installed on your machine.
+        An Internet connection for downloading and installing the package.
 
 Installation
 
-Open a command prompt or terminal window.
-Install the Windbg Copilot Python Code package using pip:
+        Open a command prompt or terminal window, install the Windbg Copilot packages using pip:
 
-pip install pyttsx3==2.90
-pip install openai
-pip install windbg_copilot
+        pip install pyttsx3==2.90
+        pip install openai
+        pip install windbg_copilot
 
-The package will be downloaded and installed automatically.
+        The packages will be downloaded and installed automatically.
 
 Usage
 
-Open command line and run windbg_copilot:
+        Open command line and run windbg_copilot:
 
-python windbg_copilot.py
+        python windbg_copilot.py
 
-Use the module to interact with Windbg Copilot. You can call functions to execute commands and retrieve suggestions and assistance based on its machine learning models.
+        Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
-        !chat <you may ask anything related to debugging>
-        !ask <ask any question for the above output>
-        !explain: explain the last output
-        !suggest: suggest how to do next
-        !q: quit
+                !chat <you may ask anything related to debugging>
+                !ask <ask any question for the above output>
+                !explain: explain the last output
+                !suggest: suggest how to do next
+                !q: quit
 
-Note: Windbg Copilot Python Code requires an active Internet connection to function properly, as it relies on cloud-based machine learning models.
+        Note: Windbg Copilot requires an active Internet connection to function properly, as it relies on Openai API.
 
 Uninstallation
 
-Open a command prompt or terminal window.
-Use pip to uninstall the Windbg Copilot Python Code package:
+        Open a command prompt or terminal window.
+        Use pip to uninstall the Windbg Copilot package:
 
-pip uninstall windbg_copilot
+        pip uninstall pyttsx3
+        pip uninstall openai
+        pip uninstall windbg_copilot
 
-The package will be uninstalled automatically.
+        The packages will be uninstalled automatically.
 
 Conclusion
 
-Windbg Copilot Python Code is a powerful package that allows you to use the machine learning capabilities of Windbg Copilot directly in your Python code. With its simple installation process and intuitive API, Windbg Copilot Python Code is an essential tool for anyone working on complex Windows applications or drivers using Python.
+Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. With its simple installation process and intuitive API, Windbg Copilot is an essential tool for anyone working on complex Windows debugging.
```

### Comparing `windbg_copilot-1.0.0/README.md` & `windbg_copilot-1.0.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-README for Running Windbg Copilot Python Code
+README for Windbg Copilot
 
-Windbg Copilot Python Code is a package that allows you to use the machine learning capabilities of Windbg Copilot directly in your Python code. This readme file provides instructions for running Windbg Copilot Python Code on your local machine.
+Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. This readme file provides instructions for running Windbg Copilot on your local machine.
 
 Prerequisites
 
-A Windows machine running Windows 11
-Add environmet variable OPENAI_API_KEY with your openai api key
-The Windows Debugger (Windbg) installed on your machine C:\Program Files (x86)\Windows Kits\10\Debuggers\x64
-Python 3.9 or later installed on your machine
-An Internet connection for downloading and installing the package
+        A Windows machine running Windows 11, add environmet variable OPENAI_API_KEY with your openai api key.
+        The Windows Debugger (Windbg) installed on your machine C:\Program Files (x86)\Windows Kits\10\Debuggers\x64.
+        Python 3.9 or later installed on your machine.
+        An Internet connection for downloading and installing the package.
 
 Installation
 
-Open a command prompt or terminal window.
-Install the Windbg Copilot Python Code package using pip:
+        Open a command prompt or terminal window, install the Windbg Copilot packages using pip:
 
-pip install pyttsx3==2.90
-pip install openai
-pip install windbg_copilot
+        pip install pyttsx3==2.90
+        pip install openai
+        pip install windbg_copilot
 
-The package will be downloaded and installed automatically.
+        The packages will be downloaded and installed automatically.
 
 Usage
 
-Open command line and run windbg_copilot:
+        Open command line and run windbg_copilot:
 
-python windbg_copilot.py
+        python windbg_copilot.py
 
-Use the module to interact with Windbg Copilot. You can call functions to execute commands and retrieve suggestions and assistance based on its machine learning models.
+        Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
-        !chat <you may ask anything related to debugging>
-        !ask <ask any question for the above output>
-        !explain: explain the last output
-        !suggest: suggest how to do next
-        !q: quit
+                !chat <you may ask anything related to debugging>
+                !ask <ask any question for the above output>
+                !explain: explain the last output
+                !suggest: suggest how to do next
+                !q: quit
 
-Note: Windbg Copilot Python Code requires an active Internet connection to function properly, as it relies on cloud-based machine learning models.
+        Note: Windbg Copilot requires an active Internet connection to function properly, as it relies on Openai API.
 
 Uninstallation
 
-Open a command prompt or terminal window.
-Use pip to uninstall the Windbg Copilot Python Code package:
+        Open a command prompt or terminal window.
+        Use pip to uninstall the Windbg Copilot package:
 
-pip uninstall windbg_copilot
+        pip uninstall pyttsx3
+        pip uninstall openai
+        pip uninstall windbg_copilot
 
-The package will be uninstalled automatically.
+        The packages will be uninstalled automatically.
 
 Conclusion
 
-Windbg Copilot Python Code is a powerful package that allows you to use the machine learning capabilities of Windbg Copilot directly in your Python code. With its simple installation process and intuitive API, Windbg Copilot Python Code is an essential tool for anyone working on complex Windows applications or drivers using Python.
+Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. With its simple installation process and intuitive API, Windbg Copilot is an essential tool for anyone working on complex Windows debugging.
```

### Comparing `windbg_copilot-1.0.0/setup.cfg` & `windbg_copilot-1.0.1/setup.cfg`

 * *Files 21% similar despite different names*

```diff
@@ -14,44 +14,45 @@
 000000d0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
 000000e0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
 000000f0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
 00000100: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
 00000110: 6578 742f 6d61 726b 646f 776e 0d0a 7572  ext/markdown..ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f73 7561 6e6e 6169 3233  ub.com/suannai23
-00000140: 312f 4368 6174 4750 540d 0a64 6f77 6e6c  1/ChatGPT..downl
-00000150: 6f61 645f 7572 6c20 3d20 0d0a 6c69 6365  oad_url = ..lice
-00000160: 6e73 6520 3d20 4d49 540d 0a6c 6963 656e  nse = MIT..licen
-00000170: 7365 5f66 696c 6573 203d 204c 4943 454e  se_files = LICEN
-00000180: 5345 2e74 7874 0d0a 636c 6173 7369 6669  SE.txt..classifi
-00000190: 6572 7320 3d20 0d0a 0944 6576 656c 6f70  ers = ...Develop
-000001a0: 6d65 6e74 2053 7461 7475 7320 3a3a 2035  ment Status :: 5
-000001b0: 202d 2050 726f 6475 6374 696f 6e2f 5374   - Production/St
-000001c0: 6162 6c65 0d0a 0949 6e74 656e 6465 6420  able...Intended 
-000001d0: 4175 6469 656e 6365 203a 3a20 4465 7665  Audience :: Deve
-000001e0: 6c6f 7065 7273 0d0a 0954 6f70 6963 203a  lopers...Topic :
-000001f0: 3a20 536f 6674 7761 7265 2044 6576 656c  : Software Devel
-00000200: 6f70 6d65 6e74 203a 3a20 4275 696c 6420  opment :: Build 
-00000210: 546f 6f6c 730d 0a09 4c69 6365 6e73 6520  Tools...License 
-00000220: 3a3a 204f 5349 2041 7070 726f 7665 6420  :: OSI Approved 
-00000230: 3a3a 204d 4954 204c 6963 656e 7365 0d0a  :: MIT License..
-00000240: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
-00000250: 6775 6167 6520 3a3a 2050 7974 686f 6e0d  guage :: Python.
-00000260: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-00000270: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-00000280: 203a 3a20 332e 380d 0a09 5072 6f67 7261   :: 3.8...Progra
-00000290: 6d6d 696e 6720 4c61 6e67 7561 6765 203a  mming Language :
-000002a0: 3a20 5079 7468 6f6e 203a 3a20 332e 390d  : Python :: 3.9.
-000002b0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
-000002c0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
-000002d0: 203a 3a20 332e 3130 0d0a 0950 726f 6772   :: 3.10...Progr
-000002e0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
-000002f0: 3a3a 2050 7974 686f 6e20 3a3a 2033 2e31  :: Python :: 3.1
-00000300: 310d 0a0d 0a5b 6f70 7469 6f6e 735d 0d0a  1....[options]..
-00000310: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000320: 203d 200d 0a09 7079 7474 7378 3320 3d3d   = ...pyttsx3 ==
-00000330: 2032 2e39 300d 0a09 6f70 656e 6169 203e   2.90...openai >
-00000340: 3d20 302e 3237 2e32 0d0a 7079 7468 6f6e  = 0.27.2..python
-00000350: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000360: 390d 0a0d 0a5b 6567 675f 696e 666f 5d0d  9....[egg_info].
-00000370: 0a74 6167 5f62 7569 6c64 203d 200d 0a74  .tag_build = ..t
-00000380: 6167 5f64 6174 6520 3d20 300d 0a0d 0a    ag_date = 0....
+00000140: 312f 5769 6e64 6267 5f43 6f70 696c 6f74  1/Windbg_Copilot
+00000150: 0d0a 646f 776e 6c6f 6164 5f75 726c 203d  ..download_url =
+00000160: 200d 0a6c 6963 656e 7365 203d 204d 4954   ..license = MIT
+00000170: 0d0a 6c69 6365 6e73 655f 6669 6c65 7320  ..license_files 
+00000180: 3d20 4c49 4345 4e53 452e 7478 740d 0a63  = LICENSE.txt..c
+00000190: 6c61 7373 6966 6965 7273 203d 200d 0a09  lassifiers = ...
+000001a0: 4465 7665 6c6f 706d 656e 7420 5374 6174  Development Stat
+000001b0: 7573 203a 3a20 3520 2d20 5072 6f64 7563  us :: 5 - Produc
+000001c0: 7469 6f6e 2f53 7461 626c 650d 0a09 496e  tion/Stable...In
+000001d0: 7465 6e64 6564 2041 7564 6965 6e63 6520  tended Audience 
+000001e0: 3a3a 2044 6576 656c 6f70 6572 730d 0a09  :: Developers...
+000001f0: 546f 7069 6320 3a3a 2053 6f66 7477 6172  Topic :: Softwar
+00000200: 6520 4465 7665 6c6f 706d 656e 7420 3a3a  e Development ::
+00000210: 2042 7569 6c64 2054 6f6f 6c73 0d0a 094c   Build Tools...L
+00000220: 6963 656e 7365 203a 3a20 4f53 4920 4170  icense :: OSI Ap
+00000230: 7072 6f76 6564 203a 3a20 4d49 5420 4c69  proved :: MIT Li
+00000240: 6365 6e73 650d 0a09 5072 6f67 7261 6d6d  cense...Programm
+00000250: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+00000260: 5079 7468 6f6e 0d0a 0950 726f 6772 616d  Python...Program
+00000270: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+00000280: 2050 7974 686f 6e20 3a3a 2033 2e38 0d0a   Python :: 3.8..
+00000290: 0950 726f 6772 616d 6d69 6e67 204c 616e  .Programming Lan
+000002a0: 6775 6167 6520 3a3a 2050 7974 686f 6e20  guage :: Python 
+000002b0: 3a3a 2033 2e39 0d0a 0950 726f 6772 616d  :: 3.9...Program
+000002c0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
+000002d0: 2050 7974 686f 6e20 3a3a 2033 2e31 300d   Python :: 3.10.
+000002e0: 0a09 5072 6f67 7261 6d6d 696e 6720 4c61  ..Programming La
+000002f0: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000300: 203a 3a20 332e 3131 0d0a 0d0a 5b6f 7074   :: 3.11....[opt
+00000310: 696f 6e73 5d0d 0a69 6e73 7461 6c6c 5f72  ions]..install_r
+00000320: 6571 7569 7265 7320 3d20 0d0a 0970 7974  equires = ...pyt
+00000330: 7473 7833 203d 3d20 322e 3930 0d0a 096f  tsx3 == 2.90...o
+00000340: 7065 6e61 6920 3e3d 2030 2e32 372e 320d  penai >= 0.27.2.
+00000350: 0a70 7974 686f 6e5f 7265 7175 6972 6573  .python_requires
+00000360: 203d 203e 3d33 2e39 0d0a 0d0a 5b65 6767   = >=3.9....[egg
+00000370: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
+00000380: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
+00000390: 2030 0d0a 0d0a                            0....
```

### Comparing `windbg_copilot-1.0.0/windbg_copilot/windbg_copilot.py` & `windbg_copilot-1.0.1/windbg_copilot/windbg_copilot.py`

 * *Files identical despite different names*

### Comparing `windbg_copilot-1.0.0/windbg_copilot.egg-info/PKG-INFO` & `windbg_copilot-1.0.1/windbg_copilot.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: windbg-copilot
-Version: 1.0.0
+Version: 1.0.1
 Summary: "windbg copilot"
-Home-page: https://github.com/suannai231/ChatGPT
+Home-page: https://github.com/suannai231/Windbg_Copilot
 Download-URL: 
 Author: Jack Yin
 Author-email: suannai231@gmail.com
 License: MIT
 Keywords: windbg,copilot
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -18,59 +18,59 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-README for Running Windbg Copilot Python Code
+README for Windbg Copilot
 
-Windbg Copilot Python Code is a package that allows you to use the machine learning capabilities of Windbg Copilot directly in your Python code. This readme file provides instructions for running Windbg Copilot Python Code on your local machine.
+Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. This readme file provides instructions for running Windbg Copilot on your local machine.
 
 Prerequisites
 
-A Windows machine running Windows 11
-Add environmet variable OPENAI_API_KEY with your openai api key
-The Windows Debugger (Windbg) installed on your machine C:\Program Files (x86)\Windows Kits\10\Debuggers\x64
-Python 3.9 or later installed on your machine
-An Internet connection for downloading and installing the package
+        A Windows machine running Windows 11, add environmet variable OPENAI_API_KEY with your openai api key.
+        The Windows Debugger (Windbg) installed on your machine C:\Program Files (x86)\Windows Kits\10\Debuggers\x64.
+        Python 3.9 or later installed on your machine.
+        An Internet connection for downloading and installing the package.
 
 Installation
 
-Open a command prompt or terminal window.
-Install the Windbg Copilot Python Code package using pip:
+        Open a command prompt or terminal window, install the Windbg Copilot packages using pip:
 
-pip install pyttsx3==2.90
-pip install openai
-pip install windbg_copilot
+        pip install pyttsx3==2.90
+        pip install openai
+        pip install windbg_copilot
 
-The package will be downloaded and installed automatically.
+        The packages will be downloaded and installed automatically.
 
 Usage
 
-Open command line and run windbg_copilot:
+        Open command line and run windbg_copilot:
 
-python windbg_copilot.py
+        python windbg_copilot.py
 
-Use the module to interact with Windbg Copilot. You can call functions to execute commands and retrieve suggestions and assistance based on its machine learning models.
+        Use the following commands to interact with Windbg Copilot. You can chat, ask question and retrieve suggestions and assistance based on ChatGPT model.
 
-        !chat <you may ask anything related to debugging>
-        !ask <ask any question for the above output>
-        !explain: explain the last output
-        !suggest: suggest how to do next
-        !q: quit
+                !chat <you may ask anything related to debugging>
+                !ask <ask any question for the above output>
+                !explain: explain the last output
+                !suggest: suggest how to do next
+                !q: quit
 
-Note: Windbg Copilot Python Code requires an active Internet connection to function properly, as it relies on cloud-based machine learning models.
+        Note: Windbg Copilot requires an active Internet connection to function properly, as it relies on Openai API.
 
 Uninstallation
 
-Open a command prompt or terminal window.
-Use pip to uninstall the Windbg Copilot Python Code package:
+        Open a command prompt or terminal window.
+        Use pip to uninstall the Windbg Copilot package:
 
-pip uninstall windbg_copilot
+        pip uninstall pyttsx3
+        pip uninstall openai
+        pip uninstall windbg_copilot
 
-The package will be uninstalled automatically.
+        The packages will be uninstalled automatically.
 
 Conclusion
 
-Windbg Copilot Python Code is a powerful package that allows you to use the machine learning capabilities of Windbg Copilot directly in your Python code. With its simple installation process and intuitive API, Windbg Copilot Python Code is an essential tool for anyone working on complex Windows applications or drivers using Python.
+Windbg Copilot is a powerful package that allows you to use the ChatGPT capabilities of OpenAI directly in Windows Debugger. With its simple installation process and intuitive API, Windbg Copilot is an essential tool for anyone working on complex Windows debugging.
```

