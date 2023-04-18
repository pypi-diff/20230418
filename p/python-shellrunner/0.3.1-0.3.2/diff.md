# Comparing `tmp/python_shellrunner-0.3.1.tar.gz` & `tmp/python_shellrunner-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_shellrunner-0.3.1.tar", last modified: Mon Mar 27 03:06:39 2023, max compression
+gzip compressed data, was "python_shellrunner-0.3.2.tar", last modified: Tue Apr 18 00:59:38 2023, max compression
```

## Comparing `python_shellrunner-0.3.1.tar` & `python_shellrunner-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1070 2023-03-27 02:58:01.365366 python_shellrunner-0.3.1/LICENSE
--rw-r--r--   0        0        0     7935 2023-03-27 02:58:01.365366 python_shellrunner-0.3.1/README.md
--rw-r--r--   0        0        0     2196 2023-03-27 03:06:39.875238 python_shellrunner-0.3.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-27 02:58:01.365366 python_shellrunner-0.3.1/src/__init__.py
--rw-r--r--   0        0        0     2637 2023-03-27 02:58:01.365366 python_shellrunner-0.3.1/src/helpers.py
--rw-r--r--   0        0        0     9205 2023-03-27 03:01:54.105308 python_shellrunner-0.3.1/src/shellrunner.py
--rw-r--r--   0        0        0    14278 2023-03-27 02:58:01.365366 python_shellrunner-0.3.1/src/test_shellrunner.py
--rw-r--r--   0        0        0     8763 1970-01-01 00:00:00.000000 python_shellrunner-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-04-18 00:39:00.987500 python_shellrunner-0.3.2/LICENSE
+-rw-r--r--   0        0        0     7899 2023-04-18 00:42:25.717481 python_shellrunner-0.3.2/README.md
+-rw-r--r--   0        0        0     2218 2023-04-18 00:59:38.757380 python_shellrunner-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-18 00:39:00.987500 python_shellrunner-0.3.2/src/__init__.py
+-rw-r--r--   0        0        0     2651 2023-04-18 00:52:29.617422 python_shellrunner-0.3.2/src/helpers.py
+-rw-r--r--   0        0        0     9205 2023-04-18 00:39:00.987500 python_shellrunner-0.3.2/src/shellrunner.py
+-rw-r--r--   0        0        0    14278 2023-04-18 00:39:00.987500 python_shellrunner-0.3.2/src/test_shellrunner.py
+-rw-r--r--   0        0        0     8756 1970-01-01 00:00:00.000000 python_shellrunner-0.3.2/PKG-INFO
```

### Comparing `python_shellrunner-0.3.1/LICENSE` & `python_shellrunner-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_shellrunner-0.3.1/README.md` & `python_shellrunner-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,16 +21,14 @@
 - [Options](#options)
   - [Output](#output)
   - [Environment Variables](#environment-variables)
 - [Examples](#examples)
 
 ## Install
 
-ShellRunner has zero dependencies.
-
 ```
 pip install -U python-shellrunner
 ```
 
 ## Usage
 
 ```python
```

### Comparing `python_shellrunner-0.3.1/pyproject.toml` & `python_shellrunner-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 [project]
 name = "python-shellrunner"
-version = "0.3.1"
+version = "0.3.2"
 description = "Write safe shell scripts in Python."
 authors = [
     { name = "adamhl8", email = "adamhl@pm.me" },
 ]
-dependencies = []
+dependencies = [
+    "psutil>=5.9.5",
+]
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3.10",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX",
@@ -32,19 +34,19 @@
 [project.urls]
 Homepage = "https://github.com/adamhl8/python-shellrunner"
 Source = "https://github.com/adamhl8/python-shellrunner"
 "Bug Tracker" = "https://github.com/adamhl8/python-shellrunner/issues"
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "black>=23.1.0",
-    "ruff>=0.0.257",
-    "pytest>=7.2.2",
-    "types-psutil>=5.9.5.10",
+    "black>=23.3.0",
+    "ruff>=0.0.261",
+    "pytest>=7.3.1",
     "pyroma>=4.2",
+    "types-psutil>=5.9.5.11",
 ]
 
 [tool.pdm.scripts.test]
 cmd = "pytest src"
 
 [tool.pdm.scripts.pyright]
 shell = "pyright src"
```

### Comparing `python_shellrunner-0.3.1/src/helpers.py` & `python_shellrunner-0.3.2/src/helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import os
 from pathlib import Path
 from shutil import which
 from typing import NamedTuple, TypeVar
 
+from psutil import Process
+
 
 class ShellCommandResult(NamedTuple):
     out: str
     status: int
     pipestatus: list[int]
 
 
@@ -30,15 +32,15 @@
     pass
 
 
 # Returns the full path of parent process/shell. That way commands are executed using the same shell that invoked this script.
 # TODO test if executable is a shell, if not default to bash
 def get_parent_shell_path() -> Path:
     try:
-        return Path(f"/proc/{os.getppid()}/exe").readlink().resolve(strict=True)
+        return Path(Process().parent().exe()).resolve(strict=True)
     except Exception as e:  # noqa: BLE001
         message = "An error occured when trying to get the path of the parent shell."
         raise ShellResolutionError(message) from e
 
 
 # Returns the full path of a given path or executable name. e.g. "/bin/bash" or "bash"
 def resolve_shell_path(shell: str) -> Path:
```

### Comparing `python_shellrunner-0.3.1/src/shellrunner.py` & `python_shellrunner-0.3.2/src/shellrunner.py`

 * *Files identical despite different names*

### Comparing `python_shellrunner-0.3.1/src/test_shellrunner.py` & `python_shellrunner-0.3.2/src/test_shellrunner.py`

 * *Files identical despite different names*

### Comparing `python_shellrunner-0.3.1/PKG-INFO` & `python_shellrunner-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-shellrunner
-Version: 0.3.1
+Version: 0.3.2
 Summary: Write safe shell scripts in Python.
 Keywords: shell scripting bash zsh fish
 Author-Email: adamhl8 <adamhl@pm.me>
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Classifier: Programming Language :: Unix Shell
 Classifier: Topic :: System :: Shells
 Classifier: Topic :: System :: System Shells
 Project-URL: Homepage, https://github.com/adamhl8/python-shellrunner
 Project-URL: Source, https://github.com/adamhl8/python-shellrunner
 Project-URL: Bug tracker, https://github.com/adamhl8/python-shellrunner/issues
 Requires-Python: >=3.10
+Requires-Dist: psutil>=5.9.5
 Description-Content-Type: text/markdown
 
 <div align="center">
   <img width="250" src="https://user-images.githubusercontent.com/1844269/226196799-402898d6-c363-4735-be23-57c0ba9e1035.png">
 </div>
 <br>
 <p align="center">
@@ -42,16 +43,14 @@
 - [Options](#options)
   - [Output](#output)
   - [Environment Variables](#environment-variables)
 - [Examples](#examples)
 
 ## Install
 
-ShellRunner has zero dependencies.
-
 ```
 pip install -U python-shellrunner
 ```
 
 ## Usage
 
 ```python
```

