# Comparing `tmp/VidUniq-1.2.1.tar.gz` & `tmp/VidUniq-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "VidUniq-1.2.1.tar", last modified: Mon Apr  3 15:26:26 2023, max compression
+gzip compressed data, was "VidUniq-2.0.0.tar", last modified: Tue Apr 18 20:10:05 2023, max compression
```

## Comparing `VidUniq-1.2.1.tar` & `VidUniq-2.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-03 15:26:26.571569 VidUniq-1.2.1/
--rw-rw-rw-   0        0        0    35149 2023-04-03 13:58:40.000000 VidUniq-1.2.1/LICENSE.md
--rw-rw-rw-   0        0        0     2111 2023-04-03 15:26:26.571569 VidUniq-1.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1111 2023-04-03 15:26:06.000000 VidUniq-1.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-03 15:26:26.566583 VidUniq-1.2.1/VidUniq/
--rw-rw-rw-   0        0        0     4085 2023-04-03 15:22:02.000000 VidUniq-1.2.1/VidUniq/VideoUniquelizer.py
--rw-rw-rw-   0        0        0      252 2023-04-03 15:25:59.000000 VidUniq-1.2.1/VidUniq/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-03 15:26:26.571569 VidUniq-1.2.1/VidUniq.egg-info/
--rw-rw-rw-   0        0        0     2111 2023-04-03 15:26:26.000000 VidUniq-1.2.1/VidUniq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      241 2023-04-03 15:26:26.000000 VidUniq-1.2.1/VidUniq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-03 15:26:26.000000 VidUniq-1.2.1/VidUniq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-04-03 15:26:26.000000 VidUniq-1.2.1/VidUniq.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-03 15:26:26.000000 VidUniq-1.2.1/VidUniq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      114 2023-04-03 15:26:26.572565 VidUniq-1.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-04-03 15:25:55.000000 VidUniq-1.2.1/setup.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-04-18 20:10:05.740231 VidUniq-2.0.0/
+-rw-rw-r--   0 denis     (1000) denis     (1000)    35149 2023-04-18 18:18:58.000000 VidUniq-2.0.0/LICENSE.md
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2143 2023-04-18 20:10:05.740231 VidUniq-2.0.0/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1203 2023-04-18 20:02:57.000000 VidUniq-2.0.0/README.md
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-04-18 20:10:05.736230 VidUniq-2.0.0/VidUniq/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     8367 2023-04-18 19:55:53.000000 VidUniq-2.0.0/VidUniq/VideoUniquelizer.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      243 2023-04-18 19:31:15.000000 VidUniq-2.0.0/VidUniq/__init__.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      662 2023-04-18 19:31:06.000000 VidUniq-2.0.0/VidUniq/decorators.py
+-rw-rw-r--   0 denis     (1000) denis     (1000)      798 2023-04-18 19:31:06.000000 VidUniq-2.0.0/VidUniq/utils.py
+drwxrwxr-x   0 denis     (1000) denis     (1000)        0 2023-04-18 20:10:05.740231 VidUniq-2.0.0/VidUniq.egg-info/
+-rw-rw-r--   0 denis     (1000) denis     (1000)     2143 2023-04-18 20:10:05.000000 VidUniq-2.0.0/VidUniq.egg-info/PKG-INFO
+-rw-rw-r--   0 denis     (1000) denis     (1000)      280 2023-04-18 20:10:05.000000 VidUniq-2.0.0/VidUniq.egg-info/SOURCES.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        1 2023-04-18 20:10:05.000000 VidUniq-2.0.0/VidUniq.egg-info/dependency_links.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)       39 2023-04-18 20:10:05.000000 VidUniq-2.0.0/VidUniq.egg-info/requires.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)        8 2023-04-18 20:10:05.000000 VidUniq-2.0.0/VidUniq.egg-info/top_level.txt
+-rw-rw-r--   0 denis     (1000) denis     (1000)      106 2023-04-18 20:10:05.740231 VidUniq-2.0.0/setup.cfg
+-rw-rw-r--   0 denis     (1000) denis     (1000)     1351 2023-04-18 19:31:06.000000 VidUniq-2.0.0/setup.py
```

### Comparing `VidUniq-1.2.1/LICENSE.md` & `VidUniq-2.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `VidUniq-1.2.1/PKG-INFO` & `VidUniq-2.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,67 @@
-Metadata-Version: 2.1
-Name: VidUniq
-Version: 1.2.1
-Summary: A simple video uniquelizer
-Home-page: https://github.com/1floppa3/VidUniqLib
-Download-URL: https://github.com/1floppa3/VidUniqLib/archive/main.zip
-Author: 1Floppa3
-Author-email: denis.kochetkov2006@gmail.com
-License: GPL-3.0 license
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# VidUniqLib
-
-![Language](https://img.shields.io/badge/Language-Python3.10-yellow.svg?style=flat)
-![License](https://img.shields.io/pypi/l/VidUniqLib?color=blueviolet)
-
-_**PyPi**_ Video Uniquelizer Library
-###### The purpose of the library is to slightly modify the video so that it cannot be matched with the original video
-
-## Installation
-Install the current version with [PyPI](https://pypi.org/project/VidUniqLib/):
-```bash
-pip install VidUniq
-```
-Or from GitHub:
-```bash
-pip install https://github.com/1floppa3/VidUniqLib/archive/main.zip
-```
-
-## Usage
-You can generate a token for clubhouse by going to the account section and generating a new token
-```python
-from VidUniq import VideoUniquelizer
-
-url: str = 'https://some_invalid_site.site/api.php?wtf=invalid.mp4' #  Could be list
-path_list: list[str] = [ #  Could bee 'str' or 'pathlib.Path'
-    'some_invalid_folder_IdnaP19f/',
-    'some_invalid_file_dmAgo30z.mp4'
-]
-
-uniq = VideoUniquelizer(path=path_list, url=url)
-uniq.uniquelize('uniquelized/')
-```
-
-## Example
-You can find an example of usage here: [VidUniq](https://github.com/1floppa3/VidUniq)
+Metadata-Version: 2.1
+Name: VidUniq
+Version: 2.0.0
+Summary: A light video uniquelizer
+Home-page: https://github.com/1floppa3/VidUniqLib
+Download-URL: https://github.com/1floppa3/VidUniqLib/archive/main.zip
+Author: 1Floppa3
+Author-email: denis.kochetkov2006@gmail.com
+License: GPL-3.0 license
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# VidUniqLib
+
+![Python](https://img.shields.io/badge/Language-Python3.10-yellow.svg?style=flat)
+![License](https://img.shields.io/pypi/l/VidUniq?color=blueviolet)
+![Version](https://img.shields.io/pypi/v/VidUniq?color=orange)
+
+_**PyPi**_ Video Uniquelizer Library
+###### The purpose of the library is to slightly modify the video so that it cannot be matched with the original video
+
+## Installation
+Install the current version with [PyPI](https://pypi.org/project/VidUniqLib/):
+```bash
+pip install VidUniq
+```
+Or from GitHub:
+```bash
+pip install https://github.com/1floppa3/VidUniqLib/archive/main.zip
+```
+
+## Usage
+```python
+from VidUniq import VideoUniquelizer
+
+url = 'https://some_invalid_site.site/api.php?wtf=invalid.mp4'
+path_list = [
+    'some_invalid_folder_IdnaP19f/',
+    'some_invalid_file_dmAgo30z.mp4'
+]
+
+uniq = VideoUniquelizer(True)
+
+uniq.add_video(url=url)
+# uniq.add_video_by_url(url)  Also working
+
+for path in path_list:
+    uniq.add_video_by_path(path, remove_after_save_uniquelized=True)
+
+uniq.uniquelize(fadein=1, fadeout=3, speedx=1.1)
+
+uniq.save_videos('uniquelized_videos/')
+```
+
+## Example
+You can find an example of usage here: [VidUniq](https://github.com/1floppa3/VidUniq)
```

