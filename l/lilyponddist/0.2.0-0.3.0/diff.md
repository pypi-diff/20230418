# Comparing `tmp/lilyponddist-0.2.0.tar.gz` & `tmp/lilyponddist-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lilyponddist-0.2.0.tar", last modified: Tue Apr 18 15:32:13 2023, max compression
+gzip compressed data, was "lilyponddist-0.3.0.tar", last modified: Tue Apr 18 16:00:21 2023, max compression
```

## Comparing `lilyponddist-0.2.0.tar` & `lilyponddist-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 15:32:12.996585 lilyponddist-0.2.0/
--rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-0.2.0/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)      965 2023-04-18 15:32:12.995585 lilyponddist-0.2.0/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      688 2023-04-18 15:30:21.000000 lilyponddist-0.2.0/README.rst
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 15:32:12.992585 lilyponddist-0.2.0/lilyponddist/
--rw-rw-r--   0 em        (1000) em        (1000)     6840 2023-04-18 15:28:14.000000 lilyponddist-0.2.0/lilyponddist/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 15:32:12.994585 lilyponddist-0.2.0/lilyponddist.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)      965 2023-04-18 15:32:12.000000 lilyponddist-0.2.0/lilyponddist.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)      245 2023-04-18 15:32:12.000000 lilyponddist-0.2.0/lilyponddist.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-18 15:32:12.000000 lilyponddist-0.2.0/lilyponddist.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       20 2023-04-18 15:32:12.000000 lilyponddist-0.2.0/lilyponddist.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       13 2023-04-18 15:32:12.000000 lilyponddist-0.2.0/lilyponddist.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-18 15:32:12.996585 lilyponddist-0.2.0/setup.cfg
--rwxrwxr-x   0 em        (1000) em        (1000)      721 2023-04-18 15:31:22.000000 lilyponddist-0.2.0/setup.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 15:32:12.995585 lilyponddist-0.2.0/test/
--rw-r--r--   0 em        (1000) em        (1000)       97 2023-04-17 21:46:56.000000 lilyponddist-0.2.0/test/test1.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.126271 lilyponddist-0.3.0/
+-rw-r--r--   0 em        (1000) em        (1000)     2079 2023-04-17 21:56:53.000000 lilyponddist-0.3.0/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)      965 2023-04-18 16:00:21.126271 lilyponddist-0.3.0/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      688 2023-04-18 15:30:21.000000 lilyponddist-0.3.0/README.rst
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.124271 lilyponddist-0.3.0/lilyponddist/
+-rw-rw-r--   0 em        (1000) em        (1000)     6872 2023-04-18 16:00:13.000000 lilyponddist-0.3.0/lilyponddist/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.125271 lilyponddist-0.3.0/lilyponddist.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)      965 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)      245 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       20 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       13 2023-04-18 16:00:21.000000 lilyponddist-0.3.0/lilyponddist.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-04-18 16:00:21.127271 lilyponddist-0.3.0/setup.cfg
+-rwxrwxr-x   0 em        (1000) em        (1000)      720 2023-04-18 15:49:06.000000 lilyponddist-0.3.0/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-04-18 16:00:21.126271 lilyponddist-0.3.0/test/
+-rw-r--r--   0 em        (1000) em        (1000)      328 2023-04-18 15:58:18.000000 lilyponddist-0.3.0/test/test1.py
```

### Comparing `lilyponddist-0.2.0/LICENSE` & `lilyponddist-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lilyponddist-0.2.0/PKG-INFO` & `lilyponddist-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 0.2.0
+Version: 0.3.0
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 lilyponddist
```

### Comparing `lilyponddist-0.2.0/README.rst` & `lilyponddist-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `lilyponddist-0.2.0/lilyponddist/__init__.py` & `lilyponddist-0.3.0/lilyponddist/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,30 @@
-from pathlib import Path
 import sys
+
+
+__VERSION__ = "0.3.0"
+
+if __name__ == '__main__':
+    if len(sys.argv) > 1 and sys.argv[1] == '--version':
+        print(__VERSION__)
+    sys.exit(0)
+
+
+from pathlib import Path
 import platform
 import sysconfig
 import os
 import logging
 import urllib.request
 import tempfile
 import appdirs
 import shutil
 import progressbar
 from typing import Union
 
-__VERSION__ = "0.2.0"
-
 
 logger = logging.getLogger("lilyponddist")
 
 
 class _ProgressBar():
 
     def __init__(self):
@@ -57,15 +65,15 @@
             z.extractall(destfolder)
 
     def _targzextract(f: Path, destfolder: Path):
         import tarfile
         tfile = tarfile.open(f)
         tfile.extractall(destfolder)
 
-    destfolder.mkdir(exist_ok=True)
+    destfolder.mkdir(exist_ok=True, parents=True)
 
     if path.name.endswith('.zip'):
         _zipextract(path, destfolder)
     elif path.name.endswith('.tar.gz'):
         _targzextract(path, destfolder)
     else:
         raise RuntimeError(f"File format of {path} not supported")
@@ -209,13 +217,10 @@
         binary = 'lilypond.exe'
     else:
         binary = 'lilypond'
 
     return lilypondroot() / 'bin' / binary
 
 
-if __name__ == '__main__':
-    if len(sys.argv) > 1 and sys.argv[1] == '--version':
-        print(__VERSION__)
-elif _is_first_run():
+if _is_first_run():
     print("lilyponddist -- First Run. Will download lilypond")
     _initlib()
```

### Comparing `lilyponddist-0.2.0/lilyponddist.egg-info/PKG-INFO` & `lilyponddist-0.3.0/lilyponddist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lilyponddist
-Version: 0.2.0
+Version: 0.3.0
 Summary: Distribute lilypond as a pypi package
 Home-page: https://github.com/gesellkammer/lilyponddist
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
 lilyponddist
```

### Comparing `lilyponddist-0.2.0/setup.py` & `lilyponddist-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 Programming Language :: Python :: 3
 """
 
 def get_version():
     return subprocess.check_output([sys.executable, "lilyponddist/__init__.py", "--version"]).decode('utf8').strip()
 
 
-
 setup(name='lilyponddist',
       version=get_version(),
       url='https://github.com/gesellkammer/lilyponddist',
       description='Distribute lilypond as a pypi package', 
       long_description=open('README.rst').read(),
       classifiers=[l.strip() for l in classifiers.splitlines() if l.strip()],
       packages=['lilyponddist'],
```