### Comparing `VidUniq-1.2.1/VidUniq.egg-info/PKG-INFO` & `VidUniq-2.0.0/VidUniq.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,58 +1,67 @@
-Metadata-Version: 2.1
-Name: VidUniq
-Version: 1.2.1
-Summary: A simple video uniquelizer
-Home-page: https://github.com/1floppa3/VidUniqLib
-Download-URL: https://github.com/1floppa3/VidUniqLib/archive/main.zip
-Author: 1Floppa3
-Author-email: denis.kochetkov2006@gmail.com
-License: GPL-3.0 license
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: Implementation :: PyPy
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# VidUniqLib
-
-![Language](https://img.shields.io/badge/Language-Python3.10-yellow.svg?style=flat)
-![License](https://img.shields.io/pypi/l/VidUniqLib?color=blueviolet)
-
-_**PyPi**_ Video Uniquelizer Library
-###### The purpose of the library is to slightly modify the video so that it cannot be matched with the original video
-
-## Installation
-Install the current version with [PyPI](https://pypi.org/project/VidUniqLib/):
-```bash
-pip install VidUniq
-```
-Or from GitHub:
-```bash
-pip install https://github.com/1floppa3/VidUniqLib/archive/main.zip
-```
-
-## Usage
-You can generate a token for clubhouse by going to the account section and generating a new token
-```python
-from VidUniq import VideoUniquelizer
-
-url: str = 'https://some_invalid_site.site/api.php?wtf=invalid.mp4' #  Could be list
-path_list: list[str] = [ #  Could bee 'str' or 'pathlib.Path'
-    'some_invalid_folder_IdnaP19f/',
-    'some_invalid_file_dmAgo30z.mp4'
-]
-
-uniq = VideoUniquelizer(path=path_list, url=url)
-uniq.uniquelize('uniquelized/')
-```
-
-## Example
-You can find an example of usage here: [VidUniq](https://github.com/1floppa3/VidUniq)
+Metadata-Version: 2.1
+Name: VidUniq
+Version: 2.0.0
+Summary: A light video uniquelizer
+Home-page: https://github.com/1floppa3/VidUniqLib
+Download-URL: https://github.com/1floppa3/VidUniqLib/archive/main.zip
+Author: 1Floppa3
+Author-email: denis.kochetkov2006@gmail.com
+License: GPL-3.0 license
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Operating System :: OS Independent
+Classifier: Intended Audience :: End Users/Desktop
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: Implementation :: PyPy
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
+# VidUniqLib
+
+![Python](https://img.shields.io/badge/Language-Python3.10-yellow.svg?style=flat)
+![License](https://img.shields.io/pypi/l/VidUniq?color=blueviolet)
+![Version](https://img.shields.io/pypi/v/VidUniq?color=orange)
+
+_**PyPi**_ Video Uniquelizer Library
+###### The purpose of the library is to slightly modify the video so that it cannot be matched with the original video
+
+## Installation
+Install the current version with [PyPI](https://pypi.org/project/VidUniqLib/):
+```bash
+pip install VidUniq
+```
+Or from GitHub:
+```bash
+pip install https://github.com/1floppa3/VidUniqLib/archive/main.zip
+```
+
+## Usage
+```python
+from VidUniq import VideoUniquelizer
+
+url = 'https://some_invalid_site.site/api.php?wtf=invalid.mp4'
+path_list = [
+    'some_invalid_folder_IdnaP19f/',
+    'some_invalid_file_dmAgo30z.mp4'
+]
+
+uniq = VideoUniquelizer(True)
+
+uniq.add_video(url=url)
+# uniq.add_video_by_url(url)  Also working
+
+for path in path_list:
+    uniq.add_video_by_path(path, remove_after_save_uniquelized=True)
+
+uniq.uniquelize(fadein=1, fadeout=3, speedx=1.1)
+
+uniq.save_videos('uniquelized_videos/')
+```
+
+## Example
+You can find an example of usage here: [VidUniq](https://github.com/1floppa3/VidUniq)
```

